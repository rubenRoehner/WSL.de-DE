---
title: Anmerkungen zu dieser Version für Windows-Subsystem für Linux
description: Versionshinweise für das Windows-Subsystem für Linux.  Wöchentlich aktualisiert.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, ubuntu
author: benhillis
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 36ea641e-4d49-4881-84eb-a9ca85b1cdf4
ms.custom: seodec18
ms.openlocfilehash: 3eee7ff6d1f8302e98cde84fccabf5d9113c83f2
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063628"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a>Anmerkungen zu dieser Version für Windows-Subsystem für Linux

## <a name="build-18342"></a>Build 18342
Allgemeine Windows Informationen zum Build 18342 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).

### <a name="wsl"></a>WSL
* Wir haben die Möglichkeit für Benutzer von Windows auf Linux-Dateien in einem WSL-Distribution, die hinzugefügt werden. Diese Dateien können über die Befehlszeile und auch den Windows-apps wie VSCode Datei-Explorer zugegriffen werden, usw. können mit diesen Dateien interagieren. Zugriff auf Ihre Dateien durch Navigieren zu \\ \\Wsl$\\< Distro_name >, oder sehen Sie eine Liste der ausgeführten Verteilungen durch Navigieren zu \\ \\Wsl$
* Fügen Sie zusätzliche CPU-Info-Tags hinzu, und beheben Sie Cpus_allowed [_list]-Werte [GH 2234]
* Unterstützung von Exec nicht übergeordneten Threads [GH 3800]
* Fehler beim Update der Konfiguration wird als nicht schwerwiegenden [GH 3785] behandeln.
* Aktualisieren von Binfmt um ordnungsgemäß zu behandeln, die Offsets [GH 3768]
* Aktivieren der Zuordnung Netzlaufwerke für planen 9 [GH 3854]
* Unterstützung für Windows > Linux und Linux -> Windows-Pfad-Übersetzung für bindungseinbindungen
* Erstellen Sie schreibgeschützte Abschnitte für die Zuordnungen auf geöffnete Dateien, schreibgeschützt

## <a name="build-18334"></a>Build 18334
Allgemeine Windows Informationen zum Build 18334 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).

### <a name="wsl"></a>WSL
* Ändern Sie die Möglichkeit, dass Windows-Zeitzone in eine Linux-Zeitzone [GH 3747] zugeordnet ist
* Beheben Sie Speicherverluste und Hinzufügen von neuen Funktionen für Zeichenfolgen-Übersetzung [GH 3746]
* SIGCONT auf eine Threadgroup ohne Threads ist ein nicht möglich [GH 3741] 
* Lassen Sie Socket und Epoll Dateideskriptoren in /proc/self/fd korrekt anzeigen

## <a name="build-18305"></a>Build 18305
Allgemeine Windows Informationen zum Build 18305 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).

### <a name="wsl"></a>WSL
* Pthreads verlieren den Zugriff auf Dateien aus, wenn der primäre Thread [GH 3589] beendet wird.
* TIOCSCTTY den "Force"-Parameter ignorieren soll, es sei denn, dies erforderlich ist [GH 3652]
* wsl.exe Befehlszeile Verbesserungen und Hinzufügen von import / export-Funktionalität.
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
Allgemeine Windows Informationen zum Build 18277 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).

### <a name="wsl"></a>WSL
* Beheben von "Schnittstelle nicht unterstützt"-Fehler in Build 18272 [GH 3645] eingeführt wurden
* Ignorieren Sie das Flag MNT_FORCE für Umount Syscall [GH 3605]
* Wechseln Sie WSL-Interop für die offizielle CreatePseudoConsole-API verwenden.
* Behalten Sie kein Timeoutwert bei, wenn FUTEX_WAIT neu gestartet wird

## <a name="build-18272"></a>Build 18272
Allgemeine Windows Informationen zum Build 18272 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).

### <a name="wsl"></a>WSL
* **WARNUNG:** In diesem Build, die WSL defekt ist vorliegt ein Problem. Beim Versuch, Ihre Verteilung zu starten, sehen Sie einen "Schnittstelle nicht unterstützt"-Fehler. Das Problem wurde behoben und werden in der nächsten Woche schnell Insider-Build. Wenn Sie installiert haben diese erstellen, die Sie auf den vorherigen Windows-Build mithilfe von "Wechseln Sie zu der vorherigen Version von Windows 10" in den Einstellungen zurücksetzen können -> Update und Sicherheit -> Recovery.

## <a name="build-18267"></a>Build 18267
Allgemeine Windows Informationen zum Build 18267 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).

### <a name="wsl"></a>WSL
* Korrigiert: Fehler, in denen Zombie-Prozess kann nicht kam werden und bleibt auf unbestimmte Zeit.
* WslRegisterDistribution reagiert, wenn die Fehlermeldung [GH 3592] die maximalen Länge überschreitet
* Zulassen von Fsync clientauftrags für schreibgeschützte Dateien auf DrvFs [GH 3556]
* Stellen Sie sicher, dass "/ bin" und einen Verzeichnisse vorhanden sind, vor dem erstellen symbolische Verknüpfungen in [GH 3584]
* Eine Instanz beenden-Timeoutmechanismus für WSL-Instanzen wird hinzugefügt. Das Timeout ist so eingerichtet, 15 Sekunden, was bedeutet, dass die Instanz beendet wird, 15 Sekunden, nach der letzten WSL-Prozess beendet wird. Um eine Verteilung sofort zu beenden, verwenden Sie:
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a>Build 17763 (1809)
Allgemeine Windows Informationen zum Build 17763 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).

### <a name="wsl"></a>WSL
* SetPriority Syscall Überprüfung der Berechtigung zum Ändern der gleichen Priorität der Threads [GH 1838] zu streng.
* Stellen Sie sicher, dass ausgewogene Interruptzeit für den Systemstart verwendet wird, um zu vermeiden, Zurückgeben des negativen Werte für die clock_gettime(CLOCK_BOOTTIME) [3434 ein GH.]
* Behandeln Sie symbolische Verknüpfungen im WSL Binfmt Interpreter [GH 3424]
* Eine bessere Verarbeitung von Threadgroup übergeordneten Datei Deskriptor bereinigen.
* Wechseln Sie WSL KeQueryInterruptTimePrecise statt KeQueryPerformanceCounter mit Überlauf [GH 3252]
* Fügen Sie Ptrace Mai führen zur fehlerhaften Rückgabewert Systemaufrufe [GH 1731]
* Lösung, die mehrere AF_UNIX bezogene Probleme [GH 3371]
* Korrigieren von Problem, WSL-Interop aufgrund dessen für fehl, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen [GH 3379]
* Vermeiden Sie die Verzögerung von einer Sekunde Fehler bei Loopbackverbindungen auf nicht existierende Ports [GH 3286]
* Hinzufügen von /proc/sys/fs/file-max-Stub-Datei [GH 2893]
* Genauere Informationen für die IPV6-Bereich.
* PR_SET_PTRACER-Unterstützung [GH 3053]
* Pipe-Dateisystem versehentlich löschen Epoll Edge ausgelöstes Ereignis [GH 3276]
* Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.
* Verbesserte Zombie-Unterstützung [GH 1353]
* Fügen Sie wsl.conf Einträge zum Steuern der Windows-interopverhalten [GH 1493]
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* Korrektur für Getsockname nicht immer Zurückgeben von UNIX-Socket-Familientyp [GH 1774]
* Hinzufügen von Unterstützung für TIOCSTI [GH 1863]
* Nicht blockierenden Sockets gerade eine Verbindung herstellen sollte EAGAIN für Schreibzugriff Versuche [GH 2846] zurückgegeben.
* Unterstützen von Interop auf bereitgestellten VHDs [GH 3246, 3291]
* Beheben von berechtigungsüberprüfungen Problem Stammordner [GH 3304]
* Eingeschränkte Unterstützung für TTY Tastatur Ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.
* Windows-Anwendungsbenutzeroberflächen sollte ausgeführt werden, auch wenn im Hintergrund gestartet.
* Fügen Sie die Wsl -u "oder"--Benutzer Option [GH 1203]
* WSL starten Probleme zu beheben, wenn Schnellstart aktiviert ist [GH 2576]
* UNIX-Sockets müssen getrennt Peer-Anmeldeinformationen [GH 3183] beibehalten werden sollen.
* Nicht blockierende Unix-Sockets auf unbestimmte Zeit führt zu dem EAGAIN [GH 3191]
* Fall = off ist der neue Standard-Drvfs einbinden Typ [GH 2937, 3212, 3328]
    * Finden Sie unter [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) für Weitere Informationen.
* Hinzufügen von Wslconfig / zum Beenden Verteilungen zu beenden.
* Beheben Sie ein Problem mit dem Shell-Kontext WSL Menüeinträge, die Pfade mit Leerzeichen nicht ordnungsgemäß behandelt werden.
* Machen Sie die Groß-/Kleinschreibung pro Verzeichnis als ein erweitertes Attribut
* ARM64: Cache-Wartungsvorgänge zu emulieren. Beheben [Dotnet Problem](https://github.com/dotnet/core/issues/1561).
* DrvFs: unescape-Zeichen im privaten Bereich entsprechen, die nur auf ein Escapezeichen.
* Beheben Sie deaktiviert ein Fehler in ELF Parser-Interpreter eine längenüberprüfung [GH 3154]
* WSL absolute Zeitgeber mit einer Uhrzeit in der Vergangenheit werden [GH 3091] nicht ausgelöst werden.
* Vergewissern Sie sich neu erstellte Analysepunkte als solche in das übergeordnete Verzeichnis aufgeführt sind.
* Erstellen Sie Groß-/ Kleinschreibung Verzeichnisse werden atomar in DrvFs.
* Korrigiert: zusätzliche Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist. [GH 2712]
* Festen WSL starten Fehler auf, wenn UMCI aktiviert ist. [GH 3020]
* Fügen Sie die Explorer-Kontextmenü zum Starten von WSL [GH 437, 603 1836] hinzu. Zu verwenden, halten die UMSCHALTTASTE gedrückt, und mit der rechten Maustaste in einem Explorer-Fenster.
* Beheben von Unix-Socket nicht blockierende Verhalten [GH 2822, 3100]
* Fix hängende NETLINK-Befehl aus, wie in GH 2026 angegeben.
* Hinzufügen von Unterstützung für Mount-Weitergabeflags [GH 2911].
* Problem mit der truncate nicht zu Inotify Ereignisse [GH 2978] behoben.
* Fügen Sie hinzu – Exec-Option für wsl.exe um eine einzelne Binärdatei ohne eine Shell aufzurufen.
* Fügen Sie hinzu – die Verteilungsoption für wsl.exe-Distribution, die eine bestimmte Auswahl.
* Eingeschränkte Unterstützung für "dmesg". Anwendungen können jetzt in "dmesg" protokollieren. WSL-treiberprotokolle eingeschränkte Informationen zu "dmesg". Dies kann in Zukunft erweitert werden, um weitere Informationen/Diagnosedaten aus dem Treiber durchzuführen.
    * Hinweis: "dmesg" wird über derzeit unterstützt die `/dev/kmsg` Geräteschnittstelle. `syslog` Syscall-Schnittstelle ist noch nicht unterstützt. Und natürlich einige von der `dmesg` Befehlszeilenoptionen wie z. B. `-S`, `-C` funktionieren nicht.
* Standard-Gruppen-ID und Modus der seriellen Geräten nativ [GH 3042] entsprechend zu ändern
* DrvFs unterstützt jetzt erweiterte Attribute.
    * Hinweis: DrvFs gelten einige Einschränkungen auf den Namen der erweiterten Attribute. Einige Zeichen (z. B. '/', ':' und '\*") nicht zulässig sind, und erweitert Attributnamen wird nicht in der Groß-/ Kleinschreibung auf DrvFs

## <a name="build-18252-skip-ahead"></a>Erstellen von 18252 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 18252 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).

### <a name="wsl"></a>WSL
* Verschieben Sie Init "und" Bsdtar Binärdateien aus Lxssmanager Dll und in einem separaten Tools-Ordner
* Beheben von Rennen um Dateideskriptor geschlossen, wenn CLONE_FILES verwenden
* Behandeln von optionalen Feldern in /proc/pid/mountinfo beim Übersetzen von DrvFs Pfade
* Können Sie DrvFs Mknod ohne metadatenunterstützung für S_IFREG erfolgreich ausgeführt werden
* ReadOnly-Dateien, die auf DrvFs erstellt sollte das Readonly-Attribut [GH 3411] festgelegt sein.
* Hinzufügen von /sbin/mount.drvfs-Hilfsprogramm zum Behandeln von DrvFs einbinden
* Verwenden Sie Umbenennen von POSIX in DrvFs.
* Ermöglichen Sie Pfad Übersetzung auf Volumes ohne einer Volume-GUID.

## <a name="build-17738-fast"></a>Build 17738 (Fast)
Allgemeine Windows Informationen zum Build 17738 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).

### <a name="wsl"></a>WSL
* SetPriority Syscall Überprüfung der Berechtigung zum Ändern der gleichen Priorität der Threads [GH 1838] zu streng.
* Stellen Sie sicher, dass ausgewogene Interruptzeit für den Systemstart verwendet wird, um zu vermeiden, Zurückgeben des negativen Werte für die clock_gettime(CLOCK_BOOTTIME) [3434 ein GH.]
* Behandeln Sie symbolische Verknüpfungen im WSL Binfmt Interpreter [GH 3424]
* Eine bessere Verarbeitung von Threadgroup übergeordneten Datei Deskriptor bereinigen.

## <a name="build-17728-fast"></a>Erstellen von 17728 (Fast)
Allgemeine Windows Informationen zum Build 17728 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).

### <a name="wsl"></a>WSL
* Wechseln Sie WSL KeQueryInterruptTimePrecise statt KeQueryPerformanceCounter mit Überlauf [GH 3252]
* Fügen Sie Ptrace Mai führen zur fehlerhaften Rückgabewert Systemaufrufe [GH 1731]
* Lösung, die eine Reihe von AF_UNIX Bezug Probleme [GH 3371]
* Korrigieren von Problem, WSL-Interop aufgrund dessen für fehl, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen [GH 3379]

## <a name="build-18204-skip-ahead"></a>Erstellen von 18204 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 18204 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).

### <a name="wsl"></a>WSL
* Übergeben von Dateisystem Inadvertenly Epoll Edge ausgelöstes Ereignis [GH 3276] deaktivieren
* Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.

## <a name="build-17723-fast"></a>Erstellen von 17723 (Fast)
Allgemeine Windows Informationen zum Build 17723 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).

### <a name="wsl"></a>WSL
* Vermeiden Sie die Verzögerung von einer Sekunde Fehler bei Loopbackverbindungen auf nicht existierende Ports [GH 3286]
* Hinzufügen von /proc/sys/fs/file-max-Stub-Datei [GH 2893]
* Genauere Informationen für die IPV6-Bereich.
* PR_SET_PTRACER-Unterstützung [GH 3053]
* Übergeben von Dateisystem Inadvertenly Epoll Edge ausgelöstes Ereignis [GH 3276] deaktivieren
* Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.

## <a name="build-17713"></a>Build 17713
Allgemeine Windows Informationen zum Build 17713 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).

### <a name="wsl"></a>WSL
* Verbesserte Zombie-Unterstützung [GH 1353]
* Fügen Sie wsl.conf Einträge zum Steuern der Windows-interopverhalten [GH 1493]
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* Korrektur für Getsockname nicht immer Zurückgeben von UNIX-Socket-Familientyp [GH 1774]
* Hinzufügen von Unterstützung für TIOCSTI [GH 1863]
* Nicht blockierenden Sockets gerade eine Verbindung herstellen sollte EAGAIN für Schreibzugriff Versuche [GH 2846] zurückgegeben.
* Unterstützen von Interop auf bereitgestellten VHDs [GH 3246, 3291]
* Beheben von berechtigungsüberprüfungen Problem Stammordner [GH 3304]
* Eingeschränkte Unterstützung für TTY Tastatur Ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.
* Windows-Anwendungsbenutzeroberflächen sollte ausgeführt werden, auch wenn im Hintergrund gestartet.

## <a name="build-17704"></a>Build 17704
Allgemeine Windows Informationen zum Build 17704 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).

### <a name="wsl"></a>WSL
* Fügen Sie die Wsl -u "oder"--Benutzer Option [GH 1203]
* WSL starten Probleme zu beheben, wenn Schnellstart aktiviert ist [GH 2576]
* UNIX-Sockets müssen getrennt Peer-Anmeldeinformationen [GH 3183] beibehalten werden sollen.
* Nicht blockierende Unix-Sockets auf unbestimmte Zeit führt zu dem EAGAIN [GH 3191]
* Fall = off ist der neue Standard-Drvfs einbinden Typ [GH 2937, 3212, 3328]
    * Finden Sie unter [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) für Weitere Informationen.
* Hinzufügen von Wslconfig / zum Beenden Verteilungen zu beenden.

## <a name="build-17692"></a>Build 17692
Allgemeine Windows Informationen zum Build 17692 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).

### <a name="wsl"></a>WSL
* Beheben Sie ein Problem mit dem Shell-Kontext WSL Menüeinträge, die Pfade mit Leerzeichen nicht ordnungsgemäß behandelt werden.
* Machen Sie die Groß-/Kleinschreibung pro Verzeichnis als ein erweitertes Attribut
* ARM64: Cache-Wartungsvorgänge zu emulieren. Beheben [Dotnet Problem](https://github.com/dotnet/core/issues/1561).
* DrvFs: unescape-Zeichen im privaten Bereich entsprechen, die nur auf ein Escapezeichen.

## <a name="build-17686"></a>Build 17686
Allgemeine Windows Informationen zum Build 17686 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).

### <a name="wsl"></a>WSL
* Beheben Sie deaktiviert ein Fehler in ELF Parser-Interpreter eine längenüberprüfung [GH 3154]
* WSL absolute Zeitgeber mit einer Uhrzeit in der Vergangenheit werden [GH 3091] nicht ausgelöst werden.
* Vergewissern Sie sich neu erstellte Analysepunkte als solche in das übergeordnete Verzeichnis aufgeführt sind.
* Erstellen Sie Groß-/ Kleinschreibung Verzeichnisse werden atomar in DrvFs.

## <a name="build-17677"></a>Build 17677
Allgemeine Windows Informationen zum Build 17677 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).

### <a name="wsl"></a>WSL
* Korrigiert: zusätzliche Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist. [GH 2712]
* Festen WSL starten Fehler auf, wenn UMCI aktiviert ist. [GH 3020]

## <a name="build-17666"></a>Build 17666
Allgemeine Windows Informationen zum Build 17666 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).

### <a name="wsl"></a>WSL
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a>WARNUNG: Es liegt ein Problem verhindert, dass WSL auf einige AMD Chipsätzen [GH 3134] ausgeführt wird. Ein Fix ist bereit und machen die Möglichkeit, den Branch Insider-Build.
* Fügen Sie die Explorer-Kontextmenü zum Starten von WSL [GH 437, 603 1836] hinzu. Hold-Schicht und mit der rechten Maustaste in einem Explorer-Fenster zu verwenden.
* Beheben von Unix-Socket nicht blockierende Verhalten [GH 2822, 3100]
* Fix hängende NETLINK-Befehl aus, wie in GH 2026 angegeben.
* Hinzufügen von Unterstützung für Mount-Weitergabeflags [GH 2911].
* Problem mit der truncate nicht zu Inotify Ereignisse [GH 2978] behoben.
* Fügen Sie hinzu – Exec-Option für wsl.exe um eine einzelne Binärdatei ohne eine Shell aufzurufen.
* Fügen Sie hinzu – die Verteilungsoption für wsl.exe-Distribution, die eine bestimmte Auswahl.

## <a name="build-17655-skip-ahead"></a>Erstellen von 17655 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 17655 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Eingeschränkte Unterstützung für "dmesg". Anwendungen können jetzt in "dmesg" protokollieren. WSL-treiberprotokolle eingeschränkte Informationen zu "dmesg". Dies kann in Zukunft erweitert werden, um weitere Informationen/Diagnosedaten aus dem Treiber durchzuführen.
    * Hinweis: "dmesg" wird über derzeit unterstützt die `/dev/kmsg` Geräteschnittstelle. `syslog` Sycall-Schnittstelle ist noch nicht unterstützt. Und natürlich einige von der `dmesg` Befehlszeilenoptionen wie z. B. `-S`, `-C` funktionieren nicht.
* Problem behoben, Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist. [GH 2712]

## <a name="build-17639-skip-ahead"></a>Erstellen von 17639 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 17639 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Standard-Gruppen-ID und Modus der seriellen Geräten nativ [GH 3042] entsprechend zu ändern
* DrvFs unterstützt jetzt erweiterte Attribute.
    * Hinweis: DrvFs gelten einige Einschränkungen auf den Namen der erweiterten Attribute. Insbesondere einige Zeichen (wie '/', ':' und '\*") nicht zulässig sind, und erweiterte Attributnamen wird nicht in der Groß-/ Kleinschreibung auf DrvFs

## <a name="build-17133-fast"></a>Erstellen von 17133 (Fast)
Allgemeine Windows Informationen zum Build 17133 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).

### <a name="wsl"></a>WSL
* Korrektur für hänger in WSL. [GH 3039, 3034]

## <a name="build-17128-fast"></a>Erstellen von 17128 (Fast)
Allgemeine Windows Informationen zum Build 17128 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).

### <a name="wsl"></a>WSL
* Keine

## <a name="build-17627-skip-ahead"></a>Erstellen von 17627 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 17627 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).

### <a name="wsl"></a>WSL
* Hinzufügen von Unterstützung für die Pi-fähigen Futex-Vorgänge. [GH 1006]
    * Beachten Sie, dass Prioritäten nicht aktuell ein unterstütztes Feature von WSL sind daher Einschränkungen bestehen, aber die Standardverwendung muss aufgehoben werden.
* Windows-Firewall-Unterstützung für die WSL-Prozesse. [GH 1852]
    * Damit können die WSL verarbeiten, z. B. Python an einem beliebigen Port lauschen, verwenden Sie die Eingabeaufforderung mit erhöhten Windows:
```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```
    * Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)
* Berücksichtigen Sie bei Verwendung von wsl.exe Standardshell des Benutzers. [GH 2372]
* Melden Sie alle Netzwerkschnittstellen, als Ethernet. [GH 2996]
* Eine bessere Verarbeitung von beschädigt/etc/passwd-Datei. [GH 3001]

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17618-skip-ahead"></a>Erstellen von 17618 (jetzt überspringen)
Allgemeine Windows Informationen zum Build 17618 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).

### <a name="wsl"></a>WSL
* Einführen von Pseudoconsole-Funktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].
* Die ältere Installationsmechanismus (lxrun.exe) wurde als veraltet markiert. Die unterstützte Mechanismus für die Installation von Verteilungen erfolgt über den Microsoft Store.

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17110"></a>Build 17110
Allgemeine Windows Informationen zum Build 17110 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).

### <a name="wsl"></a>WSL
* Zulassen Sie/Init von Windows [GH 2928] beendet werden soll.
* DrvFs jetzt pro Verzeichnis Groß-/Kleinschreibung wird standardmäßig verwendet (entspricht der "Fall Dir =" Bereitstellungsoption).
    * Mithilfe von "Case Force =" (das alte Verhalten) erfordert einen Registrierungsschlüssel festlegen. Führen Sie den folgenden Befehl zum Aktivieren "Fall Force =" Wenn Sie sie verwenden möchten: Reg hinzufügen HKLM\SYSTEM\CurrentControlSet\Services\lxss/v DrvFsAllowForceCaseSensitivity/t REG_DWORD/d 1
    * Wenn Sie vorhandene Verzeichnisse mit WSL erstellt werden, in früheren Version von Windows die Groß-/Kleinschreibung beachtet werden müssen haben, "fsutil.exe" verwenden, die um Groß-/ Kleinschreibung zu markieren: fsutil.exe Datei Setcasesensitiveinfo <path> aktivieren
* Zeichenfolgenende auf NULL aus dem Uname Syscall zurückgegeben.

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17107"></a>Build 17107
Allgemeine Windows Informationen zum Build 17107 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).

### <a name="wsl"></a>WSL
* Unterstützen Sie TCSETSF und TCSETSW für master Pty-Endpunkte [GH 2552] an.
* Interop-Prozesse gleichzeitig starten kann dazu führen, dass EINVAL [GH 2813].
* Beheben Sie PTRACE_ATTACH zum Anzeigen des Status der entsprechenden Ablaufverfolgung in /proc/pid/status.
* Fix Race, in denen kurzlebige Prozesse mit CLEARTID sowohl SETTID Flags geklont, konnte beenden, ohne die TID-Adresse löschen.
* Beim Aktualisieren der Linux-Dateisystemverzeichnisse beim aus einem Build vor – 17093 verschieben, wird eine Meldung angezeigt. Weitere Informationen zu den 17093 dateisystemänderungen, finden Sie unter den Versionshinweisen für [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17101"></a>Build 17101
Allgemeine Windows Informationen zum Build 17101 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).

### <a name="wsl"></a>WSL
* Unterstützung für Signalfd. [GH 129]
* Unterstützung von Dateinamen, NTFS ungültige Zeichen durch Codierung als private Unicode-Zeichen enthält. [GH 1514]
* Automatische Bereitstellung erfolgt ein Fallback auf nur-Lese beim Schreiben nicht unterstützt wird. [GH 2603]
* Ermöglichen Sie Einfügen der Unicode-Ersatzpaare (z. B. Emoji Zeichen). [GH 2765]
* Pseudo-Dateien in/proc und /sys soll gelesen und schreiben kann jetzt von Select "," Abruf "," Epoll, Et Al. [GH 2838]
* Korrigieren von Problem, Service in Endlosschleife zu wechseln aufgrund dessen, wenn die Registrierung manipuliert wurde, oder beschädigt ist.
* Beheben Sie Netlink Nachrichten mit neueren (upstream 4.14) Version von iproute2 funktioniert.

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17093"></a>Build 17093
Allgemeine Windows Informationen zum Build 17093 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).

#### <a name="important"></a>Wichtig:
Wenn WSL zum ersten Mal nach dem Upgrade auf diesen Build gestartet wird, muss sie ein Upgrade der Linux-Dateisystemverzeichnisse Arbeit ausführen. Dieser Vorgang kann mehrere Minuten dauern, sodass WSL angezeigt werden kann, zu einem verlangsamten start. Dies sollte nur auftreten, nachdem für jede Verteilung Sie aus dem Store installiert haben.
* Verbesserte Unterstützung für die Groß-/Kleinschreibung in DrvFs.
    * DrvFs unterstützt jetzt pro Verzeichnis Groß-/Kleinschreibung beachtet. Dies ist ein neues Flag, das festgelegt werden kann Verzeichnisse, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen behandelt werden sollen, Groß-/ Kleinschreibung, dadurch können auch Windows-Anwendungen zum ordnungsgemäß Öffnen von Dateien, die sich nur durch Fall unterscheiden.
    * DrvFs hat neue Bereitstellungsoption Steuerung der Groß-/Kleinschreibung in einer Basis pro Verzeichnis
        * Fall = erzwingen: alle Verzeichnisse werden in der Groß-/ Kleinschreibung (mit Ausnahme der Stamm des Laufwerks) behandelt. Neue mit WSL erstellt Verzeichnisse werden Groß-/ Kleinschreibung markiert. Dies ist das Legacyverhalten mit Ausnahme von markieren die neuen Verzeichnisse Groß-/Kleinschreibung beachtet.
        * Fall Dir =: behandelt nur die Verzeichnisse mit dem Flag pro Verzeichnis Groß-/Kleinschreibung wie Groß-/ Kleinschreibung beachtet. andere Verzeichnisse, die Groß-/Kleinschreibung beachtet werden. Neue mit WSL erstellt Verzeichnisse werden Groß-/ Kleinschreibung markiert.
        * Fall = off: behandelt nur die Verzeichnisse mit dem Flag pro Verzeichnis Groß-/Kleinschreibung wie Groß-/ Kleinschreibung beachtet. andere Verzeichnisse, die Groß-/Kleinschreibung beachtet werden. Neue Verzeichnisse mit WSL erstellt wurden, werden als Groß-/Kleinschreibung markiert.
    * Hinweis: durch WSL in früheren Versionen erstellten Verzeichnisse keine dieses Flag festgelegt, sodass nicht behandelt wird Groß-/ Kleinschreibung bei der Verwendung, die "Fall Dir =" Option. Eine Möglichkeit, dieses Flag festgelegt wird, auf vorhandene Verzeichnisse wird bald verfügbar sein.
    * Beispiel für die Bereitstellung mit den folgenden Optionen (für vorhandene Laufwerke, Sie müssen zuerst die Einbindung aufheben, bevor Sie mit verschiedenen Optionen bereitstellen können): Sudo Mount -t Drvfs "c:" / Mnt/C - e/a Fall Dir =
    * Case-vorerst = Force ist immer noch die Standardoption. Dies wird in Fall geändert Dir in der Zukunft =.
* Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, beim Einbinden von DrvFs, z. B.: "sudo" einbinden -t Drvfs //server/share /mnt/share
* WSL verarbeitet nun die Datei/etc/fstab beim Start der Instanz [GH 2636].
    * Dies ist möglich, vor dem Bereitstellen von automatisch DrvFs-Laufwerken. alle Laufwerke, die bereits von "fstab" eingebunden wurden werden nicht automatisch erneut bereitgestellt werden können Sie den Bereitstellungspunkt für bestimmte Laufwerke zu ändern.
    * Dieses Verhalten kann mithilfe von wsl.conf deaktiviert werden.
* Die Bereitstellung, Mountinfo Mountstats Dateien in/proc Escapesonderzeichen ordnungsgemäß wie umgekehrte Schrägstriche und Leerzeichen [GH 2799]
* Spezielle Dateien, die mit DrvFs z. B. WSL symbolischer Verknüpfungen oder Fifos und Sockets erstellt wird, wenn Metadaten aktiviert ist, können jetzt kopiert und von Windows verschoben werden.

#### <a name="wsl-is-more-configurable-with-wslconf"></a>WSL ist mit wsl.conf mehr konfigurierbar.
Wir haben eine Methode für das bestimmte Funktionen automatisch in WSL zu konfigurieren, die jedes Mal, wenn Sie das Subsystem starten angewendet werden hinzugefügt. Dazu gehören Optionen für die automatische Bereitstellung und Konfiguration des Netzwerks. Weitere Informationen finden sie in unserem Blogbeitrag unter: https://aka.ms/wslconf

#### <a name="afunix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a>AF_UNIX ermöglicht das WebSocket-Verbindungen zwischen Linux-Prozessen für WSL und native Windows-Prozesse
WSL und Windows-Anwendungen können jetzt über Unix-Sockets miteinander kommunizieren. Angenommen Sie, Sie möchten das Ausführen eines Diensts in Windows und sowohl Windows als auch WSL-apps zur Verfügung stellen. Das ist möglich, mit Unix-Sockets. Lesen Sie mehr in unserem Blog unter Posten https://aka.ms/afunixinterop

### <a name="wsl"></a>WSL
* Unterstützung von mmap() mit MAP_NORESERVE [GH 121, 2784]
* Unterstützen Sie CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]
* Behandeln von nicht-SIGCHLD Beendigungssignal in Klon [GH 121, 2781]
* Stub-/proc/sys/fs/inotify/max_user_instances und /proc/sys/fs/inotify/max_user_watches [GH 1705]
* Fehler beim Laden der ELF-Binärdateien, die Load-Header mit nicht-NULL-Offsets [GH 1884] enthalten.
* 0 (null) nicht mehr nachfolgende Seite Bytes beim Laden von Bildern.
* Reduzieren von Fällen, in denen Execve im Hintergrund Prozess beendet wird

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17083"></a>Build 17083
Allgemeine Windows Informationen zum Build 17083 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).

### <a name="wsl"></a>WSL
* Feste fehlerüberprüfung im Zusammenhang mit Epoll [GH 2798, 2801, 2857]
* Feste hängt, wenn es sich bei deaktiviert ASLR [GH 1185, 2870]
* Stellen Sie sicher, dass Vorgänge für "mmap" atomic [GH 2732] angezeigt werden

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17074"></a>Build 17074
Allgemeine Windows Informationen zum Build 17074 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).

### <a name="wsl"></a>WSL
* Feste Speicherformat DrvFs Metadaten [GH 2777] </br>
**Wichtig:** DrvFs-Metadaten erstellt, bevor Sie diesen Build nicht ordnungsgemäß oder überhaupt nicht angezeigt wird. Verwenden Sie zum Beheben betroffener Dateien Chmod und Chown, um die Metadaten erneut anzuwenden.
* Korrigiert: Probleme mit mehreren Signale und neu startbar Syscalls.

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17063"></a>Build 17063
Allgemeine Windows Informationen zum Build 17063 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).

### <a name="wsl"></a>WSL
* DrvFs unterstützt zusätzliche Linux-Metadaten. Dies ermöglicht das Festlegen der Besitzer und den Modus der Dateien, indem Sie Chmod/Chown und die Erstellung von speziellen Dateien wie Fifos, Unix-Sockets und Device-Dateien. Dies ist standardmäßig für jetzt deaktiviert, da er noch experimentell ist.
**Hinweis**:  Ein Fehler wurde in den Metadaten-Format von DrvFs verwendet. Metadaten für diesen Build für Experimente funktioniert, zwar werden zukünftige Builds nicht ordnungsgemäß Metadaten, die von diesem Build erstellte gelesen werden.  Müssen Sie möglicherweise Besitzer für die geänderten Dateien manuell aktualisieren und auf Geräten mit einem benutzerdefinierten Geräte-ID werden neu erstellt werden.

  Um DrvFs bereitstellen, mit der Metadatenoption zu aktivieren (um es zu einer vorhandenen Bereitstellung aktivieren, Sie müssen zunächst aufheben):

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  Linux-Berechtigungen werden als zusätzliche Metadaten zu der Datei hinzugefügt; Sie wirken sich nicht auf die Windows-Berechtigungen.  Beachten Sie, dass eine Datei mit einem Windows-Editor bearbeiten, die Metadaten entfernen kann. In diesem Fall wird die Datei auf die Standardberechtigungen zurückgesetzt.

* Hinzugefügte Mount-Optionen um DrvFs für Dateien ohne Metadaten.
  * UID: die Benutzer-ID für den Besitzer aller Dateien verwendet.
  * Gruppen-ID: die Gruppen-ID für den Besitzer aller Dateien verwendet.
  * "umask": eine oktale Maske von Berechtigungen für alle Dateien und Verzeichnisse ausschließen.
  * fMask: eine oktale Maske von Berechtigungen für alle regulären Dateien ausschließen.
  * Dmask: eine oktale Maske von Berechtigungen für alle Verzeichnisse ausschließen.

  Zum Beispiel:
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  Kombinieren Sie mit der Metadatenoption ", geben Sie die Standardberechtigungen für Dateien ohne Metadaten.

* Eingeführt, eine neue Umgebungsvariable `WSLENV`, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32-ausgetauscht werden.

  Zum Beispiel:

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  `WSLENV` ist eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozesse von Win32- oder Win32-Prozesse WSL aufgenommen werden kann.  Jede Variable kann als Suffix versehen werden, mit einem Schrägstrich, gefolgt von Flags, die angeben, wie diese umgesetzt werden können.
  * p: Der Wert ist ein Pfad, der zwischen WSL-Pfade und Pfade der Win32-übersetzt werden soll.
  * l: Der Wert ist eine Liste von Pfaden an. In WSL ist es sich um eine durch Doppelpunkte getrennte Liste. In Win32 ist es sich um eine durch Semikolons getrennte Liste.
  * u: Der Wert darf nur enthalten sein beim Aufrufen von WSL über Win32
  * w: Der Wert darf nur enthalten sein beim Aufrufen von Win32 von WSL

  Sie können festlegen, `WSLENV` in bashrc oder die benutzerdefinierte Windows-Umgebung für den Benutzer.

* Drvfs Mounts behält ordnungsgemäß Zeitstempel Tar, cp -p (GH 1939)
* Drvfs Symlinks melden die richtige Größe (GH 2641)
* Lese-/Schreibzugriff funktioniert bei sehr großen e/a-Größen (GH 2653)
* Waitpid funktioniert mit Gruppen IDs (GH 2534)
* erheblich verbesserte "mmap" Leistung für große Reserve-Regionen. verbessert die Leistung der Ghc (GH 1671)
* Persönlichkeit für READ_IMPLIES_EXEC unterstützt werden; Korrekturen Maxima und Clisp (GH 1185)
* Mprotect unterstützt PROT_GROWSDOWN; Korrekturen Clisp (GH 1128)
* Seite im Fehler enthaltenen Updates overcommit Modus; Korrekturen Sbcl (GH 1128)
* Klonen unterstützt mehr Kombinationen der flags
* Auswählen/Epoll Epoll-Dateien (zuvor keine Aktion) zu unterstützen.
* Benachrichtigen Sie Ptrace von nicht implementierte Syscalls.
* Ignorieren Sie Schnittstellen, die nicht aktiv, beim Generieren von "resolv.conf" Nameservers [GH 2694 sind]
* Auflisten von Netzwerkschnittstellen ohne physische Adresse. [GH 2685]
* Zusätzliche Fehlerbehebungen und Verbesserungen.

### <a name="linux-tools-available-to-developers-on-windows"></a>Linux-Tools für Entwickler für Windows

* Windows-Befehlszeile Toolkette enthält Bsdtar (Tar) und Curl.
  Lesen [diesen Blog](https://aka.ms/tarcurlwindows) erfahren mehr über das Hinzufügen dieser zwei neue Tools und wie sie die entwicklererfahrung für Windows strukturiert sind.

*   `AF_UNIX` ist in der Windows-Insider-SDK (17061 und höher) verfügbar.
  Lesen [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) erfahren Sie mehr über `AF_UNIX` und wie Entwickler Windows sie verwenden können.

### <a name="console"></a>Console
* Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.


## <a name="build-17046"></a>Build 17046

Allgemeine Windows Informationen zum Build 17046 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).

### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Können Sie Prozesse, ohne eine aktive Terminaldienste ausgeführt werden. [GH 709, 1007, 1511, 2252, 2391, et al.]
- Eine bessere Unterstützung für CLONE_VFORK und CLONE_VM zu erhalten. [GH 1878, 2615]
- Überspringen Sie TDI-Filtertreiber WSL networking Vorgänge. [GH 1554]
- DrvFs erstellt NT symbolische Verknüpfungen, wenn bestimmte Bedingungen erfüllt sind. [GH 353, 1475, 2602]
    - Das Ziel des Links relativ sein muss, muss keine Bereitstellungspunkte oder symbolische Verknüpfungen überschreiten und muss vorhanden sein.
    - Der Benutzer benötigen SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (Dies müssen Sie normalerweise wsl.exe mit erhöhten Rechten starten), es sei denn, der Entwicklermodus aktiviert ist.
    - In allen anderen Fällen wird DrvFs weiterhin WSL symbolische Verknüpfungen erstellt.
- Ermöglichen Sie die mit erhöhten Rechten und ohne erhöhte Rechte WSL-Instanzen gleichzeitig ausgeführt werden.
- Unterstützung von /proc/sys/kernel/yama/ptrace_scope
- Fügen Sie Wslpath dazu WSL <> – Windows-Pfad-Konvertierungen. [GH 522, 1243, 1834, 2327, et al.]
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a>Console
- Keine Reparaturen.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.


## <a name="build-17040"></a>Build 17040

Allgemeine Windows Informationen zum Build 17040 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Keine Fehlerbehebungen seit 17035.

#### <a name="console"></a>Console
- Keine Fehlerbehebungen seit 17035.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17035"></a>Build 17035

Allgemeine Windows Informationen zum Build 17035 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Zugreifen auf Dateien auf DrvFs konnte mit dem EINVAL gelegentlich fehl. [GH 2448]

#### <a name="console"></a>Console
- Einige Farbe verloren gehen, beim Einfügen/Löschen von Zeilen im VT-Modus.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17025"></a>Build 17025

Allgemeine Windows Informationen zum Build 17025 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Starten Sie in einer neuen Gruppe für Vordergrund-Prozess [GH 1653, 2510] erste Prozesse.
- SIGHUP Delivery behebt [GH 2496].
- Standardname für die virtuellen Bridge zu generieren, wenn kein [GH 2497].
- Implementieren Sie /proc/sys/kernel/random/boot_id [GH 2518].
- Mehr interop Stdout/Stderr-Pipe behoben.
- Stub-Syncfs Systemaufruf.

#### <a name="console"></a>Console
- Korrigieren der Eingabe VT-Übersetzung für Drittanbieter-Konsolen [GH 111]

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="build-17017"></a>Build 17017

Allgemeine Windows Informationen zum Build 17017 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ignorieren Sie die leere ELF-Anwendung-Header [GH 330].
- LxssManager zum Erstellen von WSL-Instanzen für nicht interaktive Benutzer zuzulassen (ssh und geplante Tasks-Unterstützung) [GH 777 1602].
- Win32-Unterstützung WSL > WSL ("Einführung")-Szenarios [GH 1228] ->.
- Eingeschränkte Unterstützung für die Beendigung der Konsolen-apps, die über Interop [GH 1614] aufgerufen.
- Mount-Supportoptionen für Devpts [GH 1948].
- Ptrace untergeordneten Start [GH 2333] blockiert.
- EPOLLET fehlen einige Ereignisse [GH 2462].
- Geben Sie weitere Daten für PTRACE_GETSIGINFO zurück.
- Getdents mit Lseek gibt falsche Ergebnisse.
- Beheben Sie einige Win32-Interop-app-Abstürze, warten auf Eingabe für eine Pipe, die keine Daten mehr.
- O_ASYNC-Unterstützung für tty/Pty-Dateien.
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests werden durchgeführt.

## <a name="fall-creators-update"></a>Fall Creators Update

## <a name="build-16288"></a>Build 16288

Allgemeine Windows Informationen zum Build 16288 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ordnungsgemäß zu initialisieren Sie und zu melden Sie, Uid und Gid-Modus für Socket Dateideskriptoren [GH 2490]
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16278"></a>Build 16278

Allgemeine Windows Informationen zum Build 162738 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Aufheben Sie explizit zugeordnete Ansichten der Abschnitte der Datei, wenn LX MM Wiederherstellungsoptionen [GH 2415] liegen.
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16275"></a>Build 16275

Allgemeine Windows Informationen zum Build 162735 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Keine WSL im Zusammenhang mit Änderungen in dieser Version.

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Keine Änderung seit 16273

## <a name="build-16273"></a>Build 16273

Allgemeine Windows Informationen zum Build 16273 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Ein Problem wurde behoben, bei dem gemeldet DrvFs manchmal des falschen Typs für Verzeichnisse [GH 2392]
- Zulassen der Erstellung von NETLINK_KOBJECT_UEVENT Sockets Programme Blockierung aufheben, Uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]
- Hinzufügen von Unterstützung für nicht blockierende connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]
- Implementieren Sie CLONE_FS Klonen Aufruf Systemflag [GH 2242]
- Beheben von Problemen hinsichtlich der Behandlung von nicht Registerkarten oder Anführungszeichen ordnungsgemäß in NT-Interop [GH 1625, 2164]
- Zugriff verweigert, Fehler beim Versuch, WSL neu starten [GH 651, 2095]-Instanzen zu beheben
- Implementieren Sie Futex FUTEX_REQUEUE und FUTEX_CMP_REQUEUE Vorgänge [GH 2242]
- Korrigieren Sie die Berechtigungen für verschiedene SysFs-Dateien [GH 2214]
- Beheben von Haskell Stack Absturz während des Setups [GH 2290]
- Implementieren von Binfmt_misc 'C' ' O' und 'P' Flags [GH 2103]
- Hinzufügen von /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]
- Hinzufügen von teilweise Unterstützung für Ioprio_set Systemaufruf [GH 498]
- Stub-SO_REUSEPORT und Hinzufügen von Unterstützung für SO_PASSCRED für Netlink Sockets [GH 69]
- Verschiedene Fehlercodes aus RegisterDistribuiton zurück, wenn derzeit eine Verteilung wird installiert oder deinstalliert.
- Aufheben der Registrierung, der teilweise installierten WSL Verteilungen über wslconfig.exe zulassen
- Beheben Sie die Python-Socket Test hängt vom udp::msg_peek
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Tests insgesamt: 1904<br/>
Gesamtzahl von übersprungenen Tests: 209<br/>
Fehler beim von insgesamt: 229<br/>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a>Build 16257

Allgemeine Windows Informationen zum Build 16257 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Implementieren von prlimit64 Systemaufruf
- Hinzufügen von Unterstützung für Ulimit – n (Setrlimit RLIMIT_NOFILE) [GH 1688]
- Stub MSG_MORE für TCP-Sockets [GH 2351]
- Korrigieren Sie Ungültiger AT_EXECFN zusätzliche Vektor Verhalten [GH 2133]
- Zu beheben Sie, kopieren und Einfügen-Verhalten für Konsole/tty, und fügen Sie eine bessere vollen Puffer behandeln [GH 2204, 2131]
- Legen Sie AT_SECURE in zusätzlichen Vektor für Set-Benutzer-ID "und" Set-Gruppen-ID-Programme [GH 2031]
- Pseudonamens-Terminal masterendpunkt TIOCPGRP [GH 1063] nicht behandelt
- Korrektur Lseek wird dies, um die Verzeichnisse im LxFs [GH 2310] rewind
- /dev/ptmx stürzt ab, nach einer hohen Auslastung [GH 1882]
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Korrektur für horizontale Linien/Unterstriche überall [GH 2168]
- Korrektur für die prozessreihenfolge schwieriger zu [GH 2170] zu schließen und NPM geändert
- Unser neues Farbschema wird hinzugefügt: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/

### <a name="ltp-results"></a>LTP Ergebnisse:
Keine Änderung seit 16251

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`prlimit64`<br/>

### <a name="known-issues"></a>Bekannte Probleme
#### [<a name="github-issue-2392-windows-folders-not-recognized-by-wsl-"></a>GitHub-Problem 2392: Windows-Ordner, die nicht von WSL erkannt...](https://github.com/Microsoft/BashOnWindows/issues/2392)
Im Build 16257 WSL verfügt über Probleme beim Aufzählen von Windows-Dateien und Ordner über `/mnt/c/...`.
Dieses Problem wurde behoben und freigegeben werden soll, im Insiders-build während der Woche ab ab 8/14/2017.

<br/>

## <a name="build-16251"></a>Build 16251

Allgemeine Windows Informationen zum Build 16251 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Beta-Tag von WSL optionale Komponente entfernen, finden Sie unter [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) Details.
- Richtig initialisiert gespeichert-Set-Uid und Gid für Set-Benutzer-ID "und" Set-Gruppen-ID-Binärdateien auf Exec [GH 962, 1415, 2072]
- Unterstützung für Ptrace PTRACE_O_TRACEEXIT [GH 555]
- Unterstützung für Ptrace PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555]
- Informationen zum Beenden für ignoriert Signale Ptrace behoben
- Weitere Verbesserungen und Fehlerbehebungen

#### <a name="console"></a>Console
- Keine Konsole im Zusammenhang mit Änderungen in dieser Version.

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der erfolgreichen Tests: 768</br>
Anzahl der fehlgeschlagenen Tests: 244</br>
Anzahl der übersprungenen Tests: 96</br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a>Build 16241

Allgemeine Windows Informationen zum Build 16241 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).<br/>


### <a name="fixed"></a>Fest
#### <a name="wsl"></a>WSL
- Keine WSL im Zusammenhang mit Änderungen in dieser Version.

#### <a name="console"></a>Console
- Fehlerbehebung für die Ausgabe des falschen Zeichens für den DEC überschreiten Linien ursprünglich gemeldet [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)
- Fehlerbehebung für die kein Ausgabetext angezeigt wird, in der Codepage 65001 (UTF-8)
- Übertragen Sie RGB-Werte auf andere Teile der Palette für die Änderung der Auswahl einer Farbe vorgenommenen Änderungen werden nicht werden. Dadurch wird die Eigenschaftenseite für die Konsole ein viel einfacher zu bedienen.
- STRG + S nicht angezeigt werden, ordnungsgemäß funktioniert
- Nicht fett /-Dim vollständig fehlende aus ANSI-Escapesequenzen [GH 2174]
- Konsole unterstützt nicht ordnungsgemäß Vim-Farbdesigns [GH 1706].
- Bestimmte Zeichen [GH 2149] kann nicht eingefügt werden.
- Ändern der Größe geänderte flussrichtung interagiert seltsam Ändern der Größe einer Bash-Fenster, wenn alles in der Bearbeiten/Befehlszeile [GH ConEmu 1123] verwendet wird
- STRG + L, verlässt den modifizierte Bildschirm [GH 1978]
- Konsole Rendering-Fehler beim Anzeigen von VT auf HDPI [GH 1907]
- Japanischen Zeichen seltsam mit Unicode-Zeichen U + 30FB [GH 2146]
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16237"></a>Build 16237

Allgemeine Windows Informationen zum Build 16237 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).<br/>


### <a name="fixed"></a>Fest
- Verwenden Sie Standardattribute für Dateien ohne EAs im Lxfs ("Root", "Root", "0000")
- Unterstützung für Distributionen, die erweiterte Attribute verwenden
- Beheben Sie Abstand für die von Getdents und getdents64 zurückgegebenen Einträge
- Korrigieren der Überprüfung der Berechtigungen für die Shmctl SHM_STAT Systemaufruf [GH 2068]
- Status des festen falsche anfängliche Epoll für Schreibtelefone [GH 2231]
- Beheben von DrvFs Verz. zurückgeben nicht alle Einträge [GH 2077]
- Beheben von LxFs Verz., wenn Dateien nicht verknüpfte [GH 2077]
- Erlauben Sie aufgehoben Drvfs-Dateien, die über procfs erneut geöffnet werden.
- Überschreiben des globalen Registrierung für das Deaktivieren der WSL Funktionen hinzugefügt (Interop / Laufwerk einbinden)
- Beheben Sie die Anzahl der falschen Block in "Stat" für DrvFs (und LxFs) [GH 1894]
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16232"></a>Build 16232

Allgemeine Windows Informationen zum Build 16232 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).<br/>


### <a name="fixed"></a>Fest
- Keine WSL im Zusammenhang mit Änderungen in dieser Version.

</br>

## <a name="build-16226"></a>Build 16226

Allgemeine Windows Informationen zum Build 16226 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).<br/>


### <a name="fixed"></a>Fest
- Xattr im Zusammenhang mit Syscalls-Unterstützung (Getxattr, Setxattr, Listxattr, Removexattr).
- Security.capablity Xattr-Unterstützung.
- Verbesserte Kompatibilität mit bestimmten Dateisysteme und Filter verwenden, einschließlich nicht - MS-SMB-Server. [GH #1952]
- Verbesserte Unterstützung für OneDrive-Platzhalter, GVFS Platzhalter und Compact OS komprimierte Dateien.
- Weitere Verbesserungen und Fehlerbehebungen

</br>

## <a name="build-16215"></a>Build 16215

Allgemeine Windows Informationen zum Build 16215 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).<br/>


### <a name="fixed"></a>Fest
- WSL muss nicht mehr den Entwicklermodus.
- Verzeichnisverbindungen in Drvfs unterstützt.
- Behandeln Sie die Deinstallation von WSL Verteilung Appx-Paketen.
- Update procfs anzuzeigenden private und freigegebene Zuordnungen.
- Fügen Sie die Möglichkeit wslconfig.exe zum Bereinigen von Verteilungen, die teilweise installiert oder deinstalliert werden.
- Unterstützung für IP_MTU_DISCOVER für TCP-Sockets hinzugefügt. [GH 1639, 2115, 2205]
- Die Protokollfamilie für Routen, um AF_INADDR abgeleitet werden.
- Verbesserungen der seriellen Gerät [GH 1929].

</br>

## <a name="build-16199"></a>Build 16199

Allgemeine Windows Informationen zum Build 16199 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).<br/>


### <a name="fixed"></a>Fest
- Keine WSL im Zusammenhang mit Änderungen in diesen Versionen.

</br>

## <a name="build-16193"></a>Build 16193

Allgemeine Windows Informationen zum Build 16193 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).<br/>


### <a name="fixed"></a>Fest
- Racebedingung zwischen dem Senden der SIGCONT und eine Threadgroup beendet [GH 1973]
- Ändern Sie die tty und Pty-Geräte in Bericht FILE_DEVICE_NAMED_PIPE statt FILE_DEVICE_CONSOLE [GH 1840]
- Beheben von SSH für IP_OPTIONS
- Init-Daemon DrvFs Einbindung verschoben [GH 1862, 1968, 1767, 1933]
- Unterstützung in DrvFs für die folgenden NT symbolische Verknüpfungen.

</br>

## <a name="build-16184"></a>Build 16184

Allgemeine Windows Informationen zum Build 16184 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).<br/>


### <a name="fixed"></a>Fest
- Entfernt die Wartungstask "apt-Paket" (lxrun.exe/Update)
- Ausgabe des festen nicht auftauchen von Windows-Prozessen in node.js [GH 1840]
- Lockern Sie ausrichtungsanforderungen in Lxcore [GH 1794]
- Korrektur der Verarbeitung des AT_EMPTY_PATH Flags in eine Anzahl von Systemaufrufen.
- Problem behoben, bei dem Datei, die nicht definierten Verhalten [GH 544,966,1357,1535,1615] verursacht wird DrvFs-Dateien mit offenen Handles zu löschen
- / Etc/Hosts übernimmt jetzt Einträge aus der Windows-Hosts-Datei (% windir%\system32\drivers\etc\hosts) [GH 1495]

</br>

## <a name="build-16179"></a>Build 16179

Allgemeine Windows Informationen zum Build 16179 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).<br/>


### <a name="fixed"></a>Fest
- Keine Änderungen der WSL diese Woche.

</br>

## <a name="build-16176"></a>Build 16176

Allgemeine Windows Informationen zum Build 16176 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).<br/>


### <a name="fixed"></a>Fest

- [Serielle Unterstützung aktiviert](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- Zusätzliche IP-Socket-Option IP_OPTIONS [GH 1116]
- Pwritev-Funktion (während eine Datei hochladen, um Nginx/PHP-FPM) implementiert [GH 1506]
- Hinzugefügt von IP-Socket-Optionen IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]
- Unterstützung für Socketoption IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]
- Hinzugefügte IP-(IPv6) _MTU Socketoption auf den Knoten "apps", "Traceroute", "informieren Sie sich", "Nslookup", "host
- Zusätzliche IP-Socket-Option IPV6_UNICAST_HOPS
- [Dateisystem-Verbesserungen](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * Bereitstellen von UNC-Pfade zulassen
    * CDFS-Unterstützung in Drvfs aktivieren
    * Verarbeiten Sie Berechtigungen für die Netzwerk-Dateisysteme auf Drvfs ordnungsgemäß
    * Hinzufügen von Unterstützung für die remote-Laufwerke zu drvfs
    * Aktivieren von FAT-Unterstützung in Drvfs
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse
Keine Änderungen seit der 15042

</br>

## <a name="build-16170"></a>Build 16170

Allgemeine Windows Informationen zum Build 16170 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).<br/>

Veröffentlicht eine neue [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) erläutern unsere bemühungen um WSL zu testen.

### <a name="fixed"></a>Fest

- Unterstützung für Socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]
- Hinzufügen von Unterstützung für PTRACE_OLDSETOPTIONS. [GH 1692]
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse
Keine Änderungen seit der 15042

</br>

## <a name="build-15046-to-windows-10-creators-update"></a>Erstellen 15046 zu Windows 10 Creators Update
Es sind keine weiteren WSL Korrekturen oder Funktionen an, für die Aufnahme in die auf Windows 10 Creators Update. Anmerkungen zu dieser Version für WSL werden fortgesetzt, in den kommenden Wochen für Ergänzungen, die für das nächste größere Update für Windows. Für allgemeine Windows Informationen zu Builds 15046 und zukünftige Insider-Versionen finden Sie unter den [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/). <br/><br/>
 <br/>

## <a name="build-15042"></a>Build 15042

Allgemeine Windows Informationen zum Build 15042 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).<br/>


### <a name="fixed"></a>Fest

- Für einen Deadlock zu beheben, entfernen Sie einen Pfad auf "..."
- Ein Problem wurde behoben, in denen FIONBIO keine 0 bei Erfolg [GH 1683] zurückgibt
- Korrigiert: Probleme mit der Zeichenfolge der Länge Null Lesevorgänge Inet Datagrammsockets
- Beheben Sie mögliches Deadlock aufgrund eines Race-Bedingung in Drvfs Inode Lookup [GH 1675]
- Erweiterte Unterstützung für Unix-Socket-Zusatzdaten; SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613 1326]
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 737</br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255

</br>

## <a name="build-15031"></a>Build 15031

Allgemeine Windows Informationen zum Build 15031 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).<br/>


### <a name="fixed"></a>Fest

- Korrektur eines Fehlers, in denen time(2) sporadisch problemereignis würde.
- Behoben, und geben Sie die Where * SIGPROCMASK Syscalls Signal-Maske kann beschädigt werden.
- Nun gibt die vollständige Befehlszeilenlänge in WSL Benachrichtigung über Erstellung des Prozesses zurück. [GH 1632]
- WSL meldet jetzt Threadbeendigung über Ptrace für GDB Hängenbleiben. [GH 1196]
- Korrektur von Bug, in denen Ptys nach hohe Tmux e/a hängen bleiben würde. [GH 1358]
- Feste Timeout-Validierung in viele Systemaufrufe (Futex, Semtimedop, Ppoll, Sigtimedwait, "itimer", Timer_create)
- Hinzugefügte Eventfd EFD_SEMAPHORE Unterstützung [GH 452]
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 737</br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a>Build 15025

Allgemeine Windows Informationen zum Build 15025 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).<br/>


### <a name="fixed"></a>Fest

- Korrektur für Fehler, kaputt Grep 2,27 [GH 1578]
- Implementierten EFD_SEMAPHORE-Flag für eventfd2 Syscall [GH 452]
- Implementiert die /proc/ [ProzessID] / Net/ipv6_route [GH 1608]
- Signal-driven e/a-Unterstützung für Unix-Streamsockets [GH 393, 68]
- Unterstützen Sie F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]
- Implementieren von recvmmsg() Syscall [GH 1531]
- Korrektur von Bug, in denen epoll_wait() [GH 1609] wartet, wurde nicht
- Implementieren von /proc/version_signature
- Tee Syscall gibt jetzt Fehler, wenn beide Dateideskriptoren auf dieselbe Leitung verweisen
- Richtige implementierte Verhalten für SO_PEERCRED für Unix-sockets
- Behandlung von festen Tkill Syscall ungültige parameter
- Änderungen an der Preformace von Drvfs erhöhen
- Kleinere Fehlerbehebung für Ruby e/a-Blockierung
- Feste recvmsg() EINVAL zurückgeben, für das Flag MSG_DONTWAIT für Inet-Sockets [GH 1296]
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 732</br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a>Build 15019

Allgemeine Windows Informationen zum Build 15019 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).<br/>


### <a name="fixed"></a>Fest

- Der Fehler behoben, die falsch, CPU-Auslastung in gemeldet procfs für Tools wie Htop (GH 823, 945, 971)
- Beim Aufrufen von open() mit O_TRUNC auf einem vorhandenen generiert Datei Inotify jetzt IN_MODIFY vor IN_OPEN
- Fehlerbehebungen für Unix-Socket-Getsockopt SO_ERROR Postgress [GH-61, 1354] aktivieren
- Implementieren von /proc/sys/net/core/somaxconn für die GO-Sprache
- Update-Hintergrundaufgabe Apt-Get-Paket wird nun ausgeführt ausgeblendeten aus der Ansicht
- Klare Bereich für ipv6 "localhost" (Spring-Framework(Java) Fehler).
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 714 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 249 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a>Build 15014

Allgemeine Windows Informationen zum Build 15014 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).<br/>


### <a name="fixed"></a>Fest

- STRG + C jetzt funktioniert wie vorgesehen
- einfach und Ps Auxw jetzt richtig ressourcennutzung (GH #516)
- Einfache Übersetzung der NT-Ausnahmen auf Signale. (GH #513)
- Fallocate schlägt jetzt mit ENOSPC fehl, wenn nur noch wenig Speicherplatz statt EINVAL (GH #1571)
- Hinzugefügte /proc/sys/kernel/sem.
- Implementierten Semop und Semtimedop Systemaufrufe
- Feste Nslookup-Fehler mit IP_RECVTOS & IPV6_RECVTCLASS-Socketoption (GH 69)
- Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 709 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a>Syscall-Zusammenfassung
Insgesamt Syscalls: 384 </br>
Die gesamte Implementierung: 235 </br>
Insgesamt, die ein Stub ausgeführt werden: 22 </br>
Insgesamt, nicht implementiert: 127 </br>
[Detaillierte Aufschlüsselung](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a>Build 15007

Allgemeine Windows Informationen zum Build 15007 finden Sie auf die [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).<br/>


### <a name="known-issue"></a>Bekanntes Problem

- Es ist ein bekanntes Problem, das die Konsole, in denen keine einige STRG erkennt + <key> Eingabe.  Dies schließt den Strg-c-Befehl die als eine normale "C" Keypress fungiert.

  - Problemumgehung: Ordnen Sie einen alternativen Schlüssel STRG + C. Zuordnen beispielsweise STRG + K, STRG + C ausführen: `stty intr \^k`.  Diese Zuordnung erfolgt pro Terminal, und müssen erfolgen *jeder* Zeit Bash gestartet wird. Benutzer können die Option zum Einschließen in untersuchen ihre `.bashrc`

### <a name="fixed"></a>Fest

- Das Problem, in denen WSL mit 100 % der CPU-Kern beansprucht, korrigiert
- Socketoption IP_PKTINFO, IPV6_RECVPKTINFO jetzt unterstützt. (GH #851, 987)
- Physische Adresse für die Netzwerkschnittstelle von 16 Bytes Lxcore Truncate (GH #1452, 1414, 1343, 468, 308)
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 709 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a>Build 15002

Allgemeine Windows Build 15002 Informationen finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).<br/>


### <a name="known-issue"></a>Bekanntes Problem

Zwei bekannte Probleme:
- Es ist ein bekanntes Problem, das die Konsole, in denen keine einige STRG erkennt + <key> Eingabe.  Dies schließt den Strg-c-Befehl die als eine normale "C" Keypress fungiert.

  - Problemumgehung: Ordnen Sie einen alternativen Schlüssel STRG + C. Zuordnen beispielsweise STRG + K, STRG + C ausführen: `stty intr \^k`.  Diese Zuordnung erfolgt pro Terminal, und müssen erfolgen *jeder* Zeit Bash gestartet wird. Benutzer können die Option zum Einschließen in untersuchen ihre `.bashrc`

- Während der Ausführung WSL verbraucht Systemthread 100 % der CPU-Kern.  Die zugrunde liegende Ursache wurde behoben und intern behoben.

### <a name="fixed"></a>Fest

- Alle Bash-Sitzungen müssen jetzt auf der gleichen Berechtigungsstufe erstellt werden.  Es wird versucht, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.  Dies bedeutet, dass der Administrator als auch nicht-Administrator-Konsole zur gleichen Zeit ausgeführt werden können. (GH #626)
<br/>
- Implementiert die folgenden NETLINK_ROUTE-Meldungen (erfordert Windows-Administrator)
     - RTM_NEWADDR (unterstützt `ip addr add`)
     - RTM_NEWROUTE (unterstützt `ip route add`)
     - RTM_DELADDR (unterstützt `ip addr del`)
     - RTM_DELROUTE (unterstützt `ip route del`)
- Geplante Aufgabe überprüfen zum Aktualisieren von Paketen werden einer getakteten Verbindung (GH #1371) nicht mehr ausgeführt.
- Fehler behoben wird, in denen hängen Pipeline ruft z. B. Bash - C "ls - AlR /" | bash -c "Cat" (GH #1214)
- Implementierten TCP_KEEPCNT-Socketoption (GH #843)
- Implementierten IP_MTU_DISCOVER INET-Socketoption (720 des GH #, 717, 170, 69)
- Entfernt die alte Funktion für die NT-Binärdateien von Init mit NT-Pfad-Suche ausgeführt. (GH #1325)
- Modus der Kmsg/Dev/Gruppe / andere Lesezugriff (0644) (GH #1321) zu beheben
- Implementierten /proc/sys/kernel/random/uuid (GH #1092)
- Fehler, in denen Startzeit des Prozesses als Jahr 2432 (GH #974) angezeigt wurden, behoben
- Switched standardmäßige Begriff-Umgebungsvariable auf Xterm-256color (GH #1446)
- Die Möglichkeit, die Commits verarbeiten wird berechnet, während der Prozess Fork geändert. (GH #1286)
- Implementierten /proc/sys/vm/overcommit_memory. (GH #1286)
- Implementierten /proc/net/route-Datei (GH #69)
- Fehler wurde behoben, bei denen Verknüpfungsnamen falsch war, lokalisiert (GH #696)
- Feste Elf Analyselogik, die nicht ordnungsgemäß die Programm-Header überprüft muss kleiner als (oder gleich) PATH_MAX. (GH #1048)
- Implementierten Statfs Rückruf für die procfs Sysfs Cgroupfs und Binfmtfs (GH #1378)
- Feste AptPackageIndexUpdate Windows (GH #1184, auch in GH #1193 behandelt) wird nicht das Schließen
- ASLR-Persönlichkeit ADDR_NO_RANDOMIZE-Unterstützung hinzugefügt. (GH #1148, 1128)
- Verbesserte PTRACE_GETSIGINFO, SIGSEGV, für die ordnungsgemäße Gdb stapelüberwachungen während AV (GH #875)
- Elf nicht mehr analysieren, die für Patchelf Binärdateien schlägt fehl. (GH #471)
- VPN DNS weitergegeben wird, um /etc/resolv.conf (GH #416, 1350)
- Verbesserungen bei TCP zuverlässiger Datenübertragungen schließen. (GH #610, 616, 1025, 1335)
- Nun kehren richtigen Fehlercode, wenn zu viele Dateien sind geöffnet (EMFILE). (GH #1126, 2090)
- Windows Audit Log jetzt-Berichte nennen Sie das Image im Prozess erstellen, überwachen.
- Beim Starten von bash.exe aus in einer Bash-Fenster nun ordnungsgemäß abgebrochen
- Hinzugefügte Fehlermeldung beim Interop-kann nicht auf ein Arbeitsverzeichnis unter LxFs (z. B. notepad.exe bashrc) zugreifen.
- Problem behoben, in denen Windows-Pfad in WSL abgeschnitten wurde
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 690 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 274 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a>Build 14986

Allgemeine Windows Informationen zum Build 14986 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).<br/>


### <a name="fixed"></a>Fest

- Feste Stoppfehler mit Netlink und Pty IOCTLs
- Kernel-Version meldet jetzt 4.4.0-43 für Konsistenz mit Xenial
- Bash.exe aufrief, bei der Eingabe an geleitet ' Nul: "(GH #1259)
- Thread-IDs jetzt korrekt gemeldet in procfs (GH #967)
- IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR-Flags, die jetzt in inotify_add_watch() (GH #1280) unterstützt.
- Implementieren Timer_create und verwandte Systemaufrufe.  Dies ermöglicht die GHC-Unterstützung (GH #307)
- Problem behoben, in dem Ping für eine Zeit von 0.000ms (GH #1296) zurückgegeben
- Geben Sie richtige Fehlercode zurück, wenn zu viele Dateien geöffnet sind.
- Korrigiert: Problem in WSL, in denen Netlink datenanforderung Netzwerk-Schnittstelle mit EINVAL fehlschlagen würde, ist die Adresse der Schnittstelle Hardware 32-Byte (z. B. die Teredo-Schnittstelle)
   - Beachten Sie, dass das Hilfsprogramm "Linux"Ip"einen Fehler enthält, in dem er stürzt ab, wenn WSL eine 32-Byte-Hardwareadresse meldet. Dies ist ein Fehler in "Ip", nicht WSL. Die "Ip" Dienstprogramm hartcodierung die Länge des Zeichenfolgenpuffers verwendet, um die Hardwareadresse zu drucken, und diesen Puffer ist zu klein für eine 32-Byte-Hardwareadresse zu drucken.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 669 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 258 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a>Build 14971

Allgemeine Windows Informationen zum Build 14971 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.  Regelmäßig geplanter Updates werden auf die nächste Version fortgesetzt.

### <a name="ltp-results"></a>LTP Ergebnisse:
14965 gegenüber </br>
Anzahl der bestandenen Test: 664 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a>Build 14965

Allgemeine Windows Informationen zum Build 14965 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).<br/>


### <a name="fixed"></a>Fest

- Unterstützung für Netlink sockets des Protokolls NETLINK_ROUTE RTM_GETLINK und RTM_GETADDR (GH #468)
  - Ermöglicht die "ifconfig" und die IP-Befehlen für die Netzwerk-enumeration
  - Weitere Informationen finden Sie unserem [Blogbeitrag WSL Networking](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).

- einen befindet sich nun im Benutzerpfad standardmäßig
- NT-Benutzerrollen-Datenpfad jetzt auf den Pfad WSL angehängt, in der Standardeinstellung (d. h. Sie jetzt notepad.exe eingeben, ohne "System32" auf den Linux-Pfad hinzufügen)
- Unterstützung für /proc/sys/kernel/cap_last_cap
- NT-Binärdateien können jetzt über WSL gestartet werden, wenn das aktuelle Arbeitsverzeichnis nicht-Ansi-Zeichen (GH #1254) enthält
- Ermöglichen Sie Herunterfahren auf getrennten Unix-Stream-Socket.
- Unterstützung für PR_GET_PDEATHSIG hinzugefügt.
- Unterstützung für CLONE_PARENT
- Fehler behoben wird, in denen hängen Pipeline ruft z. B. Bash - C "ls - AlR /" | bash -c "Cat" (GH #1214)
- Verarbeitung von Abfragen für die Verbindung zum aktuellen Terminal.
- Markieren Sie /proc/<pid>/oom_score_adj als schreibbar.
- Fügen Sie /sys/fs/cgroup-Ordner.
- Sched_setaffinity sollte die Anzahl der Bits-Affinitätsmaske zurückgeben.
- Beheben Sie ELF Validierungslogik für die fälschlicherweise angenommen, dass der Interpreter Pfade weniger als 64 Zeichen lang sein müssen. (GH #743)
- Öffnen von Dateideskriptoren können Konsolenfenster geöffnet (GH #1187) beibehalten.
- Fixeed Fehler, in denen Rename()"mit nachgestellten Schrägstrich Zielname (GH #1008)
- Implementieren von /proc/net/dev-Datei
- Feste 0.000ms Pingt aufgrund der zeitgeberauflösung.
- Implementierten /proc/self/environ (GH #730)
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 664 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a>Build 14959

Allgemeine Windows Informationen zum Build 14959 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).<br/>


### <a name="fixed"></a>Fest

- Verbesserte des Pico-Prozess-Benachrichtigung für Windows.  Weitere Informationen finden Sie auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).
- Verbesserte Stabilität, die mit Windows-Interoperabilität
- Korrigieren des Fehlers 0 x 80070057 beim bash.exe zu starten, wenn die Enterprise Data Protection (EDP) aktiviert ist
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 665 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a>Erstellen von 14955

Allgemeine Windows Informationen zum Build 14955 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.  Regelmäßig geplanter Updates werden auf die nächste Version fortgesetzt.

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 665 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a>Build 14951

Allgemeine Windows Informationen zum Build 14951 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).<br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a>Neues Feature: Windows / Ubuntu Interoperability
Windows-Binärdateien können jetzt direkt über die Befehlszeile WSL aufgerufen werden.  Dies ermöglicht Benutzern die Interaktion mit ihrer Windows-Umgebung und das System in einer Weise, die nicht möglich war.  Als kurzes Beispiel ist es jetzt möglich, damit Benutzer die folgenden Befehle ausführen:

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

Weitere Informationen finden Sie unter:

- [WSL-Teamblog für Interop](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [Interop-MSDN-Dokumentation](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a>Fest

- Ubuntu 16.04 (Xenial) ist jetzt für alle neuen WSL-Instanzen installiert.  Benutzer mit vorhandenen 14.04 (bewährte)-Instanzen werden nicht automatisch aktualisiert werden.
- Während der Installation festgelegten Gebietsschema wird jetzt angezeigt.
- Der Terminalserver einschließlich Fehler, bei denen einen WSL-Prozess in eine Datei umleiten nicht immer ermöglicht, arbeiten
- Konsole Lebensdauer sollte bash.exe Lebensdauer gebunden werden
- Konsolenfenster sollte sichtbar Größe, nicht die Puffergröße verwendet.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 665 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a>Build 14946

Allgemeine Windows Informationen zum Build 14946 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).<br/>


### <a name="fixed"></a>Fest

- Ein Problem wurde behoben, die verhindert, Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen, die Leerzeichen oder Anführungszeichen enthalten. 
- Ändern Sie VolFs und DrvFs damit 0 für die Anzahl von des Verzeichnisses links im Stat zurückgegeben werden soll.
- IPV6_MULTICAST_HOPS-Socketoption zu unterstützen.
- Eine einzige Konsole e/a-Schleife pro tty begrenzt. Beispiel: der folgende Befehl ist möglich:
  - bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"

- Ersetzen Sie Leerzeichen mit Tabstopps in /proc/cpuinfo (GH #1115)
- DrvFs wird nun in Mountinfo mit einem Namen, der bereitgestelltes Windows Volume entspricht angezeigt.
- / Home erscheinen/Root nun und in Mountinfo mit den richtigen Namen
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 665 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a>Build 14942

Allgemeine Windows Informationen zum Build 14942 finden Sie auf die [Windows Blog](https://aka.ms/onefourninefourtwoooooo).<br/>


### <a name="fixed"></a>Fest

- Eine Anzahl von Stoppfehler behoben, einschließlich des "versucht Ausführen von"keinausführen "Speichers" networking Absturz die SSH blockiert wurde
- Unterstützung von Windows-Anwendungen auf DrvFs generierten Benachrichtigungen Inotifiy ist jetzt in
- Implementieren Sie TCP_KEEPIDLE und TCP_KEEPINTVL für "mongod" ein. (GH #695)
- Implementieren von Pivot_root Systemaufruf
- Implementieren der Socketoption auf den SO_DONTROUTE
- Zusätzliche Fehlerbehebungen und Verbesserungen


### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 665 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a>Build 14936

Allgemeine Windows Informationen zum Build 14936 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).<br/>


Hinweis: WSL wird Ubuntu Version 16.04 (Xenial) anstelle von Ubuntu 14.04 (treuen) in einer zukünftigen Version installiert werden.  Diese Änderung gilt für Insider neue Instanzen (lxrun.exe/install oder erste Ausführung des bash.exe) installieren.  Vorhandene Instanzen mit treuen werden nicht automatisch aktualisiert werden. Benutzer können ihr Softwareverwaltungssystem-Image auf Xenial mithilfe des Befehls-Release-Upgrade aktualisieren.

### <a name="known-issue"></a>Bekanntes Problem
WSL ist ein Problem mit einigen Socketimplementierungen.  Die fehlerüberprüfung manifestiert sich selbst als ein Absturz mit dem Fehler "Es wurde versucht Ausführen von"keinausführen "Arbeitsspeicher".  Die am häufigsten verwendeten Manifestation dieses Problems ist ein Absturz auf, wenn ssh verwenden.  Die zugrunde liegende Ursache ist für interne Builds festgelegt und wird bei nächstmöglicher Gelegenheit für Insider übertragen werden.

### <a name="fixed"></a>Fest

- Implementiert die Chroot Systemaufruf
- Verbesserungen bei der Inotify ~~einschließlich der Unterstützung von Windows-Anwendungen auf DrvFs generierten Benachrichtigungen~~
  - Korrektur: Inotify Unterstützung für Änderungen, die von Windows-Anwendungen, die zu diesem Zeitpunkt nicht verfügbar.
- Socket-Bindung zu IPV6::<port n> unterstützt jetzt IPV6_V6ONLY (68 des GH #, #157 "," #393 "," #460 "," #674 "," #740 "," #982 "," #996)
- WNOWAIT Waitid Systemcall implementiert (GH #638)
- Unterstützung für IP-Socket-Optionen IP_HDRINCL und IP_TTL
- Mit der Länge Null read() sollte sofort zurückgeben (GH #975)
- Ordnungsgemäß verarbeiten Sie, Dateinamen und den Dateinamen Präfixe, die einen NULL-Terminator in einer TAR-Datei enthalten.
- Epoll-Unterstützung für/dev/null
- Beheben von /dev/alarm Zeitquelle
- Bash -c kann nun in eine Datei umleiten
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 664 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 264 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`chroot`<br/>
<br/>

## <a name="build-14931"></a>Build 14931

Allgemeine Windows Informationen zum Build 14931 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).<br/>


### <a name="fixed"></a>Fest

 - Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.  Geplante regelmäßige Updates werden in der nächsten Version fortgesetzt.

<br/>

## <a name="build-14926"></a>Build 14926

Allgemeine Windows Informationen zum Build 14926 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).<br/>


### <a name="fixed"></a>Fest

- Ping funktioniert jetzt in der Konsolen, die nicht über Administratorberechtigungen verfügen
- Nun unterstützt, auch ohne Administratorrechte ping6
- Inotify-Unterstützung für Dateien, die über WSL geändert. (GH #216)
  - Flags, die unterstützt werden:
    - inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK
    - Inotify_add_watch-Ereignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF
    - Inotify_add_watch Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR
    - Lesen Sie die Ausgabe: LX_IN_ISDIR, LX_IN_IGNORED
  - Bekanntes Problem: Ändern von Dateien aus Windows-Anwendungen keine Ereignisse generiert keine
- UNIX-Socket unterstützt jetzt SCM_CREDENTIALS

### <a name="ltp-results"></a>LTP Ergebnisse:
Anzahl der bestandenen Test: 651 </br>
Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 258 </br>
[LTP Testlauf-Protokolle](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a>Build 14915

Allgemeine Windows Informationen zum Build 14915 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).<br/>


### <a name="fixed"></a>Fest
-  Socketpair für Unix-Datagrammsockets (GH #262)
- UNIX-Socket-Unterstützung für SO_REUSEADDR
- UNIX-Socket-Unterstützung für SO_BROADCAST (GH #568)
- UNIX-Socket-Unterstützung für SOCK_SEQPACKET (GH #758, #546)
- Hinzufügen von Unterstützung für Unix-Datagramm Socket senden, empfangen und Herunterfahren
- Beheben Sie die fehlerprüfung aufgrund ungültiger "mmap" parametervalidierung für Adressen nicht festgelegt. (GH #847)
- Unterstützung für das Anhalten / Fortsetzen von Terminaldienste-Status
- Unterstützung für TIOCPKT Ioctl zum Entsperren des Bildschirms-Dienstprogramms (GH #774)
    - Bekanntes Problem: Funktionstasten nicht funktionsfähig
- Korrigiert ein Race in TimerFd, die einen freigegebenen Member 'ReaderReady' für den Zugriff durch LxpTimerFdWorkerRoutine (GH #814) verursachen können
- Aktivieren Sie neu startbares Aufruf systemunterstützung für Futex, abrufen und clock_nanosleep
- Hinzugefügte Bindung Mount-Unterstützung
- Aufheben der Freigabe für Mount-Namespace-Unterstützung
    - Bekanntes Problem: Beim Erstellen einer neuen Bereitstellung-Namespace mit `unshare(CLONE_NEWNS)` weiterhin das aktuelle Arbeitsverzeichnis auf den alten Namespace zu verweisen
- Weitere Verbesserungen und Fehlerbehebungen

<br/>

## <a name="build-14905"></a>Erstellen von 14905

Allgemeine Windows Informationen zum Build 14905 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).<br/>


### <a name="fixed"></a>Fest
- Neu startbares System jetzt in Aufrufe werden unterstützt (GH #349, GH #520)
- Symbolische Verknüpfungen zu Verzeichnissen im / jetzt operative endet (GH #650)
- Implementierten RNDGETENTCNT Ioctl für/dev/Random
- Implementiert die /proc/ [ProzessID] / durchführte, /proc/ [ProzessID] / Mountinfo und /proc/ [ProzessID] / Mountstats-Dateien
- Zusätzliche Fehlerbehebungen und Verbesserungen

</br>

## <a name="build-14901"></a>Build 14901
Erste Insider-build für den Post-Version von Windows 10 Anniversary Update.

Allgemeine Windows Informationen zum Build 14901 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).<br/>


### <a name="fixed"></a>Fest
- Nachgestellten Schrägstrich behoben
    - Befehle wie `$ mv a/c/ a/b/` funktioniert
- Installieren von jetzt aufgefordert, wenn es sich bei Ubuntu-Gebietsschema auf Windows-Gebietsschema festgelegt werden soll
- Procfs Unterstützung für Ordner "ns"
- Hinzugefügt bereitstellen und Aufheben der Bereitstellung für Tmpfs, procfs und Dateisysteme Sysfs
- Beheben von Mknod [at] 32-Bit-ABI-Signatur
- UNIX-Sockets verschoben wird, um Modell zu senden.
- INET Socket empfangene Puffergröße festgelegt wird, verwenden die Setsockopt sollten berücksichtigt werden
- Implementieren MSG_CMSG_CLOEXEC-Unix-Socket empfängt Nachricht kennzeichnen
- Linux-Prozess "Stdin/stdout" Pipe Umleitung (GH #2)
    - Ermöglicht das Weiterleiten der Bash - C-Befehle in cmd ein.  Beispiel: > Dir | bash -c "Foo" Grep"
- Bash kann auf Systemen mit mehreren Auslagerungsdateien (GH #538, #358) jetzt installiert werden
- INET-Socket-Standardpuffergröße sollte mit der Standard-Ubuntu-Setup übereinstimmen.
- Xattr Syscalls zu Listxattr ausrichten
- Nur Schnittstellen mit einer gültigen IPv4-Adresse von SIOCGIFCONF zurück
- Beheben von Signal Standardaktion, wenn durch Ptrace eingefügt
- Implementieren von /proc/sys/vm/min_free_kbytes
- Verwenden Sie Computer registrieren Kontextwerte, beim Wiederherstellen der Kontext in sigreturn
    - Dadurch wird das Problem behoben, in denen wurden Java- und Javac für einige Benutzer hängende
- Implementieren von /proc/sys/kernel/hostname

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a>Erstellen von 14388 auf Windows 10 Anniversary Update
Allgemeine Windows Informationen zum Build 14388 finden Sie auf die [Windows Blog](https://aka.ms/14388wip). <br/>

### <a name="fixed"></a>Fest
- Fehlerbehebungen für die Vorbereitung auf Windows 10 Anniversary Update auf 8/2
  - Weitere Informationen zu WSL, in dem Anniversary-Update finden Sie auf unserer [Blog](https://blogs.msdn.microsoft.com/wsl/)

<br/>

## <a name="build-14376"></a>Build 14376
Allgemeine Windows Informationen zum Build 14376 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/). <br/>

### <a name="fixed"></a>Fest
- Einigen Fällen, in dem apt-Get (GH #493) hängt, entfernt
- Ein Problem wurde behoben, in denen leere Mounts nicht ordnungsgemäß verarbeitet wurden
- Ein Problem wurde behoben, von dem Ramdisks nicht ordnungsgemäß bereitgestellt wurden
- Änderung von Unix-Socket akzeptiert wird, zur Unterstützung von Flags (partielle GH #451)
- Feste allgemeine netzwerkbezogenen bluescreen
- Bluescreen behoben, wenn /proc/ [ProzessID] den Zugriff auf / task (GH #523)
- Feste hohe CPU-Auslastung für einige Pty-Szenarien (GH #488, #504)
- Zusätzliche Fehlerbehebungen und Verbesserungen

<br/>

## <a name="build-14371"></a>Build 14371
Allgemeine Windows Informationen zum Build 14371 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/). <br/>

### <a name="fixed"></a>Fest
- Timing Race mit SIGCHLD und wait() korrigiert, wenn Sie Ptrace verwenden
- Einige Verhalten korrigiert, wenn ein nachstehender-Pfade verfügen. / (GH #432)
- Korrigiert: beim Umbenennen und Aufheben der Verknüpfung Fehler aufgrund eines offenen Handles zu untergeordneten Elementen
- Zusätzliche Fehlerbehebungen und Verbesserungen

<br/>

## <a name="build-14366"></a>Build 14366
Allgemeine Windows Informationen zum Build 14366 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/). <br/>

### <a name="fixed"></a>Fest
- Beheben Sie im dateierstellung bis hin zur symbolische Verknüpfungen
-   Hinzugefügte Listxattr für Python (GH 385)
-   Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
-   Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`listxattr`<br/>
<br/>

## <a name="build-14361"></a>Build 14361
Allgemeine Windows Informationen zum Build 14361 finden Sie auf die [Windows Blog](https://aka.ms/wip14361). <br/>

### <a name="fixed"></a>Fest
- DrvFs ist jetzt Groß-/Kleinschreibung beachtet, wenn in Bash auf Ubuntu unter Windows ausgeführt.
  - Benutzer Mai case.txt und Groß-/KLEINSCHREIBUNG. TXT, auf die c/Mnt/Laufwerke
  - Groß-/Kleinschreibung wird nur in Bash auf Ubuntu unter Windows unterstützt. Wenn außerhalb der Bash-NTFS-Dateien ordnungsgemäß gemeldet wird, aber kann unerwartetes Verhalten auftreten, interagieren mit den Dateien von Windows.
  - Der Stamm des jedes Volume (d. h. /mnt/c) ist keine Groß-/Kleinschreibung beachten
  - Weitere Informationen zur Behandlung dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).
- Verbesserte Pty / tty unterstützt.  Anwendungen wie TMUX jetzt unterstützt (GH #-40).
- Problem mit der festen Installation, in denen Benutzerkonten nicht immer erstellt
- Optimiert die Befehlszeile Arg-Struktur, die sehr lange Argumentliste ermöglicht. (GH #153)
- Kann nun zum Löschen und Chmod-Dateien Read_only DrvFs
- Feste einigen Fällen, in dem der Terminaldienste Systemstillstand auf (GH #43) trennen
- Chmod und Chown sind jetzt für tty-Geräte
- Lassen Sie die Verbindung auf "0.0.0.0" und:: als "localhost" (GH #388)
- Sendmsg/Recvmsg jetzt eine e/a-Vektor-Länge des behandeln > 1 (partielle GH #376)
- Benutzer können nun automatisch generierte Datei "Hosts" (GH #398) deaktivieren
- Entsprechen Sie, Linux-Gebietsschema, das das NT-Gebietsschema automatisch während der Installation (GH #11)
- Die Datei /proc/sys/vm/swappiness (GH #306) hinzugefügt
- "strace" wird jetzt beendet ordnungsgemäß
- Zulassen von Pipes, um über /proc/self/fd (GH #222) erneut geöffnet werden.
- Blenden Sie die Verzeichnisse unter %LOCALAPPDATA%\lxss aus DrvFs (GH #270)
- Bessere Verarbeitung von bash.exe ~.  Befehle wie "bash ~ - C ls" unterstützt jetzt (GH #467)
- Sockets benachrichtigen jetzt Epoll lesen, die während des Herunterfahrens (GH #271) zur Verfügung.
- Lxrun / uninstall ist besser Löschen von Dateien und Ordner
- Korrigierte Ps -f (GH #246)
- Verbesserte Unterstützung für X11 apps wie xEmacs (GH #481)
- Anfängliche Thread Stapelgröße Ubuntu-Standardeinstellung und die Größe ordnungsgemäß an die Get_rlimit Syscall (GH #172, #258) Berichten entsprechend aktualisiert
- Verbesserte berichterstellung mit Pico-Prozess-imagenamen (z. B. für die Überwachung)
- Implementierten /proc/mountinfo für df-Befehl
- Festen "Symlink" den Fehlercode für den Namen fest. und...
- Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a>Build 14352
Allgemeine Windows Informationen zum Build 14352 finden Sie auf die [Windows Blog](https://aka.ms/wip14352).<br/>


### <a name="fixed"></a>Fest
- Korrigiert: Problem, in dem große Dateien wurden heruntergeladen / nicht ordnungsgemäß erstellt.  Dies sollte Npm und andere Szenarien (GH-3, GH #313) zulassen.
- Entfernt einige Instanzen, in denen Sockets hängen
- Einige Ptrace Fehler korrigiert
- Korrigiert: Probleme mit WSL Dateinamen, die länger als 255 Zeichen zulassen
- Verbesserte Unterstützung für nicht-englische Zeichen
- Aktuelle Windows-Timezone-Daten hinzufügen und als Standard festlegen
- Eindeutige Geräte-Id für die einzelnen einbindungspunkt (Jre-Fix: GH Nr. 49)
- Beheben Sie Fehler mit Pfaden, die mit "." und ".."
- Fifo-Unterstützung (GH #71)
- Aktualisierte Format von "resolv.conf" muss entsprechend der systemeigenen Ubuntu-format
- Einige Bereinigungsschritte procfs
- Aktivierte Ping für Administratorkonsolen (GH Nr. 18)

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a>Build 14342
Informationen zum Erstellen für allgemeine Windows 14342 der [Windows Blog](https://aka.ms/wip14342). <br/>

Informationen zu VolFs und DriveFs finden Sie auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl). <br/>

### <a name="fixed"></a>Fest
- Install-Problem wurde behoben, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen hat.
- Die Updates von apt-Get-Udev-problemumgehung in den häufig gestellten Fragen wird nun standardmäßig bei der ersten Ausführung bereitgestellt werden.
- Symbolische Verknüpfungen in DriveFs aktiviert (/mnt/<drive>) Verzeichnisse
- Symbolische Verknüpfungen funktionieren jetzt zwischen DriveFs und VolFs
- Adressierte Top Level Pfad Problem analysieren: ls. / / funktioniert nun wie erwartet
- Npm installieren, auf DriveFs und die -g-Optionen sind jetzt funktionsfähig.
- Problem behoben, die verhindert, dass PHP-Server starten
- Aktualisierte Umgebung Standardwerte, z. B. $PATH näher übereinstimmen der native Ubuntu
- Eine wöchentliche Wartungsaufgabe hinzugefügt, in Windows den apt-Paketcache aktualisieren
- Problem mit ELF headerüberprüfung wurde behoben, unterstützt die WSL jetzt alle Melkor-Optionen
- Zsh Shell funktioniert.
- Vorkompilierte Go-Binärdateien werden jetzt unterstützt.
- Aufforderung für den anpassungs-Bash.exe ist jetzt ordnungsgemäß lokalisiert
- /proc/meminfo gibt jetzt Informationen zurück.
- Sockets, die jetzt im virtuellen Dateisystem unterstützt.
- können jetzt als Tempfs eingebunden.
- FIFO-Prinzip jetzt unterstützt.
- Multicore-Systeme, die nun ordnungsgemäß angezeigt werden, in dem/Proc/cpuinfo
- Weitere Verbesserungen und Fehlermeldungen, die während der ersten Ausführung herunterladen
- Syscall-Verbesserungen und Fehlerbehebungen. Unterstützt Syscall-Liste unten.
- Zusätzliche Fehlerbehebungen und Verbesserungen

### <a name="known-issues"></a>Bekannte Probleme
- Nicht auflösen '..' ordnungsgemäß auf DriveFs in einigen Fällen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben. Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

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

Allgemeine Windows Informationen zum Build 14332 finden Sie auf die [Windows Blog](https://aka.ms/wip14332). <br/>


### <a name="fixed"></a>Fest
- Eine bessere "resolv.conf" Generation einschließlich Priorisieren von DNS-Einträge
- Problem beim Verschieben von Dateien und Verzeichnisse zwischen enthaltenen und nicht- / Mnt-Laufwerke
- TAR-Dateien können jetzt mit symbolische Verknüpfungen erstellt werden
- Hinzugefügte /run/lock Standardverzeichnis für die instanzerstellung
- Update/dev/NULL zurückzugebenden richtigen Stat-Informationen
- Weitere Fehler beim Herunterladen von während der ersten Ausführung
- Syscall-Verbesserungen und Fehlerbehebungen. Unterstützt Syscall-Liste unten.
- Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Im folgenden finden Sie die neue Syscall, die eine Implementierung in WSL aufweist. Die Syscall in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise nicht, dass alle Parameter eine unterstützte zu diesem Zeitpunkt.

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a>Build 14328

Allgemeine Windows Informationen zum Build 14332 finden Sie auf die [Windows Blog](https://aka.ms/wip14328). <br/>


### <a name="new-features"></a>Neue Features
* Unterstützt nun Linux-Benutzer.  Installieren von Bash unter Ubuntu unter Windows werden für die Erstellung eines Linux-Benutzers aufgefordert.  Weitere Informationen finden Sie unter https://aka.ms/wslusers
* Hostname wird jetzt auf den Namen des Windows-Computers nicht mehr festgelegt @localhost
* Weitere Informationen zum Erstellen von 14328 unterstützen, finden Sie unter: https://aka.ms/wip14328

### <a name="fixed"></a>Fest
* Verbesserungen des "Symlink" für nicht /mnt/<drive> Dateien
    * die Installation funktioniert nun npm
    * JDK / Jre jetzt installierbare anhand der Anweisungen [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).
    * bekanntes Problem: symbolische Links funktionieren nicht für Windows bindet.  Funktionen werden in eine höhere Version verfügbar sein.
* Top und einfach zeigen jetzt
* Installieren Sie weitere Fehlermeldungen für einige Fehler
* Syscall-Verbesserungen und Fehlerbehebungen.  Unterstützt Syscall-Liste unten.
* Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen

### <a name="syscall-support"></a>Syscall-Unterstützung
Es folgt eine Liste der Syscalls, die eine Implementierung in WSL zu haben.  Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.

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
