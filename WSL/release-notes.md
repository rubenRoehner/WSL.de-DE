---
title: Versions Hinweise für das Windows-Subsystem für Linux
description: Versions Hinweise für das Windows-Subsystem für Linux.  Wöchentlich aktualisiert.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu
author: benhillis
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 36ea641e-4d49-4881-84eb-a9ca85b1cdf4
ms.custom: seodec18
ms.openlocfilehash: b03d837e0ab3a371fd676e37b5c65a173824f84c
ms.sourcegitcommit: 9175a28f04573f25338358faf61d73b1a5d1ade6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "68832117"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a>Versions Hinweise für das Windows-Subsystem für Linux


## <a name="build-18945"></a>Build 18945
Allgemeine Windows-Informationen zu Build 18945 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).

### <a name="wsl"></a>WSL
* [WSL2] Ermöglicht den Zugriff auf das lauschen von TCP-Sockets in WSL2 über den Host mithilfe von "localhost: Port".
* [WSL2] Fehlerbehebungen für Installations-und Konvertierungs Fehler und zusätzliche Diagnose zur Verfolgung zukünftiger Probleme [GH 4105] 
* [WSL2] Verbessern der Diagnose von Netzwerkproblemen WSL2
* [WSL2] Kernel Version auf 4.19.55 aktualisieren
* [WSL2] Aktualisieren des Kernels mit Konfigurationsoptionen, die für docker erforderlich sind [GH 4165]
* [WSL2] Erhöhen Sie die Anzahl der CPUs, die dem Lightweight-Hilfsprogramm-VM zugewiesen sind, damit Sie mit dem Host identisch ist (zuvor auf 8 durch CONFIG_NR_CPUS in der Kernelkonfiguration begrenzt) [GH 4137]
* [WSL2] Erstellen einer Auslagerungs Datei für die WSL2-Lightweight-VM
* [WSL2] Zulassen, dass Benutzer Bereitstellungen über \\ \\WSL $\\Distribution (z. b. sshfs) sichtbar sind [GH 4172]
* [WSL2] Verbessern der Systemleistung von 9P
* [WSL2] Sicherstellen, dass die VHD-ACL nicht unbegrenzt wächst [GH 4126]
* [WSL2] Aktualisieren der Kernelkonfiguration zur Unterstützung von "squashfs" und "xt_conntrack" [GH 4107, 4123]
* [WSL2] Behebung für Interop. aktivierte/etc/WSL.conf Option [GH 4140]
* [WSL2] Rückgabe von "umotsup", wenn das Dateisystem EAS nicht unterstützt
* [WSL2] Korrigieren von CopyFile- \\hängen mit \\WSL $
* Standard umask in 0022 umschalten und File System. umask-Einstellung zu/etc/WSL.conf hinzufügen
* Korrigieren von wslpath, um symlinks ordnungsgemäß aufzulösen, dies wurde in 19h1 zurückgegangen [GH 4078]
* Führen Sie die Datei "\\% User Profile%. wslconfig" für die Optimierung der WSL2-Einstellungen ein.
```
[wsl2]
kernel=<path>              # An absolute Windows path to a custom Linux kernel.
memory=<size>              # How much memory to assign to the WSL2 VM.
processors=<number>        # How many processors to assign to the WSL2 VM.
swap=<size>                # How much swap space to add to the WSL2 VM. 0 for no swap file.
swapFile=<path>            # An absolute Windows path to the swap vhd.
localhostForwarding=<bool> # Boolean specifying if ports bound to wildcard or localhost in the WSL2 VM should be connectable from the host via localhost:port (default true).

# <path> entries must be absolute Windows paths with escaped backslashes, for example C:\\Users\\Ben\\kernel
# <size> entries must be size followed by unit, for example 8GB or 512MB
```

## <a name="build-18917"></a>Build 18917
Allgemeine Windows-Informationen zu Build 18917 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).

### <a name="wsl"></a>WSL
* WSL 2 ist jetzt verfügbar! Weitere Informationen finden Sie im [Blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) .
* Korrektur einer Regression, bei der das Starten von Windows-Prozessen über symlinks nicht ordnungsgemäß funktioniert hat [GH 3999]
* Fügen Sie die Optionen "WSL. exe--list--Verbose", "WSL. exe--list--quiet" und "WSL. exe--Import--Version" zu "WSL. exe" hinzu.
* Add WSL. exe--Option zum Herunterfahren
* Plan 9: Das Öffnen eines Verzeichnisses für einen erfolgreichen Schreibvorgang zulassen

## <a name="build-18890"></a>Build 18890
Allgemeine Windows-Informationen zu Build 18890 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).

### <a name="wsl"></a>WSL
* Nicht blockierender socketleck [GH 2913]
* EOF-Eingabe zum Terminal kann nachfolgende Lesevorgänge blockieren [GH 3421]
* Aktualisieren Sie den resolv. conf-Header so, dass er auf WSL. conf verweist [in GH 3928 erläutert].
* Deadlock im epoll-Lösch Code [GH 3922]
* Behandeln von Leerzeichen in Argumenten für "--Import" und "– Export" [GH 3932]
* Erweitern von mmap-'d-Dateien funktioniert nicht ordnungsgemäß [GH 3939]
* Beheben von Problemen mit \\ARM64 WSL $ Access funktioniert nicht ordnungsgemäß
* Besseres Standard Symbol für "WSL. exe" hinzufügen

## <a name="build-18342"></a>Build 18342
Allgemeine Windows-Informationen zu Build 18342 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).

### <a name="wsl"></a>WSL
* Wir haben Benutzern die Möglichkeit hinzugefügt, auf Linux-Dateien in einer WSL-Distribution von Windows zuzugreifen. Auf diese Dateien kann über die Befehlszeile zugegriffen werden. Außerdem können Windows-apps wie der Datei-Explorer, vscode usw. mit diesen Dateien interagieren. Greifen Sie auf Ihre Dateien zu \\, indem Sie\\zu \\WSL $ < distro_name > navigieren, oder zeigen Sie eine Liste \\der laufenden Distributionen an, indem Sie zu \\WSL $ navigieren
* Hinzufügen zusätzlicher CPU-Infotags und korrigieren der Cpus_allowed [_list]-Werte [GH 2234]
* Unterstützung von exec von einem nicht-führenden Thread [GH 3800]
* Behandeln von Fehlern bei der Konfigurations Aktualisierung als nicht schwerwiegend [GH 3785]
* Aktualisieren von binfmt, damit Offsets ordnungsgemäß behandelt werden [GH 3768]
* Aktivieren der Zuordnung von Netzwerklaufwerken für Plan 9 [GH 3854]
* Unterstützung von Windows-> Linux-und Linux-> Windows-Pfad Übersetzung für Bindungs Zustellungen
* Erstellen Sie schreibgeschützte Abschnitte für Zuordnungen in Dateien, die schreibgeschützt geöffnet sind.

## <a name="build-18334"></a>Build 18334
Allgemeine Windows-Informationen zu Build 18334 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).

### <a name="wsl"></a>WSL
* Umgestalten der Art und Weise, in der die Windows-Zeitzone einer Linux-Zeitzone zugeordnet ist [GH 3747]
* Beheben von Speicher Verlusten und Hinzufügen neuer Zeichen folgen Übersetzungsfunktionen [GH 3746]
* Sigmt für eine Thread Gruppe ohne Threads ist ein No-op [GH 3741] 
* Korrekter Anzeige von Socket-und epoll-Dateideskriptoren in/proc/self/fd

## <a name="build-18305"></a>Build 18305
Allgemeine Windows-Informationen zu Build 18305 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).

### <a name="wsl"></a>WSL
* pthreads verlieren den Zugriff auf Dateien, wenn der primäre Thread beendet wird [GH 3589]
* "Tiocsctty" sollte den "Force"-Parameter ignorieren, es sei denn, er ist erforderlich [GH 3652]
* Verbesserungen an der Befehlszeile von WSL. exe und zusätzliche Import-/Exportfunktionen.
```
Usage: wsl.exe [Argument] [Options...] [CommandLine]

Arguments to run Linux binaries:

    If no command line is provided, wsl.exe launches the default shell.

    --exec, -e <CommandLine>
        Execute the specified command without using the default Linux shell.

    --
        Pass the remaining command line as is.

Options:
    --distribution, -d <DistributionName>
        Run the specified distribution.

    --user, -u <UserName>
        Run as the specified user.

Arguments to manage Windows Subsystem for Linux:

    --export <DistributionName> <FileName>
        Exports the distribution to a tar file.
        The filename can be - for standard output.

    --import <DistributionName> <InstallLocation> <FileName>
        Imports the specified tar file as a new distribution.
        The filename can be - for standard input.

    --list, -l [Options]
        Lists distributions.

        Options:
            --all
                List all distributions, including distributions that are currently
                being installed or uninstalled.

            --running
                List only distributions that are currently running.

    -setdefault, -s <DistributionName>
        Sets the distribution as the default.

    --terminate, -t <DistributionName>
        Terminates the distribution.

    --unregister <DistributionName>
        Unregisters the distribution.

    --upgrade <DistributionName>
        Upgrades the distribution to the WslFs file system format.

    --help
        Display usage information.
```

## <a name="build-18277"></a>Build 18277
Allgemeine Windows-Informationen zu Build 18277 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).

### <a name="wsl"></a>WSL
* Fehlerbehebung "keine solche Schnittstelle unterstützt" in Build 18272 [GH 3645] eingeführt
* MNT_FORCE-Flag für aufheben syscall ignorieren [GH 3605]
* Wechseln von WSL-Interop zur Verwendung der offiziellen "deepseudoconsole"-API
* Keinen Timeout Wert beibehalten, wenn FUTEX_WAIT neu gestartet wird

## <a name="build-18272"></a>Build 18272
Allgemeine Windows-Informationen zu Build 18272 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).

### <a name="wsl"></a>WSL
* **DAVOR** In diesem Build ist ein Problem aufgetreten, das WSL als nicht funktionsfähig macht. Wenn Sie versuchen, die Distribution zu starten, wird die Fehlermeldung "Es wird keine solche Schnittstelle unterstützt" angezeigt. Das Problem wurde behoben und ist der Insider-schnell Build der nächsten Woche. Wenn Sie diesen Build installiert haben, können Sie ein Rollback auf den vorherigen Windows-Build durchführen, indem Sie unter "Einstellungen-> Update & Sicherheit > Wiederherstellung" zurück zur vorherigen Version von Windows 10 wechseln.

## <a name="build-18267"></a>Build 18267
Allgemeine Windows-Informationen zu Build 18267 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).

### <a name="wsl"></a>WSL
* Behebung eines Problems, bei dem der Zombie Prozess möglicherweise nicht wiederholt wird und unbegrenzt bleibt.
* Wslregisterdistribution hängt ab, wenn die Fehlermeldung die maximale Länge überschreitet [GH 3592]
* Zulassen der erfolgreichen Ausführung von fsync für schreibgeschützte Dateien auf drvfs [GH 3556]
* Stellen Sie sicher, dass die Verzeichnisse "/bin" und/sbin vorhanden sind, bevor Sie symlinks in [GH 3584] erstellen
* Es wurde ein Timeout Mechanismus für Instanzen Beendigung für WSL-Instanzen hinzugefügt. Der Timeout Wert ist derzeit auf 15 Sekunden festgelegt. das bedeutet, dass die Instanz 15 Sekunden nach Beendigung des letzten WSL-Prozesses beendet wird. Um eine Verteilung sofort zu beenden, verwenden Sie Folgendes:
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a>Build 17763 (1809)
Allgemeine Windows-Informationen zu Build 17763 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).

### <a name="wsl"></a>WSL
* Die SetPriority-syscall-Berechtigung zum Ändern der gleichen Thread Priorität ist zu streng. [GH 1838]
* Stellen Sie sicher, dass eine unausgewogene Interruptzeit für die Startzeit verwendet wird, um die Rückgabe negativer Werte für clock_gettime (CLOCK_BOOTTIME) zu vermeiden. [GH 3434]
* Behandeln von Symlinks im WSL binf-Interpreter [GH 3424]
* Bessere Behandlung der Bereinigung der Thread Gruppen-Dateideskriptoren.
* Wechseln von WSL zur Verwendung von kequeryinterrupttimepräzisen anstelle von KeQueryPerformanceCounter, um einen Überlauf zu vermeiden [GH 3252]
* Ptrace-Anfüge Vorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]
* Beheben mehrerer AF_UNIX bezogener Probleme [GH 3371]
* Behebung eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]
* Vermeiden einer Sekunde verzögert fehlerhafte Loopback Verbindungen mit nicht vorhandenen Ports [GH 3286]
* /Proc/sys/FS/File-Max Stub-Datei hinzufügen [GH 2893]
* Genauere IPv6-Bereichs Informationen.
* PR_SET_PTRACER-Unterstützung [GH 3053]
* Pipe-Dateisystem versehentlich Löschen eines Edge-ausgelösten epoll-Ereignisses [GH 3276]
* Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen
* Verbesserte Zombie Unterstützung [GH 1353]
* Hinzufügen von WSL. conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* Behebung für "getsockname" gibt nicht immer den UNIX-socketfamilientyp [GH 1774] zurück.
* Hinzufügen von Unterstützung für tiocsti [GH 1863]
* Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche "eagain" zurückgeben [GH 2846]
* Unterstützung von Interop auf bereitgestellten VHDs [GH 3246, 3291]
* Beheben von Problemen mit der Berechtigungsüberprüfung im Stamm Ordner [GH 3304]
* Eingeschränkte Unterstützung für die TTY-Tastatur IOCTLs kdgkbtype, kdgkbmode und kdskbmode.
* Windows-Benutzeroberflächen-apps sollten ausgeführt werden, auch wenn Sie im Hintergrund gestartet werden.
* Add WSL-u oder--User-Option [GH 1203]
* Beheben von WSL-Startproblemen, wenn der schnelle Start aktiviert ist [GH 2576]
* Unix-Sockets müssen getrennte Peer-Anmelde Informationen beibehalten [GH 3183]
* Nicht blockierende Unix-Sockets, die unbegrenzt mit eagain auftreten [GH 3191]
* Case = off ist der neue standardmäßige drvfs-Einstellungstyp [GH 2937, 3212, 3328]
    * Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) .
* Fügen Sie wslconfig/Terminate hinzu, um die Ausführung von Verteilungen anzuhalten
* Beheben Sie das Problem mit den Kontextmenü Einträgen von WSL Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.
* Stellen Sie die Groß-/Kleinschreibung nach Verzeichnis als erweitertes Attribut bereit.
* ARM64 Emulieren von Cache Wartungs Vorgängen. Beheben von [dotnet-Problemen](https://github.com/dotnet/core/issues/1561).
* Drvfs: nur Escapezeichen im privaten Bereich, die einem Escapezeichen entsprechen.
* Fehlerbehebung bei einem Fehler in der Überprüfung der Länge des elf-parserinterpreters [GH 3154]
* Absolute WSL-Timer mit einer Zeit in der Vergangenheit werden nicht ausgelöst [GH 3091]
* Stellen Sie sicher, dass neu erstellte Analyse Punkte als solche im übergeordneten Verzeichnis aufgelistet werden.
* Erstellen Sie in drvfs atomarisch Fälle mit Berücksichtigung von Groß-und klein
* Es wurde ein zusätzliches Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist. [GH 2712]
* Fehler beim Starten des WSL-Starts, wenn die Option "-Konfigurations- [GH 3020]
* Fügen Sie den Explorer-Kontextmenü zum Starten von WSL [GH 437, 603, 1836] hinzu. Halten Sie die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, wenn Sie in einem Explorer-Fenster
* Korrigieren des nicht blockierenden UNIX-socketverhaltens [GH 2822, 3100]
* Korrigieren Sie den hängenden NetLink-Befehl, wie in GH 2026 gemeldet.
* Unterstützung für einstellungsweitergabeflags [GH 2911] hinzufügen
* Beheben von Problemen mit TRUNCATE, die keine inotify-Ereignisse verursachen [GH 2978].
* Fügen Sie die Option "--exec" für WSL. exe ein, um eine einzelne Binärdatei ohne Shell aufzurufen.
* Fügen Sie die Option "--Distribution" für "WSL. exe" hinzu, um eine bestimmte Distribution auszuwählen.
* Eingeschränkte Unterstützung für dmesg. Anwendungen können sich jetzt an dmesg anmelden. Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg. In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnosen vom Treiber übertragen werden.
    * Hinweis: dmesg wird derzeit über die `/dev/kmsg` Geräteschnittstelle unterstützt. `syslog`Die syscall-Schnittstelle wird noch nicht unterstützt. Und daher funktionieren einige `dmesg` der Befehlszeilenoptionen `-S`, wie z. b `-C` ., nicht.
* Ändern der Standard-gid und des Modus von seriellen Geräten entsprechend der systemeigenen [GH 3042]
* Drvfs unterstützt jetzt erweiterte Attribute.
    * Hinweis: Bei drvfs gelten einige Einschränkungen für den Namen erweiterter Attribute. Einige Zeichen (z. b. "/", ":\*" und "") sind nicht zulässig, und erweiterte Attributnamen werden bei drvfs nicht groß-und Kleinschreibung beachtet.

## <a name="build-18252-skip-ahead"></a>Build 18252 (überspringen)
Allgemeine Windows-Informationen zu Build 18252 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).

### <a name="wsl"></a>WSL
* Verschieben von init-und bsdtar-Binärdateien aus der lxssmanager-dll und in einen separaten Tool Ordner
* Korrektur des raceumschließens des Datei Deskriptors bei Verwendung von CLONE_FILES
* Behandeln optionaler Felder in/proc/PID/mountinfo bei der Übersetzung von drvfs-Pfaden
* Zulassen, dass drvfs-mklod ohne Metadatenunterstützung für S_IFREG erfolgreich ist
* Für schreibgeschützte Dateien, die auf drvfs erstellt wurden, muss das schreibgeschützte Attribut festgelegt werden [GH 3411]
* Hinzufügen von/sbin/mount.drvfs Helper zur Behandlung der drvfs-Einbindung
* Verwenden Sie die POSIX-Umbenennung in drvfs.
* Ermöglicht die Pfad Übersetzung auf Volumes ohne Volume-GUID.

## <a name="build-17738-fast"></a>Build 17738 (fast)
Allgemeine Windows-Informationen zu Build 17738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).

### <a name="wsl"></a>WSL
* Die SetPriority-syscall-Berechtigung zum Ändern der gleichen Thread Priorität ist zu streng. [GH 1838]
* Stellen Sie sicher, dass eine unausgewogene Interruptzeit für die Startzeit verwendet wird, um die Rückgabe negativer Werte für clock_gettime (CLOCK_BOOTTIME) zu vermeiden. [GH 3434]
* Behandeln von Symlinks im WSL binf-Interpreter [GH 3424]
* Bessere Behandlung der Bereinigung der Thread Gruppen-Dateideskriptoren.

## <a name="build-17728-fast"></a>Build 17728 (fast)
Allgemeine Windows-Informationen zu Build 17728 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).

### <a name="wsl"></a>WSL
* Wechseln von WSL zur Verwendung von kequeryinterrupttimepräzisen anstelle von KeQueryPerformanceCounter, um einen Überlauf zu vermeiden [GH 3252]
* Ptrace-Anfüge Vorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]
* Beheben einer Reihe von AF_UNIX-bezogenen Problemen [GH 3371]
* Behebung eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]

## <a name="build-18204-skip-ahead"></a>Build 18204 (überspringen)
Allgemeine Windows-Informationen zu Build 18204 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).

### <a name="wsl"></a>WSL
* Pipe-Dateisystem versehentlich löschen von Edge-ausgelösten epoll-Ereignissen [GH 3276]
* Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen

## <a name="build-17723-fast"></a>Build 17723 (fast)
Allgemeine Windows-Informationen zu Build 17723 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).

### <a name="wsl"></a>WSL
* Vermeiden einer Sekunde verzögert fehlerhafte Loopback Verbindungen mit nicht vorhandenen Ports [GH 3286]
* /Proc/sys/FS/File-Max Stub-Datei hinzufügen [GH 2893]
* Genauere IPv6-Bereichs Informationen.
* PR_SET_PTRACER-Unterstützung [GH 3053]
* Pipe-Dateisystem versehentlich löschen von Edge-ausgelösten epoll-Ereignissen [GH 3276]
* Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen

## <a name="build-17713"></a>Build 17713
Allgemeine Windows-Informationen zu Build 17713 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).

### <a name="wsl"></a>WSL
* Verbesserte Zombie Unterstützung [GH 1353]
* Hinzufügen von WSL. conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* Behebung für "getsockname" gibt nicht immer den UNIX-socketfamilientyp [GH 1774] zurück.
* Hinzufügen von Unterstützung für tiocsti [GH 1863]
* Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche "eagain" zurückgeben [GH 2846]
* Unterstützung von Interop auf bereitgestellten VHDs [GH 3246, 3291]
* Beheben von Problemen mit der Berechtigungsüberprüfung im Stamm Ordner [GH 3304]
* Eingeschränkte Unterstützung für die TTY-Tastatur IOCTLs kdgkbtype, kdgkbmode und kdskbmode.
* Windows-Benutzeroberflächen-apps sollten ausgeführt werden, auch wenn Sie im Hintergrund gestartet werden.

## <a name="build-17704"></a>Build 17704
Allgemeine Windows-Informationen zu Build 17704 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).

### <a name="wsl"></a>WSL
* Add WSL-u oder--User-Option [GH 1203]
* Beheben von WSL-Startproblemen, wenn der schnelle Start aktiviert ist [GH 2576]
* Unix-Sockets müssen getrennte Peer-Anmelde Informationen beibehalten [GH 3183]
* Nicht blockierende Unix-Sockets, die unbegrenzt mit eagain auftreten [GH 3191]
* Case = off ist der neue standardmäßige drvfs-Einstellungstyp [GH 2937, 3212, 3328]
    * Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) .
* Fügen Sie wslconfig/Terminate hinzu, um die Ausführung von Verteilungen anzuhalten

## <a name="build-17692"></a>Build 17692
Allgemeine Windows-Informationen zu Build 17692 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).

### <a name="wsl"></a>WSL
* Beheben Sie das Problem mit den Kontextmenü Einträgen von WSL Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.
* Stellen Sie die Groß-/Kleinschreibung nach Verzeichnis als erweitertes Attribut bereit.
* ARM64 Emulieren von Cache Wartungs Vorgängen. Beheben von [dotnet-Problemen](https://github.com/dotnet/core/issues/1561).
* Drvfs: nur Escapezeichen im privaten Bereich, die einem Escapezeichen entsprechen.

## <a name="build-17686"></a>Build 17686
Allgemeine Windows-Informationen zu Build 17686 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).

### <a name="wsl"></a>WSL
* Fehlerbehebung bei einem Fehler in der Überprüfung der Länge des elf-parserinterpreters [GH 3154]
* Absolute WSL-Timer mit einer Zeit in der Vergangenheit werden nicht ausgelöst [GH 3091]
* Stellen Sie sicher, dass neu erstellte Analyse Punkte als solche im übergeordneten Verzeichnis aufgelistet werden.
* Erstellen Sie in drvfs atomarisch Fälle mit Berücksichtigung von Groß-und klein

## <a name="build-17677"></a>Build 17677
Allgemeine Windows-Informationen zu Build 17677 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).

### <a name="wsl"></a>WSL
* Es wurde ein zusätzliches Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist. [GH 2712]
* Fehler beim Starten des WSL-Starts, wenn die Option "-Konfigurations- [GH 3020]

## <a name="build-17666"></a>Build 17666
Allgemeine Windows-Informationen zu Build 17666 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).

### <a name="wsl"></a>WSL
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a>WARNUNG: Es gibt ein Problem, das das Ausführen von WSL in einigen AMD-Chipsätzen [GH 3134] verhindert. Ein Fix ist bereit und stellt den Insider-Build-Branch dar.
* Fügen Sie den Explorer-Kontextmenü zum Starten von WSL [GH 437, 603, 1836] hinzu. , Wenn Sie die Halt-Umschalttaste verwenden möchten, und klicken Sie mit der rechten Maustaste auf den
* Korrigieren des nicht blockierenden UNIX-socketverhaltens [GH 2822, 3100]
* Korrigieren Sie den hängenden NetLink-Befehl, wie in GH 2026 gemeldet.
* Unterstützung für einstellungsweitergabeflags [GH 2911] hinzufügen
* Beheben von Problemen mit TRUNCATE, die keine inotify-Ereignisse verursachen [GH 2978].
* Fügen Sie die Option "--exec" für WSL. exe ein, um eine einzelne Binärdatei ohne Shell aufzurufen.
* Fügen Sie die Option "--Distribution" für "WSL. exe" hinzu, um eine bestimmte Distribution auszuwählen.

## <a name="build-17655-skip-ahead"></a>Build 17655 (überspringen)
Allgemeine Windows-Informationen zu Build 17655 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Eingeschränkte Unterstützung für dmesg. Anwendungen können sich jetzt an dmesg anmelden. Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg. In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnosen vom Treiber übertragen werden.
    * Hinweis: dmesg wird derzeit über die `/dev/kmsg` Geräteschnittstelle unterstützt. `syslog`die sycallcenter-Schnittstelle wird noch nicht unterstützt. Und daher funktionieren einige `dmesg` der Befehlszeilenoptionen `-S`, wie z. b `-C` ., nicht.
* Es wurde ein Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist. [GH 2712]

## <a name="build-17639-skip-ahead"></a>Build 17639 (überspringen)
Allgemeine Windows-Informationen zu Build 17639 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Ändern der Standard-gid und des Modus von seriellen Geräten entsprechend der systemeigenen [GH 3042]
* Drvfs unterstützt jetzt erweiterte Attribute.
    * Hinweis: Bei drvfs gelten einige Einschränkungen für den Namen erweiterter Attribute. Bestimmte Zeichen (z. b. "/", ":" und "\*") sind nicht zulässig, und erweiterte Attributnamen werden bei drvfs nicht Groß-/Kleinschreibung unterschieden.

## <a name="build-17133-fast"></a>Build 17133 (fast)
Allgemeine Windows-Informationen zu Build 17133 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).

### <a name="wsl"></a>WSL
* Fehlerbehebung für den Absturz in WSL. [GH 3039, 3034]

## <a name="build-17128-fast"></a>Build 17128 (fast)
Allgemeine Windows-Informationen zu Build 17128 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).

### <a name="wsl"></a>WSL
* Keine

## <a name="build-17627-skip-ahead"></a>Build 17627 (überspringen)
Allgemeine Windows-Informationen zu Build 17627 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Unterstützung für die Futex-Pi-fähigen Vorgänge hinzufügen. [GH 1006]
    * Beachten Sie, dass es sich bei den Prioritäten derzeit nicht um eine unterstützte WSL-Funktion handelt, sodass die Blockierung der Standard Auslastung aufgehoben werden muss.
* Windows-Firewall-Unterstützung für WSL-Prozesse. [GH 1852]
    * Um beispielsweise zuzulassen, dass der WSL-python-Prozess an einem beliebigen Port lauschen kann, verwenden Sie das Windows-cmd mit erhöhten Rechten:```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```
    * Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)
* Beachten Sie die Standardshell des Benutzers bei der Verwendung von WSL. exe. [GH 2372]
* Alle Netzwerkschnittstellen als Ethernet melden. [GH 2996]
* Bessere Behandlung von beschädigten "/etc/passwd"-Dateien. [GH 3001]

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17618-skip-ahead"></a>Build 17618 (überspringen)
Allgemeine Windows-Informationen zu Build 17618 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).

### <a name="wsl"></a>WSL
* Einführung in pseudoconsole-Funktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].
* Der Legacy Installationsmechanismus (lxrun. exe) ist veraltet. Der unterstützte Mechanismus zum Installieren von Verteilungen ist die Microsoft Store.

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17110"></a>Build 17110
Allgemeine Windows-Informationen zu Build 17110 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).

### <a name="wsl"></a>WSL
* Zulassen, dass/init von Windows [GH 2928] beendet wird.
* Drvfs verwendet standardmäßig die Groß-/Kleinschreibung nach Groß-/Kleinschreibung (entspricht der Bereitstellungsoption "Case = dir").
    * Wenn Sie "Case = Force" verwenden (das alte Verhalten), muss ein Registrierungsschlüssel festgelegt werden. Führen Sie den folgenden Befehl aus, um "Case = Force" zu aktivieren, wenn Sie ihn verwenden müssen: reg Add hklm\system\currentcontrolset\services\lxss/v drvfsallowforcecasesensitivity/t REG_DWORD/d 1
    * Wenn Sie über vorhandene Verzeichnisse verfügen, die in einer älteren Version von Windows mit WSL erstellt wurden, bei denen die Groß-/Kleinschreibung beachtet werden muss, verwenden Sie "fsutil. exe", um Sie als Unterscheidung <path> nach Groß-/Kleinschreibung zu kennzeichnen.
* NULL-Beendigungs Zeichenfolgen werden von uname syscall zurückgegeben.

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17107"></a>Build 17107
Allgemeine Windows-Informationen zu Build 17107 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).

### <a name="wsl"></a>WSL
* Unterstützung von tcot TSF und tccot auf den Master-Pty-Endpunkten [GH 2552].
* Das Starten von gleichzeitigen Interop-Prozessen kann zu "Inval [GH 2813]" führen.
* Korrigieren Sie PTRACE_ATTACH, um den richtigen Ablauf verfolgungsstatus in/proc/PID/Status. anzuzeigen.
* Korrektur des Race, bei dem kurzlebige Prozesse, die mit dem cleartid-und dem Abgleich-Flags geklont wurden, ohne Löschen der TID-Adresse beendet werden könnten
* Anzeigen einer Meldung beim Aktualisieren der Linux-Dateisystem Verzeichnisse beim Umstieg von einem Pre-17093-Build. Weitere Informationen zu den Änderungen des 17093-Dateisystems finden Sie in den Anmerkungen zu dieser Version von [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17101"></a>Build 17101
Allgemeine Windows-Informationen zu Build 17101 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).

### <a name="wsl"></a>WSL
* Unterstützung für signalfd. [GH 129]
* Unterstützung von Dateinamen, die ungültige NTFS-Zeichen enthalten, durch Codieren als private Unicode-Zeichen. [GH 1514]
* Das automatische einbinden wird auf schreibgeschützt zurückgreifen, wenn Schreibvorgänge nicht unterstützt werden. [GH 2603]
* Ermöglicht das Einfügen von Unicode-Ersatz Zeichen Paaren (z. b. Emoji-Zeichen). [GH 2765]
* Pseudo Dateien in/proc und/sys sollten Lese-und Schreibvorgänge aus SELECT, Abruf, epoll, et al. [GH 2838] zurückgeben.
* Beheben Sie Probleme, die dazu führen könnten, dass der Dienst in eine Endlosschleife wechselt, wenn die Registrierung manipuliert wurde oder beschädigt ist.
* Korrigieren Sie Netlink-Nachrichten, sodass Sie mit neueren Versionen von iproute2 (Upstream 4,14) funktionieren.

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17093"></a>Build 17093
Allgemeine Windows-Informationen zu Build 17093 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).

#### <a name="important"></a>Wichtig:
Wenn Sie WSL zum ersten Mal nach dem Upgrade auf diesen Build starten, müssen Sie einige Aufgaben durchführen, um die Linux-Dateisystem Verzeichnisse zu aktualisieren. Dieser Vorgang kann einige Minuten in Anspruch nehmen, sodass WSL möglicherweise langsam gestartet wird. Dies sollte nur einmal für jede Distribution erfolgen, die Sie aus dem Speicher installiert haben.
* Verbesserte Unterscheidung nach Groß-/Kleinschreibung in drvfs.
    * Drvfs unterstützt jetzt die Berücksichtigung der Groß-/Kleinschreibung. Dies ist ein neues Flag, das für Verzeichnisse festgelegt werden kann, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen als Unterscheidung nach Groß-/Kleinschreibung behandelt werden sollen, sodass sogar Windows-Anwendungen Dateien ordnungsgemäß öffnen können
    * Drvfs verfügt über neue Bereitstellungs Optionen, die die Berücksichtigung der Groß-/Kleinschreibung pro Verzeichnis steuern.
        * Case = Force: alle Verzeichnisse werden unter Berücksichtigung der Groß-/Kleinschreibung behandelt (mit Ausnahme des Laufwerks Stamms). Neue Verzeichnisse, die mit WSL erstellt werden, werden als Groß-/Kleinschreibung beachtet Dies ist das Legacy Verhalten, außer wenn die Groß-/Kleinschreibung neuer Verzeichnisse gekennzeichnet wird
        * Case = dir: nur Verzeichnisse mit der Unterscheidung nach Groß-/Kleinschreibung werden bei der Groß-/Kleinschreibung beachtet. bei anderen Verzeichnissen wird die Groß-/Kleinschreibung Neue Verzeichnisse, die mit WSL erstellt werden, werden als Groß-/Kleinschreibung beachtet
        * Case = off: nur Verzeichnisse mit der Unterscheidung nach Groß-/Kleinschreibung werden bei der Groß-/Kleinschreibung beachtet. bei anderen Verzeichnissen wird die Groß-/Kleinschreibung Neue Verzeichnisse, die mit WSL erstellt werden, werden als groß-und Kleinschreibung markiert
    * Hinweis: bei Verzeichnissen, die in früheren Versionen von WSL erstellt wurden, ist dieses Flag nicht festgelegt, sodass bei Verwendung der Option "Case = dir" nicht die Groß-/Kleinschreibung beachtet wird. Eine Möglichkeit, dieses Flag für vorhandene Verzeichnisse festzulegen, ist in Kürze verfügbar.
    * Beispiel für die Bereitstellung mit diesen Optionen (für vorhandene Laufwerke müssen Sie zuerst die Bereitstellung aufheben, bevor Sie die Bereitstellung mit anderen Optionen ausführen können): sudo mount-t drvfs C:/mnt/c-o Case = dir
    * Für den Moment ist Case = Force immer noch die Standardoption. Dies wird in der Zukunft in Case = dir geändert.
* Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, wenn Sie drvfs einbinden, z. b.: sudo mount-t drvfs//Server/Share/mnt/Share
* WSL verarbeitet nun die "/etc/fstab"-Datei während des instanzstarts [GH 2636].
    * Dies erfolgt vor der automatischen Einbindung von drvfs-Laufwerken. alle Laufwerke, die bereits von fstab bereitgestellt wurden, werden nicht automatisch erneut bereitgestellt, sodass Sie den Einstellungspunkt für bestimmte Laufwerke ändern können.
    * Dieses Verhalten kann mithilfe von "WSL. conf" ausgeschaltet werden.
* Die Dateien Mount, mountinfo und mountstats in/proc haben Sonderzeichen wie umgekehrte Schrägstriche und Leerzeichen ordnungsgemäß Escapezeichen [GH 2799]
* Sonderdateien, die mit drvfs erstellt wurden, z. b. symbolische Verknüpfungen von WSL oder bei aktivierter Metadaten, können nun aus Windows kopiert und verschoben werden.

#### <a name="wsl-is-more-configurable-with-wslconf"></a>WSL ist mit "WSL. conf" konfigurierbar.
Wir haben eine Methode hinzugefügt, mit der Sie bestimmte Funktionen in WSL automatisch konfigurieren können, die bei jedem Start des Subsystems angewendet werden. Dies umfasst die automatischen Optionen und die Netzwerkkonfiguration. Weitere Informationen hierzu finden Sie in unserem Blogbeitrag unter: https://aka.ms/wslconf

#### <a name="af_unix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a>AF_UNIX ermöglicht Socketverbindungen zwischen Linux-Prozessen auf WSL-und nativen Windows-Prozessen.
WSL-und Windows-Anwendungen können nun über Unix-Sockets miteinander kommunizieren. Stellen Sie sich vor, Sie möchten einen Dienst in Windows ausführen und sowohl für Windows-als auch für WSL-apps verfügbar machen. Das ist mit UNIX-Sockets möglich. Weitere Informationen finden Sie in unserem Blogbeitrag unter https://aka.ms/afunixinterop

### <a name="wsl"></a>WSL
* Unterstützung von mmap () mit MAP_NORESERVE [GH 121, 2784]
* Support CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]
* Behandeln von nicht-SIGCHLD-Beendigungs Signalen im Klon [GH 121, 2781]
* Stub/proc/sys/fs/inotify/max_user_instances und/proc/sys/fs/inotify/max_user_watches [GH 1705]
* Fehler beim Laden von elf Binärdateien, die Lade Header mit nicht-NULL-Offsets enthalten [GH 1884]
* Beim Laden von Bildern werden keine nachfolgenden Seiten Bytes angezeigt.
* Fälle reduzieren, in denen execve den Prozess unbeaufsichtigt beendet

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17083"></a>Build 17083
Allgemeine Windows-Informationen zu Build 17083 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).

### <a name="wsl"></a>WSL
* Korrigiert Fehlercode im Zusammenhang mit epoll [GH 2798, 2801, 2857]
* Beim Ausschalten von ASLR festgelegte Abstürze [GH 1185, 2870]
* Sicherstellen, dass mmap-Vorgänge atomarisch erscheinen [GH 2732]

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17074"></a>Build 17074
Allgemeine Windows-Informationen zu Build 17074 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).

### <a name="wsl"></a>WSL
* Festes Speicherformat der drvfs-Metadaten [GH 2777] </br>
**Wichtig:** Die vor diesem Build erstellten drvfs-Metadaten werden falsch oder überhaupt nicht angezeigt. Um betroffene Dateien zu beheben, verwenden Sie chmod und chown zum erneuten Anwenden der Metadaten.
* Problem mit mehreren Signalen und neu startbaren syscalls behoben.

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17063"></a>Build 17063
Allgemeine Windows-Informationen zu Build 17063 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).

### <a name="wsl"></a>WSL
* Drvfs unterstützt zusätzliche Linux-Metadaten. Dies ermöglicht das Festlegen des Besitzers und des Dateimodus mit chmod/chown sowie das Erstellen spezieller Dateien, z. b. von der Erstellung von Dateien, Unix-Sockets und Gerätedateien. Diese Option ist standardmäßig deaktiviert, da Sie noch experimentell ist.
**Hinweis**:  Wir haben einen Fehler im Metadatenformat behoben, das von drvfs verwendet wird. Obwohl Metadaten in diesem Build für Experimente funktionieren, lesen zukünftige Builds die von diesem Build erstellten Metadaten nicht ordnungsgemäß.  Möglicherweise müssen Sie den Besitzer für geänderte Dateien manuell aktualisieren, und Geräte mit einer benutzerdefinierten Geräte-ID müssen neu erstellt werden.

  Um dies zu aktivieren, einbinden Sie drvfs mit der Metadatenoption (um Sie für eine vorhandene Bereitstellung zu aktivieren):

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  Linux-Berechtigungen werden der Datei als zusätzliche Metadaten hinzugefügt. Sie wirken sich nicht auf die Windows-Berechtigungen aus.  Beachten Sie, dass beim Bearbeiten einer Datei mithilfe eines Windows-Editors die Metadaten möglicherweise entfernt werden. In diesem Fall wird die Datei auf die Standard Berechtigungen zurückgesetzt.

* Der drvfs wurden Bereitstellungsoptionen hinzugefügt, um Dateien ohne Metadaten zu steuern.
  * UID: die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird.
  * gid: die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird.
  * "um Ask": eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen.
  * fmask: eine oktale Maske von Berechtigungen, die für alle regulären Dateien ausgeschlossen werden sollen.
  * dmask: eine oktale Maske von Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen.

  Zum Beispiel:
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  Kombinieren Sie mit der Option Metadata, um Standard Berechtigungen für Dateien ohne Metadaten anzugeben.

* In wurde eine neue Umgebungsvariable `WSLENV`,, eingeführt, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32 fließen.

  Zum Beispiel:

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  `WSLENV`eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozessen von Win32-oder Win32-Prozessen von WSL eingeschlossen werden können.  Jeder Variablen kann ein Schrägstrich gefolgt von Flags angehängt werden, um anzugeben, wie Sie übersetzt werden soll.
  * cker Der Wert ist ein Pfad, der zwischen WSL-Pfaden und Win32-Pfaden übersetzt werden soll.
  * int Der Wert ist eine Liste von Pfaden. In WSL ist es eine durch Doppelpunkte getrennte Liste. In Win32 ist es eine durch Semikolons getrennte Liste.
  * u Der Wert sollte nur beim Aufrufen von WSL aus Win32 eingeschlossen werden.
  * Löw Der Wert sollte nur eingeschlossen werden, wenn Win32 von WSL aus aufgerufen wird.

  Sie können in `WSLENV` . bashrc oder für Ihren Benutzer in der benutzerdefinierten Windows-Umgebung festlegen.

* drvfs-bereit Stellungen speichert Zeitstempel ordnungsgemäß aus tar, CP-p (GH 1939)
* drvfs-symlinks melden die richtige Größe (GH 2641)
* Lese-/Schreibvorgänge funktionieren für sehr große e/a-Größen (GH 2653)
* waitpid funktioniert mit Prozessgruppen-IDs (GH 2534)
* erheblich verbesserte mmap-Leistung für große Reserve Regionen; Verbesserung der Leistung von GHC (GH 1671)
* "Personality" unterstützt für READ_IMPLIES_EXEC; korrigiert von Maxima und clisp (GH 1185)
* mprotect unterstützt PROT_GROWSDOWN; Fixes clisp (GH 1128)
* Seiten Fehlerbehebungen im übercommitmodus; Fixes sbcl (GH 1128)
* Klon unterstützt weitere Flags-Kombinationen
* Unterstützung von SELECT/epoll von epoll-Dateien (zuvor ein No-op-Vorgang).
* Ptrace über nicht implementierte syscalls benachrichtigen.
* Beim Erstellen von resolv. conf-Namen Server nicht Aufforderungs Schnittstellen ignorieren [GH 2694]
* Listet Netzwerkschnittstellen ohne physische Adresse auf. [GH 2685]
* Zusätzliche Fehlerbehebungen und Verbesserungen.

### <a name="linux-tools-available-to-developers-on-windows"></a>Linux-Tools für Entwickler unter Windows

* Die Windows-Befehlszeilen-Toolkette enthält bsdtar (tar) und curl.
  Lesen Sie [diesen Blog](https://aka.ms/tarcurlwindows) , um mehr über das Hinzufügen dieser beiden neuen Tools zu erfahren, und erfahren Sie, wie Sie die Entwickler Darstellung unter Windows strukturieren.

*   `AF_UNIX`ist im Windows Insider SDK (17061 +) verfügbar.
  Lesen Sie [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) , um mehr `AF_UNIX` darüber zu erfahren, wie Entwickler in Windows ihn verwenden können.

### <a name="console"></a>Console
* Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.


## <a name="build-17046"></a>Build 17046

Allgemeine Windows-Informationen zu Build 17046 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).

### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ermöglicht das Ausführen von Prozessen ohne ein aktives Terminal. [GH 709, 1007, 1511, 2252, 2391, et al.]
- Bessere Unterstützung von CLONE_VFORK und CLONE_VM. [GH 1878, 2615]
- Überspringen Sie die TDI-Filtertreiber für WSL-Netzwerk Vorgänge. [GH 1554]
- Drvfs erstellt NT-Symlinks, wenn bestimmte Bedingungen erfüllt sind. [GH 353, 1475, 2602]
    - Das Linkziel muss relativ sein, darf keine Bereitstellungs Punkte oder symlinks überschreiten und muss vorhanden sein.
    - Der Benutzer muss über SE_CREATE_SYMBOLIC_LINK_PRIVILEGE verfügen (Dies erfordert normalerweise, dass Sie "WSL. exe" mit erhöhten Rechten starten), sofern der Entwicklermodus nicht aktiviert ist.
    - In allen anderen Situationen erstellt drvfs weiterhin WSL-symlinks.
- Ermöglicht das gleichzeitige Ausführen von erweiterten und nicht erhöhten WSL-Instanzen.
- Support/proc/sys/kernel/Yama/ptrace_scope
- Fügen Sie wslpath zum Durchführen von WSL-< > Windows-Pfad Konvertierungen hinzu. [GH 522, 1243, 1834, 2327, et al.]
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a>Console
- Keine Korrekturen.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.


## <a name="build-17040"></a>Build 17040

Allgemeine Windows-Informationen zu Build 17040 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Keine Korrekturen seit 17035.

#### <a name="console"></a>Console
- Keine Korrekturen seit 17035.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17035"></a>Build 17035

Allgemeine Windows-Informationen zu Build 17035 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Der Zugriff auf Dateien auf drvfs kann gelegentlich mit EINVAL fehlschlagen. [GH 2448]

#### <a name="console"></a>Console
- Ein Farbverlust beim Einfügen/Löschen von Zeilen im VT-Modus.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17025"></a>Build 17025

Allgemeine Windows-Informationen zu Build 17025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Starten Sie anfängliche Prozesse in einer neuen Vordergrund-Prozessgruppe [GH 1653, 2510].
- Problem Behebungen für die Übermittlung [GH 2496]
- Standardname für virtuelle Bridge generieren, wenn keine Angabe erfolgt [GH 2497].
- Implementieren Sie/proc/sys/kernel/Random/boot_id [GH 2518].
- Weitere Interop stdout/stderr-pipekorrekturen.
- Der Stub-syncfs-System Aufruf.

#### <a name="console"></a>Console
- Korrigieren der Eingabe-VT-Übersetzung für Drittanbieter Konsolen [GH 111]

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="build-17017"></a>Build 17017

Allgemeine Windows-Informationen zu Build 17017 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ignoriert leere elf-Programm Header [GH 330].
- Ermöglicht lxssmanager das Erstellen von WSL-Instanzen für nicht interaktive Benutzer (Unterstützung für SSH-und geplante Aufgaben) [GH 777, 1602].
- Unterstützung von WSL-> Win32-> WSL-Szenarios ("Inception") [GH 1228].
- Eingeschränkte Unterstützung für das Beenden von Konsolen-apps, die über Interop [GH 1614] aufgerufen wurden.
- Unterstützung von Einstellungsoptionen für devpts [GH 1948].
- Ptrace blockiert den untergeordneten Start [GH 2333].
- Im epollet fehlen einige Ereignisse [GH 2462].
- Gibt weitere Daten für PTRACE_GETSIGINFO zurück.
- Getdents mit lseek haben falsche Ergebnisse.
- Beheben Sie einige Win32-Interop-apps, die auf Eingaben in einer Pipe warten, die keine weiteren Daten enthält.
- O_ASYNC Unterstützung für TTY/Pty-Dateien.
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests werden ausgeführt.

## <a name="fall-creators-update"></a>Fall Creators Update

## <a name="build-16288"></a>Build 16288

Allgemeine Windows-Informationen zu Build 16288 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ordnungsgemäße Initialisierung und Berichts-UID, gid und Modus für socketdateideskriptoren [GH 2490]
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16278"></a>Build 16278

Allgemeine Windows-Informationen zu Build 162738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Zuordnung zugeordneter Sichten von Datei gestützten Abschnitten explizit aufheben, wenn der LX mm-Status beendet wird [GH 2415]
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16275"></a>Build 16275

Allgemeine Windows-Informationen zu Build 162735 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- In dieser Version gibt es keine WSL-bezogenen Änderungen.

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16273"></a>Build 16273

Allgemeine Windows-Informationen zu Build 16273 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Es wurde ein Problem behoben, bei dem drvfs manchmal den falschen Dateityp für Verzeichnisse gemeldet hat [GH 2392]
- Erstellung von NETLINK_KOBJECT_UEVENT Sockets zum Entsperren von Programmen zulassen, die uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]
- Unterstützung für nicht blockierende Verbindung hinzufügen [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]
- Implementierende CLONE_FS Clone System-aufrufsflag [GH 2242]
- Beheben von Problemen im Zusammenhang mit der korrekten Behandlung von Registerkarten oder Anführungszeichen in NT-Interop [GH 1625, 2164]
- Beheben des Fehlers "Zugriff verweigert" beim erneuten Starten von WSL-Instanzen [GH 651, 2095]
- Implementieren von Futex-FUTEX_REQUEUE und FUTEX_CMP_REQUEUE-Vorgängen [GH 2242]
- Korrigieren von Berechtigungen für verschiedene sysfs-Dateien [GH 2214]
- Korrigieren des haskell-Stapel Staus während des Setups [GH 2290]
- Implementieren der binfmt_misc-Flags "C", "O" und "P" [GH 2103]
- Add/proc/sys/kernel/SHMMAX/shmmni &/Threads-Max [GH 1753]
- Hinzufügen partieller Unterstützung für ioprio_set-Systemaufrufe [GH 498]
- Stub SO_REUSEPORT & Hinzufügen von Unterstützung für SO_PASSCRED für netLINK-Sockets [GH 69]
- Gibt andere Fehlercodes von registerdistribuiton zurück, wenn derzeit eine Distribution installiert oder deinstalliert wird.
- Aufheben der Registrierung von teilweise installierten WSL-Verteilungen über "wslconfig. exe" zulassen
- Korrigieren Sie den python-sockettestabsturz von UDP:: msg_peek
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Tests gesamt: 1904<br/>
Übersprungene Tests insgesamt: 209<br/>
Gesamtanzahl der Fehler: 229<br/>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a>Build 16257

Allgemeine Windows-Informationen zu Build 16257 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Prlimit64-Systemaufrufe implementieren
- Hinzufügen von Unterstützung für ulimit-n (RLIMIT_NOFILE Limit) [GH 1688]
- Stub MSG_MORE für TCP-Sockets [GH 2351]
- Korrigieren von ungültigem AT_EXECFN-Hilfsvektor Verhalten [GH 2133]
- Korrigieren von Kopier-/Einfügeverhalten für Konsole/TTY und Hinzufügen einer besseren vollständigen Puffer Verarbeitung [GH 2204, 2131]
- Set AT_SECURE im Hilfsvektor für Set-User-ID und Set-Group-ID-Programme [GH 2031]
- Psuedo-Terminal Master Endpunkt behandelt nicht tiocpgrp [GH 1063]
- Korrigieren von lseek zum Zurückspulen von Verzeichnissen in lxfs [GH 2310]
- /dev/ptmx sperrt nach hoher Auslastung [GH 1882]
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Behebung für horizontale Linien/Unterstriche überall [GH 2168]
- Behebung von Änderungen an der Prozess Reihenfolge, die das Schließen von NPM erschwert [GH 2170]
- Neues Farbschema hinzugefügt: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/

### <a name="ltp-results"></a>LTP-Ergebnisse:
Keine Änderung seit 16251

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`prlimit64`<br/>

### <a name="known-issues"></a>Bekannte Probleme
#### <a name="github-issue-2392-windows-folders-not-recognized-by-wsl-httpsgithubcommicrosoftbashonwindowsissues2392"></a>[GitHub-Problem 2392: Windows-Ordner, die nicht von WSL erkannt werden...](https://github.com/Microsoft/BashOnWindows/issues/2392)
In Build 16257 hat WSL Probleme, wenn Windows-Dateien/-Ordner über `/mnt/c/...`aufgelistet werden.
Dieses Problem wurde behoben und sollte in Insider-Builds in der Woche ab 8/14/2017 veröffentlicht werden.

<br/>

## <a name="build-16251"></a>Build 16251

Allgemeine Windows-Informationen zu Build 16251 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Entfernen Sie das Beta-Tag aus der optionalen WSL-Komponente. Weitere Informationen finden Sie im [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) .
- Ordnungsgemäße Initialisierung der gespeicherten Set-UID und GID für die Binärdateien "Set-User-ID" und "Set-Group-ID" bei EXEC [GH 962, 1415, 2072]
- Hinzugefügte Unterstützung für ptrace PTRACE_O_TRACEEXIT [GH 555]
- Unterstützung für ptrace PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555] wurde hinzugefügt.
- Ptrace korrigiert, um bei ignorierten Signalen anzuhalten
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsolen bezogenen Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 768</br>
Anzahl der fehlgeschlagenen Tests: 244</br>
Anzahl übersprungener Tests: 96</br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a>Build 16241

Allgemeine Windows-Informationen zu Build 16241 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- In dieser Version gibt es keine WSL-bezogenen Änderungen.

#### <a name="console"></a>Console
- Korrektur für die Ausgabe des falschen Zeichens für die Übergänge, die ursprünglich [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/) gemeldet wurden
- Behebung, dass kein Ausgabetext in Codepage 65001 (UTF8) angezeigt wird
- Übertragen Sie an den RGB-Werten einer Farbe vorgenommene Änderungen nicht an andere Teile der Palette bei Auswahl Änderungen. Dadurch wird die Verwendung des Konsolen Eigenschaften Blatts erheblich vereinfacht.
- STRG + S funktioniert anscheinend nicht ordnungsgemäß
- Unbold/-Dim in ANSI-Escapecodes vollständig nicht vorhanden [GH 2174]
- Die Konsole unterstützt vim Color-Designs nicht ordnungsgemäß [GH 1706]
- Bestimmte Zeichen können nicht eingefügt werden [GH 2149]
- Die Größenänderung von reflows interagiert seltsam mit der Größenänderung eines bash-Fensters, wenn sich die Inhalte in der Bearbeitungs-/Befehlszeile befinden [GH-Verbindung 1123]
- STRG + L lässt den Bildschirm nicht geändert [GH 1978]
- Fehler beim Rendern der Konsole beim Anzeigen von VT auf hdpi [GH 1907]
- Japansese-Zeichen sehen seltsam mit Unicode-Zeichen U + 30FB [GH 2146]
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16237"></a>Build 16237

Allgemeine Windows-Informationen zu Build 16237 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).<br/>


### <a name="fixed"></a>Fest
- Standard Attribute für Dateien ohne EAS in lxfs verwenden (root, root, 0000)
- Unterstützung für Verteilungen mit erweiterten Attributen hinzugefügt
- Korrigieren der Auffüll Zeichen für von getdents und getdents64 zurückgegebene Einträge
- Korrektur der Berechtigungsüberprüfung für den shmctl SHM_STAT-Systembefehl [GH 2068]
- Korrigiert falscher ursprünglicher epoll-Status für Schreib Telefone [GH 2231]
- Korrigiert drvfs-Fehler beim Zurückgeben aller Einträge [GH 2077]
- Korrigieren von lxfs-Nachrichten, wenn Dateien nicht verknüpft sind [GH 2077]
- Wieder öffnen nicht verknüpfter drvfs-Dateien über procfs zulassen
- Außer Kraft setzung des globalen Registrierungsschlüssels zum Deaktivieren von WSL-Features (Interop/Laufwerk Einbindung) wurde hinzugefügt.
- Korrektur falscher Block Anzahl in "stat" für drvfs (und lxfs) [GH 1894]
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16232"></a>Build 16232

Allgemeine Windows-Informationen zu Build 16232 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).<br/>


### <a name="fixed"></a>Fest
- In dieser Version gibt es keine WSL-bezogenen Änderungen.

</br>

## <a name="build-16226"></a>Build 16226

Allgemeine Windows-Informationen zu Build 16226 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).<br/>


### <a name="fixed"></a>Fest
- Unterstützung von xattr-bezogenen syscalls (getxattr, setxattr, listxattr, removexattr).
- Security. capablity xattr-Unterstützung.
- Verbesserte Kompatibilität mit bestimmten Dateisystemen und Filtern, einschließlich nicht-MS-SMB-Servern. [GH #1952]
- Verbesserte Unterstützung für onedrive-Platzhalter, gvfs-Platzhalter und komprimierte Compact OS-Dateien.
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16215"></a>Build 16215

Allgemeine Windows-Informationen zu Build 16215 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).<br/>


### <a name="fixed"></a>Fest
- Für WSL ist der Entwicklermodus nicht mehr erforderlich.
- Unterstützung von Verzeichnis Verbindungen in drvfs.
- Die Installation von AppX-Paketen der WSL-Verteilung wird durchgeführt.
- Aktualisieren Sie procfs, um private und freigegebene Zuordnungen anzuzeigen.
- Fügen Sie "wslconfig. exe" die Möglichkeit hinzu, Verteilungen zu bereinigen, die teilweise installiert oder deinstalliert wurden.
- Unterstützung für IP_MTU_DISCOVER für TCP-Sockets hinzugefügt. [GH 1639, 2115, 2205]
- Leiten Sie die Protokollfamilie für Routen zu AF_INADDR ein.
- Verbesserungen an seriellen Geräten [GH 1929].

</br>

## <a name="build-16199"></a>Build 16199

Allgemeine Windows-Informationen zu Build 16199 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).<br/>


### <a name="fixed"></a>Fest
- Keine WSL-bezogenen Änderungen in diesen Releases.

</br>

## <a name="build-16193"></a>Build 16193

Allgemeine Windows-Informationen zu Build 16193 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).<br/>


### <a name="fixed"></a>Fest
- Racebedingung zwischen dem Senden von sigtt und einer Thread Gruppe, die beendet wird [GH 1973]
- Ändern von TTY-und Pty-Geräten in Report FILE_DEVICE_NAMED_PIPE anstelle von FILE_DEVICE_CONSOLE [GH 1840]
- SSH-Fix für IP_OPTIONS
- Verschieben der drvfs-Einbindung in den init-Daemon [GH 1862, 1968, 1767, 1933]
- Unterstützung in drvfs wurde für die folgenden NT-symlinks hinzugefügt.

</br>

## <a name="build-16184"></a>Build 16184

Allgemeine Windows-Informationen zu Build 16184 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).<br/>


### <a name="fixed"></a>Fest
- Der Task "apt Package Maintenance" (lxrun. exe/Update) wurde entfernt.
- In "Node. js" wird eine Fehlerausgabe, die von Windows-Prozessen in Node. 1840 js nicht angezeigt wird
- Lockern der Ausrichtungs Anforderungen in lxcore [GH 1794]
- Korrigiert der Behandlung des AT_EMPTY_PATH-Flags in einem Zahl von Systemaufrufen.
- Problem behoben, bei dem das Löschen von drvfs-Dateien mit geöffneten Handles bewirkt, dass die Datei nicht definiertes Verhalten aufweist [GH 544, 966, 1357, 1535, 1615]
- "/etc/hosts" erbt nun Einträge von der Windows-Hostdatei (%windir%\system32\drivers\etc\hosts) [GH 1495]

</br>

## <a name="build-16179"></a>Build 16179

Allgemeine Windows-Informationen zu Build 16179 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).<br/>


### <a name="fixed"></a>Fest
- In dieser Woche ändert sich keine WSL-Datei.

</br>

## <a name="build-16176"></a>Build 16176

Allgemeine Windows-Informationen zu Build 16176 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).<br/>


### <a name="fixed"></a>Fest

- [Aktivierte serielle Unterstützung](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- Hinzugefügte IP-Socketoption IP_OPTIONS [GH 1116]
- Implementierte pschreitev-Funktion (beim Hochladen der Datei nach nginx/php-FPM) [GH 1506]
- Hinzugefügte IP-Socket-Optionen IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]
- Unterstützung für Socketoption IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]
- Added IP (V6) _MTU Socketoption für den Knoten apps, traceroute, Dig, nslookup, Host
- IP-Socketoption IPV6_UNICAST_HOPS hinzugefügt
- [Dateisystem Verbesserungen](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * Einbinden von UNC-Pfaden zulassen
    * Aktivieren der CDFS-Unterstützung in drvfs
    * Ordnungsgemäße Handhabung von Berechtigungen für Netzwerkdatei Systeme in drvfs
    * Unterstützung für Remote Laufwerke zu drvfs hinzufügen
    * Aktivieren der FAT-Unterstützung in drvfs
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse
Keine Änderungen seit 15042

</br>

## <a name="build-16170"></a>Build 16170

Allgemeine Windows-Informationen zu Build 16170 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).<br/>

Wir haben einen neuen [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) veröffentlicht, der unsere Anstrengungen zum Testen von WSL erörtert.

### <a name="fixed"></a>Fest

- Support Socketoption IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]
- Unterstützung für PTRACE_OLDSETOPTIONS hinzufügen. [GH 1692]
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse
Keine Änderungen seit 15042

</br>

## <a name="build-15046-to-windows-10-creators-update"></a>Build 15046 mit Windows 10 Creators Update
Es gibt keine weiteren WSL-Korrekturen oder-Funktionen, die für die Einbindung in das Creators Update in Windows 10 geplant sind. Die Anmerkungen zu dieser Version von WSL werden in den kommenden Wochen fortgesetzt, um Ergänzungen für die nächsten Haupt Windows Update zu Unternehmen. Allgemeine Windows-Informationen zu Build 15046 und zukünftigen Insider Releases finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/). <br/><br/>
 <br/>

## <a name="build-15042"></a>Build 15042

Allgemeine Windows-Informationen zu Build 15042 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).<br/>


### <a name="fixed"></a>Fest

- Behebung eines Deadlocks beim Entfernen eines Pfades, der in ".." endet
- Es wurde ein Problem behoben, bei dem "fonbio" bei 1683 Erfolg "0" nicht zurückgibt
- Problem bei Lesevorgängen mit einer Länge von inet-Datagramm-Sockets
- Behebung eines möglichen Deadlocks aufgrund einer Racebedingung in der drvfs-tatsächliche-Suche [GH 1675]
- Erweiterte Unterstützung für UNIX-sockethilfdaten; SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613, 1326]
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 737</br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255

</br>

## <a name="build-15031"></a>Build 15031

Allgemeine Windows-Informationen zu Build 15031 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).<br/>


### <a name="fixed"></a>Fest

- Es wurde ein Fehler behoben, bei dem sich die Zeit (2) sporadisch nicht verhält.
- Korrigiert und Problem, dass die Signal Maske von * sigprocmask-syscalls beschädigt werden konnte.
- Gibt jetzt die vollständige Befehlszeilen Länge in der WSL-Prozess Erstellungs Benachrichtigung zurück. [GH 1632]
- WSL meldet jetzt die Thread Exit-über-ptrace für gdb-Abstürze. [GH 1196]
- Es wurde ein Fehler behoben, bei dem PTYs nach hoher tmux-e/a hängen [GH 1358]
- Korrigieren der Timeout Validierung in vielen Systemaufrufen (Futex, SEMTIMEDOP, ppoll, sigtimedwait, itimer, timer_create)
- Hinzugefügte eventfd EFD_SEMAPHORE-Unterstützung [GH 452]
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 737</br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a>Build 15025

Allgemeine Windows-Informationen zu Build 15025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).<br/>


### <a name="fixed"></a>Fest

- Behebung von Fehlern, bei denen die grep 2,27 [GH 1578] abgebrochen wurde
- Implementiertes EFD_SEMAPHORE-Flag für eventfd2 syscall [GH 452]
- Implementiertes/proc/[PID]/NET/ipv6_route [GH 1608]
- Signal gestützte IO-Unterstützung für UNIX-Streamsockets [GH 393, 68]
- Support F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]
- Implementieren von recvmmsg () syscall [GH 1531]
- Fehler behoben, bei dem epoll_wait () nicht gewartet hat [GH 1609]
- Implementieren von/proc/version_signature
- Tee syscall gibt jetzt einen Fehler zurück, wenn beide Dateideskriptoren auf dieselbe Pipe verweisen
- Implementiertes korrektes Verhalten für SO_PEERCRED für UNIX-Sockets
- Korrigieren der Behandlung von ungültigen tkill syscall-Parametern
- Änderungen zum Vergrößern des vorformace von drvfs
- Kleinere Behebung für Ruby IO-Blockierung
- Korrigieren von recvmsg () beim Zurückgeben von EINVAL für das MSG_DONTWAIT-Flag für inet Sockets [GH 1296]
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 732</br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a>Build 15019

Allgemeine Windows-Informationen zu Build 15019 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).<br/>


### <a name="fixed"></a>Fest

- Es wurde ein Fehler behoben, der fälschlicherweise die CPU-Auslastung in procfs für Tools wie htop (GH 823, 945, 971) gemeldet hat.
- Beim Aufrufen von "Open () with O_TRUNC" für eine vorhandene Datei "inotify" generiert nun IN_MODIFY vor IN_OPEN
- Fehlerbehebungen für den UNIX-Socket getsockopt SO_ERROR zum Aktivieren des Postgress [GH 61, 1354]
- Implementieren von/proc/sys/net/Core/somaxconn für die Sprache go
- Apt-get Package Update background-Task wird jetzt ausgeblendet aus der Ansicht
- Löschen Sie den Bereich für IPv6 localhost (Spring-Framework (Java)-Fehler).
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 714 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 249 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a>Build 15014

Allgemeine Windows-Informationen zu Build 15014 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).<br/>


### <a name="fixed"></a>Fest

- STRG + C funktioniert nun wie beabsichtigt
- htop und PS-Lösung zeigen jetzt die korrekte Ressourcenverwendung an (GH #516)
- Grundlegende Übersetzung von NT-Ausnahmen in Signale. (GH #513)
- bei der Aufhebung der Speicherplatz Ausführung von "ENOSPC" tritt nun ein Fehler auf, wenn nicht mehr als EINVAL (GH #1571)
- /Proc/sys/kernel/SEM. hinzugefügt
- Implementierte semop-und SEMTIMEDOP-Systemaufrufe
- Korrigiert nslookup-Fehler mit der Option IP_RECVTOS & IPV6_RECVTCLASS Socket (GH 69)
- Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 709 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a>Syscall-Zusammenfassung
Gesamtanzahl der syscalls: 384 </br>
Implementiertes gesamt: 235 </br>
Stub gesamt: 22 </br>
Nicht implementiert gesamt: 127 </br>
[Ausführliche Aufschlüsselung](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a>Build 15007

Allgemeine Windows-Informationen zu Build 15007 finden Sie im [Windows-Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).<br/>


### <a name="known-issue"></a>Bekanntes Problem

- Es gibt einen bekannten Fehler, bei dem die Konsole eine STRG + <key> Eingabe nicht erkennt.  Dies schließt den Strg-c-Befehl ein, der als normales ' c '-KeyPress fungiert.

  - Problemumgehung: Ordnen Sie einen alternativen Schlüssel zu STRG + C zu. Um z. b. STRG + K zu STRG + C zuzuordnen, `stty intr \^k`führen Sie Folgendes aus:.  Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn bash gestartet wird. Benutzer können die Option zum Einbeziehen der`.bashrc`

### <a name="fixed"></a>Fest

- Das Problem wurde behoben, bei dem die Ausführung von WSL 100% eines CPU-Kerns verbraucht.
- Socketoption IP_PKTINFO, IPV6_RECVPKTINFO wird jetzt unterstützt. (GH #851, 987)
- Die physische Adresse der Netzwerkschnittstelle wird in lxcore (GH #1452, 1414, 1343, 468, 308) auf 16 Bytes abgeschnitten.
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 709 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a>Build 15002

Allgemeine Windows-Informationen zu Build 15002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).<br/>


### <a name="known-issue"></a>Bekanntes Problem

Zwei bekannte Probleme:
- Es gibt einen bekannten Fehler, bei dem die Konsole eine STRG + <key> Eingabe nicht erkennt.  Dies schließt den Strg-c-Befehl ein, der als normales ' c '-KeyPress fungiert.

  - Problemumgehung: Ordnen Sie einen alternativen Schlüssel zu STRG + C zu. Um z. b. STRG + K zu STRG + C zuzuordnen, `stty intr \^k`führen Sie Folgendes aus:.  Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn bash gestartet wird. Benutzer können die Option zum Einbeziehen der`.bashrc`

- Während der Ausführung von WSL werden von einem System Thread 100% eines CPU-Kerns beansprucht.  Die Ursache wurde intern behoben und behoben.

### <a name="fixed"></a>Fest

- Alle bash-Sitzungen müssen jetzt auf derselben Berechtigungsebene erstellt werden.  Der Versuch, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.  Dies bedeutet, dass Administrator-und nicht-Administrator Konsolen nicht gleichzeitig ausgeführt werden können. (GH #626)
<br/>
- Die folgenden NETLINK_ROUTE-Nachrichten wurden implementiert (erfordert Windows-Administrator).
     - RTM_NEWADDR (unter `ip addr add`stützt)
     - RTM_NEWROUTE (unter `ip route add`stützt)
     - RTM_DELADDR (unter `ip addr del`stützt)
     - RTM_DELROUTE (unter `ip route del`stützt)
- Die geplante Task Überprüfung für zu Aktualisier Ende Pakete wird nicht mehr über eine getaktete Verbindung (GH #1371) ausgeführt.
- Es wurde ein Fehler behoben, bei dem die Weiterleitung unterbrochen wird, d.h. bash-c "ls-ALR/" | bash-c "Cat" (GH #1214)
- Implementierte TCP_KEEPCNT-Socketoption (GH #843)
- Implementierte IP_MTU_DISCOVER inet-Socketoption (GH #720, 717, 170, 69)
- Ältere Funktionalität zum Ausführen von NT-Binärdateien aus init mit NT-Pfad Suche entfernt. (GH #1325)
- Korrekturmodus von/dev/Kmsg zum Zulassen von Gruppen-/sonstigen Lesezugriff (0644) (GH #1321)
- Implementiertes/proc/sys/kernel/Random/UUID (GH #1092)
- Der Fehler wurde behoben, bei dem die Startzeit des Prozesses als Jahr 2432 (GH #974) angezeigt wurde.
- Der Standardbegriff "Umgebungsvariable" wird in "xterm-256 Color" (GH #1446) gewechselt.
- Änderung der Art und Weise, in der der prozesscommit während der Prozess Verzweigung berechnet wird (GH #1286)
- Implementiertes/proc/sys/VM/overcommit_memory. (GH #1286)
- Implementierte/proc/net/Route-Datei (GH #69)
- Fehler behoben, bei dem der Verknüpfungs Name falsch lokalisiert wurde (GH #696)
- Eine fehlerhafte ELF-Verarbeitungslogik, die die Programm Header nicht ordnungsgemäß überprüft, muss kleiner als (oder gleich) PATH_MAX sein. (GH #1048)
- Implementierter Status von "procfs", "sysfs", "cgroupfs" und "binf" (#1378)
- Korrigieren von aptpackageindexupdate-Fenstern, die nicht geschlossen werden (GH #1184, auch in GH #1193 erläutert)
- ASLR-Persönlichkeit ADDR_NO_RANDOMIZE-Unterstützung hinzugefügt. (GH #1148, 1128)
- Verbessertes PTRACE_GETSIGINFO, Signatur Segment v, für ordnungsgemäße gdb-Stapel Überwachungen während der AV (GH #875)
- Die elf-Verarbeitung schlägt für patchelf-Binärdateien nicht mehr fehl. (GH #471)
- VPN-DNS-Weitergabe an/etc/resolv.conf (GH #416, 1350)
- Verbesserungen an TCP Close für eine zuverlässigere Datenübertragung. (GH #610, 616, 1025, 1335)
- Geben Sie nun den richtigen Fehlercode zurück, wenn zu viele Dateien (EMFILE) geöffnet werden. (GH #1126, 2090)
- Windows Audit Log meldet jetzt den Image Namen in Process create Audit.
- Fehler beim Starten von bash. exe in einem bash-Fenster ordnungsgemäß.
- Es wurde eine Fehlermeldung hinzugefügt, wenn Interop nicht auf ein Arbeitsverzeichnis unter lxfs zugreifen kann (z.b. "Notepad. exe. bashrc").
- Problem behoben, bei dem der Windows-Pfad in WSL abgeschnitten wurde
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 690 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 274 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a>Build 14986

Allgemeine Windows-Informationen zu Build 14986 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).<br/>


### <a name="fixed"></a>Fest

- Bugprüfungen mit NetLink und Pty IOCTLs korrigiert
- Nun meldet die Kernel Version 4.4.0-43 aus Gründen der Konsistenz mit xenial.
- Bash. exe wird jetzt gestartet, wenn die Eingabe an "NUL:" (GH #1259) gerichtet ist.
- Thread-IDs werden nun ordnungsgemäß in procfs gemeldet (GH #967)
- IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR-Flags werden jetzt in inotify_add_watch () (GH #1280) unterstützt.
- Implementieren Sie timer_create und verwandte Systemaufrufe.  Dies ermöglicht die Unterstützung von GHC (GH #307).
- Problem behoben, bei dem Ping eine Zeit von 0.000 ms zurück gab (GH #1296)
- Geben Sie den richtigen Fehlercode zurück, wenn zu viele Dateien geöffnet werden.
- Es wurde ein Problem in WSL behoben, bei dem die NETLink-Anforderung für Netzwerkschnittstellen Daten mit EINVAL fehlgeschlagen ist, wenn die Hardwareadresse der Schnittstelle 32 Bytes (z. b. die Teredo-Schnittstelle
   - Beachten Sie, dass das Linux-Hilfsprogramm "IP" einen Fehler enthält, bei dem ein Absturz erfolgt, wenn WSL eine 32-Byte-Hardwareadresse meldet. Dies ist ein Fehler in "IP", nicht bei WSL. Mit dem Hilfsprogramm "IP" wird die Länge des Zeichen folgen Puffers fest codiert, der zum Drucken der Hardwareadresse verwendet wird, und dieser Puffer ist zu klein, um eine 32-Byte-Hardwareadresse auszugeben.
- Zusätzliche Korrekturen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 669 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 258 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a>Build 14971

Allgemeine Windows-Informationen zu Build 14971 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.  Regelmäßig geplante Updates werden bei der nächsten Version fortgesetzt.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Unverändert gegenüber 14965 </br>
Anzahl der bestandenen Tests: 664 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a>Build 14965

Allgemeine Windows-Informationen zu Build 14965 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).<br/>


### <a name="fixed"></a>Fest

- Unterstützung für netLINK Sockets NETLINK_ROUTE Protocol RTM_GETLINK und RTM_GETADDR (GH #468)
  - Aktiviert ifconfig-und IP-Befehle für die netzwerkenumeration.
  - Weitere Informationen finden Sie im [Blogbeitrag zu WSL-Netzwerken](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).

- /sbin befindet sich jetzt standardmäßig im Pfad des Benutzers.
- Der NT-Benutzer Pfad wird jetzt standardmäßig an den WSL-Pfad angefügt (Sie können nun Notepad. exe eingeben, ohne dem Linux-Pfad System32 hinzuzufügen).
- Unterstützung für/proc/sys/kernel/cap_last_cap hinzugefügt
- NT-Binärdateien können nun von WSL aus gestartet werden, wenn das aktuelle Arbeitsverzeichnis nicht-ANSI-Zeichen (GH #1254) enthält.
- Zulassen des herunter Fahrens auf einem nicht verbundenen UNIX-Streamsocket
- Unterstützung für PR_GET_PDEATHSIG hinzugefügt.
- Unterstützung für CLONE_PARENT hinzugefügt
- Es wurde ein Fehler behoben, bei dem die Weiterleitung unterbrochen wird, d.h. bash-c "ls-ALR/" | bash-c "Cat" (GH #1214)
- Verarbeitet Anforderungen zum Herstellen einer Verbindung mit dem aktuellen Terminal.
- Markieren Sie<pid>/proc//oom_score_adj als beschreibbar.
- /Sys/fs/CGroup Ordner hinzufügen.
- sched_setaffinity sollte die Anzahl der Affinitäts Bits Mask zurückgeben.
- Korrektur der elf-Validierungs Logik, die fälschlicherweise annimmt, dass interpreterpfade weniger als 64 Zeichen lang sein müssen. (GH #743)
- Dateideskriptoren öffnen können das Konsolenfenster geöffnet lassen (GH #1187)
- Fixeed-Fehler, bei dem Rename () mit einem nachgestellten Schrägstrich am Zielnamen (GH #1008) fehlgeschlagen
- Implementieren der/proc/net/dev-Datei
- Korrigiert 0.000 ms Pings aufgrund der Zeit Geber Auflösung.
- Implementiertes/proc/self/Environ (GH #730)
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 664 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a>Build 14959

Allgemeine Windows-Informationen zu Build 14959 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).<br/>


### <a name="fixed"></a>Fest

- Verbesserte Pico-Prozess Benachrichtigung für Windows.  Weitere Informationen finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).
- Verbesserte Stabilität durch Windows-Interoperabilität
- Fehler 0x80070057 beim Starten von bash. exe behoben, wenn der Unternehmens Datenschutz (Enterprise Data Protection, EDP) aktiviert ist
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 665 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a>Build 14955

Allgemeine Windows-Informationen zu Build 14955 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.  Regelmäßig geplante Updates werden bei der nächsten Version fortgesetzt.

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 665 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a>Build 14951

Allgemeine Windows-Informationen zu Build 14951 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).<br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a>Neues Feature: Interoperabilität von Windows/Ubuntu
Windows-Binärdateien können jetzt direkt über die WSL-Befehlszeile aufgerufen werden.  Dadurch haben Benutzer die Möglichkeit, mit Ihrer Windows-Umgebung und dem System auf eine Weise zu interagieren, die nicht möglich war.  Als kurzes Beispiel können Benutzer nun die folgenden Befehle ausführen:

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

Weitere Informationen finden Sie unter:

- [WSL-Teamblog für Interop](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [MSDN-Interop-Dokumentation](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a>Fest

- Ubuntu 16,04 (xenial) ist jetzt für alle neuen WSL-Instanzen installiert.  Benutzer mit vorhandenen 14,04-Instanzen (trusty) werden nicht automatisch aktualisiert.
- Das während der Installation festgelegte Gebiets Schema wird jetzt angezeigt.
- Terminal Verbesserungen, einschließlich des Fehlers bei der Umleitung eines WSL-Prozesses an eine Datei, funktioniert nicht immer
- Die Konsolen Lebensdauer muss an die Lebensdauer von bash. exe gebunden sein
- Die Größe des Konsolenfensters sollte die sichtbare Größe und nicht die Puffergröße verwenden.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 665 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a>Build 14946

Allgemeine Windows-Informationen zu Build 14946 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).<br/>


### <a name="fixed"></a>Fest

- Es wurde ein Problem behoben, das das Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen, die Leerzeichen oder Anführungszeichen enthalten 
- Ändern Sie "volfs" und "drvfs" so, dass für die Verknüpfungs Anzahl der Verzeichnisse in der
- Support IPV6_MULTICAST_HOPS Socketoption.
- Beschränken auf eine einzige Konsolen-e/a-Schleife pro TTY. Beispiel: der folgende Befehl ist möglich:
  - bash-c "Echo Daten" | bash-c "SSH user@example.com " cat > foo. txt ""

- Ersetzen von Leerzeichen durch Registerkarten in/proc/cpuinfo (GH #1115)
- Drvfs wird jetzt in mountinfo mit einem Namen angezeigt, der dem bereitgestellten Windows-Volume entspricht.
- /Home und/root werden nun in mountinfo mit korrekten Namen angezeigt.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 665 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a>Build 14942

Allgemeine Windows-Informationen zu Build 14942 finden Sie im [Windows-Blog](https://aka.ms/onefourninefourtwoooooo).<br/>


### <a name="fixed"></a>Fest

- Eine Reihe von bugprüfungen, einschließlich des Netzwerk Absturzes "versuchte Ausführung des noexecute-Speichers", der SSH blockiert hat
- Unterstützung von Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf drvfs generiert werden, ist jetzt in
- Implementieren Sie TCP_KEEPIDLE und TCP_KEEPINTVL für mongod. (GH #695)
- Implementieren des pivot_root-System Aufrufes
- Implementieren der Socketoption für SO_DONTROUTE
- Zusätzliche Fehlerbehebungen und Verbesserungen


### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 665 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a>Build 14936

Allgemeine Windows-Informationen zu Build 14936 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).<br/>


Hinweis: WSL wird in einer zukünftigen Version Ubuntu-Version 16,04 (xenial) anstelle von Ubuntu 14,04 (trusty) installieren.  Diese Änderung gilt für Insider, die neue Instanzen installieren (lxrun. exe/install oder die erste Ausführen von bash. exe).  Vorhandene Instanzen mit trusty werden nicht automatisch aktualisiert. Benutzer können mit dem Befehl "Do-Release-Upgrade" Ihr trusty-Bild auf "xenial" aktualisieren.

### <a name="known-issue"></a>Bekanntes Problem
Bei WSL treten Probleme mit einigen Socketimplementierungen auf.  Der Fehlercode manifestiert sich selbst als Absturz mit dem Fehler "Es wurde versucht, den noexecute-Speicher auszuführen".  Die häufigste Erscheinung dieses Problems ist ein Absturz bei der Verwendung von SSH.  Die Ursache ist bei internen Builds korrigiert und wird zu Beginn der frühesten Gelegenheit an Insider übermittelt.

### <a name="fixed"></a>Fest

- Der chroot-Systemaufrufe wurde implementiert.
- Verbesserungen bei der inotifizierungen ~~einschließlich Unterstützung für von Windows-Anwendungen generierte Benachrichtigungen auf drvfs~~
  - Berichtigungs Die Unterstützung von Änderungen, die von Windows-Anwendungen stammen, ist zurzeit nicht verfügbar.
- Socketbindung an IPv6:<port n> : unterstützt jetzt IPV6_V6ONLY (GH #68, #157, #393, #460, #674, #740, #982)
- Wnowait-Verhalten für waitid systemcallimplementiertes (GH #638)
- Unterstützung für IP-Socketoptionen IP_HDRINCL und IP_TTL
- Lesevorgänge () der Länge 0 (null) sollten sofort (GH #975) zurückgeben.
- Ordnungsgemäße Behandlung von Dateinamen und Dateinamen Präfixen, die keinen null-Terminator in einer tar-Datei enthalten.
- epoll-Unterstützung für/dev/null
- Fix/dev/Alarm Zeit Quelle
- Bash-c kann nun zu einer Datei umgeleitet werden.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 664 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 264 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`chroot`<br/>
<br/>

## <a name="build-14931"></a>Build 14931

Allgemeine Windows-Informationen zu Build 14931 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.  Regelmäßig geplante Updates werden in der nächsten Version fortgesetzt.

<br/>

## <a name="build-14926"></a>Build 14926

Allgemeine Windows-Informationen zu Build 14926 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).<br/>


### <a name="fixed"></a>Fest

- Ping funktioniert nun in-Konsolen, die nicht über Administratorrechte verfügen.
- Ping6 wird jetzt auch ohne Administratorrechte unterstützt.
- Unterstützung von Dateien, die über WSL geändert wurden (GH #216)
  - Unterstützte Flags:
    - inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK
    - inotify_add_watch-Ereignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF
    - inotify_add_watch-Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR
    - Ausgabe lesen: LX_IN_ISDIR, LX_IN_IGNORED
  - Bekanntes Problem: Durch das Ändern von Dateien aus Windows-Anwendungen werden keine Ereignisse generiert.
- UNIX-Socket unterstützt jetzt SCM_CREDENTIALS

### <a name="ltp-results"></a>LTP-Ergebnisse:
Anzahl der bestandenen Tests: 651 </br>
Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 258 </br>
[Test Laufprotokolle von LTP](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a>Build 14915

Allgemeine Windows-Informationen zu Build 14915 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).<br/>


### <a name="fixed"></a>Fest
-  Socketpair für UNIX Datagramm-Sockets (GH #262)
- Unterstützung für UNIX-Sockets für SO_REUSEADDR
- Unterstützung von UNIX-Sockets für SO_BROADCAST (GH #568)
- Unterstützung für UNIX-Sockets für sock_seqpacket (GH #758 #546)
- Hinzufügen von Unterstützung für UNIX Datagram Socket Send, empfangener und Shutdown
- Korrigieren Sie Fehlercode aufgrund einer ungültigen Überprüfung des mmap-Parameters für nicht feste Adressen. (GH #847)
- Unterstützung für das aussetzen/fortsetzen von Terminal Zuständen
- Unterstützung für tiocpkt ioctl zum Entsperren des Bildschirm Hilfsprogramms (GH #774)
    - Bekanntes Problem: Funktionstasten sind nicht funktionsfähig.
- Es wurde ein Race in timerfd korrigiert, das dazu führen kann, dass ein frei gegebener Member "readerready" von lxptimerfdworkerroutine (GH #814) aufgerufen wird.
- Aktivieren der Unterstützung für den erneuten Start baren System Abruf für Futex, Abruf und clock_nanosleep
- Unterstützung für Bindungs einbinden hinzugefügt
- Freigabe für einstellungsnamespace-Unterstützung aufheben
    - Bekanntes Problem: Beim Erstellen eines neuen Mount-Namespace `unshare(CLONE_NEWNS)` mit dem aktuellen Arbeitsverzeichnis wird weiterhin auf den alten Namespace verweisen.
- Weitere Verbesserungen und Fehlerbehebungen

<br/>

## <a name="build-14905"></a>Build 14905

Allgemeine Windows-Informationen zu Build 14905 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).<br/>


### <a name="fixed"></a>Fest
- Neu Start Bare Systemaufrufe werden jetzt unterstützt (GH #349, GH #520)
- Symlinks zu Verzeichnissen, die mit/jetzt funktionstüchtig (GH #650) enden
- Implementierte rndgetentcnt ioctl für "/dev/random"
- Die/proc/[PID]/Mounts,/proc/[PID]/mountinfo und/proc/[PID]/mountstats-Dateien wurden implementiert.
- Zusätzliche Fehlerbehebungen und Verbesserungen

</br>

## <a name="build-14901"></a>Build 14901
Der erste Insider-Build für die Windows 10 Anniversary Update-Version.

Allgemeine Windows-Informationen zu Build 14901 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).<br/>


### <a name="fixed"></a>Fest
- Korrigieren des nachfolgenden Schrägstrichs
    - Befehle wie `$ mv a/c/ a/b/` jetzt funktionieren.
- Bei der Installation werden jetzt Aufforderungen angezeigt, wenn Ubuntu-Gebiets Schema auf Windows
- Procfs-Unterstützung für den NS-Ordner
- Hinzufügen und Entfernen von Bereitstellungs-, procfs-und sysfs-Dateisystemen
- Korrigieren von mklod [at] 32-Bit-ABI-Signatur
- In Dispatch-Modell verschobene Unix-Sockets
- Die mit setsockopt festgelegte inet-Socket-empfangener-Puffergröße muss berücksichtigt werden.
- MSG_CMSG_CLOEXEC UNIX-Socket-Empfangs Nachrichtenflag implementieren
- Linux-Prozess stdin/stdout-Pipe-Umleitung (GH #2)
    - Ermöglicht das Weiterleiten von bash-c-Befehlen in cmd.  Beispiel: > dir | bash-c "grep foo"
- Bash kann nun auf Systemen mit mehreren Seiten Dateien (GH #538 #358) installiert werden.
- Die standardmäßige inet-socketpuffergröße sollte mit der standardmäßigen Ubuntu-Einrichtung
- Ausrichten von xattr-syscalls an listxattr
- Gibt nur Schnittstellen mit einer gültigen IPv4-Adresse von siocgifconf zurück.
- Signal Standardaktion korrigieren, wenn von ptrace eingefügt
- Implementieren von/proc/sys/VM/min_free_kbytes
- Beim Wiederherstellen von Kontext in sigreturn Werte für den Computer Kontext Register verwenden
    - Dadurch wird das Problem behoben, dass Java und javac für einige Benutzer hängen.
- Implementieren von/proc/sys/kernel/Hostname

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a>Build 14388 bis Windows 10 Anniversary Update
Allgemeine Windows-Informationen zu Build 14388 finden Sie im [Windows-Blog](https://aka.ms/14388wip). <br/>

### <a name="fixed"></a>Fest
- Korrekturen für die Vorbereitung auf das Windows 10 Anniversary Update auf 8/2
  - Weitere Informationen zu WSL im Anniversary Update finden Sie in unserem [Blog](https://blogs.msdn.microsoft.com/wsl/) .

<br/>

## <a name="build-14376"></a>Build 14376
Allgemeine Windows-Informationen zu Build 14376 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/). <br/>

### <a name="fixed"></a>Fest
- Einige Instanzen entfernt, bei denen apt-get nicht mehr reagiert (GH #493)
- Ein Problem wurde behoben, bei dem leere bereit Stellungen nicht ordnungsgemäß behandelt wurden
- Ein Problem wurde behoben, bei dem Ramdisks nicht ordnungsgemäß bereitgestellt wurde
- Ändern der UNIX-Socket-Annahme zur Unterstützung von Flags (Teil-GH-#451
- Ein gängiger Netzwerk bezogener Bluescreen wurde korrigiert.
- Festes Bluescreen beim Zugriff auf/proc/[PID] > Task (GH #523)
- Hohe CPU-Auslastung für einige Pty-Szenarien (GH #488 #504) korrigiert
- Zusätzliche Fehlerbehebungen und Verbesserungen

<br/>

## <a name="build-14371"></a>Build 14371
Allgemeine Windows-Informationen zu Build 14371 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/). <br/>

### <a name="fixed"></a>Fest
- Korrigiertes zeitlichen Rennen mit SIGCHLD und Wait () bei Verwendung von ptrace
- Es wurde ein gewisses Verhalten korrigiert, wenn Pfade eine nachfolgende/(GH #432)
- Problem mit Fehler beim Umbenennen/Aufheben der Verknüpfung aufgrund von geöffneten Handles für untergeordnete Elemente behoben
- Zusätzliche Fehlerbehebungen und Verbesserungen

<br/>

## <a name="build-14366"></a>Build 14366
Allgemeine Windows-Informationen zu Build 14366 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/). <br/>

### <a name="fixed"></a>Fest
- Korrektur beim Erstellen von Dateien durch symlinks
-   Hinzugefügter listxattr für python (GH 385)
-   Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
-   Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`listxattr`<br/>
<br/>

## <a name="build-14361"></a>Build 14361
Allgemeine Windows-Informationen zu Build 14361 finden Sie im [Windows-Blog](https://aka.ms/wip14361). <br/>

### <a name="fixed"></a>Fest
- Bei der Ausführung in bash unter Ubuntu unter Windows wird bei drvfs nun die Groß-/Kleinschreibung beachtet.
  - Benutzer können Case. txt und Case. TXT auf Ihren/mnt/c-Laufwerken
  - Die Groß-/Kleinschreibung wird nur in bash unter Ubuntu unter Windows unterstützt. Wenn die Dateien außerhalb von bash-NTFS korrekt gemeldet werden, kann es bei der Interaktion mit den Dateien von Windows zu unerwartetem Verhalten kommen.
  - Beim Stamm der einzelnen Volumes (d.h./mnt/c) wird die Groß-/Kleinschreibung nicht beachtet.
  - Weitere Informationen zum Verarbeiten dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).
- Stark verbesserte Pty-/TTY-Unterstützung.  Anwendungen wie tmux werden jetzt unterstützt (GH #40)
- Installationsproblem behoben, bei dem Benutzerkonten nicht immer erstellt wurden
- Optimierte Befehlszeilen-arg-Struktur, die eine extrem lange Argumentliste zulässt. (GH #153)
- Jetzt können READ_ONLY-Dateien und chmod-Dateien aus drvfs gelöscht werden.
- Es wurden einige Instanzen behoben, bei denen das Terminal beim Trennen nicht mehr reagiert (GH #43)
- chmod und chown funktionieren jetzt auf TTY-Geräten
- Verbindung mit 0.0.0.0 und:: As localhost zulassen (GH #388)
- Sendmsg/recvmsg behandelt nun eine IO-Vektor Länge von > 1 (partielle GH-#376)
- Benutzer können jetzt die automatisch generierte Hostdatei ablehnen (GH #398).
- Automatisches Zuordnen von Linux-Gebiets Schemas zum NT-Gebiets Schema während der Installation (GH #11)
- /Proc/sys/VM/swappiness-Datei hinzugefügt (GH #306)
- "strace" wird jetzt ordnungsgemäß beendet.
- Erneuten Öffnen von Pipes über/proc/self/fd (GH #222) zulassen
- Ausblenden von Verzeichnissen unter "%LocalAppData%\lxss" aus drvfs (GH #270)
- Bessere Behandlung von bash. exe ~.  Befehle wie "bash ~-c ls" werden jetzt unterstützt (GH #467).
- Sockets Benachrichtigen, dass epoll beim Herunterfahren verfügbar ist (GH #271)
- lxrun/Uninstall bietet eine bessere Aufgabe zum Löschen der Dateien und Ordner.
- Korrigierte PS-f (GH #246)
- Verbesserte Unterstützung für X11-apps, z. b. XEmacs (GH #481)
- Aktualisierte anfängliche Thread Stapelgröße, um der standardmäßigen Ubuntu-Einstellung zu entsprechen und die Größe ordnungsgemäß an get_rlimit syscall (GH #172 #258) zu melden.
- Verbesserte Berichterstellung von Namen von Pico-Prozess Images (z. b. für die Überwachung)
- Implementierter/proc/mountinfo for DF-Befehl
- Der Symlink-Fehlercode für den untergeordneten Namen wurde korrigiert. und..
- Weitere Verbesserungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a>Build 14352
Allgemeine Windows-Informationen zu Build 14352 finden Sie im [Windows-Blog](https://aka.ms/wip14352).<br/>


### <a name="fixed"></a>Fest
- Ein Problem wurde behoben, bei dem große Dateien nicht ordnungsgemäß heruntergeladen/erstellt wurden.  Dadurch wird die Blockierung von NPM und anderen Szenarien (GH #3, GH #313) verhindert.
- Einige Instanzen entfernt, bei denen Sockets hängen.
- Einige ptrace-Fehler wurden korrigiert.
- Problem mit WSL behoben, das die Angabe von Dateinamen mit mehr als 255 Zeichen zulässt
- Verbesserte Unterstützung für nicht englische Zeichen
- Aktuelle Windows-Zeit Zonendaten hinzufügen und als Standard festlegen
- Eindeutige Geräte-IDs für jeden Einstellungspunkt (JRE Fix – GH #49)
- Korrigieren eines Problems mit Pfaden, die "." enthalten. und ".."
- Hinzugefügte FIFO-Unterstützung (GH #71)
- Aktualisiertes Format von "resolv. conf" entsprechend dem systemeigenen Ubuntu-Format
- Einige procfs-Bereinigung
- Aktiviertes Ping für Administrator Konsolen (GH #18)

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a>Build 14342
Allgemeine Windows-Informationen zu Build 14342 im [Windows-Blog](https://aka.ms/wip14342). <br/>

Informationen zu volfs und drivefs finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl). <br/>

### <a name="fixed"></a>Fest
- Installationsproblem behoben, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen enthielt
- Die Problem Umgehung "apt-get update udev" in den FAQ wird jetzt standardmäßig bei der ersten Ausführung bereitgestellt.
- Aktivierte symlinks in drivefs-<drive>Verzeichnissen (im)
- Symlinks funktionieren nun zwischen drivefs und volfs
- Problem bei der übergeordneten Pfad Verarbeitung adressiert: ls.//funktioniert jetzt erwartungsgemäß.
- NPM-Installation auf drivefs und die-g-Optionen funktionieren jetzt
- Problem behoben, das den Start des PHP-Servers verhindert
- Aktualisierte Standard Umgebungs Werte, z. b. $Path, um System eigenes Ubuntu zu erreichen
- Ein wöchentlicher Wartungs Task in Windows zum Aktualisieren des APT-Paket Caches wurde hinzugefügt.
- Problem bei der Überprüfung elf Header behoben, WSL unterstützt jetzt alle Melkor-Optionen
- Zsh Shell ist funktionsfähig
- Vorkompilierte go-Binärdateien werden jetzt unterstützt.
- Eingabeaufforderung für bash. exe: erste Testlauf ist nun ordnungsgemäß lokalisiert.
- /proc/meminfo gibt jetzt korrekte Informationen zurück.
- Sockets werden jetzt in VFS unterstützt.
- /dev jetzt als tempfs eingebunden
- FIFO wird jetzt unterstützt
- Mehr Kernsysteme werden nun ordnungsgemäß in/proc/cpuinfo angezeigt
- Weitere Verbesserungen und Fehlermeldungen, die während der ersten Testlauf
- Syscall-Verbesserungen und Fehlerbehebungen. Unterstützte syscall-Liste weiter unten.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="known-issues"></a>Bekannte Probleme
- ".." Wird nicht aufgelöst. in einigen Fällen ordnungsgemäß auf drivefs

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können. Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`FCHOWNAT`<br/>
`GETEUID`<br/>
`GETGID`<br/>
`GETRESUID`<br/>
`GETXATTR`<br/>
`PTRACE`<br/>
`SETGID`<br/>
`SETGROUPS`<br/>
`SETHOSTNAME`<br/>
`SETXATTR`<br/>
<br/>

## <a name="build-14332"></a>Build 14332

Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14332). <br/>


### <a name="fixed"></a>Fest
- Bessere resolv. conf-Generierung einschließlich Priorisieren von DNS-Einträgen
- Problem beim Verschieben von Dateien und Verzeichnissen zwischen/mnt-und nicht-/mnt-Laufwerken
- Tar-Dateien können jetzt mit symlinks erstellt werden.
- Standardmäßiges/Run/Lock-Verzeichnis bei der Instanzerstellung hinzugefügt
- Aktualisieren von/dev/null, um die richtigen stat-Informationen zurückzugeben
- Weitere Fehler beim Herunterladen während der ersten Testlauf
- Syscall-Verbesserungen und Fehlerbehebungen. Unterstützte syscall-Liste weiter unten.
- Weitere Verbesserungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie den neuen syscall-Wert, der in WSL implementiert ist. Der syscall in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a>Build 14328

Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14328). <br/>


### <a name="new-features"></a>Neue Funktionen
* Unterstützt jetzt Linux-Benutzer.  Wenn Sie bash unter Ubuntu unter Windows installieren, werden Sie aufgefordert, einen Linux-Benutzer zu erstellen.  Weitere Informationen finden Sie unter https://aka.ms/wslusers
* Der Hostname ist jetzt auf den Windows-Computernamen festgelegt.@localhost
* Weitere Informationen zu Build 14328 finden Sie unter: https://aka.ms/wip14328

### <a name="fixed"></a>Fest
* Symlink-Verbesserungen<drive> für nicht-im-Dateien
    * NPM-Installation funktioniert jetzt
    * JDK/JRE kann nun mithilfe der [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html)gefundenen Anweisungen installiert werden.
    * bekanntes Problem: symlinks funktionieren bei Windows-bereit Stellungen nicht.  Funktionen werden in einem späteren Build verfügbar sein.
* Top und htop jetzt anzeigen
* Zusätzliche Fehlermeldungen bei einigen Installationsfehlern
* Syscall-Verbesserungen und Fehlerbehebungen.  Unterstützte syscall-Liste weiter unten.
* Weitere Verbesserungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der syscalls, die eine Implementierung in WSL aufweisen.  Syscalls für diese Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.

`ACCEPT`<br/>
`ACCEPT4`<br/>
`ACCESS`<br/>
`ALARM`<br/>
`ARCH_PRCTL`<br/>
`BIND`<br/>
`BRK`<br/>
`CAPGET`<br/>
`CAPSET`<br/>
`CHDIR`<br/>
`CHMOD`<br/>
`CHOWN`<br/>
`CLOCK_GETRES`<br/>
`CLOCK_GETTIME`<br/>
`CLOCK_NANOSLEEP`<br/>
`CLONE`<br/>
`CLOSE`<br/>
`CONNECT`<br/>
`CREAT`<br/>
`DUP`<br/>
`DUP2`<br/>
`DUP3`<br/>
`EPOLL_CREATE`<br/>
`EPOLL_CREATE1`<br/>
`EPOLL_CTL`<br/>
`EPOLL_WAIT`<br/>
`EVENTFD`<br/>
`EVENTFD2`<br/>
`EXECVE`<br/>
`EXIT`<br/>
`EXIT_GROUP`<br/>
`FACCESSAT`<br/>
`FADVISE64`<br/>
`FCHDIR`<br/>
`FCHMOD`<br/>
`FCHMODAT`<br/>
`FCHOWN`<br/>
`FCHOWNAT`<br/>
`FCNTL64`<br/>
`FDATASYNC`<br/>
`FLOCK`<br/>
`FORK`<br/>
`FSETXATTR`<br/>
`FSTAT64`<br/>
`FSTATAT64`<br/>
`FSTATFS64`<br/>
`FSYNC`<br/>
`FTRUNCATE`<br/>
`FTRUNCATE64`<br/>
`FUTEX`<br/>
`GETCPU`<br/>
`GETCWD`<br/>
`GETDENTS`<br/>
`GETDENTS64`<br/>
`GETEGID`<br/>
`GETEGID16`<br/>
`GETEUID`<br/>
`GETEUID16`<br/>
`GETGID`<br/>
`GETGID16`<br/>
`GETGROUPS`<br/>
`GETPEERNAME`<br/>
`GETPGID`<br/>
`GETPGRP`<br/>
`GETPID`<br/>
`GETPPID`<br/>
`GETPRIORITY`<br/>
`GETRESGID`<br/>
`GETRESGID16`<br/>
`GETRESUID`<br/>
`GETRESUID16`<br/>
`GETRLIMIT`<br/>
`GETRUSAGE`<br/>
`GETSID`<br/>
`GETSOCKNAME`<br/>
`GETSOCKOPT`<br/>
`GETTID`<br/>
`GETTIMEOFDAY`<br/>
`GETUID`<br/>
`GETUID16`<br/>
`GETXATTR`<br/>
`GET_ROBUST_LIST`<br/>
`GET_THREAD_AREA`<br/>
`INOTIFY_ADD_WATCH`<br/>
`INOTIFY_INIT`<br/>
`INOTIFY_RM_WATCH`<br/>
`IOCTL`<br/>
`IOPRIO_GET`<br/>
`IOPRIO_SET`<br/>
`KEYCTL`<br/>
`KILL`<br/>
`LCHOWN`<br/>
`LINK`<br/>
`LINKAT`<br/>
`LISTEN`<br/>
`LLSEEK`<br/>
`LSEEK`<br/>
`LSTAT64`<br/>
`MADVISE`<br/>
`MKDIR`<br/>
`MKDIRAT`<br/>
`MKNOD`<br/>
`MLOCK`<br/>
`MMAP`<br/>
`MMAP2`<br/>
`MOUNT`<br/>
`MPROTECT`<br/>
`MREMAP`<br/>
`MSYNC`<br/>
`MUNLOCK`<br/>
`MUNMAP`<br/>
`NANOSLEEP`<br/>
`NEWUNAME`<br/>
`OPEN`<br/>
`OPENAT`<br/>
`PAUSE`<br/>
`PERF_EVENT_OPEN`<br/>
`PERSONALITY`<br/>
`PIPE`<br/>
`PIPE2`<br/>
`POLL`<br/>
`PPOLL`<br/>
`PRCTL`<br/>
`PREAD64`<br/>
`PROCESS_VM_READV`<br/>
`PROCESS_VM_WRITEV`<br/>
`PSELECT6`<br/>
`PTRACE`<br/>
`PWRITE64`<br/>
`READ`<br/>
`READLINK`<br/>
`READV`<br/>
`REBOOT`<br/>
`RECV`<br/>
`RECVFROM`<br/>
`RECVMSG`<br/>
`RENAME`<br/>
`RMDIR`<br/>
`RT_SIGACTION`<br/>
`RT_SIGPENDING`<br/>
`RT_SIGPROCMASK`<br/>
`RT_SIGRETURN`<br/>
`RT_SIGSUSPEND`<br/>
`RT_SIGTIMEDWAIT`<br/>
`SCHED_GETAFFINITY`<br/>
`SCHED_GETPARAM`<br/>
`SCHED_GETSCHEDULER`<br/>
`SCHED_GET_PRIORITY_MAX`<br/>
`SCHED_GET_PRIORITY_MIN`<br/>
`SCHED_SETAFFINITY`<br/>
`SCHED_SETPARAM`<br/>
`SCHED_SETSCHEDULER`<br/>
`SCHED_YIELD`<br/>
`SELECT`<br/>
`SEND`<br/>
`SENDMMSG`<br/>
`SENDMSG`<br/>
`SENDTO`<br/>
`SETDOMAINNAME`<br/>
`SETGID`<br/>
`SETGROUPS`<br/>
`SETHOSTNAME`<br/>
`SETITIMER`<br/>
`SETPGID`<br/>
`SETPRIORITY`<br/>
`SETREGID`<br/>
`SETRESGID`<br/>
`SETRESUID`<br/>
`SETREUID`<br/>
`SETRLIMIT`<br/>
`SETSID`<br/>
`SETSOCKOPT`<br/>
`SETTIMEOFDAY`<br/>
`SETUID`<br/>
`SETXATTR`<br/>
`SET_ROBUST_LIST`<br/>
`SET_THREAD_AREA`<br/>
`SET_TID_ADDRESS`<br/>
`SHUTDOWN`<br/>
`SIGACTION`<br/>
`SIGALTSTACK`<br/>
`SIGPENDING`<br/>
`SIGPROCMASK`<br/>
`SIGRETURN`<br/>
`SIGSUSPEND`<br/>
`SOCKET`<br/>
`SOCKETCALL`<br/>
`SOCKETPAIR`<br/>
`SPLICE`<br/>
`STAT64`<br/>
`STATFS64`<br/>
`SYMLINK`<br/>
`SYMLINKAT`<br/>
`SYNC`<br/>
`SYSINFO`<br/>
`TEE`<br/>
`TGKILL`<br/>
`TIME`<br/>
`TIMERFD_CREATE`<br/>
`TIMERFD_GETTIME`<br/>
`TIMERFD_SETTIME`<br/>
`TIMES`<br/>
`TKILL`<br/>
`TRUNCATE`<br/>
`TRUNCATE64`<br/>
`UMASK`<br/>
`UMOUNT`<br/>
`UMOUNT2`<br/>
`UNLINK`<br/>
`UNLINKAT`<br/>
`UNSHARE`<br/>
`UTIME`<br/>
`UTIMENSAT`<br/>
`UTIMES`<br/>
`VFORK`<br/>
`WAIT4`<br/>
`WAITPID`<br/>
`WRITE`<br/>
`WRITEV`<br/>
