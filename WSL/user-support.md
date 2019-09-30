---
title: Linux-Benutzerkonto und -Berechtigungen
description: Referenz für Benutzerkonten und Berechtigungsverwaltung mit dem Windows-Subsystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, user accounts
author: scooley
ms.author: scooley
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: de18c128854ef9a39a26551db2ea0aee97b8ab4f
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122685"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a>Benutzerkonten und Berechtigungen für das Windows-Subsystem für Linux

Das Erstellen eines Linux-Benutzers ist der erste Schritt beim Einrichten einer neuen Linux-Distribution unter WSL.  Das erste Benutzerkonto, das Sie erstellen, wird automatisch mit einigen speziellen Attributen konfiguriert:

1. Dies ist der Standardbenutzer, der sich beim Start automatisch anmeldet.
1. Standardmäßig ist dies der Linux-Administrator (Mitglied der Gruppe „sudo“).

Jede Linux-Distribution, die unter dem Windows-Subsystem für Linux ausgeführt wird, verfügt über eigene Linux-Benutzerkonten und -Kennwörter.  Sie müssen ein Linux-Benutzerkonto konfigurieren, wenn Sie eine Distribution hinzufügen, erneut installieren oder zurücksetzen.  Linux-Benutzerkonten sind nicht nur pro Distribution unabhängig, sondern auch von Ihrem Windows-Benutzerkonto unabhängig.

## <a name="resetting-your-linux-password"></a>Zurücksetzen Ihres Linux-Kennworts

Wenn Sie Zugriff auf Ihr Linux-Benutzerkonto haben und Ihr aktuelles Kennwort kennen, ändern Sie es mit den Tools für die Linux-Kennwortzurücksetzung dieser Distribution (höchstwahrscheinlich `passwd`).

Wenn dies nicht möglich ist, können Sie je nach Distribution Ihr Kennwort zurücksetzen, indem Sie den Standardbenutzer zurücksetzen.

WSL bietet ein Standardbenutzertag, um zu ermitteln, welches Benutzerkonto beim Starten einer WSL-Sitzung automatisch angemeldet wird.  Da viele Distributionen Befehle enthalten, um den Standardbenutzer auf „root“ und auch einen root-Benutzer ohne Kennwort festzulegen, ist das Ändern des Standardbenutzers in „root“ eine praktisches Möglichkeit für die Kennwortzurücksetzung.

### <a name="for-creators-update-and-earlier"></a>Creators Update und frühere Versionen
Wenn Sie Windows 10 Creators Update oder eine frühere Version ausführen, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:

1. Ändern Sie den Standardbenutzer in `root`:

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. Führen `bash.exe` Sie aus, um sich jetzt als `root` anzumelden:

    ```console
    C:\> bash.exe
    ```

1. Setzen Sie Ihr Kennwort mit dem Kennwortbefehl der Distribution zurück, und schließen Sie die Linux-Konsole:

    ```BASH
    $ passwd username
    $ exit
    ```

1. Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto:

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a>Fall Creators Update und höhere Versionen
Um anzuzeigen, welche Befehle für eine bestimmte Distribution verfügbar sind, führen Sie `[distro.exe] /?` aus.
    
Beispielsweise bei einer Ubuntu-Installation:

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

Schrittweise Anleitungen für Ubuntu:

1. Öffnen Sie CMD.
1. Legen Sie den Linux -Standardbenutzer auf `root` fest:

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. Starten Sie Ihre Linux-Distribution (`ubuntu`).  Sie werden automatisch als `root` angemeldet:

1. Setzen Sie Ihr Kennwort mit dem Befehl `passwd` zurück:

    ```BASH
    $ passwd username
    ```

1. Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto.

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a>Berechtigungen

Es gibt zwei wichtige Konzepte, die Sie beachten sollten, wenn es um Berechtigungen in WSL geht:

1. Mit dem Windows-Berechtigungsmodell werden die Rechte eines Prozesses für Windows-Ressourcen gesteuert.
2. Mit dem Linux-Berechtigungsmodell werden die Rechte eines Prozesses für Linux-Ressourcen gesteuert.

Bei der Ausführung von Linux unter WSL verfügt Linux über dieselben Windows-Berechtigungen wie der Prozess, der die Anwendung startet. Linux kann mit einer von zwei Berechtigungsstufen gestartet werden:

* Normal (ohne erhöhte Rechte): Linux wird mit den Berechtigungen des angemeldeten Benutzers ausgeführt.
* Erhöhte Rechte/Administrator: Linux wird mit erhöhten Rechten/Windows-Administratorberechtigungen ausgeführt.

> Da Prozesse mit erhöhten Rechten auf systemweite Einstellungen und systemweite/geschützte Daten zugreifen bzw. diese ändern (und dadurch beschädigen) können , sollten Sie es **VERMEIDEN**, erhöhte Prozesse zu starten, es sei denn, dies ist unbedingt erforderlich. Dabei ist es gleichgültig, ob es sich um Windows- oder Linux- Anwendungen/Tools/Shells handelt!

Die oben genannten Windows-Berechtigungen sind unabhängig von den Berechtigungen innerhalb einer Linux-Instanz: „root-Berechtigungen“ von Linux wirken sich nur auf die Rechte des Benutzers in der Linux-Umgebung und im -Dateisystem aus. Sie besitzen keine Auswirkung auf die gewährten Windows-Berechtigungen. Folglich werden durch das Ausführen eines Linux-Prozesses als „root“ ( z.B. über `sudo`) dem Prozess nur die Administratorrechte innerhalb der Linux-Umgebung erteilt.

**Beispiel:**     
Eine Bash-Sitzung mit Windows-Administratorberechtigungen kann auf `cd /mnt/c/Users/Administrator` zugreifen, während in einer Bash-Sitzung ohne Administratorberechtigungen der Fehler „Permission Denied“ (Berechtigung verweigert) angezeigt wird.

Unter Linux gewährt die Eingabe von `sudo cd /mnt/c/Users/Administrator` keinen Zugriff auf das Verzeichnis des Administrators, da Berechtigungen innerhalb von Windows von Windows verwaltet werden.

Das Linux-Berechtigungsmodell ist in der Linux-Umgebung wichtig, wenn der Benutzer über Berechtigungen verfügt, die auf dem aktuellen Linux-Benutzer basieren.

**Beispiel:**  
Ein Benutzer in der Gruppe „sudo“ kann `sudo apt update`ausführen.
