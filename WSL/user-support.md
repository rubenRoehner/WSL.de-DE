---
title: Linux-Benutzerkonto und-Berechtigungen
description: Referenz für Benutzerkonten und Berechtigungs Verwaltung mit dem Windows-Subsystem für Linux.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Benutzerkonten
author: scooley
ms.author: scooley
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: de18c128854ef9a39a26551db2ea0aee97b8ab4f
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122685"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a>Benutzerkonten und Berechtigungen für das Windows-Subsystem für Linux

Das Erstellen eines Linux-Benutzers ist der erste Schritt beim Einrichten einer neuen Linux-Distribution auf WSL.  Das erste Benutzerkonto, das Sie erstellen, wird automatisch mit einigen speziellen Attributen konfiguriert:

1. Dies ist der Standardbenutzer, der sich beim Start automatisch anmeldet.
1. Standardmäßig ist dies der Linux-Administrator (Mitglied der Gruppe "sudo").

Jede Linux-Distribution, die unter dem Windows-Subsystem für Linux ausgeführt wird, verfügt über eigene Linux-Benutzerkonten und Kenn Wörter.  Sie müssen ein Linux-Benutzerkonto konfigurieren, wenn Sie eine Verteilung hinzufügen, neu installieren oder zurücksetzen.  Linux-Benutzerkonten sind nicht nur pro Verteilung unabhängig, sondern auch unabhängig von Ihrem Windows-Benutzerkonto.

## <a name="resetting-your-linux-password"></a>Zurücksetzen Ihres Linux-Kennworts

Wenn Sie Zugriff auf Ihr Linux-Benutzerkonto haben und Ihr aktuelles Kennwort kennen, ändern Sie es mit den Tools für die Linux-Kenn Wort `passwd`Zurücksetzung dieser Verteilung (höchstwahrscheinlich).

Wenn dies nicht möglich ist, können Sie je nach Verteilung Ihr Kennwort zurücksetzen, indem Sie den Standardbenutzer zurücksetzen.

WSL bietet ein Standard Benutzertag, um zu ermitteln, welches Benutzerkonto beim Starten eines WSL automatisch angemeldet wird.  Da viele Verteilungen Befehle enthalten, um den Standardbenutzer auf root festzulegen, und auch ein root-Benutzer ohne Kennwort festgelegt ist, ist das Ändern des Standard Benutzers in root ein praktisches Tool für die Kenn Wort Zurücksetzung.

### <a name="for-creators-update-and-earlier"></a>Für Creators Update und früher
Wenn Sie Windows 10 Creators Update oder eine frühere Version ausführen, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:

1. Ändern Sie den Standardbenutzer `root`in:

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. Führen `bash.exe` Sie aus, um `root`sich jetzt als anzumelden:

    ```console
    C:\> bash.exe
    ```

1. Setzen Sie Ihr Kennwort mit dem Kenn Wort Befehl der Verteilung zurück, und schließen Sie die Linux-Konsole:

    ```BASH
    $ passwd username
    $ exit
    ```

1. Setzen Sie Ihren Standardbenutzer von Windows CMD zurück auf Ihr normales Linux-Benutzerkonto:

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a>Für Fall Creators Update und höher
Um anzuzeigen, welche Befehle für eine bestimmte Verteilung verfügbar sind, `[distro.exe] /?`führen Sie aus.
    
Beispielsweise bei installiertem Ubuntu:

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

Schritt-für-Schritt-Anleitungen unter Verwendung von Ubuntu:

1. Cmd öffnen
1. Legen Sie den Standard-Linux `root`-Benutzer auf fest:

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. Starten Sie Ihre Linux-`ubuntu`Distribution ().  Sie werden automatisch wie `root`folgt anmelden:

1. Setzen Sie Ihr Kennwort `passwd` mit dem folgenden Befehl zurück:

    ```BASH
    $ passwd username
    ```

1. Setzen Sie Ihren Standardbenutzer von Windows cmd auf Ihr normales Linux-Benutzerkonto zurück.

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a>Berechtigungen

Es gibt zwei wichtige Konzepte, die Sie beachten sollten, wenn es um Berechtigungen in WSL geht:

1. Mit dem Windows-Berechtigungs Modell wird eine Prozess Berechtigung für Windows-Ressourcen geregelt.
2. Das Linux-Berechtigungs Modell steuert die Rechte eines Prozesses für Linux-Ressourcen.

Bei der Ausführung von Linux auf WSL hat Linux dieselben Windows-Berechtigungen wie der Prozess, von dem die Anwendung gestartet wird. Linux kann mit einer von zwei Berechtigungsstufen gestartet werden:

* Normal (ohne erhöhte Rechte): Linux wird mit den Berechtigungen des angemeldeten Benutzers ausgeführt.
* Erhöht/admin: Linux wird mit erhöhten/Administrator-Windows-Berechtigungen ausgeführt.

> Da erweiterte Prozesse auf systemweite Einstellungen und systemweite/geschützte Daten zugreifen bzw. diese ändern (und dadurch beschädigen) können, **vermeiden** Sie das Starten von erweiterten Prozessen, es sei denn, Sie müssen unbedingt die Windows-oder Linux-Anwendungen/Tools/ Bomben!

Die obigen Windows-Berechtigungen sind unabhängig von den Berechtigungen innerhalb einer Linux-Instanz: Linux-"Root-Berechtigungen" wirken sich nur auf die Rechte des Benutzers in der Linux-Umgebung & File System aus; Sie haben keine Auswirkung auf die gewährten Windows-Berechtigungen. Folglich werden durch das Ausführen eines Linux-Prozesses als Stamm ( `sudo`z. b. via) nur die Administratorrechte innerhalb der Linux-Umgebung erteilt.

**Beispiel:**     
Eine bash-Sitzung mit Windows-Administrator Berechtigungen `cd /mnt/c/Users/Administrator` kann auf zugreifen, während einer bash-Sitzung ohne Administratorrechte der Fehler "Berechtigung verweigert" angezeigt wird.

Unter Linux gewährt die `sudo cd /mnt/c/Users/Administrator` Eingabe keinen Zugriff auf das Administrator Verzeichnis, da Berechtigungen in Windows von Windows verwaltet werden.

Das Linux-Berechtigungs Modell ist wichtig, wenn der Benutzer in der Linux-Umgebung über Berechtigungen verfügt, die auf dem aktuellen Linux-Benutzer basiert.

**Beispiel:**  
Ein Benutzer in der sudo-Gruppe kann `sudo apt update`ausführen.
