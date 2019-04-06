---
title: Installieren oder Entfernen von auf Windows 10 Anniversary Update oder Creators Update
description: Anweisungen zur der Vorgängerversion, die Beta-Distribution, die auf Windows 10 Anniversary Update oder Creators Update-Installation und Deinstallation
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10, legacy, beta, install, remove, uninstall, un-install, delete, deprecated
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: b31bb3a542b8481c723df42292e20e364680722d
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063588"
---
# <a name="guide-to-install-or-uninstall-windows-subsystem-for-linux-on-windows-10-anniversary-update-and-creators-update"></a>Anleitung zum Installieren oder Deinstallieren von Windows-Subsystem für Linux auf Windows 10 Anniversary Update und Creators Update 

Wenn Sie Windows 10 Creators Update ausführen, oder höher, bitte [führen Sie die installationsanweisungen für Windows 10](install-win10.md).

<strong><em><span style="color: #f28014">Die folgenden Anweisungen gelten für Benutzer, die Windows 10 Anniversary Update oder Windows 10 Creators Update</span></em></strong>

Vor Windows 10 Fall Creators Update (Version 1709) WSL als Betafunktion veröffentlicht wurde und eine einzelne Instanz von Ubuntu bei "Bash auf Ubuntu unter Windows" (oder Bash.exe) zuerst ausgeführt wurde.

> Während Sie die WSL unter früheren Versionen von Windows 10 verwenden können, ist diese Betaversion "legacy-Distribution, die" als veraltet eingestuft. Wir empfehlen Ihnen, führen Sie die neueste Version von Windows 10 verfügbar. Jeder neuen Windows 10-Version enthält viele Hunderte von Fehlerbehebungen und Verbesserungen in WSL eigenständig verwendet, sodass immer Linux-Tools und apps für WSL ordnungsgemäß ausgeführt.

Wenn Sie nicht auf Fall Creators Update oder höher aktualisieren können, führen Sie die folgenden Schritte zum Aktivieren und Verwenden von WSL:

1. Entwickler-Modus für die Ausführung WSL auf Windows 10 Anniversary Update oder Creators Update aktivieren, müssen Sie den Entwicklermodus aktivieren:

    Open **Einstellungen** -> **Update und Sicherheit** -> **für Entwickler**

    Wählen Sie das Optionsfeld Entwicklermodus  
    ![Aktivieren des Entwicklermodus](media/updateAndSecurity.png)

    > Die Anforderung zum Aktivieren der Entwicklermodus wurde [in Windows 10 Fall Creators Update entfernt](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/)

1. Öffnen Sie eine Eingabeaufforderung.  Typ `bash` und die EINGABETASTE drücken

    Beim ersten Ausführen von Bash auf Ubuntu unter Windows, werden Sie aufgefordert, Canonical Lizenz zu akzeptieren. Sobald Accpted, WSL heruntergeladen und installiert die Ubuntu-Instanz auf dem Computer, und eine "Bash auf Ubuntu unter Windows"-Verknüpfung Ihrem Startmenü hinzugefügt werden wird.

    ![Aufforderung zur Installation von Ubuntu](media/bashShellInstall.png)

    Beim ersten Ausführen von Bash auf Ubuntu unter Windows, werden Sie aufgefordert werden UNIX-Benutzername und Kennwort zu erstellen. Führen Sie die [Anweisungen für die neue Distribution Instanz](initialize-distro.md) zum Abschließen der Installations

1. Starten Sie eine neue Ubuntu-Shell, indem entweder:
    * Ausführung `bash` an einer Eingabeaufforderung
    * Klicken Sie auf die Verknüpfung im Startmenü "Bash auf Ubuntu unter Windows"

    
## <a name="uninstallingremoving-the-legacy-distro"></a>Die legacy-Distribution Deinstallieren/Entfernen
Wenn Sie von einer früheren Version von Windows 10, Windows 10 Fall Creators Update auf denen WSL installiert aktualisieren, sind Ihre vorhandenen Distribution bleibt unverändert. Allerdings wir dringend empfohlen, eine neue Store bereitgestellte Distribution ASAP installieren und migrieren alle erforderlichen Dateien, Daten usw. aus Ihrem legacy-Distribution, die zu Ihrer neuen Distribution.

Um die legacy-Distribution, die von Ihrem Computer zu entfernen, führen Sie Folgendes von einer Befehlszeile oder PowerShell ein:

```console
lxrun /uninstall /full
```

### <a name="manually-deleting-the-legacy-distro"></a>Die legacy-Distribution, die manuell zu löschen
Wenn Sie möchten, können Sie Ihre legacy-Instanz manuell löschen. Dies kann erforderlich sein, wenn deinstallieren, die mithilfe des legacy-Distribution, die Probleme auftreten `lxrun.exe`, oder Windows 10 Frühjahr 2018 Update ausgeführt werden (oder höher) der werden nicht im Lieferumfang `lxrun.exe`.

Um Ihre älteren WSL Distribution erzwungen zu löschen, löschen die `%localappdata%\lxss\` Ordner (und alle es handelt sich um untergeordneten Inhalt) mithilfe von Windows Datei-Explorer oder die Befehlszeile:

Mithilfe der PowerShell
```powershell
rm -Recurse $env:localappdata/lxss/
```

Verwenden Cmd ein:
```console
DEL /S %localappdata%\lxss\
```
