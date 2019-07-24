---
title: Windows-Subsystem für Linux (Befehlsreferenz)
description: Liste der Befehle, mit denen das Windows-Subsystem für Linux verwaltet wird
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu
author: scooley
ms.author: scooley
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.openlocfilehash: 465f55f8ba210cd366adc66d433f1873e295136f
ms.sourcegitcommit: ead64b13501d6cb7170adafbb5624f4984a0af16
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/21/2019
ms.locfileid: "67307654"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a>Befehlsreferenz für Windows-Subsystem für Linux

Die beste Möglichkeit, mit dem Windows-Subsystem für Linux zu interagieren, ist `wsl.exe` die Verwendung des-Befehls. 

## `wsl.exe` 

Im folgenden finden Sie eine Liste mit allen Optionen `wsl.exe` , wenn Sie ab Windows Version 1903 verwenden.

* Argumente für das Ausführen von Linux-Binärdateien:

    * Wenn keine Befehlszeile angegeben wird, wird die Standardshell von WSL. exe gestartet.

    * --Exec,-e<CommandLine>
        * Führen Sie den angegebenen Befehl ohne die Linux-Standard Shell aus.

    * --
        * Übergeben Sie die verbleibende Befehlszeile unverändert.

* Optionen:
    * --Distribution,-d<Distro>
        * Führt die angegebene Verteilung aus.

    * --Benutzer,-u<UserName>
        * Ausführen als angegebener Benutzer.

* Argumente für die Verwaltung des Windows-Subsystems für Linux:

    * --Export <Distro><FileName>
        * Exportiert die Verteilung in eine tar-Datei.
        Der Dateiname kann für die Standardausgabe sein.

    * --Import <Distro> <InstallLocation>[Optionen <FileName> ]
        * Importiert die angegebene tar-Datei als neue Verteilung.
        Der Dateiname kann für die Standardeingabe sein.

        * Optionen:
            * --Version <Version> gibt die Version an, die für die neue Verteilung verwendet werden soll.

    * --List,-l [Optionen]
        * Listet Verteilungen auf.

        * Optionen:
            * --Alle
                * Auflisten aller Verteilungen, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.

            * --wird ausgeführt
                * Listet nur Verteilungen auf, die zurzeit ausgeführt werden.

    * --Set-Default,-s<Distro>
        * Legt die Verteilung als Standard fest.

    * --Set-Default-Version<Version>
        * Ändert die Standard Installationsversion für neue Verteilungen.

    * --Set-Version <Distro><Version>
        * Ändert die Version der angegebenen Verteilung.

    * --beenden,-t<Distro>
        * Beendet die angegebene Verteilung.

    * --Registrierung aufheben<Distro>
        * Hebt die Registrierung der Verteilung auf.

    * --help
        * Anzeigen von Nutzungsinformationen.

## <a name="additional-commands"></a>Weitere Befehle

Es gibt auch historische Befehle für die Interaktion mit dem Windows-Subsystem für Linux. Ihre Funktionalität ist in `wsl.exe`enthalten, Sie sind jedoch weiterhin zur Verwendung verfügbar. 

### `wslconfig.exe`

Mit diesem Befehl können Sie Ihre WSL-Verteilung konfigurieren. Im folgenden finden Sie eine Liste der zugehörigen Optionen.

* /l,/List [Option]
    * Listet registrierte Verteilungen auf.
        * /All: Optional können Sie alle Distributionen auflisten, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.

        * /Running: nur Verteilungen auflisten, die zurzeit ausgeführt werden.

* /s,/SetDefault<DistributionName>
    * Legt die Verteilung als Standard fest.

* /t,/Terminate<DistributionName>
    * Beendet die Verteilung.

* /u,/Unregister<DistributionName>
    * Hebt die Registrierung der Verteilung auf.

### `bash.exe`

Dieser Befehl wird verwendet, um eine bash-Shell zu starten. Im folgenden finden Sie die Optionen, die Sie mit diesem Befehl verwenden können.

* Keine Option angegeben.
    * Starten der bash-Shell im aktuellen Verzeichnis. Wenn die bash-Shell nicht installiert ist, wird automatisch ausgeführt.`lxrun /install`

* bash ~
    * Hiermit wird die bash-Shell in das Basisverzeichnis des Benutzers gestartet.  Vergleichbar mit dem `cd ~`Ausführen von.

* bash-c "&lt;Befehl&gt;"
    * Führt den Befehl aus, druckt die Ausgabe und wird zurück zur Windows-Eingabeaufforderung. <br/> <br/> Beispiel`bash -c "ls"`

## <a name="deprecated-commands"></a>Als veraltet markierte Befehle

`lxrun.exe` War der erste Befehl, der zum Installieren und Verwalten des Windows-Subsystems für Linux verwendet wurde. Sie ist ab Windows 10 1803 und höher veraltet.

Der Befehl `lxrun.exe` kann verwendet werden, um direkt mit dem [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) zu interagieren.  Diese Befehle werden im `\Windows\System32` Verzeichnis installiert und können in einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.

| Befehl                     | Beschreibung                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | Der lxrun-Befehl wird verwendet, um die WSL-Instanz zu verwalten. |
| `lxrun /install`            | Startet den Download-und Installationsvorgang. <br/> **/y** kann hinzugefügt werden, um alle Eingabe Aufforderungen zu umgehen.  Die Bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer ist auf root festgelegt.          |
| `lxrun /uninstall`          | Deinstalliert und löscht das Ubuntu-Image.  Standardmäßig wird hierdurch nicht das Ubuntu-Basisverzeichnis des Benutzers entfernt. <br/> **/y** kann hinzugefügt werden, um die Bestätigungsaufforderung automatisch zu akzeptieren. <br/>**/Full** deinstalliert und löscht das Ubuntu-Basisverzeichnis des Benutzers.         |
| `lxrun /setdefaultuser <userName>`     | Legt den Standard-bash on Ubuntu-Benutzer fest. Fordert zur Eingabe eines Kennworts auf, wenn der angegebene Benutzer nicht vorhanden ist.  Weitere Informationen finden Sie unter https://aka.ms/wslusers:. <br/> **/y** Umgeht das Kennwort.  Der Benutzer wird ohne Kennwort erstellt.|
| `lxrun /update`            | Aktualisiert den Paket Index des Subsystems.          |
