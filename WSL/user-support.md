---
title: Linux-Benutzerkonto und Berechtigungen
description: Referenz für die Benutzer- und berechtigungsverwaltung mit dem Windows-Subsystem für Linux.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Benutzerkonten
author: scooley
ms.author: scooley
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.openlocfilehash: 0d00b43d059e72edd4e2a5b9591c29441f461fca
ms.sourcegitcommit: db69625e26bc141ea379a830790b329e51ed466b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/13/2019
ms.locfileid: "67040825"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a>Benutzerkonten und Berechtigungen für Windows-Subsystem für Linux

Erstellen Ihre Linux-Benutzer ist der erste Schritt zum Einrichten einer neuen Linux-Distribution für WSL.  Das erste Benutzerkonto an, die, das Sie erstellen, wird automatisch mit ein paar spezielle Attribute konfiguriert:

1. Es ist Ihre Standardbenutzer – es meldet sich automatisch beim Start.
1. Linux-Administrator (Mitglied der Gruppe "Sudo") in der Standardeinstellung ist.

Jede Linux-Distribution, die das Windows-Subsystem für Linux unter verfügt über einen eigenen Linux-Benutzerkonten und Kennwörter.  Sie müssen ein Linux-Benutzerkonto jederzeit konfigurieren, Sie fügen eine Verteilung, neu installieren oder zurücksetzen.  Linux-Benutzerkonten sind nicht nur pro Verteilung voneinander unabhängig, sie sind auch unabhängig von Ihrem Windows-Benutzerkonto.

## <a name="resetting-your-linux-password"></a>Zurücksetzen Ihres Kennworts Linux

Wenn Sie Zugriff auf Ihre Linux-Benutzerkonto haben und wissen Ihr aktuelle Kennwort ein, ändern Sie es unter Verwendung von Linux kennwortzurücksetzung Tools dieser Distribution – wahrscheinlich `passwd`.

Wenn dies nicht möglich, je nach der Verteilung ist können Sie zum Zurücksetzen Ihres Kennworts durch Standardbenutzer zurücksetzen können.

WSL bietet, dass ein Standard-Benutzer-Tag, welches Benutzerkonto automatisch zu identifizieren anmeldet, wenn Sie eine WSL starten.  Da viele Verteilungen Befehle zum Festlegen von Standardbenutzer-Stamm und auch als Root-Benutzer mit kein Kennwort festgelegt sind, ist das Ändern der Stamm des Standardbenutzers ein nützliches Tool für Aufgaben wie das Zurücksetzen des Kennworts aus.

### <a name="for-creators-update-and-earlier"></a>Für Creators Update und frühere Versionen
Wenn Sie ausführen, wird Windows 10 Creators update oder haben, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:

1. Ändern den standardmäßigen Benutzer `root`:

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. Führen Sie `bash.exe` , melden Sie sich jetzt als `root`:

    ```console
    C:\> bash.exe
    ```

1. Zurücksetzen Sie des Kennworts, mit der Distribution-Kennwort-Befehl aus, und schließen Sie die Linux-Konsole:

    ```BASH
    $ passwd username
    $ exit
    ```

1. Über Windows-CMD den Standardbenutzer auf Ihre normalen Linux-Benutzerkonto zurückgesetzt werden:

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a>Für den Fall Creators Update und höher
Um festzustellen, welche Befehle für eine bestimmte Verteilung verfügbar sind, führen `[distro.exe] /?`.
    
Z. B. mit Ubuntu installiert:

```console
C:\> ubuntu.exe /?

Launches or configures a linux distribution.

Usage:
    <no args>
      - Launches the distro's default behavior. By default, this launches your default shell.

    run <command line>
      - Run the given command line in that distro, using the default configuration.
      - Everything after `run ` is passed to the linux LaunchProcess cal

    config [setting [value]]
      - Configure certain settings for this distro.
      - Settings are any of the following (by default)
        - `--default-user <username>`: Set the default user for this distro to <username>

    clean
      - Uninstalls the distro. The appx remains on your machine. This can be
        useful for "factory resetting" your instance. This removes the linux
        filesystem from the disk, but not the app from your PC, so you don't
        need to redownload the entire tar.gz again.

    help
      - Print this usage message.
```

Schritt-für-Schritt-Anweisungen, die mit Ubuntu:

1. Open CMD
1. Legen Sie den Standard-Linux-Benutzer auf `root`:

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. Starten Sie Ihre Linux-Distribution (`ubuntu`).  Sie werden automatisch melden Sie sich als `root`:

1. Zurücksetzen, Ihr Kennwort mithilfe der `passwd` Befehl:

    ```BASH
    $ passwd username
    ```

1. Über Windows-CMD wird zurücksetzen Sie den Standardbenutzer auf Ihre normalen Linux-Benutzerkonto.

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a>Berechtigungen

Es gibt zwei wichtige Konzepte zu bedenken, wenn es um die Berechtigungen in WSL geht:

1. Das Windows-Berechtigungsmodell regelt eines Prozesses Rechte für die Windows-Ressourcen
2. Das Linux-Berechtigungsmodell steuert eines Prozesses Rechte für die Linux-Ressourcen

Wenn Linux auf WSL ausführen zu können, müssen Linux die gleichen Windows-Berechtigungen wie der Prozess, das es startet. Linux kann in einem der beiden Berechtigungsstufen gestartet werden:

* Normal (ohne erhöhte Rechte): Linux, die mit den Berechtigungen des angemeldeten Benutzers ausgeführt wird
* Mit erhöhten Rechten/Admin: Linux, die mit erhöhten Windows/Administratorberechtigungen ausgeführt wird

> Da Prozesse mit erhöhten Rechten können Access/ändern (und daher beschädigen) systemweiten Einstellungen und System-Wide/geschützte Daten **vermeiden** Prozesse mit erhöhten Rechten starten, es sei denn, Sie unbedingt, ob sie Windows oder Linux sind Anwendungen/Tools/Shells!

Die oben aufgeführten Windows-Berechtigungen werden unabhängig von Ihren Berechtigungen innerhalb einer Linux-Instanz: Linux "Stammberechtigungen" wirken sich nur auf die Rechte des Benutzers innerhalb des Linux-Umgebung & Filesystem; Sie haben keine Auswirkung auf die Windows-Berechtigungen erteilt. Daher einen Linux-Prozess ausgeführt, als Root-Benutzer (z.B. über die `sudo`) nur gewährt, die über Administratorrechte in der Linux-Umgebung zu verarbeiten.

**Beispiel:**     
Eine Bash-Sitzung mit Administratorrechten für Windows möglicherweise Zugriff auf `cd /mnt/c/Users/Administrator` zwar eine Bash-Sitzung, ohne über Administratorrechte für einen Fehler "Zugriff verweigert" finden Sie unter würde.

Unter Linux eingeben `sudo cd /mnt/c/Users/Administrator` Zugriff auf das Administratorkennwort Verzeichnis wird nicht gewährt werden, da Berechtigungen in Windows, die von Windows verwaltet werden.

Das Linux-Berechtigungsmodell ist wichtig, in die Linux-Umgebung, in denen der Benutzer die Berechtigungen, die basierend auf dem aktuellen Linux-Benutzer verfügt.

**Beispiel:**  
Ein Benutzer in der Gruppe "sudo" ausgeführt `sudo apt update`.
