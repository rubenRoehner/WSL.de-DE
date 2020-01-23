---
title: Dateiberechtigungen
description: Grundlegendes zur Bestimmung der Dateiberechtigungen in Windows mit WSL
keywords: Bashonwindows, bash, WSL, wsl2, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10, Datei, Berechtigungen
ms.date: 01/14/2020
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 4566fc86cf14df986bde80cf3a6cfb9267b23308
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520859"
---
# <a name="file-permissions-for-wsl"></a>Dateiberechtigungen für WSL

Auf dieser Seite wird erläutert, wie Linux-Dateiberechtigungen über das Windows-Subsystem für Linux interpretiert werden, insbesondere beim Zugriff auf Ressourcen innerhalb von Windows auf dem NT-Dateisystem. In dieser Dokumentation wird ein grundlegendes Verständnis der [Struktur der Linux-Dateisystem Berechtigungen](https://wiki.archlinux.org/index.php/File_permissions_and_attributes) vorausgesetzt. <!--TODO: Double check that it's okay to add these links--> und den [Befehl "um Ask](https://en.wikipedia.org/wiki/Umask)".

Beim Zugriff auf Windows-Dateien von WSL werden die Dateiberechtigungen entweder aus Windows-Berechtigungen berechnet, oder Sie werden aus Metadaten gelesen, die von WSL der Datei hinzugefügt wurden. Diese Metadaten sind standardmäßig nicht aktiviert. 

## <a name="wsl-metadata-on-windows-files"></a>WSL-Metadaten für Windows-Dateien

Wenn Metadaten in WSL als Bereitstellungs Option aktiviert sind, können erweiterte Attribute für Windows NT-Dateien hinzugefügt und interpretiert werden, um Linux-Dateisystem Berechtigungen bereitzustellen. 

WSL kann vier erweiterte NTFS-Attribute hinzufügen:

| Attributname | Beschreibung |
| --- | --- |
| $LXUID | Benutzer Besitzer-ID |
| $LXGID | Gruppenbesitzer-ID |
| $LXMOD | Dateimodus (Dateisystem-Berechtigungs-oktale und-Typ, z. b. 0777) |
| $LXDEV | Gerät, wenn es sich um eine Gerätedatei handelt |

Außerdem verfügen alle Dateien, bei denen es sich nicht um reguläre Dateien oder Verzeichnisse handelt (z. b. Symlinks, Anlagen, Blockgeräte, Unix-Sockets und Zeichengeräte), ebenfalls über einen NTFS-Analyse [Punkt](https://docs.microsoft.com/en-us/windows/win32/fileio/reparse-points). Dadurch wird es viel schneller, die Art der Datei in einem bestimmten Verzeichnis zu ermitteln, ohne die erweiterten Attribute Abfragen zu müssen. 
<!-- TODO: For the blog include ONeDrive detail -->

## <a name="file-access-scenarios"></a>Datei Zugriffs Szenarien

Im folgenden finden Sie eine Beschreibung der Art und Weise, wie Berechtigungen beim Zugriff auf Dateien auf verschiedene Weise mithilfe des Windows-Subsystems für Linux bestimmt werden

### <a name="accessing-files-in-the-windows-drive-file-system-drvfs-from-linux"></a>Zugreifen auf Dateien im Windows Drive File System (drvfs) von Linux

Diese Szenarien treten auf, wenn Sie von WSL aus auf Ihre Windows-Dateien zugreifen, höchstwahrscheinlich über `/mnt/c`. 

#### <a name="reading-file-permissions-from-an-existing-windows-file"></a>Lesen von Dateiberechtigungen aus einer vorhandenen Windows-Datei

Das Ergebnis hängt davon ab, ob die Datei bereits über vorhandene Metadaten verfügt.

##### <a name="the-file-does-not-have-metadata-default"></a>**Die Datei hat keine Metadaten (Standard).**

Wenn der Datei keine Metadaten zugeordnet sind, übersetzen wir die effektiven Berechtigungen des Windows-Benutzers in Bits mit Lese-/Schreibzugriff, und legen Sie diese als denselben Wert für "User", "Group" und "Other" fest. Wenn Ihr Windows-Benutzerkonto z. b. Lese-und Ausführungs Zugriff hat, aber keinen Schreibzugriff auf die Datei hat, wird dies als `r-x` für "Benutzer", "Gruppe" und "andere" angezeigt. Wenn für die Datei das Attribut "schreibgeschützt" in Windows festgelegt ist, erteilen wir keinen Schreibzugriff in Linux.

##### <a name="the-file-has-metadata"></a>Die Datei enthält Metadaten.

Wenn in der Datei Metadaten vorhanden sind, verwenden wir einfach diese Metadatenwerte anstelle der Übersetzung effektiver Berechtigungen des Windows-Benutzers.

#### <a name="changing-file-permissions-on-an-existing-windows-file-using-chmod"></a>Ändern von Dateiberechtigungen für eine vorhandene Windows-Datei mit chmod

Das Ergebnis hängt davon ab, ob die Datei bereits über vorhandene Metadaten verfügt.

##### <a name="the-file-does-not-have-metadata-default"></a>**Die Datei hat keine Metadaten (Standard).**

Chmod hat nur einen Effekt, wenn Sie alle Schreib Attribute einer Datei entfernen, wird das "Read only"-Attribut in der Windows-Datei festgelegt, da dies das gleiche Verhalten wie CIFS (Common Internet File System) ist, bei dem es sich um den SMB-Client (Server Message Block) in Linux handelt.

##### <a name="the-file-has-metadata"></a>Die Datei enthält Metadaten.

Chmod ändert oder fügt Metadaten in Abhängigkeit von den bereits vorhandenen Metadaten der Datei ein. 

Denken Sie daran, dass Sie nicht mehr Zugriff haben als bei Windows, auch wenn die Metadaten dies tun. Beispielsweise können Sie die Metadaten so festlegen, dass Sie über `chmod 777`Schreibberechtigungen für eine Datei haben, aber wenn Sie versucht haben, auf diese Datei zuzugreifen, können Sie trotzdem nicht in diese schreiben. Dies ist dank der Interopability möglich, da alle Lese-oder Schreib Befehle an Windows-Dateien durch Ihre Windows-Benutzerberechtigungen geleitet werden.

#### <a name="creating-a-file-in-drivefs"></a>Erstellen einer Datei in drivefs

Das Ergebnis hängt davon ab, ob Metadaten aktiviert sind.

##### <a name="metadata-is-not-enabled-default"></a>Metadaten sind nicht aktiviert (Standard)

Die Windows-Berechtigungen der neu erstellten Datei sind identisch mit dem Erstellen der Datei in Windows ohne eine bestimmte Sicherheits Beschreibung. Sie erben die Berechtigungen des übergeordneten Elements. 

##### <a name="metadata-is-enabled"></a>Metadaten sind aktiviert

Die Berechtigungsbits der Datei sind so festgelegt, dass Sie der Linux-""-Umfrage folgen, und die Datei wird mit Metadaten gespeichert.

#### <a name="which-linux-user-and-linux-group-owns-the-file"></a>Welche Linux-Benutzer-und Linux-Gruppe besitzt die Datei? 

Das Ergebnis hängt davon ab, ob die Datei bereits über vorhandene Metadaten verfügt.

##### <a name="the-file-does-not-have-metadata-default"></a>**Die Datei hat keine Metadaten (Standard).**
Im Standardszenario legen wir beim Automatisieren von Windows-Laufwerken fest, dass die Benutzer-ID (UID) für eine beliebige Datei auf die Benutzer-ID des WSL-Benutzers und die Gruppen-ID (GID) auf die Prinzipal Gruppen-ID des WSL-Benutzers festgelegt ist. 

##### <a name="the-file-has-metadata"></a>Die Datei enthält Metadaten.

Die in den Metadaten angegebene UID und GID werden als Benutzer Besitzer und Gruppenbesitzer der Datei angewendet. 

### <a name="accessing-linux-files-from-windows-using-wsl"></a>Zugreifen auf Linux-Dateien aus Windows mithilfe von `\\wsl$`

Wenn Sie über `\\wsl$` auf Linux-Dateien zugreifen, wird der Standardbenutzer ihrer WSL-Distribution verwendet. Daher hat jede Windows-APP, die auf Linux-Dateien zugreift, dieselben Berechtigungen wie der Standardbenutzer.

#### <a name="creating-a-new-file"></a>Erstellen einer neuen Datei

Beim Erstellen einer neuen Datei in einer WSL-Distribution von Windows wird die Standard-"Umschlag"-Sequenz angewendet. Der Standardwert für "umask" ist `022`, d. h., er ermöglicht alle Berechtigungen mit Ausnahme von Schreibberechtigungen für Gruppen und andere. 

### <a name="accessing-files-in-the-linux-root-file-system-from-linux"></a>Zugreifen auf Dateien im Linux-Stammdatei System unter Linux

Alle Dateien, die im Linux-Stammdatei System erstellt, geändert oder darauf zugegriffen werden, folgen den Linux-Standard Konventionen, z. b. das Anwenden von umask auf eine neu erstellte Datei.

## <a name="configuring-file-permissions"></a>Konfigurieren von Dateiberechtigungen

Sie können Ihre Dateiberechtigungen innerhalb Ihrer Windows-Laufwerke mithilfe der Einstellungsoptionen in "WSL. conf" konfigurieren. Mit den Einstellungsoptionen können Sie `umask`, `dmask` und `fmask` Berechtigungs Masken festlegen. Der `umask` wird auf alle Dateien angewendet, die `dmask` wird nur auf Verzeichnisse angewendet, und die `fmask` wird nur auf Dateien angewendet. Diese Berechtigungs Masken werden dann durch eine logische OR-Operation durchgeführt, wenn Sie auf Dateien angewendet werden, z. b. Wenn Sie den `umask` Wert `023` und einen `fmask` Wert `022` haben, wird die resultierende Berechtigungs Maske für Dateien `023`. 

Anweisungen zur Vorgehensweise finden Sie auf der Dokument Seite [Verwalten von Linux-Distributionen](./wsl-config.md) .
<!-- TODO: Add # to the link-->

