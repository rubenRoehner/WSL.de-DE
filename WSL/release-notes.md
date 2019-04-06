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
# <a name="release-notes-for-windows-subsystem-for-linux"></a><span data-ttu-id="d8d1c-105">Anmerkungen zu dieser Version für Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="d8d1c-105">Release Notes for Windows Subsystem for Linux</span></span>

## <a name="build-18342"></a><span data-ttu-id="d8d1c-106">Build 18342</span><span class="sxs-lookup"><span data-stu-id="d8d1c-106">Build 18342</span></span>
<span data-ttu-id="d8d1c-107">Allgemeine Windows Informationen zum Build 18342 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-107">For general Windows information on build 18342 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-108">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-108">WSL</span></span>
* <span data-ttu-id="d8d1c-109">Wir haben die Möglichkeit für Benutzer von Windows auf Linux-Dateien in einem WSL-Distribution, die hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-109">We've added the ability for users to access Linux files in a WSL distro from Windows.</span></span> <span data-ttu-id="d8d1c-110">Diese Dateien können über die Befehlszeile und auch den Windows-apps wie VSCode Datei-Explorer zugegriffen werden, usw. können mit diesen Dateien interagieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-110">These files can be accessed through the command line, and also Windows apps, like file explorer, VSCode, etc. can interact with these files.</span></span> <span data-ttu-id="d8d1c-111">Zugriff auf Ihre Dateien durch Navigieren zu \\ \\Wsl$\\< Distro_name >, oder sehen Sie eine Liste der ausgeführten Verteilungen durch Navigieren zu \\ \\Wsl$</span><span class="sxs-lookup"><span data-stu-id="d8d1c-111">Access your files by navigating to \\\\wsl$\\<distro_name>, or see a list of running distributions by navigating to \\\\wsl$</span></span>
* <span data-ttu-id="d8d1c-112">Fügen Sie zusätzliche CPU-Info-Tags hinzu, und beheben Sie Cpus_allowed [_list]-Werte [GH 2234]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-112">Add additional CPU info tags and fix Cpus_allowed[_list] values [GH 2234]</span></span>
* <span data-ttu-id="d8d1c-113">Unterstützung von Exec nicht übergeordneten Threads [GH 3800]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-113">Support exec from non-leader thread [GH 3800]</span></span>
* <span data-ttu-id="d8d1c-114">Fehler beim Update der Konfiguration wird als nicht schwerwiegenden [GH 3785] behandeln.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-114">Treat configuration update failures as non-fatal [GH 3785]</span></span>
* <span data-ttu-id="d8d1c-115">Aktualisieren von Binfmt um ordnungsgemäß zu behandeln, die Offsets [GH 3768]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-115">Update binfmt to properly handle offsets [GH 3768]</span></span>
* <span data-ttu-id="d8d1c-116">Aktivieren der Zuordnung Netzlaufwerke für planen 9 [GH 3854]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-116">Enable mapping network drives for Plan 9 [GH 3854]</span></span>
* <span data-ttu-id="d8d1c-117">Unterstützung für Windows > Linux und Linux -> Windows-Pfad-Übersetzung für bindungseinbindungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-117">Support Windows -> Linux and Linux -> Windows path translation for bind mounts</span></span>
* <span data-ttu-id="d8d1c-118">Erstellen Sie schreibgeschützte Abschnitte für die Zuordnungen auf geöffnete Dateien, schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-118">Create read-only sections for mappings on files opened read-only</span></span>

## <a name="build-18334"></a><span data-ttu-id="d8d1c-119">Build 18334</span><span class="sxs-lookup"><span data-stu-id="d8d1c-119">Build 18334</span></span>
<span data-ttu-id="d8d1c-120">Allgemeine Windows Informationen zum Build 18334 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-120">For general Windows information on build 18334 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-121">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-121">WSL</span></span>
* <span data-ttu-id="d8d1c-122">Ändern Sie die Möglichkeit, dass Windows-Zeitzone in eine Linux-Zeitzone [GH 3747] zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="d8d1c-122">Redesign the way that Windows time zone is mapped to a  Linux time zone [GH 3747]</span></span>
* <span data-ttu-id="d8d1c-123">Beheben Sie Speicherverluste und Hinzufügen von neuen Funktionen für Zeichenfolgen-Übersetzung [GH 3746]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-123">Fix memory leaks and add new string translation functions [GH 3746]</span></span>
* <span data-ttu-id="d8d1c-124">SIGCONT auf eine Threadgroup ohne Threads ist ein nicht möglich [GH 3741]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-124">SIGCONT on a threadgroup with no threads is a no-op [GH 3741]</span></span> 
* <span data-ttu-id="d8d1c-125">Lassen Sie Socket und Epoll Dateideskriptoren in /proc/self/fd korrekt anzeigen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-125">Correctly display socket and epoll file descriptors in /proc/self/fd</span></span>

## <a name="build-18305"></a><span data-ttu-id="d8d1c-126">Build 18305</span><span class="sxs-lookup"><span data-stu-id="d8d1c-126">Build 18305</span></span>
<span data-ttu-id="d8d1c-127">Allgemeine Windows Informationen zum Build 18305 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-127">For general Windows information on build 18305 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-128">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-128">WSL</span></span>
* <span data-ttu-id="d8d1c-129">Pthreads verlieren den Zugriff auf Dateien aus, wenn der primäre Thread [GH 3589] beendet wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-129">pthreads lose access to files when the primary thread exits [GH 3589]</span></span>
* <span data-ttu-id="d8d1c-130">TIOCSCTTY den "Force"-Parameter ignorieren soll, es sei denn, dies erforderlich ist [GH 3652]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-130">TIOCSCTTY should ignore the “force” parameter unless it is required [GH 3652]</span></span>
* <span data-ttu-id="d8d1c-131">wsl.exe Befehlszeile Verbesserungen und Hinzufügen von import / export-Funktionalität.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-131">wsl.exe command line improvements and addition of import / export functionality.</span></span>
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

## <a name="build-18277"></a><span data-ttu-id="d8d1c-132">Build 18277</span><span class="sxs-lookup"><span data-stu-id="d8d1c-132">Build 18277</span></span>
<span data-ttu-id="d8d1c-133">Allgemeine Windows Informationen zum Build 18277 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-133">For general Windows information on build 18277 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-134">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-134">WSL</span></span>
* <span data-ttu-id="d8d1c-135">Beheben von "Schnittstelle nicht unterstützt"-Fehler in Build 18272 [GH 3645] eingeführt wurden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-135">Fix "no such interface supported" error introduced in build 18272 [GH 3645]</span></span>
* <span data-ttu-id="d8d1c-136">Ignorieren Sie das Flag MNT_FORCE für Umount Syscall [GH 3605]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-136">Ignore the MNT_FORCE flag for umount syscall [GH 3605]</span></span>
* <span data-ttu-id="d8d1c-137">Wechseln Sie WSL-Interop für die offizielle CreatePseudoConsole-API verwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-137">Switch WSL interop to use the official CreatePseudoConsole API</span></span>
* <span data-ttu-id="d8d1c-138">Behalten Sie kein Timeoutwert bei, wenn FUTEX_WAIT neu gestartet wird</span><span class="sxs-lookup"><span data-stu-id="d8d1c-138">Maintain no timeout value when FUTEX_WAIT restarts</span></span>

## <a name="build-18272"></a><span data-ttu-id="d8d1c-139">Build 18272</span><span class="sxs-lookup"><span data-stu-id="d8d1c-139">Build 18272</span></span>
<span data-ttu-id="d8d1c-140">Allgemeine Windows Informationen zum Build 18272 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-140">For general Windows information on build 18272 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-141">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-141">WSL</span></span>
* <span data-ttu-id="d8d1c-142">**WARNUNG:** In diesem Build, die WSL defekt ist vorliegt ein Problem.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-142">**WARNING:** There is an issue in this build that makes WSL inoperable.</span></span> <span data-ttu-id="d8d1c-143">Beim Versuch, Ihre Verteilung zu starten, sehen Sie einen "Schnittstelle nicht unterstützt"-Fehler.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-143">When trying to launch your distribution you will see a “No such interface supported” error.</span></span> <span data-ttu-id="d8d1c-144">Das Problem wurde behoben und werden in der nächsten Woche schnell Insider-Build.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-144">The issue has been fixed and will be in next week's Insider Fast build.</span></span> <span data-ttu-id="d8d1c-145">Wenn Sie installiert haben diese erstellen, die Sie auf den vorherigen Windows-Build mithilfe von "Wechseln Sie zu der vorherigen Version von Windows 10" in den Einstellungen zurücksetzen können -> Update und Sicherheit -> Recovery.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-145">If you've installed this build you can roll back to the previous Windows build using “Go back to the previous version of Windows 10” in Settings->Update & Security->Recovery.</span></span>

## <a name="build-18267"></a><span data-ttu-id="d8d1c-146">Build 18267</span><span class="sxs-lookup"><span data-stu-id="d8d1c-146">Build 18267</span></span>
<span data-ttu-id="d8d1c-147">Allgemeine Windows Informationen zum Build 18267 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-147">For general Windows information on build 18267 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-148">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-148">WSL</span></span>
* <span data-ttu-id="d8d1c-149">Korrigiert: Fehler, in denen Zombie-Prozess kann nicht kam werden und bleibt auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-149">Fix issue where zombie process may not be reaped and remain indefinitely.</span></span>
* <span data-ttu-id="d8d1c-150">WslRegisterDistribution reagiert, wenn die Fehlermeldung [GH 3592] die maximalen Länge überschreitet</span><span class="sxs-lookup"><span data-stu-id="d8d1c-150">WslRegisterDistribution hangs if error message exceeds max length [GH 3592]</span></span>
* <span data-ttu-id="d8d1c-151">Zulassen von Fsync clientauftrags für schreibgeschützte Dateien auf DrvFs [GH 3556]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-151">Allow fsync to succeed for read-only files on DrvFs [GH 3556]</span></span>
* <span data-ttu-id="d8d1c-152">Stellen Sie sicher, dass "/ bin" und einen Verzeichnisse vorhanden sind, vor dem erstellen symbolische Verknüpfungen in [GH 3584]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-152">Ensure that /bin and /sbin directories exist before creating symlinks inside [GH 3584]</span></span>
* <span data-ttu-id="d8d1c-153">Eine Instanz beenden-Timeoutmechanismus für WSL-Instanzen wird hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-153">Added an instance termination timeout mechanism for WSL instances.</span></span> <span data-ttu-id="d8d1c-154">Das Timeout ist so eingerichtet, 15 Sekunden, was bedeutet, dass die Instanz beendet wird, 15 Sekunden, nach der letzten WSL-Prozess beendet wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-154">The timeout is currently set to 15 seconds, meaning the instance will terminate 15 seconds after the last WSL process exits.</span></span> <span data-ttu-id="d8d1c-155">Um eine Verteilung sofort zu beenden, verwenden Sie:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-155">To terminate a distribution immediately, use:</span></span>
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a><span data-ttu-id="d8d1c-156">Build 17763 (1809)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-156">Build 17763 (1809)</span></span>
<span data-ttu-id="d8d1c-157">Allgemeine Windows Informationen zum Build 17763 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-157">For general Windows information on build 17763 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-158">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-158">WSL</span></span>
* <span data-ttu-id="d8d1c-159">SetPriority Syscall Überprüfung der Berechtigung zum Ändern der gleichen Priorität der Threads [GH 1838] zu streng.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-159">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="d8d1c-160">Stellen Sie sicher, dass ausgewogene Interruptzeit für den Systemstart verwendet wird, um zu vermeiden, Zurückgeben des negativen Werte für die clock_gettime(CLOCK_BOOTTIME) [3434 ein GH.]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-160">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="d8d1c-161">Behandeln Sie symbolische Verknüpfungen im WSL Binfmt Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-161">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="d8d1c-162">Eine bessere Verarbeitung von Threadgroup übergeordneten Datei Deskriptor bereinigen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-162">Better handling of threadgroup leader file descriptor cleanup.</span></span>
* <span data-ttu-id="d8d1c-163">Wechseln Sie WSL KeQueryInterruptTimePrecise statt KeQueryPerformanceCounter mit Überlauf [GH 3252]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-163">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="d8d1c-164">Fügen Sie Ptrace Mai führen zur fehlerhaften Rückgabewert Systemaufrufe [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-164">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="d8d1c-165">Lösung, die mehrere AF_UNIX bezogene Probleme [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-165">Fix several AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="d8d1c-166">Korrigieren von Problem, WSL-Interop aufgrund dessen für fehl, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-166">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>
* <span data-ttu-id="d8d1c-167">Vermeiden Sie die Verzögerung von einer Sekunde Fehler bei Loopbackverbindungen auf nicht existierende Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-167">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="d8d1c-168">Hinzufügen von /proc/sys/fs/file-max-Stub-Datei [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-168">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="d8d1c-169">Genauere Informationen für die IPV6-Bereich.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-169">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="d8d1c-170">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-170">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="d8d1c-171">Pipe-Dateisystem versehentlich löschen Epoll Edge ausgelöstes Ereignis [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-171">Pipe filesystem inadvertently clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="d8d1c-172">Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-172">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>
* <span data-ttu-id="d8d1c-173">Verbesserte Zombie-Unterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-173">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="d8d1c-174">Fügen Sie wsl.conf Einträge zum Steuern der Windows-interopverhalten [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-174">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="d8d1c-175">Korrektur für Getsockname nicht immer Zurückgeben von UNIX-Socket-Familientyp [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-175">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="d8d1c-176">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-176">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="d8d1c-177">Nicht blockierenden Sockets gerade eine Verbindung herstellen sollte EAGAIN für Schreibzugriff Versuche [GH 2846] zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-177">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="d8d1c-178">Unterstützen von Interop auf bereitgestellten VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-178">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="d8d1c-179">Beheben von berechtigungsüberprüfungen Problem Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-179">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="d8d1c-180">Eingeschränkte Unterstützung für TTY Tastatur Ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-180">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="d8d1c-181">Windows-Anwendungsbenutzeroberflächen sollte ausgeführt werden, auch wenn im Hintergrund gestartet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-181">Windows UI apps should execute even when launched in the background.</span></span>
* <span data-ttu-id="d8d1c-182">Fügen Sie die Wsl -u "oder"--Benutzer Option [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-182">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="d8d1c-183">WSL starten Probleme zu beheben, wenn Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-183">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="d8d1c-184">UNIX-Sockets müssen getrennt Peer-Anmeldeinformationen [GH 3183] beibehalten werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-184">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="d8d1c-185">Nicht blockierende Unix-Sockets auf unbestimmte Zeit führt zu dem EAGAIN [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-185">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="d8d1c-186">Fall = off ist der neue Standard-Drvfs einbinden Typ [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-186">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="d8d1c-187">Finden Sie unter [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) für Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-187">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="d8d1c-188">Hinzufügen von Wslconfig / zum Beenden Verteilungen zu beenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-188">Add wslconfig /terminate to stop running distributions.</span></span>
* <span data-ttu-id="d8d1c-189">Beheben Sie ein Problem mit dem Shell-Kontext WSL Menüeinträge, die Pfade mit Leerzeichen nicht ordnungsgemäß behandelt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-189">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="d8d1c-190">Machen Sie die Groß-/Kleinschreibung pro Verzeichnis als ein erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="d8d1c-190">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="d8d1c-191">ARM64: Cache-Wartungsvorgänge zu emulieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-191">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="d8d1c-192">Beheben [Dotnet Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-192">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="d8d1c-193">DrvFs: unescape-Zeichen im privaten Bereich entsprechen, die nur auf ein Escapezeichen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-193">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>
* <span data-ttu-id="d8d1c-194">Beheben Sie deaktiviert ein Fehler in ELF Parser-Interpreter eine längenüberprüfung [GH 3154]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-194">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="d8d1c-195">WSL absolute Zeitgeber mit einer Uhrzeit in der Vergangenheit werden [GH 3091] nicht ausgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-195">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="d8d1c-196">Vergewissern Sie sich neu erstellte Analysepunkte als solche in das übergeordnete Verzeichnis aufgeführt sind.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-196">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="d8d1c-197">Erstellen Sie Groß-/ Kleinschreibung Verzeichnisse werden atomar in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-197">Atomically create case sensitive directories in DrvFs.</span></span>
* <span data-ttu-id="d8d1c-198">Korrigiert: zusätzliche Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-198">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="d8d1c-199">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-199">[GH 2712]</span></span>
* <span data-ttu-id="d8d1c-200">Festen WSL starten Fehler auf, wenn UMCI aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-200">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="d8d1c-201">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-201">[GH 3020]</span></span>
* <span data-ttu-id="d8d1c-202">Fügen Sie die Explorer-Kontextmenü zum Starten von WSL [GH 437, 603 1836] hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-202">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="d8d1c-203">Zu verwenden, halten die UMSCHALTTASTE gedrückt, und mit der rechten Maustaste in einem Explorer-Fenster.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-203">To use, hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="d8d1c-204">Beheben von Unix-Socket nicht blockierende Verhalten [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-204">Fix Unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="d8d1c-205">Fix hängende NETLINK-Befehl aus, wie in GH 2026 angegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-205">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="d8d1c-206">Hinzufügen von Unterstützung für Mount-Weitergabeflags [GH 2911].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-206">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="d8d1c-207">Problem mit der truncate nicht zu Inotify Ereignisse [GH 2978] behoben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-207">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="d8d1c-208">Fügen Sie hinzu – Exec-Option für wsl.exe um eine einzelne Binärdatei ohne eine Shell aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-208">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="d8d1c-209">Fügen Sie hinzu – die Verteilungsoption für wsl.exe-Distribution, die eine bestimmte Auswahl.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-209">Add --distribution option for wsl.exe to select a specific distro.</span></span>
* <span data-ttu-id="d8d1c-210">Eingeschränkte Unterstützung für "dmesg".</span><span class="sxs-lookup"><span data-stu-id="d8d1c-210">Limited support for dmesg.</span></span> <span data-ttu-id="d8d1c-211">Anwendungen können jetzt in "dmesg" protokollieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-211">Applications can now log to dmesg.</span></span> <span data-ttu-id="d8d1c-212">WSL-treiberprotokolle eingeschränkte Informationen zu "dmesg".</span><span class="sxs-lookup"><span data-stu-id="d8d1c-212">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="d8d1c-213">Dies kann in Zukunft erweitert werden, um weitere Informationen/Diagnosedaten aus dem Treiber durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-213">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="d8d1c-214">Hinweis: "dmesg" wird über derzeit unterstützt die `/dev/kmsg` Geräteschnittstelle.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-214">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> `syslog` <span data-ttu-id="d8d1c-215">Syscall-Schnittstelle ist noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-215">syscall interface is not yet supported.</span></span> <span data-ttu-id="d8d1c-216">Und natürlich einige von der `dmesg` Befehlszeilenoptionen wie z. B. `-S`, `-C` funktionieren nicht.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-216">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="d8d1c-217">Standard-Gruppen-ID und Modus der seriellen Geräten nativ [GH 3042] entsprechend zu ändern</span><span class="sxs-lookup"><span data-stu-id="d8d1c-217">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="d8d1c-218">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-218">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="d8d1c-219">Hinweis: DrvFs gelten einige Einschränkungen auf den Namen der erweiterten Attribute.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-219">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="d8d1c-220">Einige Zeichen (z. B. '/', ':' und '\*") nicht zulässig sind, und erweitert Attributnamen wird nicht in der Groß-/ Kleinschreibung auf DrvFs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-220">Some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-18252-skip-ahead"></a><span data-ttu-id="d8d1c-221">Erstellen von 18252 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-221">Build 18252 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-222">Allgemeine Windows Informationen zum Build 18252 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-222">For general Windows information on build 18252 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-223">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-223">WSL</span></span>
* <span data-ttu-id="d8d1c-224">Verschieben Sie Init "und" Bsdtar Binärdateien aus Lxssmanager Dll und in einem separaten Tools-Ordner</span><span class="sxs-lookup"><span data-stu-id="d8d1c-224">Move init and bsdtar binaries out of lxssmanager dll and into a separate tools folder</span></span>
* <span data-ttu-id="d8d1c-225">Beheben von Rennen um Dateideskriptor geschlossen, wenn CLONE_FILES verwenden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-225">Fix race around closing file descriptor when using CLONE_FILES</span></span>
* <span data-ttu-id="d8d1c-226">Behandeln von optionalen Feldern in /proc/pid/mountinfo beim Übersetzen von DrvFs Pfade</span><span class="sxs-lookup"><span data-stu-id="d8d1c-226">Handle optional fields in /proc/pid/mountinfo when translating DrvFs paths</span></span>
* <span data-ttu-id="d8d1c-227">Können Sie DrvFs Mknod ohne metadatenunterstützung für S_IFREG erfolgreich ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-227">Allow DrvFs mknod to succeed without metadata support for S_IFREG</span></span>
* <span data-ttu-id="d8d1c-228">ReadOnly-Dateien, die auf DrvFs erstellt sollte das Readonly-Attribut [GH 3411] festgelegt sein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-228">Readonly files created on DrvFs should have the readonly attribute set [GH 3411]</span></span>
* <span data-ttu-id="d8d1c-229">Hinzufügen von /sbin/mount.drvfs-Hilfsprogramm zum Behandeln von DrvFs einbinden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-229">Add /sbin/mount.drvfs helper to handle DrvFs mounting</span></span>
* <span data-ttu-id="d8d1c-230">Verwenden Sie Umbenennen von POSIX in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-230">Use POSIX rename in DrvFs.</span></span>
* <span data-ttu-id="d8d1c-231">Ermöglichen Sie Pfad Übersetzung auf Volumes ohne einer Volume-GUID.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-231">Allow path translation on volumes without a volume GUID.</span></span>

## <a name="build-17738-fast"></a><span data-ttu-id="d8d1c-232">Build 17738 (Fast)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-232">Build 17738 (Fast)</span></span>
<span data-ttu-id="d8d1c-233">Allgemeine Windows Informationen zum Build 17738 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-233">For general Windows information on build 17738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-234">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-234">WSL</span></span>
* <span data-ttu-id="d8d1c-235">SetPriority Syscall Überprüfung der Berechtigung zum Ändern der gleichen Priorität der Threads [GH 1838] zu streng.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-235">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="d8d1c-236">Stellen Sie sicher, dass ausgewogene Interruptzeit für den Systemstart verwendet wird, um zu vermeiden, Zurückgeben des negativen Werte für die clock_gettime(CLOCK_BOOTTIME) [3434 ein GH.]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-236">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="d8d1c-237">Behandeln Sie symbolische Verknüpfungen im WSL Binfmt Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-237">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="d8d1c-238">Eine bessere Verarbeitung von Threadgroup übergeordneten Datei Deskriptor bereinigen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-238">Better handling of threadgroup leader file descriptor cleanup.</span></span>

## <a name="build-17728-fast"></a><span data-ttu-id="d8d1c-239">Erstellen von 17728 (Fast)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-239">Build 17728 (Fast)</span></span>
<span data-ttu-id="d8d1c-240">Allgemeine Windows Informationen zum Build 17728 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-240">For general Windows information on build 17728 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-241">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-241">WSL</span></span>
* <span data-ttu-id="d8d1c-242">Wechseln Sie WSL KeQueryInterruptTimePrecise statt KeQueryPerformanceCounter mit Überlauf [GH 3252]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-242">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="d8d1c-243">Fügen Sie Ptrace Mai führen zur fehlerhaften Rückgabewert Systemaufrufe [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-243">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="d8d1c-244">Lösung, die eine Reihe von AF_UNIX Bezug Probleme [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-244">Fix a number of AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="d8d1c-245">Korrigieren von Problem, WSL-Interop aufgrund dessen für fehl, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-245">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>

## <a name="build-18204-skip-ahead"></a><span data-ttu-id="d8d1c-246">Erstellen von 18204 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-246">Build 18204 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-247">Allgemeine Windows Informationen zum Build 18204 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-247">For general Windows information on build 18204 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-248">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-248">WSL</span></span>
* <span data-ttu-id="d8d1c-249">Übergeben von Dateisystem Inadvertenly Epoll Edge ausgelöstes Ereignis [GH 3276] deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-249">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="d8d1c-250">Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-250">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17723-fast"></a><span data-ttu-id="d8d1c-251">Erstellen von 17723 (Fast)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-251">Build 17723 (Fast)</span></span>
<span data-ttu-id="d8d1c-252">Allgemeine Windows Informationen zum Build 17723 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-252">For general Windows information on build 17723 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-253">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-253">WSL</span></span>
* <span data-ttu-id="d8d1c-254">Vermeiden Sie die Verzögerung von einer Sekunde Fehler bei Loopbackverbindungen auf nicht existierende Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-254">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="d8d1c-255">Hinzufügen von /proc/sys/fs/file-max-Stub-Datei [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-255">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="d8d1c-256">Genauere Informationen für die IPV6-Bereich.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-256">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="d8d1c-257">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-257">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="d8d1c-258">Übergeben von Dateisystem Inadvertenly Epoll Edge ausgelöstes Ereignis [GH 3276] deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-258">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="d8d1c-259">Ausführbaren Win32-Datei über NTFS "Symlink" gestartet "Symlink"-Name [GH 2909] nicht berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-259">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17713"></a><span data-ttu-id="d8d1c-260">Build 17713</span><span class="sxs-lookup"><span data-stu-id="d8d1c-260">Build 17713</span></span>
<span data-ttu-id="d8d1c-261">Allgemeine Windows Informationen zum Build 17713 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-261">For general Windows information on build 17713 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-262">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-262">WSL</span></span>
* <span data-ttu-id="d8d1c-263">Verbesserte Zombie-Unterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-263">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="d8d1c-264">Fügen Sie wsl.conf Einträge zum Steuern der Windows-interopverhalten [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-264">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="d8d1c-265">Korrektur für Getsockname nicht immer Zurückgeben von UNIX-Socket-Familientyp [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-265">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="d8d1c-266">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-266">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="d8d1c-267">Nicht blockierenden Sockets gerade eine Verbindung herstellen sollte EAGAIN für Schreibzugriff Versuche [GH 2846] zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-267">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="d8d1c-268">Unterstützen von Interop auf bereitgestellten VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-268">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="d8d1c-269">Beheben von berechtigungsüberprüfungen Problem Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-269">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="d8d1c-270">Eingeschränkte Unterstützung für TTY Tastatur Ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-270">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="d8d1c-271">Windows-Anwendungsbenutzeroberflächen sollte ausgeführt werden, auch wenn im Hintergrund gestartet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-271">Windows UI apps should execute even when launched in the background.</span></span>

## <a name="build-17704"></a><span data-ttu-id="d8d1c-272">Build 17704</span><span class="sxs-lookup"><span data-stu-id="d8d1c-272">Build 17704</span></span>
<span data-ttu-id="d8d1c-273">Allgemeine Windows Informationen zum Build 17704 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-273">For general Windows information on build 17704 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-274">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-274">WSL</span></span>
* <span data-ttu-id="d8d1c-275">Fügen Sie die Wsl -u "oder"--Benutzer Option [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-275">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="d8d1c-276">WSL starten Probleme zu beheben, wenn Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-276">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="d8d1c-277">UNIX-Sockets müssen getrennt Peer-Anmeldeinformationen [GH 3183] beibehalten werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-277">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="d8d1c-278">Nicht blockierende Unix-Sockets auf unbestimmte Zeit führt zu dem EAGAIN [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-278">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="d8d1c-279">Fall = off ist der neue Standard-Drvfs einbinden Typ [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-279">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="d8d1c-280">Finden Sie unter [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) für Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-280">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="d8d1c-281">Hinzufügen von Wslconfig / zum Beenden Verteilungen zu beenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-281">Add wslconfig /terminate to stop running distributions.</span></span>

## <a name="build-17692"></a><span data-ttu-id="d8d1c-282">Build 17692</span><span class="sxs-lookup"><span data-stu-id="d8d1c-282">Build 17692</span></span>
<span data-ttu-id="d8d1c-283">Allgemeine Windows Informationen zum Build 17692 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-283">For general Windows information on build 17692 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-284">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-284">WSL</span></span>
* <span data-ttu-id="d8d1c-285">Beheben Sie ein Problem mit dem Shell-Kontext WSL Menüeinträge, die Pfade mit Leerzeichen nicht ordnungsgemäß behandelt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-285">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="d8d1c-286">Machen Sie die Groß-/Kleinschreibung pro Verzeichnis als ein erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="d8d1c-286">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="d8d1c-287">ARM64: Cache-Wartungsvorgänge zu emulieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-287">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="d8d1c-288">Beheben [Dotnet Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-288">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="d8d1c-289">DrvFs: unescape-Zeichen im privaten Bereich entsprechen, die nur auf ein Escapezeichen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-289">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>

## <a name="build-17686"></a><span data-ttu-id="d8d1c-290">Build 17686</span><span class="sxs-lookup"><span data-stu-id="d8d1c-290">Build 17686</span></span>
<span data-ttu-id="d8d1c-291">Allgemeine Windows Informationen zum Build 17686 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-291">For general Windows information on build 17686 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-292">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-292">WSL</span></span>
* <span data-ttu-id="d8d1c-293">Beheben Sie deaktiviert ein Fehler in ELF Parser-Interpreter eine längenüberprüfung [GH 3154]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-293">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="d8d1c-294">WSL absolute Zeitgeber mit einer Uhrzeit in der Vergangenheit werden [GH 3091] nicht ausgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-294">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="d8d1c-295">Vergewissern Sie sich neu erstellte Analysepunkte als solche in das übergeordnete Verzeichnis aufgeführt sind.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-295">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="d8d1c-296">Erstellen Sie Groß-/ Kleinschreibung Verzeichnisse werden atomar in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-296">Atomically create case sensitive directories in DrvFs.</span></span>

## <a name="build-17677"></a><span data-ttu-id="d8d1c-297">Build 17677</span><span class="sxs-lookup"><span data-stu-id="d8d1c-297">Build 17677</span></span>
<span data-ttu-id="d8d1c-298">Allgemeine Windows Informationen zum Build 17677 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-298">For general Windows information on build 17677 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-299">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-299">WSL</span></span>
* <span data-ttu-id="d8d1c-300">Korrigiert: zusätzliche Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-300">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="d8d1c-301">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-301">[GH 2712]</span></span>
* <span data-ttu-id="d8d1c-302">Festen WSL starten Fehler auf, wenn UMCI aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-302">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="d8d1c-303">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-303">[GH 3020]</span></span>

## <a name="build-17666"></a><span data-ttu-id="d8d1c-304">Build 17666</span><span class="sxs-lookup"><span data-stu-id="d8d1c-304">Build 17666</span></span>
<span data-ttu-id="d8d1c-305">Allgemeine Windows Informationen zum Build 17666 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-305">For general Windows information on build 17666 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-306">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-306">WSL</span></span>
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a><span data-ttu-id="d8d1c-307">WARNUNG: Es liegt ein Problem verhindert, dass WSL auf einige AMD Chipsätzen [GH 3134] ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-307">WARNING: There is an issue preventing WSL from running on some AMD chipsets [GH 3134].</span></span> <span data-ttu-id="d8d1c-308">Ein Fix ist bereit und machen die Möglichkeit, den Branch Insider-Build.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-308">A fix is ready and making its way to the Insider Build branch.</span></span>
* <span data-ttu-id="d8d1c-309">Fügen Sie die Explorer-Kontextmenü zum Starten von WSL [GH 437, 603 1836] hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-309">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="d8d1c-310">Hold-Schicht und mit der rechten Maustaste in einem Explorer-Fenster zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-310">To use hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="d8d1c-311">Beheben von Unix-Socket nicht blockierende Verhalten [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-311">Fix unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="d8d1c-312">Fix hängende NETLINK-Befehl aus, wie in GH 2026 angegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-312">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="d8d1c-313">Hinzufügen von Unterstützung für Mount-Weitergabeflags [GH 2911].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-313">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="d8d1c-314">Problem mit der truncate nicht zu Inotify Ereignisse [GH 2978] behoben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-314">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="d8d1c-315">Fügen Sie hinzu – Exec-Option für wsl.exe um eine einzelne Binärdatei ohne eine Shell aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-315">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="d8d1c-316">Fügen Sie hinzu – die Verteilungsoption für wsl.exe-Distribution, die eine bestimmte Auswahl.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-316">Add --distribution option for wsl.exe to select a specific distro.</span></span>

## <a name="build-17655-skip-ahead"></a><span data-ttu-id="d8d1c-317">Erstellen von 17655 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-317">Build 17655 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-318">Allgemeine Windows Informationen zum Build 17655 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-318">For general Windows information on build 17655 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-319">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-319">WSL</span></span>
* <span data-ttu-id="d8d1c-320">Eingeschränkte Unterstützung für "dmesg".</span><span class="sxs-lookup"><span data-stu-id="d8d1c-320">Limited support for dmesg.</span></span> <span data-ttu-id="d8d1c-321">Anwendungen können jetzt in "dmesg" protokollieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-321">Applications can now log to dmesg.</span></span> <span data-ttu-id="d8d1c-322">WSL-treiberprotokolle eingeschränkte Informationen zu "dmesg".</span><span class="sxs-lookup"><span data-stu-id="d8d1c-322">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="d8d1c-323">Dies kann in Zukunft erweitert werden, um weitere Informationen/Diagnosedaten aus dem Treiber durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-323">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="d8d1c-324">Hinweis: "dmesg" wird über derzeit unterstützt die `/dev/kmsg` Geräteschnittstelle.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-324">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> `syslog` <span data-ttu-id="d8d1c-325">Sycall-Schnittstelle ist noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-325">sycall interface is not yet supported.</span></span> <span data-ttu-id="d8d1c-326">Und natürlich einige von der `dmesg` Befehlszeilenoptionen wie z. B. `-S`, `-C` funktionieren nicht.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-326">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="d8d1c-327">Problem behoben, Vorgänge mit mehreren Threads konnten, in denen ENOENT zurückgeben, auch wenn die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-327">Fixed an issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="d8d1c-328">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-328">[GH 2712]</span></span>

## <a name="build-17639-skip-ahead"></a><span data-ttu-id="d8d1c-329">Erstellen von 17639 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-329">Build 17639 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-330">Allgemeine Windows Informationen zum Build 17639 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-330">For general Windows information on build 17639 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-331">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-331">WSL</span></span>
* <span data-ttu-id="d8d1c-332">Standard-Gruppen-ID und Modus der seriellen Geräten nativ [GH 3042] entsprechend zu ändern</span><span class="sxs-lookup"><span data-stu-id="d8d1c-332">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="d8d1c-333">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-333">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="d8d1c-334">Hinweis: DrvFs gelten einige Einschränkungen auf den Namen der erweiterten Attribute.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-334">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="d8d1c-335">Insbesondere einige Zeichen (wie '/', ':' und '\*") nicht zulässig sind, und erweiterte Attributnamen wird nicht in der Groß-/ Kleinschreibung auf DrvFs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-335">In particular, some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-17133-fast"></a><span data-ttu-id="d8d1c-336">Erstellen von 17133 (Fast)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-336">Build 17133 (Fast)</span></span>
<span data-ttu-id="d8d1c-337">Allgemeine Windows Informationen zum Build 17133 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-337">For general Windows information on build 17133 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-338">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-338">WSL</span></span>
* <span data-ttu-id="d8d1c-339">Korrektur für hänger in WSL.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-339">Fix for hang in WSL.</span></span> <span data-ttu-id="d8d1c-340">[GH 3039, 3034]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-340">[GH 3039, 3034]</span></span>

## <a name="build-17128-fast"></a><span data-ttu-id="d8d1c-341">Erstellen von 17128 (Fast)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-341">Build 17128 (Fast)</span></span>
<span data-ttu-id="d8d1c-342">Allgemeine Windows Informationen zum Build 17128 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-342">For general Windows information on build 17128 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-343">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-343">WSL</span></span>
* <span data-ttu-id="d8d1c-344">Keine</span><span class="sxs-lookup"><span data-stu-id="d8d1c-344">None</span></span>

## <a name="build-17627-skip-ahead"></a><span data-ttu-id="d8d1c-345">Erstellen von 17627 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-345">Build 17627 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-346">Allgemeine Windows Informationen zum Build 17627 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-346">For general Windows information on build 17627 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-347">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-347">WSL</span></span>
* <span data-ttu-id="d8d1c-348">Hinzufügen von Unterstützung für die Pi-fähigen Futex-Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-348">Add support for the futex pi-aware operations.</span></span> <span data-ttu-id="d8d1c-349">[GH 1006]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-349">[GH 1006]</span></span>
    * <span data-ttu-id="d8d1c-350">Beachten Sie, dass Prioritäten nicht aktuell ein unterstütztes Feature von WSL sind daher Einschränkungen bestehen, aber die Standardverwendung muss aufgehoben werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-350">Note that priorities are not currently a supported WSL feature so there are limitations, but standard usage should be unblocked.</span></span>
* <span data-ttu-id="d8d1c-351">Windows-Firewall-Unterstützung für die WSL-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-351">Windows firewall support for WSL processes.</span></span> <span data-ttu-id="d8d1c-352">[GH 1852]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-352">[GH 1852]</span></span>
    * <span data-ttu-id="d8d1c-353">Damit können die WSL verarbeiten, z. B. Python an einem beliebigen Port lauschen, verwenden Sie die Eingabeaufforderung mit erhöhten Windows:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-353">For example, to allow the WSL python process to listen on any port, use the elevated Windows cmd:</span></span>
```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```
    * <span data-ttu-id="d8d1c-354">Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-354">For additional details on how to add firewall rules, see [link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span></span>
* <span data-ttu-id="d8d1c-355">Berücksichtigen Sie bei Verwendung von wsl.exe Standardshell des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-355">Respect user's default shell when using wsl.exe.</span></span> <span data-ttu-id="d8d1c-356">[GH 2372]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-356">[GH 2372]</span></span>
* <span data-ttu-id="d8d1c-357">Melden Sie alle Netzwerkschnittstellen, als Ethernet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-357">Report all network interfaces as ethernet.</span></span> <span data-ttu-id="d8d1c-358">[GH 2996]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-358">[GH 2996]</span></span>
* <span data-ttu-id="d8d1c-359">Eine bessere Verarbeitung von beschädigt/etc/passwd-Datei.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-359">Better handling of corrupt /etc/passwd file.</span></span> <span data-ttu-id="d8d1c-360">[GH 3001]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-360">[GH 3001]</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-361">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-361">Console</span></span>
* <span data-ttu-id="d8d1c-362">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-362">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-363">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-363">LTP Results:</span></span>
<span data-ttu-id="d8d1c-364">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-364">Testing in progress.</span></span>

## <a name="build-17618-skip-ahead"></a><span data-ttu-id="d8d1c-365">Erstellen von 17618 (jetzt überspringen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-365">Build 17618 (Skip Ahead)</span></span>
<span data-ttu-id="d8d1c-366">Allgemeine Windows Informationen zum Build 17618 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-366">For general Windows information on build 17618 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-367">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-367">WSL</span></span>
* <span data-ttu-id="d8d1c-368">Einführen von Pseudoconsole-Funktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-368">Introduce pseudoconsole functionality for NT interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span></span>
* <span data-ttu-id="d8d1c-369">Die ältere Installationsmechanismus (lxrun.exe) wurde als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-369">The legacy install mechanism (lxrun.exe) has been deprecated.</span></span> <span data-ttu-id="d8d1c-370">Die unterstützte Mechanismus für die Installation von Verteilungen erfolgt über den Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-370">The supported mechanism for installing distributions is through the Microsoft Store.</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-371">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-371">Console</span></span>
* <span data-ttu-id="d8d1c-372">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-372">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-373">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-373">LTP Results:</span></span>
<span data-ttu-id="d8d1c-374">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-374">Testing in progress.</span></span>

## <a name="build-17110"></a><span data-ttu-id="d8d1c-375">Build 17110</span><span class="sxs-lookup"><span data-stu-id="d8d1c-375">Build 17110</span></span>
<span data-ttu-id="d8d1c-376">Allgemeine Windows Informationen zum Build 17110 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-376">For general Windows information on build 17110 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-377">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-377">WSL</span></span>
* <span data-ttu-id="d8d1c-378">Zulassen Sie/Init von Windows [GH 2928] beendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-378">Allow /init to be terminated from Windows [GH 2928].</span></span>
* <span data-ttu-id="d8d1c-379">DrvFs jetzt pro Verzeichnis Groß-/Kleinschreibung wird standardmäßig verwendet (entspricht der "Fall Dir =" Bereitstellungsoption).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-379">DrvFs now uses per-directory case sensitivity by default (equivalent to the “case=dir” mount option).</span></span>
    * <span data-ttu-id="d8d1c-380">Mithilfe von "Case Force =" (das alte Verhalten) erfordert einen Registrierungsschlüssel festlegen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-380">Using “case=force” (the old behavior) requires setting a registry key.</span></span> <span data-ttu-id="d8d1c-381">Führen Sie den folgenden Befehl zum Aktivieren "Fall Force =" Wenn Sie sie verwenden möchten: Reg hinzufügen HKLM\SYSTEM\CurrentControlSet\Services\lxss/v DrvFsAllowForceCaseSensitivity/t REG_DWORD/d 1</span><span class="sxs-lookup"><span data-stu-id="d8d1c-381">Run the following command to enable “case=force” if you need to use it: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span></span>
    * <span data-ttu-id="d8d1c-382">Wenn Sie vorhandene Verzeichnisse mit WSL erstellt werden, in früheren Version von Windows die Groß-/Kleinschreibung beachtet werden müssen haben, "fsutil.exe" verwenden, die um Groß-/ Kleinschreibung zu markieren: fsutil.exe Datei Setcasesensitiveinfo <path> aktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-382">If you have existing directories created with WSL in older version of Windows which need to be case sensitive, use fsutil.exe to mark them as case sensitive: fsutil.exe file setcasesensitiveinfo <path> enable</span></span>
* <span data-ttu-id="d8d1c-383">Zeichenfolgenende auf NULL aus dem Uname Syscall zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-383">NULL terminate strings returned from the uname syscall.</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-384">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-384">Console</span></span>
* <span data-ttu-id="d8d1c-385">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-385">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-386">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-386">LTP Results:</span></span>
<span data-ttu-id="d8d1c-387">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-387">Testing in progress.</span></span>

## <a name="build-17107"></a><span data-ttu-id="d8d1c-388">Build 17107</span><span class="sxs-lookup"><span data-stu-id="d8d1c-388">Build 17107</span></span>
<span data-ttu-id="d8d1c-389">Allgemeine Windows Informationen zum Build 17107 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-389">For general Windows information on build 17107 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-390">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-390">WSL</span></span>
* <span data-ttu-id="d8d1c-391">Unterstützen Sie TCSETSF und TCSETSW für master Pty-Endpunkte [GH 2552] an.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-391">Support TCSETSF and TCSETSW on master pty endpoints [GH 2552].</span></span>
* <span data-ttu-id="d8d1c-392">Interop-Prozesse gleichzeitig starten kann dazu führen, dass EINVAL [GH 2813].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-392">Starting simultaneous interop processes can result in EINVAL [GH 2813].</span></span>
* <span data-ttu-id="d8d1c-393">Beheben Sie PTRACE_ATTACH zum Anzeigen des Status der entsprechenden Ablaufverfolgung in /proc/pid/status.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-393">Fix PTRACE_ATTACH to show proper tracing status in /proc/pid/status.</span></span>
* <span data-ttu-id="d8d1c-394">Fix Race, in denen kurzlebige Prozesse mit CLEARTID sowohl SETTID Flags geklont, konnte beenden, ohne die TID-Adresse löschen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-394">Fix race where short-lived processes cloned with both the CLEARTID and SETTID flags could exit without clearing the TID address.</span></span>
* <span data-ttu-id="d8d1c-395">Beim Aktualisieren der Linux-Dateisystemverzeichnisse beim aus einem Build vor – 17093 verschieben, wird eine Meldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-395">Display a message when upgrading the Linux file system directories when moving from a pre-17093 build.</span></span> <span data-ttu-id="d8d1c-396">Weitere Informationen zu den 17093 dateisystemänderungen, finden Sie unter den Versionshinweisen für [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-396">For more details on the 17093 file system changes, see the release notes for [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-397">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-397">Console</span></span>
* <span data-ttu-id="d8d1c-398">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-398">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-399">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-399">LTP Results:</span></span>
<span data-ttu-id="d8d1c-400">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-400">Testing in progress.</span></span>

## <a name="build-17101"></a><span data-ttu-id="d8d1c-401">Build 17101</span><span class="sxs-lookup"><span data-stu-id="d8d1c-401">Build 17101</span></span>
<span data-ttu-id="d8d1c-402">Allgemeine Windows Informationen zum Build 17101 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-402">For general Windows information on build 17101 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-403">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-403">WSL</span></span>
* <span data-ttu-id="d8d1c-404">Unterstützung für Signalfd.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-404">Support for signalfd.</span></span> <span data-ttu-id="d8d1c-405">[GH 129]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-405">[GH 129]</span></span>
* <span data-ttu-id="d8d1c-406">Unterstützung von Dateinamen, NTFS ungültige Zeichen durch Codierung als private Unicode-Zeichen enthält.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-406">Support file-names containing illegal NTFS characters by encoding them as private Unicode characters.</span></span> <span data-ttu-id="d8d1c-407">[GH 1514]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-407">[GH 1514]</span></span>
* <span data-ttu-id="d8d1c-408">Automatische Bereitstellung erfolgt ein Fallback auf nur-Lese beim Schreiben nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-408">Auto mount will fallback to read-only when write is not supported.</span></span> <span data-ttu-id="d8d1c-409">[GH 2603]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-409">[GH 2603]</span></span>
* <span data-ttu-id="d8d1c-410">Ermöglichen Sie Einfügen der Unicode-Ersatzpaare (z. B. Emoji Zeichen).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-410">Allow pasting of Unicode surrogate pairs (like emoji characters).</span></span> <span data-ttu-id="d8d1c-411">[GH 2765]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-411">[GH 2765]</span></span>
* <span data-ttu-id="d8d1c-412">Pseudo-Dateien in/proc und /sys soll gelesen und schreiben kann jetzt von Select "," Abruf "," Epoll, Et Al. [GH 2838]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-412">Pseudo-files in /proc and /sys should return read and write ready from select, poll, epoll, et al. [GH 2838]</span></span>
* <span data-ttu-id="d8d1c-413">Korrigieren von Problem, Service in Endlosschleife zu wechseln aufgrund dessen, wenn die Registrierung manipuliert wurde, oder beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-413">Fix issue that could cause service to go into infinite loop when the registry has been tampered with or is corrupt.</span></span>
* <span data-ttu-id="d8d1c-414">Beheben Sie Netlink Nachrichten mit neueren (upstream 4.14) Version von iproute2 funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-414">Fix netlink messages to work with newer (upstream 4.14) version of iproute2.</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-415">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-415">Console</span></span>
* <span data-ttu-id="d8d1c-416">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-416">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-417">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-417">LTP Results:</span></span>
<span data-ttu-id="d8d1c-418">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-418">Testing in progress.</span></span>

## <a name="build-17093"></a><span data-ttu-id="d8d1c-419">Build 17093</span><span class="sxs-lookup"><span data-stu-id="d8d1c-419">Build 17093</span></span>
<span data-ttu-id="d8d1c-420">Allgemeine Windows Informationen zum Build 17093 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-420">For general Windows information on build 17093 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span></span>

#### <a name="important"></a><span data-ttu-id="d8d1c-421">Wichtig:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-421">Important:</span></span>
<span data-ttu-id="d8d1c-422">Wenn WSL zum ersten Mal nach dem Upgrade auf diesen Build gestartet wird, muss sie ein Upgrade der Linux-Dateisystemverzeichnisse Arbeit ausführen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-422">When starting WSL for the first time after upgrading to this build, it needs to perform some work upgrading the Linux file system directories.</span></span> <span data-ttu-id="d8d1c-423">Dieser Vorgang kann mehrere Minuten dauern, sodass WSL angezeigt werden kann, zu einem verlangsamten start.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-423">This may take up to several minutes, so WSL may appear to start slowly.</span></span> <span data-ttu-id="d8d1c-424">Dies sollte nur auftreten, nachdem für jede Verteilung Sie aus dem Store installiert haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-424">This should only happen once for each distribution you have installed from the store.</span></span>
* <span data-ttu-id="d8d1c-425">Verbesserte Unterstützung für die Groß-/Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-425">Improved case sensitivity support in DrvFs.</span></span>
    * <span data-ttu-id="d8d1c-426">DrvFs unterstützt jetzt pro Verzeichnis Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-426">DrvFs now supports per-directory case sensitivity.</span></span> <span data-ttu-id="d8d1c-427">Dies ist ein neues Flag, das festgelegt werden kann Verzeichnisse, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen behandelt werden sollen, Groß-/ Kleinschreibung, dadurch können auch Windows-Anwendungen zum ordnungsgemäß Öffnen von Dateien, die sich nur durch Fall unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-427">This is a new flag that can be set on directories to indicate all operations in those directories should be treated as case sensitive, which allows even Windows applications to correctly open files that differ only by case.</span></span>
    * <span data-ttu-id="d8d1c-428">DrvFs hat neue Bereitstellungsoption Steuerung der Groß-/Kleinschreibung in einer Basis pro Verzeichnis</span><span class="sxs-lookup"><span data-stu-id="d8d1c-428">DrvFs has new mount options controlling case sensitivity on a per-directory basis</span></span>
        * <span data-ttu-id="d8d1c-429">Fall = erzwingen: alle Verzeichnisse werden in der Groß-/ Kleinschreibung (mit Ausnahme der Stamm des Laufwerks) behandelt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-429">case=force: all directories are treated as case sensitive (except for the drive root).</span></span> <span data-ttu-id="d8d1c-430">Neue mit WSL erstellt Verzeichnisse werden Groß-/ Kleinschreibung markiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-430">New directories created with WSL are marked as case sensitive.</span></span> <span data-ttu-id="d8d1c-431">Dies ist das Legacyverhalten mit Ausnahme von markieren die neuen Verzeichnisse Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-431">This is the legacy behavior except for marking new directories case sensitive.</span></span>
        * <span data-ttu-id="d8d1c-432">Fall Dir =: behandelt nur die Verzeichnisse mit dem Flag pro Verzeichnis Groß-/Kleinschreibung wie Groß-/ Kleinschreibung beachtet. andere Verzeichnisse, die Groß-/Kleinschreibung beachtet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-432">case=dir: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="d8d1c-433">Neue mit WSL erstellt Verzeichnisse werden Groß-/ Kleinschreibung markiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-433">New directories created with WSL are marked as case sensitive.</span></span>
        * <span data-ttu-id="d8d1c-434">Fall = off: behandelt nur die Verzeichnisse mit dem Flag pro Verzeichnis Groß-/Kleinschreibung wie Groß-/ Kleinschreibung beachtet. andere Verzeichnisse, die Groß-/Kleinschreibung beachtet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-434">case=off: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="d8d1c-435">Neue Verzeichnisse mit WSL erstellt wurden, werden als Groß-/Kleinschreibung markiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-435">New directories created with WSL are marked as case insensitive.</span></span>
    * <span data-ttu-id="d8d1c-436">Hinweis: durch WSL in früheren Versionen erstellten Verzeichnisse keine dieses Flag festgelegt, sodass nicht behandelt wird Groß-/ Kleinschreibung bei der Verwendung, die "Fall Dir =" Option.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-436">Note: directories created by WSL in previous releases do not have this flag set, so will not be treated as case sensitive if you use the “case=dir” option.</span></span> <span data-ttu-id="d8d1c-437">Eine Möglichkeit, dieses Flag festgelegt wird, auf vorhandene Verzeichnisse wird bald verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-437">A way to set this flag on existing directories is coming soon.</span></span>
    * <span data-ttu-id="d8d1c-438">Beispiel für die Bereitstellung mit den folgenden Optionen (für vorhandene Laufwerke, Sie müssen zuerst die Einbindung aufheben, bevor Sie mit verschiedenen Optionen bereitstellen können): Sudo Mount -t Drvfs "c:" / Mnt/C - e/a Fall Dir =</span><span class="sxs-lookup"><span data-stu-id="d8d1c-438">Example of mounting with these options (for existing drives, you must first unmount before you can mount with different options): sudo mount -t drvfs C: /mnt/c -o case=dir</span></span>
    * <span data-ttu-id="d8d1c-439">Case-vorerst = Force ist immer noch die Standardoption.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-439">For now, case=force is still the default option.</span></span> <span data-ttu-id="d8d1c-440">Dies wird in Fall geändert Dir in der Zukunft =.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-440">This will be changed to case=dir in the future.</span></span>
* <span data-ttu-id="d8d1c-441">Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, beim Einbinden von DrvFs, z. B.: "sudo" einbinden -t Drvfs //server/share /mnt/share</span><span class="sxs-lookup"><span data-stu-id="d8d1c-441">You can now use forward slashes in Windows paths when mounting DrvFs, e.g.: sudo mount -t drvfs //server/share /mnt/share</span></span>
* <span data-ttu-id="d8d1c-442">WSL verarbeitet nun die Datei/etc/fstab beim Start der Instanz [GH 2636].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-442">WSL now processes the /etc/fstab file during instance start [GH 2636].</span></span>
    * <span data-ttu-id="d8d1c-443">Dies ist möglich, vor dem Bereitstellen von automatisch DrvFs-Laufwerken. alle Laufwerke, die bereits von "fstab" eingebunden wurden werden nicht automatisch erneut bereitgestellt werden können Sie den Bereitstellungspunkt für bestimmte Laufwerke zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-443">This is done prior to automatically mounting DrvFs drives; any drives that were already mounted by fstab will not be remounted automatically, allowing you to change the mount point for specific drives.</span></span>
    * <span data-ttu-id="d8d1c-444">Dieses Verhalten kann mithilfe von wsl.conf deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-444">This behavior can be turned off using wsl.conf.</span></span>
* <span data-ttu-id="d8d1c-445">Die Bereitstellung, Mountinfo Mountstats Dateien in/proc Escapesonderzeichen ordnungsgemäß wie umgekehrte Schrägstriche und Leerzeichen [GH 2799]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-445">The mount, mountinfo and mountstats files in /proc properly escape special characters like backslashes and spaces [GH 2799]</span></span>
* <span data-ttu-id="d8d1c-446">Spezielle Dateien, die mit DrvFs z. B. WSL symbolischer Verknüpfungen oder Fifos und Sockets erstellt wird, wenn Metadaten aktiviert ist, können jetzt kopiert und von Windows verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-446">Special files created with DrvFs such as WSL symbolic links, or fifos and sockets when metadata is enabled, can now be copied and moved from Windows.</span></span>

#### <a name="wsl-is-more-configurable-with-wslconf"></a><span data-ttu-id="d8d1c-447">WSL ist mit wsl.conf mehr konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-447">WSL is more configurable with wsl.conf</span></span>
<span data-ttu-id="d8d1c-448">Wir haben eine Methode für das bestimmte Funktionen automatisch in WSL zu konfigurieren, die jedes Mal, wenn Sie das Subsystem starten angewendet werden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-448">We added a method for you to automatically configure certain functionality in WSL that will be applied every time you launch the subsystem.</span></span> <span data-ttu-id="d8d1c-449">Dazu gehören Optionen für die automatische Bereitstellung und Konfiguration des Netzwerks.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-449">This includes automount options and network configuration.</span></span> <span data-ttu-id="d8d1c-450">Weitere Informationen finden sie in unserem Blogbeitrag unter: https://aka.ms/wslconf</span><span class="sxs-lookup"><span data-stu-id="d8d1c-450">Learn more about it in our blog post at: https://aka.ms/wslconf</span></span>

#### <a name="afunix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a><span data-ttu-id="d8d1c-451">AF_UNIX ermöglicht das WebSocket-Verbindungen zwischen Linux-Prozessen für WSL und native Windows-Prozesse</span><span class="sxs-lookup"><span data-stu-id="d8d1c-451">AF_UNIX allows socket connections between Linux processes on WSL and Windows native processes</span></span>
<span data-ttu-id="d8d1c-452">WSL und Windows-Anwendungen können jetzt über Unix-Sockets miteinander kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-452">WSL and Windows applications can now communicate with each other over Unix sockets.</span></span> <span data-ttu-id="d8d1c-453">Angenommen Sie, Sie möchten das Ausführen eines Diensts in Windows und sowohl Windows als auch WSL-apps zur Verfügung stellen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-453">Imagine you want to run a service in Windows and make it available to both Windows and WSL apps.</span></span> <span data-ttu-id="d8d1c-454">Das ist möglich, mit Unix-Sockets.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-454">Now, that’s possible with Unix sockets.</span></span> <span data-ttu-id="d8d1c-455">Lesen Sie mehr in unserem Blog unter Posten https://aka.ms/afunixinterop</span><span class="sxs-lookup"><span data-stu-id="d8d1c-455">Read more in our blog post at https://aka.ms/afunixinterop</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-456">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-456">WSL</span></span>
* <span data-ttu-id="d8d1c-457">Unterstützung von mmap() mit MAP_NORESERVE [GH 121, 2784]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-457">Support mmap() with MAP_NORESERVE [GH 121, 2784]</span></span>
* <span data-ttu-id="d8d1c-458">Unterstützen Sie CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-458">Support CLONE_PTRACE and CLONE_UNTRACED [GH 121, 2781]</span></span>
* <span data-ttu-id="d8d1c-459">Behandeln von nicht-SIGCHLD Beendigungssignal in Klon [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-459">Handle non-SIGCHLD termination signal in clone [GH 121, 2781]</span></span>
* <span data-ttu-id="d8d1c-460">Stub-/proc/sys/fs/inotify/max_user_instances und /proc/sys/fs/inotify/max_user_watches [GH 1705]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-460">Stub /proc/sys/fs/inotify/max_user_instances and /proc/sys/fs/inotify/max_user_watches [GH 1705]</span></span>
* <span data-ttu-id="d8d1c-461">Fehler beim Laden der ELF-Binärdateien, die Load-Header mit nicht-NULL-Offsets [GH 1884] enthalten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-461">Error loading ELF binaries that contain load headers with non-zero offsets [GH 1884]</span></span>
* <span data-ttu-id="d8d1c-462">0 (null) nicht mehr nachfolgende Seite Bytes beim Laden von Bildern.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-462">Zero out trailing page bytes when loading images.</span></span>
* <span data-ttu-id="d8d1c-463">Reduzieren von Fällen, in denen Execve im Hintergrund Prozess beendet wird</span><span class="sxs-lookup"><span data-stu-id="d8d1c-463">Reduce cases where execve silently terminates process</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-464">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-464">Console</span></span>
* <span data-ttu-id="d8d1c-465">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-465">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-466">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-466">LTP Results:</span></span>
<span data-ttu-id="d8d1c-467">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-467">Testing in progress.</span></span>

## <a name="build-17083"></a><span data-ttu-id="d8d1c-468">Build 17083</span><span class="sxs-lookup"><span data-stu-id="d8d1c-468">Build 17083</span></span>
<span data-ttu-id="d8d1c-469">Allgemeine Windows Informationen zum Build 17083 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-469">For general Windows information on build 17083 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-470">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-470">WSL</span></span>
* <span data-ttu-id="d8d1c-471">Feste fehlerüberprüfung im Zusammenhang mit Epoll [GH 2798, 2801, 2857]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-471">Fixed bugcheck related to epoll [GH 2798, 2801, 2857]</span></span>
* <span data-ttu-id="d8d1c-472">Feste hängt, wenn es sich bei deaktiviert ASLR [GH 1185, 2870]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-472">Fixed hangs when turning off ASLR [GH 1185, 2870]</span></span>
* <span data-ttu-id="d8d1c-473">Stellen Sie sicher, dass Vorgänge für "mmap" atomic [GH 2732] angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-473">Ensure mmap operations appear atomic [GH 2732]</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-474">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-474">Console</span></span>
* <span data-ttu-id="d8d1c-475">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-475">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-476">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-476">LTP Results:</span></span>
<span data-ttu-id="d8d1c-477">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-477">Testing in progress.</span></span>

## <a name="build-17074"></a><span data-ttu-id="d8d1c-478">Build 17074</span><span class="sxs-lookup"><span data-stu-id="d8d1c-478">Build 17074</span></span>
<span data-ttu-id="d8d1c-479">Allgemeine Windows Informationen zum Build 17074 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-479">For general Windows information on build 17074 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-480">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-480">WSL</span></span>
* <span data-ttu-id="d8d1c-481">Feste Speicherformat DrvFs Metadaten [GH 2777]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-481">Fixed storage format of DrvFs metadata [GH 2777]</span></span> </br>
<span data-ttu-id="d8d1c-482">**Wichtig:** DrvFs-Metadaten erstellt, bevor Sie diesen Build nicht ordnungsgemäß oder überhaupt nicht angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-482">**Important:** DrvFs metadata created before this build will show up incorrectly or not at all.</span></span> <span data-ttu-id="d8d1c-483">Verwenden Sie zum Beheben betroffener Dateien Chmod und Chown, um die Metadaten erneut anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-483">To fix affected files, use chmod and chown to re-apply the metadata.</span></span>
* <span data-ttu-id="d8d1c-484">Korrigiert: Probleme mit mehreren Signale und neu startbar Syscalls.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-484">Fixed issue with multiple signals and restartable syscalls.</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-485">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-485">Console</span></span>
* <span data-ttu-id="d8d1c-486">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-486">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-487">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-487">LTP Results:</span></span>
<span data-ttu-id="d8d1c-488">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-488">Testing in progress.</span></span>

## <a name="build-17063"></a><span data-ttu-id="d8d1c-489">Build 17063</span><span class="sxs-lookup"><span data-stu-id="d8d1c-489">Build 17063</span></span>
<span data-ttu-id="d8d1c-490">Allgemeine Windows Informationen zum Build 17063 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-490">For general Windows information on build 17063 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="d8d1c-491">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-491">WSL</span></span>
* <span data-ttu-id="d8d1c-492">DrvFs unterstützt zusätzliche Linux-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-492">DrvFs supports additional Linux metadata.</span></span> <span data-ttu-id="d8d1c-493">Dies ermöglicht das Festlegen der Besitzer und den Modus der Dateien, indem Sie Chmod/Chown und die Erstellung von speziellen Dateien wie Fifos, Unix-Sockets und Device-Dateien.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-493">This allows setting the owner and mode of files using chmod/chown, and also the creation of special files such as fifos, unix sockets and device files.</span></span> <span data-ttu-id="d8d1c-494">Dies ist standardmäßig für jetzt deaktiviert, da er noch experimentell ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-494">This is disabled by default for now since it's still experimental.</span></span>
<span data-ttu-id="d8d1c-495">**Hinweis**:  Ein Fehler wurde in den Metadaten-Format von DrvFs verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-495">**Note:**  We fixed a bug in the metadata format used by DrvFs.</span></span> <span data-ttu-id="d8d1c-496">Metadaten für diesen Build für Experimente funktioniert, zwar werden zukünftige Builds nicht ordnungsgemäß Metadaten, die von diesem Build erstellte gelesen werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-496">While metadata works on this build for experimentation, future builds will not correctly read metadata created by this build.</span></span>  <span data-ttu-id="d8d1c-497">Müssen Sie möglicherweise Besitzer für die geänderten Dateien manuell aktualisieren und auf Geräten mit einem benutzerdefinierten Geräte-ID werden neu erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-497">You might need to manually update owner for modified files and devices with a custom device ID will have to be recreated.</span></span>

  <span data-ttu-id="d8d1c-498">Um DrvFs bereitstellen, mit der Metadatenoption zu aktivieren (um es zu einer vorhandenen Bereitstellung aktivieren, Sie müssen zunächst aufheben):</span><span class="sxs-lookup"><span data-stu-id="d8d1c-498">To enable, mount DrvFs with the metadata option (to enable it on an existing mount, you must first unmount it):</span></span>

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  <span data-ttu-id="d8d1c-499">Linux-Berechtigungen werden als zusätzliche Metadaten zu der Datei hinzugefügt; Sie wirken sich nicht auf die Windows-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-499">Linux permissions are added as additional metadata to the file; they do not affect the Windows permissions.</span></span>  <span data-ttu-id="d8d1c-500">Beachten Sie, dass eine Datei mit einem Windows-Editor bearbeiten, die Metadaten entfernen kann.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-500">Remember, editing a file using a Windows editor may remove the metadata.</span></span> <span data-ttu-id="d8d1c-501">In diesem Fall wird die Datei auf die Standardberechtigungen zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-501">In this case, the file will revert to its default permissions.</span></span>

* <span data-ttu-id="d8d1c-502">Hinzugefügte Mount-Optionen um DrvFs für Dateien ohne Metadaten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-502">Added mount options to DrvFs to control files without metadata.</span></span>
  * <span data-ttu-id="d8d1c-503">UID: die Benutzer-ID für den Besitzer aller Dateien verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-503">uid: the user ID used for the owner of all files.</span></span>
  * <span data-ttu-id="d8d1c-504">Gruppen-ID: die Gruppen-ID für den Besitzer aller Dateien verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-504">gid: the group ID used for the owner of all files.</span></span>
  * <span data-ttu-id="d8d1c-505">"umask": eine oktale Maske von Berechtigungen für alle Dateien und Verzeichnisse ausschließen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-505">umask: an octal mask of permissions to exclude for all files and directories.</span></span>
  * <span data-ttu-id="d8d1c-506">fMask: eine oktale Maske von Berechtigungen für alle regulären Dateien ausschließen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-506">fmask: an octal mask of permissions to exclude for all regular files.</span></span>
  * <span data-ttu-id="d8d1c-507">Dmask: eine oktale Maske von Berechtigungen für alle Verzeichnisse ausschließen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-507">dmask: an octal mask of permissions to exclude for all directories.</span></span>

  <span data-ttu-id="d8d1c-508">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-508">For example:</span></span>
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  <span data-ttu-id="d8d1c-509">Kombinieren Sie mit der Metadatenoption ", geben Sie die Standardberechtigungen für Dateien ohne Metadaten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-509">Combine with the metadata option to specify default permissions for files without metadata.</span></span>

* <span data-ttu-id="d8d1c-510">Eingeführt, eine neue Umgebungsvariable `WSLENV`, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32-ausgetauscht werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-510">Introduced a new environment variable, `WSLENV`, to configure how environment variables flow between WSL and Win32.</span></span>

  <span data-ttu-id="d8d1c-511">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-511">For example:</span></span>

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  `WSLENV` <span data-ttu-id="d8d1c-512">ist eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozesse von Win32- oder Win32-Prozesse WSL aufgenommen werden kann.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-512">is a colon-delimited list of environment variables that can be included when launching WSL processes from Win32 or Win32 processes from WSL.</span></span>  <span data-ttu-id="d8d1c-513">Jede Variable kann als Suffix versehen werden, mit einem Schrägstrich, gefolgt von Flags, die angeben, wie diese umgesetzt werden können.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-513">Each variable can be suffixed with a slash followed by flags to specify how it is translated.</span></span>
  * <span data-ttu-id="d8d1c-514">p: Der Wert ist ein Pfad, der zwischen WSL-Pfade und Pfade der Win32-übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-514">p: The value is a path that should be translated between WSL paths and Win32 paths.</span></span>
  * <span data-ttu-id="d8d1c-515">l: Der Wert ist eine Liste von Pfaden an.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-515">l: The value is a list of paths.</span></span> <span data-ttu-id="d8d1c-516">In WSL ist es sich um eine durch Doppelpunkte getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-516">In WSL, it is a colon-delimited list.</span></span> <span data-ttu-id="d8d1c-517">In Win32 ist es sich um eine durch Semikolons getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-517">In Win32, it is a semicolon-delimited list.</span></span>
  * <span data-ttu-id="d8d1c-518">u: Der Wert darf nur enthalten sein beim Aufrufen von WSL über Win32</span><span class="sxs-lookup"><span data-stu-id="d8d1c-518">u: The value should only be included when invoking WSL from Win32</span></span>
  * <span data-ttu-id="d8d1c-519">w: Der Wert darf nur enthalten sein beim Aufrufen von Win32 von WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-519">w: The value should only be included when invoking Win32 from WSL</span></span>

  <span data-ttu-id="d8d1c-520">Sie können festlegen, `WSLENV` in bashrc oder die benutzerdefinierte Windows-Umgebung für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-520">You can set `WSLENV` in .bashrc or in the custom Windows environment for your user.</span></span>

* <span data-ttu-id="d8d1c-521">Drvfs Mounts behält ordnungsgemäß Zeitstempel Tar, cp -p (GH 1939)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-521">drvfs mounts correctly preserves timestamps from tar, cp -p (GH 1939)</span></span>
* <span data-ttu-id="d8d1c-522">Drvfs Symlinks melden die richtige Größe (GH 2641)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-522">drvfs symlinks report the correct size (GH 2641)</span></span>
* <span data-ttu-id="d8d1c-523">Lese-/Schreibzugriff funktioniert bei sehr großen e/a-Größen (GH 2653)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-523">read/write works for very large IO sizes (GH 2653)</span></span>
* <span data-ttu-id="d8d1c-524">Waitpid funktioniert mit Gruppen IDs (GH 2534)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-524">waitpid works with process group IDs (GH 2534)</span></span>
* <span data-ttu-id="d8d1c-525">erheblich verbesserte "mmap" Leistung für große Reserve-Regionen. verbessert die Leistung der Ghc (GH 1671)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-525">significantly improved mmap performance for large reserve regions; improves ghc performance (GH 1671)</span></span>
* <span data-ttu-id="d8d1c-526">Persönlichkeit für READ_IMPLIES_EXEC unterstützt werden; Korrekturen Maxima und Clisp (GH 1185)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-526">personality supports for READ_IMPLIES_EXEC; fixes maxima and clisp (GH 1185)</span></span>
* <span data-ttu-id="d8d1c-527">Mprotect unterstützt PROT_GROWSDOWN; Korrekturen Clisp (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-527">mprotect supports PROT_GROWSDOWN; fixes clisp (GH 1128)</span></span>
* <span data-ttu-id="d8d1c-528">Seite im Fehler enthaltenen Updates overcommit Modus; Korrekturen Sbcl (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-528">page fault fixes in overcommit mode; fixes sbcl (GH 1128)</span></span>
* <span data-ttu-id="d8d1c-529">Klonen unterstützt mehr Kombinationen der flags</span><span class="sxs-lookup"><span data-stu-id="d8d1c-529">clone supports more flags combinations</span></span>
* <span data-ttu-id="d8d1c-530">Auswählen/Epoll Epoll-Dateien (zuvor keine Aktion) zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-530">Support select/epoll of epoll files (previously a no-op).</span></span>
* <span data-ttu-id="d8d1c-531">Benachrichtigen Sie Ptrace von nicht implementierte Syscalls.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-531">Notify ptrace of unimplemented syscalls.</span></span>
* <span data-ttu-id="d8d1c-532">Ignorieren Sie Schnittstellen, die nicht aktiv, beim Generieren von "resolv.conf" Nameservers [GH 2694 sind]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-532">Ignore interfaces that are not up when generating resolv.conf nameservers [GH 2694]</span></span>
* <span data-ttu-id="d8d1c-533">Auflisten von Netzwerkschnittstellen ohne physische Adresse.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-533">Enumerate network interfaces with no physical address.</span></span> <span data-ttu-id="d8d1c-534">[GH 2685]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-534">[GH 2685]</span></span>
* <span data-ttu-id="d8d1c-535">Zusätzliche Fehlerbehebungen und Verbesserungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-535">Additional bug fixes and improvements.</span></span>

### <a name="linux-tools-available-to-developers-on-windows"></a><span data-ttu-id="d8d1c-536">Linux-Tools für Entwickler für Windows</span><span class="sxs-lookup"><span data-stu-id="d8d1c-536">Linux tools available to developers on Windows</span></span>

* <span data-ttu-id="d8d1c-537">Windows-Befehlszeile Toolkette enthält Bsdtar (Tar) und Curl.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-537">Windows Command line Toolchain includes bsdtar (tar) and curl.</span></span>
  <span data-ttu-id="d8d1c-538">Lesen [diesen Blog](https://aka.ms/tarcurlwindows) erfahren mehr über das Hinzufügen dieser zwei neue Tools und wie sie die entwicklererfahrung für Windows strukturiert sind.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-538">Read [this blog](https://aka.ms/tarcurlwindows) to learn more about the addition of these two new tools and see how they’re shaping the developer experience on Windows.</span></span>

*   `AF_UNIX` <span data-ttu-id="d8d1c-539">ist in der Windows-Insider-SDK (17061 und höher) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-539">is available in the Windows Insider SDK (17061+).</span></span>
  <span data-ttu-id="d8d1c-540">Lesen [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) erfahren Sie mehr über `AF_UNIX` und wie Entwickler Windows sie verwenden können.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-540">Read [this blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) to learn more about `AF_UNIX` and how developers on Windows can use it.</span></span>

### <a name="console"></a><span data-ttu-id="d8d1c-541">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-541">Console</span></span>
* <span data-ttu-id="d8d1c-542">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-542">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-543">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-543">LTP Results:</span></span>
<span data-ttu-id="d8d1c-544">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-544">Testing in progress.</span></span>


## <a name="build-17046"></a><span data-ttu-id="d8d1c-545">Build 17046</span><span class="sxs-lookup"><span data-stu-id="d8d1c-545">Build 17046</span></span>

<span data-ttu-id="d8d1c-546">Allgemeine Windows Informationen zum Build 17046 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-546">For general Windows information on build 17046 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span></span>

### <a name="fixed"></a><span data-ttu-id="d8d1c-547">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-547">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-548">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-548">WSL</span></span>
- <span data-ttu-id="d8d1c-549">Können Sie Prozesse, ohne eine aktive Terminaldienste ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-549">Allow processes to run without an active terminal.</span></span> <span data-ttu-id="d8d1c-550">[GH 709, 1007, 1511, 2252, 2391, et al.]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-550">[GH 709, 1007, 1511, 2252, 2391, et al.]</span></span>
- <span data-ttu-id="d8d1c-551">Eine bessere Unterstützung für CLONE_VFORK und CLONE_VM zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-551">Better support of CLONE_VFORK and CLONE_VM.</span></span> <span data-ttu-id="d8d1c-552">[GH 1878, 2615]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-552">[GH 1878, 2615]</span></span>
- <span data-ttu-id="d8d1c-553">Überspringen Sie TDI-Filtertreiber WSL networking Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-553">Skip TDI filter drivers for WSL networking operations.</span></span> <span data-ttu-id="d8d1c-554">[GH 1554]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-554">[GH 1554]</span></span>
- <span data-ttu-id="d8d1c-555">DrvFs erstellt NT symbolische Verknüpfungen, wenn bestimmte Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-555">DrvFs creates NT symlinks when certain conditions are met.</span></span> <span data-ttu-id="d8d1c-556">[GH 353, 1475, 2602]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-556">[GH 353, 1475, 2602]</span></span>
    - <span data-ttu-id="d8d1c-557">Das Ziel des Links relativ sein muss, muss keine Bereitstellungspunkte oder symbolische Verknüpfungen überschreiten und muss vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-557">The link target must be relative, must not cross any mount points or symlinks, and must exist.</span></span>
    - <span data-ttu-id="d8d1c-558">Der Benutzer benötigen SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (Dies müssen Sie normalerweise wsl.exe mit erhöhten Rechten starten), es sei denn, der Entwicklermodus aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-558">The user must have SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (this normally requires you to launch wsl.exe elevated), unless Developer Mode is turned on.</span></span>
    - <span data-ttu-id="d8d1c-559">In allen anderen Fällen wird DrvFs weiterhin WSL symbolische Verknüpfungen erstellt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-559">In all other situations, DrvFs still creates WSL symlinks.</span></span>
- <span data-ttu-id="d8d1c-560">Ermöglichen Sie die mit erhöhten Rechten und ohne erhöhte Rechte WSL-Instanzen gleichzeitig ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-560">Allow running elevated and non-elevated WSL instances simultaneously.</span></span>
- <span data-ttu-id="d8d1c-561">Unterstützung von /proc/sys/kernel/yama/ptrace_scope</span><span class="sxs-lookup"><span data-stu-id="d8d1c-561">Support /proc/sys/kernel/yama/ptrace_scope</span></span>
- <span data-ttu-id="d8d1c-562">Fügen Sie Wslpath dazu WSL <> – Windows-Pfad-Konvertierungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-562">Add wslpath to do WSL<->Windows path conversions.</span></span> <span data-ttu-id="d8d1c-563">[GH 522, 1243, 1834, 2327, et al.]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-563">[GH 522, 1243, 1834, 2327, et al.]</span></span>
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a><span data-ttu-id="d8d1c-564">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-564">Console</span></span>
- <span data-ttu-id="d8d1c-565">Keine Reparaturen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-565">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-566">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-566">LTP Results:</span></span>
<span data-ttu-id="d8d1c-567">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-567">Testing in progress.</span></span>


## <a name="build-17040"></a><span data-ttu-id="d8d1c-568">Build 17040</span><span class="sxs-lookup"><span data-stu-id="d8d1c-568">Build 17040</span></span>

<span data-ttu-id="d8d1c-569">Allgemeine Windows Informationen zum Build 17040 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-569">For general Windows information on build 17040 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-570">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-570">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-571">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-571">WSL</span></span>
- <span data-ttu-id="d8d1c-572">Keine Fehlerbehebungen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-572">No fixes since 17035.</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-573">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-573">Console</span></span>
- <span data-ttu-id="d8d1c-574">Keine Fehlerbehebungen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-574">No fixes since 17035.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-575">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-575">LTP Results:</span></span>
<span data-ttu-id="d8d1c-576">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-576">Testing in progress.</span></span>

## <a name="build-17035"></a><span data-ttu-id="d8d1c-577">Build 17035</span><span class="sxs-lookup"><span data-stu-id="d8d1c-577">Build 17035</span></span>

<span data-ttu-id="d8d1c-578">Allgemeine Windows Informationen zum Build 17035 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-578">For general Windows information on build 17035 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-579">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-579">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-580">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-580">WSL</span></span>
- <span data-ttu-id="d8d1c-581">Zugreifen auf Dateien auf DrvFs konnte mit dem EINVAL gelegentlich fehl.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-581">Accessing files on DrvFs could occasionally fail with EINVAL.</span></span> <span data-ttu-id="d8d1c-582">[GH 2448]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-582">[GH 2448]</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-583">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-583">Console</span></span>
- <span data-ttu-id="d8d1c-584">Einige Farbe verloren gehen, beim Einfügen/Löschen von Zeilen im VT-Modus.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-584">Some color loss when inserting/deleting lines in VT mode.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-585">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-585">LTP Results:</span></span>
<span data-ttu-id="d8d1c-586">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-586">Testing in progress.</span></span>

## <a name="build-17025"></a><span data-ttu-id="d8d1c-587">Build 17025</span><span class="sxs-lookup"><span data-stu-id="d8d1c-587">Build 17025</span></span>

<span data-ttu-id="d8d1c-588">Allgemeine Windows Informationen zum Build 17025 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-588">For general Windows information on build 17025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-589">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-589">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-590">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-590">WSL</span></span>
- <span data-ttu-id="d8d1c-591">Starten Sie in einer neuen Gruppe für Vordergrund-Prozess [GH 1653, 2510] erste Prozesse.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-591">Start initial processes in a new foreground process group [GH 1653, 2510].</span></span>
- <span data-ttu-id="d8d1c-592">SIGHUP Delivery behebt [GH 2496].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-592">SIGHUP delivery fixes [GH 2496].</span></span>
- <span data-ttu-id="d8d1c-593">Standardname für die virtuellen Bridge zu generieren, wenn kein [GH 2497].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-593">Generate default virtual bridge name if none provided [GH 2497].</span></span>
- <span data-ttu-id="d8d1c-594">Implementieren Sie /proc/sys/kernel/random/boot_id [GH 2518].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-594">Implement /proc/sys/kernel/random/boot_id [GH 2518].</span></span>
- <span data-ttu-id="d8d1c-595">Mehr interop Stdout/Stderr-Pipe behoben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-595">More interop stdout/stderr pipe fixes.</span></span>
- <span data-ttu-id="d8d1c-596">Stub-Syncfs Systemaufruf.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-596">Stub syncfs system call.</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-597">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-597">Console</span></span>
- <span data-ttu-id="d8d1c-598">Korrigieren der Eingabe VT-Übersetzung für Drittanbieter-Konsolen [GH 111]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-598">Fix input VT translation for third party consoles [GH 111]</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-599">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-599">LTP Results:</span></span>
<span data-ttu-id="d8d1c-600">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-600">Testing in progress.</span></span>

## <a name="build-17017"></a><span data-ttu-id="d8d1c-601">Build 17017</span><span class="sxs-lookup"><span data-stu-id="d8d1c-601">Build 17017</span></span>

<span data-ttu-id="d8d1c-602">Allgemeine Windows Informationen zum Build 17017 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-602">For general Windows information on build 17017 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-603">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-603">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-604">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-604">WSL</span></span>
- <span data-ttu-id="d8d1c-605">Ignorieren Sie die leere ELF-Anwendung-Header [GH 330].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-605">Ignore empty ELF program headers [GH 330].</span></span>
- <span data-ttu-id="d8d1c-606">LxssManager zum Erstellen von WSL-Instanzen für nicht interaktive Benutzer zuzulassen (ssh und geplante Tasks-Unterstützung) [GH 777 1602].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-606">Allow LxssManager to create WSL instances for non-interactive users (ssh and scheduled task support) [GH 777, 1602].</span></span>
- <span data-ttu-id="d8d1c-607">Win32-Unterstützung WSL > WSL ("Einführung")-Szenarios [GH 1228] ->.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-607">Support WSL->Win32->WSL ("inception") scenarios [GH 1228].</span></span>
- <span data-ttu-id="d8d1c-608">Eingeschränkte Unterstützung für die Beendigung der Konsolen-apps, die über Interop [GH 1614] aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-608">Limited support for termination of console apps invoked via interop [GH 1614].</span></span>
- <span data-ttu-id="d8d1c-609">Mount-Supportoptionen für Devpts [GH 1948].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-609">Support mount options for devpts [GH 1948].</span></span>
- <span data-ttu-id="d8d1c-610">Ptrace untergeordneten Start [GH 2333] blockiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-610">Ptrace blocking child startup [GH 2333].</span></span>
- <span data-ttu-id="d8d1c-611">EPOLLET fehlen einige Ereignisse [GH 2462].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-611">EPOLLET missing some events [GH 2462].</span></span>
- <span data-ttu-id="d8d1c-612">Geben Sie weitere Daten für PTRACE_GETSIGINFO zurück.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-612">Return more data for PTRACE_GETSIGINFO.</span></span>
- <span data-ttu-id="d8d1c-613">Getdents mit Lseek gibt falsche Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-613">Getdents with lseek gives incorrect results.</span></span>
- <span data-ttu-id="d8d1c-614">Beheben Sie einige Win32-Interop-app-Abstürze, warten auf Eingabe für eine Pipe, die keine Daten mehr.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-614">Fix some Win32 interop app hangs, waiting for input on a pipe that has no more data.</span></span>
- <span data-ttu-id="d8d1c-615">O_ASYNC-Unterstützung für tty/Pty-Dateien.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-615">O_ASYNC support for tty/pty files.</span></span>
- <span data-ttu-id="d8d1c-616">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-616">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-617">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-617">Console</span></span>
- <span data-ttu-id="d8d1c-618">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-618">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-619">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-619">LTP Results:</span></span>
<span data-ttu-id="d8d1c-620">Tests werden durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-620">Testing in progress.</span></span>

## <a name="fall-creators-update"></a><span data-ttu-id="d8d1c-621">Fall Creators Update</span><span class="sxs-lookup"><span data-stu-id="d8d1c-621">Fall Creators Update</span></span>

## <a name="build-16288"></a><span data-ttu-id="d8d1c-622">Build 16288</span><span class="sxs-lookup"><span data-stu-id="d8d1c-622">Build 16288</span></span>

<span data-ttu-id="d8d1c-623">Allgemeine Windows Informationen zum Build 16288 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-623">For general Windows information on build 16288 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-624">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-624">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-625">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-625">WSL</span></span>
- <span data-ttu-id="d8d1c-626">Ordnungsgemäß zu initialisieren Sie und zu melden Sie, Uid und Gid-Modus für Socket Dateideskriptoren [GH 2490]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-626">Correctly initialize and report uid, gid, and mode for socket file descriptors [GH 2490]</span></span>
- <span data-ttu-id="d8d1c-627">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-627">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-628">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-628">Console</span></span>
- <span data-ttu-id="d8d1c-629">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-629">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-630">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-630">LTP Results:</span></span>
<span data-ttu-id="d8d1c-631">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="d8d1c-631">No change since 16273</span></span>

## <a name="build-16278"></a><span data-ttu-id="d8d1c-632">Build 16278</span><span class="sxs-lookup"><span data-stu-id="d8d1c-632">Build 16278</span></span>

<span data-ttu-id="d8d1c-633">Allgemeine Windows Informationen zum Build 162738 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-633">For general Windows information on build 162738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-634">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-634">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-635">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-635">WSL</span></span>
- <span data-ttu-id="d8d1c-636">Aufheben Sie explizit zugeordnete Ansichten der Abschnitte der Datei, wenn LX MM Wiederherstellungsoptionen [GH 2415] liegen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-636">Explicitly unmap mapped views of file backed sections when tearing down LX MM state [GH 2415]</span></span>
- <span data-ttu-id="d8d1c-637">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-637">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-638">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-638">Console</span></span>
- <span data-ttu-id="d8d1c-639">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-639">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-640">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-640">LTP Results:</span></span>
<span data-ttu-id="d8d1c-641">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="d8d1c-641">No change since 16273</span></span>

## <a name="build-16275"></a><span data-ttu-id="d8d1c-642">Build 16275</span><span class="sxs-lookup"><span data-stu-id="d8d1c-642">Build 16275</span></span>

<span data-ttu-id="d8d1c-643">Allgemeine Windows Informationen zum Build 162735 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-643">For general Windows information on build 162735 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-644">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-644">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-645">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-645">WSL</span></span>
- <span data-ttu-id="d8d1c-646">Keine WSL im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-646">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-647">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-647">Console</span></span>
- <span data-ttu-id="d8d1c-648">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-648">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-649">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-649">LTP Results:</span></span>
<span data-ttu-id="d8d1c-650">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="d8d1c-650">No change since 16273</span></span>

## <a name="build-16273"></a><span data-ttu-id="d8d1c-651">Build 16273</span><span class="sxs-lookup"><span data-stu-id="d8d1c-651">Build 16273</span></span>

<span data-ttu-id="d8d1c-652">Allgemeine Windows Informationen zum Build 16273 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-652">For general Windows information on build 16273 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-653">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-653">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-654">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-654">WSL</span></span>
- <span data-ttu-id="d8d1c-655">Ein Problem wurde behoben, bei dem gemeldet DrvFs manchmal des falschen Typs für Verzeichnisse [GH 2392]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-655">Fixed an issue where DrvFs sometimes reported the wrong file type for directories [GH 2392]</span></span>
- <span data-ttu-id="d8d1c-656">Zulassen der Erstellung von NETLINK_KOBJECT_UEVENT Sockets Programme Blockierung aufheben, Uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-656">Allow creation of NETLINK_KOBJECT_UEVENT sockets to unblock programs that use uevent [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span></span>
- <span data-ttu-id="d8d1c-657">Hinzufügen von Unterstützung für nicht blockierende connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-657">Add support for non-blocking connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span></span>
- <span data-ttu-id="d8d1c-658">Implementieren Sie CLONE_FS Klonen Aufruf Systemflag [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-658">Implement CLONE_FS clone system call flag [GH 2242]</span></span>
- <span data-ttu-id="d8d1c-659">Beheben von Problemen hinsichtlich der Behandlung von nicht Registerkarten oder Anführungszeichen ordnungsgemäß in NT-Interop [GH 1625, 2164]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-659">Fix issues around not handling tabs or quotes correctly in NT interop [GH 1625, 2164]</span></span>
- <span data-ttu-id="d8d1c-660">Zugriff verweigert, Fehler beim Versuch, WSL neu starten [GH 651, 2095]-Instanzen zu beheben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-660">Resolve access denied error when trying to re-launch WSL instances [GH 651, 2095]</span></span>
- <span data-ttu-id="d8d1c-661">Implementieren Sie Futex FUTEX_REQUEUE und FUTEX_CMP_REQUEUE Vorgänge [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-661">Implement futex FUTEX_REQUEUE and FUTEX_CMP_REQUEUE operations [GH 2242]</span></span>
- <span data-ttu-id="d8d1c-662">Korrigieren Sie die Berechtigungen für verschiedene SysFs-Dateien [GH 2214]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-662">Fix permissions for various SysFs files [GH 2214]</span></span>
- <span data-ttu-id="d8d1c-663">Beheben von Haskell Stack Absturz während des Setups [GH 2290]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-663">Fix Haskell stack hang during setup [GH 2290]</span></span>
- <span data-ttu-id="d8d1c-664">Implementieren von Binfmt_misc 'C' ' O' und 'P' Flags [GH 2103]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-664">Implement binfmt_misc 'C' 'O' and 'P' flags [GH 2103]</span></span>
- <span data-ttu-id="d8d1c-665">Hinzufügen von /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-665">Add /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span></span>
- <span data-ttu-id="d8d1c-666">Hinzufügen von teilweise Unterstützung für Ioprio_set Systemaufruf [GH 498]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-666">Add partial support for ioprio_set system call [GH 498]</span></span>
- <span data-ttu-id="d8d1c-667">Stub-SO_REUSEPORT und Hinzufügen von Unterstützung für SO_PASSCRED für Netlink Sockets [GH 69]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-667">Stub SO_REUSEPORT & adding support for SO_PASSCRED for netlink sockets [GH 69]</span></span>
- <span data-ttu-id="d8d1c-668">Verschiedene Fehlercodes aus RegisterDistribuiton zurück, wenn derzeit eine Verteilung wird installiert oder deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-668">Return different error codes from RegisterDistribuiton if a distribution is currently being installed or uninstalled.</span></span>
- <span data-ttu-id="d8d1c-669">Aufheben der Registrierung, der teilweise installierten WSL Verteilungen über wslconfig.exe zulassen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-669">Allow unregistration of partially installed WSL distributions via wslconfig.exe</span></span>
- <span data-ttu-id="d8d1c-670">Beheben Sie die Python-Socket Test hängt vom udp::msg_peek</span><span class="sxs-lookup"><span data-stu-id="d8d1c-670">Fix python socket test hang from udp::msg_peek</span></span>
- <span data-ttu-id="d8d1c-671">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-671">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-672">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-672">Console</span></span>
- <span data-ttu-id="d8d1c-673">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-673">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-674">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-674">LTP Results:</span></span>
<span data-ttu-id="d8d1c-675">Tests insgesamt: 1904</span><span class="sxs-lookup"><span data-stu-id="d8d1c-675">Total Tests: 1904</span></span><br/>
<span data-ttu-id="d8d1c-676">Gesamtzahl von übersprungenen Tests: 209</span><span class="sxs-lookup"><span data-stu-id="d8d1c-676">Total Skipped Tests: 209</span></span><br/>
<span data-ttu-id="d8d1c-677">Fehler beim von insgesamt: 229</span><span class="sxs-lookup"><span data-stu-id="d8d1c-677">Total Failures: 229</span></span><br/>
[<span data-ttu-id="d8d1c-678">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-678">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a><span data-ttu-id="d8d1c-679">Build 16257</span><span class="sxs-lookup"><span data-stu-id="d8d1c-679">Build 16257</span></span>

<span data-ttu-id="d8d1c-680">Allgemeine Windows Informationen zum Build 16257 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-680">For general Windows information on build 16257 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-681">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-681">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-682">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-682">WSL</span></span>
- <span data-ttu-id="d8d1c-683">Implementieren von prlimit64 Systemaufruf</span><span class="sxs-lookup"><span data-stu-id="d8d1c-683">Implement prlimit64 system call</span></span>
- <span data-ttu-id="d8d1c-684">Hinzufügen von Unterstützung für Ulimit – n (Setrlimit RLIMIT_NOFILE) [GH 1688]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-684">Add support for ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span></span>
- <span data-ttu-id="d8d1c-685">Stub MSG_MORE für TCP-Sockets [GH 2351]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-685">Stub MSG_MORE for TCP sockets [GH 2351]</span></span>
- <span data-ttu-id="d8d1c-686">Korrigieren Sie Ungültiger AT_EXECFN zusätzliche Vektor Verhalten [GH 2133]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-686">Fix invalid AT_EXECFN auxiliary vector behavior [GH 2133]</span></span>
- <span data-ttu-id="d8d1c-687">Zu beheben Sie, kopieren und Einfügen-Verhalten für Konsole/tty, und fügen Sie eine bessere vollen Puffer behandeln [GH 2204, 2131]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-687">Fix copy/paste behavior for console/tty, and add better full buffer handling [GH 2204, 2131]</span></span>
- <span data-ttu-id="d8d1c-688">Legen Sie AT_SECURE in zusätzlichen Vektor für Set-Benutzer-ID "und" Set-Gruppen-ID-Programme [GH 2031]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-688">Set AT_SECURE in auxiliary vector for set-user-ID and set-group-ID programs [GH 2031]</span></span>
- <span data-ttu-id="d8d1c-689">Pseudonamens-Terminal masterendpunkt TIOCPGRP [GH 1063] nicht behandelt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-689">Psuedo-terminal master endpoint not handling TIOCPGRP [GH 1063]</span></span>
- <span data-ttu-id="d8d1c-690">Korrektur Lseek wird dies, um die Verzeichnisse im LxFs [GH 2310] rewind</span><span class="sxs-lookup"><span data-stu-id="d8d1c-690">Fix lseek does to rewind directories in LxFs [GH 2310]</span></span>
- <span data-ttu-id="d8d1c-691">/dev/ptmx stürzt ab, nach einer hohen Auslastung [GH 1882]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-691">/dev/ptmx locks up after heavy usage [GH 1882]</span></span>
- <span data-ttu-id="d8d1c-692">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-692">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-693">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-693">Console</span></span>
- <span data-ttu-id="d8d1c-694">Korrektur für horizontale Linien/Unterstriche überall [GH 2168]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-694">Fix for horizontal Lines/Underscores Everywhere [GH 2168]</span></span>
- <span data-ttu-id="d8d1c-695">Korrektur für die prozessreihenfolge schwieriger zu [GH 2170] zu schließen und NPM geändert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-695">Fix for process order changed making NPM harder to close [GH 2170]</span></span>
- <span data-ttu-id="d8d1c-696">Unser neues Farbschema wird hinzugefügt: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span><span class="sxs-lookup"><span data-stu-id="d8d1c-696">Added our new color scheme: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-697">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-697">LTP Results:</span></span>
<span data-ttu-id="d8d1c-698">Keine Änderung seit 16251</span><span class="sxs-lookup"><span data-stu-id="d8d1c-698">No change since 16251</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-699">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-699">Syscall Support</span></span>
<span data-ttu-id="d8d1c-700">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-700">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-701">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-701">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`prlimit64`<br/>

### <a name="known-issues"></a><span data-ttu-id="d8d1c-702">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="d8d1c-702">Known Issues</span></span>
#### [<a name="github-issue-2392-windows-folders-not-recognized-by-wsl-"></a><span data-ttu-id="d8d1c-703">GitHub-Problem 2392: Windows-Ordner, die nicht von WSL erkannt...</span><span class="sxs-lookup"><span data-stu-id="d8d1c-703">GitHub Issue 2392: Windows Folders not recognized by WSL ...</span></span>](https://github.com/Microsoft/BashOnWindows/issues/2392)
<span data-ttu-id="d8d1c-704">Im Build 16257 WSL verfügt über Probleme beim Aufzählen von Windows-Dateien und Ordner über `/mnt/c/...`.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-704">In build 16257, WSL has issues when enumerating Windows files/folders via `/mnt/c/...`.</span></span>
<span data-ttu-id="d8d1c-705">Dieses Problem wurde behoben und freigegeben werden soll, im Insiders-build während der Woche ab ab 8/14/2017.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-705">This issue has been fixed and should be released in Insiders build during week commencing 8/14/2017.</span></span>

<br/>

## <a name="build-16251"></a><span data-ttu-id="d8d1c-706">Build 16251</span><span class="sxs-lookup"><span data-stu-id="d8d1c-706">Build 16251</span></span>

<span data-ttu-id="d8d1c-707">Allgemeine Windows Informationen zum Build 16251 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-707">For general Windows information on build 16251 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-708">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-708">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-709">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-709">WSL</span></span>
- <span data-ttu-id="d8d1c-710">Beta-Tag von WSL optionale Komponente entfernen, finden Sie unter [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) Details.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-710">Remove beta tag from WSL optional component, see [blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) for details.</span></span>
- <span data-ttu-id="d8d1c-711">Richtig initialisiert gespeichert-Set-Uid und Gid für Set-Benutzer-ID "und" Set-Gruppen-ID-Binärdateien auf Exec [GH 962, 1415, 2072]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-711">Correctly initialize saved-set uid and gid for set-user-ID and set-group-ID binaries on exec [GH 962, 1415, 2072]</span></span>
- <span data-ttu-id="d8d1c-712">Unterstützung für Ptrace PTRACE_O_TRACEEXIT [GH 555]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-712">Added support for ptrace PTRACE_O_TRACEEXIT [GH 555]</span></span>
- <span data-ttu-id="d8d1c-713">Unterstützung für Ptrace PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-713">Added support for ptrace PTRACE_GETFPREGS and PTRACE_GETREGSET with NT_FPREGSET [GH 555]</span></span>
- <span data-ttu-id="d8d1c-714">Informationen zum Beenden für ignoriert Signale Ptrace behoben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-714">Fixed ptrace to stop on ignored signals</span></span>
- <span data-ttu-id="d8d1c-715">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-715">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-716">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-716">Console</span></span>
- <span data-ttu-id="d8d1c-717">Keine Konsole im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-717">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-718">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-718">LTP Results:</span></span>
<span data-ttu-id="d8d1c-719">Anzahl der erfolgreichen Tests: 768</span><span class="sxs-lookup"><span data-stu-id="d8d1c-719">Number of Passing Tests: 768</span></span></br>
<span data-ttu-id="d8d1c-720">Anzahl der fehlgeschlagenen Tests: 244</span><span class="sxs-lookup"><span data-stu-id="d8d1c-720">Number of Failing Tests: 244</span></span></br>
<span data-ttu-id="d8d1c-721">Anzahl der übersprungenen Tests: 96</span><span class="sxs-lookup"><span data-stu-id="d8d1c-721">Number of Skipped Tests: 96</span></span></br>
[<span data-ttu-id="d8d1c-722">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-722">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a><span data-ttu-id="d8d1c-723">Build 16241</span><span class="sxs-lookup"><span data-stu-id="d8d1c-723">Build 16241</span></span>

<span data-ttu-id="d8d1c-724">Allgemeine Windows Informationen zum Build 16241 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-724">For general Windows information on build 16241 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-725">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-725">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="d8d1c-726">WSL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-726">WSL</span></span>
- <span data-ttu-id="d8d1c-727">Keine WSL im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-727">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="d8d1c-728">Console</span><span class="sxs-lookup"><span data-stu-id="d8d1c-728">Console</span></span>
- <span data-ttu-id="d8d1c-729">Fehlerbehebung für die Ausgabe des falschen Zeichens für den DEC überschreiten Linien ursprünglich gemeldet [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-729">Fix for outputting the wrong character for the crossing-lines DEC, originally reported [here](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span></span>
- <span data-ttu-id="d8d1c-730">Fehlerbehebung für die kein Ausgabetext angezeigt wird, in der Codepage 65001 (UTF-8)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-730">Fix for no output text being displayed in codepage 65001 (utf8)</span></span>
- <span data-ttu-id="d8d1c-731">Übertragen Sie RGB-Werte auf andere Teile der Palette für die Änderung der Auswahl einer Farbe vorgenommenen Änderungen werden nicht werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-731">Do not transfer changes made to one color's RGB values to other parts of the palette on selection change.</span></span> <span data-ttu-id="d8d1c-732">Dadurch wird die Eigenschaftenseite für die Konsole ein viel einfacher zu bedienen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-732">This will make the console properties sheet a lot easier to use.</span></span>
- <span data-ttu-id="d8d1c-733">STRG + S nicht angezeigt werden, ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-733">Ctrl+S doesn't appear to work correctly</span></span>
- <span data-ttu-id="d8d1c-734">Nicht fett /-Dim vollständig fehlende aus ANSI-Escapesequenzen [GH 2174]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-734">Un-Bold/-Dim completely absent from ANSI escape codes [GH 2174]</span></span>
- <span data-ttu-id="d8d1c-735">Konsole unterstützt nicht ordnungsgemäß Vim-Farbdesigns [GH 1706].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-735">Console doesn't correctly support Vim color themes [GH 1706]</span></span>
- <span data-ttu-id="d8d1c-736">Bestimmte Zeichen [GH 2149] kann nicht eingefügt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-736">Cannot paste particular characters [GH 2149]</span></span>
- <span data-ttu-id="d8d1c-737">Ändern der Größe geänderte flussrichtung interagiert seltsam Ändern der Größe einer Bash-Fenster, wenn alles in der Bearbeiten/Befehlszeile [GH ConEmu 1123] verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d8d1c-737">Reflow resize interacts strangely with resizing a bash window when stuff is on the edit/command line [GH ConEmu 1123]</span></span>
- <span data-ttu-id="d8d1c-738">STRG + L, verlässt den modifizierte Bildschirm [GH 1978]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-738">Ctrl-L leaves the screen dirty [GH 1978]</span></span>
- <span data-ttu-id="d8d1c-739">Konsole Rendering-Fehler beim Anzeigen von VT auf HDPI [GH 1907]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-739">Console rendering bug when displaying VT on HDPI [GH 1907]</span></span>
- <span data-ttu-id="d8d1c-740">Japanischen Zeichen seltsam mit Unicode-Zeichen U + 30FB [GH 2146]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-740">Japansese characters look strange with Unicode Character U+30FB [GH 2146]</span></span>
- <span data-ttu-id="d8d1c-741">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-741">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16237"></a><span data-ttu-id="d8d1c-742">Build 16237</span><span class="sxs-lookup"><span data-stu-id="d8d1c-742">Build 16237</span></span>

<span data-ttu-id="d8d1c-743">Allgemeine Windows Informationen zum Build 16237 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-743">For general Windows information on build 16237 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-744">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-744">Fixed</span></span>
- <span data-ttu-id="d8d1c-745">Verwenden Sie Standardattribute für Dateien ohne EAs im Lxfs ("Root", "Root", "0000")</span><span class="sxs-lookup"><span data-stu-id="d8d1c-745">Use default attributes for files without EAs in lxfs (root, root, 0000)</span></span>
- <span data-ttu-id="d8d1c-746">Unterstützung für Distributionen, die erweiterte Attribute verwenden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-746">Added support for distributions that use extended attributes</span></span>
- <span data-ttu-id="d8d1c-747">Beheben Sie Abstand für die von Getdents und getdents64 zurückgegebenen Einträge</span><span class="sxs-lookup"><span data-stu-id="d8d1c-747">Fix padding for entries returned by getdents and getdents64</span></span>
- <span data-ttu-id="d8d1c-748">Korrigieren der Überprüfung der Berechtigungen für die Shmctl SHM_STAT Systemaufruf [GH 2068]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-748">Fix permissions check for the shmctl SHM_STAT system call [GH 2068]</span></span>
- <span data-ttu-id="d8d1c-749">Status des festen falsche anfängliche Epoll für Schreibtelefone [GH 2231]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-749">Fixed incorrect initial epoll state for ttys [GH 2231]</span></span>
- <span data-ttu-id="d8d1c-750">Beheben von DrvFs Verz. zurückgeben nicht alle Einträge [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-750">Fix DrvFs readdir not returning all entries [GH 2077]</span></span>
- <span data-ttu-id="d8d1c-751">Beheben von LxFs Verz., wenn Dateien nicht verknüpfte [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-751">Fix LxFs readdir when files are unlinked [GH 2077]</span></span>
- <span data-ttu-id="d8d1c-752">Erlauben Sie aufgehoben Drvfs-Dateien, die über procfs erneut geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-752">Allow unlinked drvfs files to be reopened through procfs</span></span>
- <span data-ttu-id="d8d1c-753">Überschreiben des globalen Registrierung für das Deaktivieren der WSL Funktionen hinzugefügt (Interop / Laufwerk einbinden)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-753">Added global registry key override for disabling WSL features (interop / drive mounting)</span></span>
- <span data-ttu-id="d8d1c-754">Beheben Sie die Anzahl der falschen Block in "Stat" für DrvFs (und LxFs) [GH 1894]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-754">Fix incorrect block count in "stat" for DrvFs (and LxFs) [GH 1894]</span></span>
- <span data-ttu-id="d8d1c-755">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-755">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16232"></a><span data-ttu-id="d8d1c-756">Build 16232</span><span class="sxs-lookup"><span data-stu-id="d8d1c-756">Build 16232</span></span>

<span data-ttu-id="d8d1c-757">Allgemeine Windows Informationen zum Build 16232 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-757">For general Windows information on build 16232 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-758">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-758">Fixed</span></span>
- <span data-ttu-id="d8d1c-759">Keine WSL im Zusammenhang mit Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-759">No WSL related changes in this release.</span></span>

</br>

## <a name="build-16226"></a><span data-ttu-id="d8d1c-760">Build 16226</span><span class="sxs-lookup"><span data-stu-id="d8d1c-760">Build 16226</span></span>

<span data-ttu-id="d8d1c-761">Allgemeine Windows Informationen zum Build 16226 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-761">For general Windows information on build 16226 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-762">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-762">Fixed</span></span>
- <span data-ttu-id="d8d1c-763">Xattr im Zusammenhang mit Syscalls-Unterstützung (Getxattr, Setxattr, Listxattr, Removexattr).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-763">xattr related syscalls support (getxattr, setxattr, listxattr, removexattr).</span></span>
- <span data-ttu-id="d8d1c-764">Security.capablity Xattr-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-764">security.capablity xattr support.</span></span>
- <span data-ttu-id="d8d1c-765">Verbesserte Kompatibilität mit bestimmten Dateisysteme und Filter verwenden, einschließlich nicht - MS-SMB-Server.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-765">Improved compatibility with certain file systems and filters, including non-MS SMB servers.</span></span> <span data-ttu-id="d8d1c-766">[GH #1952]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-766">[GH #1952]</span></span>
- <span data-ttu-id="d8d1c-767">Verbesserte Unterstützung für OneDrive-Platzhalter, GVFS Platzhalter und Compact OS komprimierte Dateien.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-767">Improved support for OneDrive placeholders, GVFS placeholders, and Compact OS compressed files.</span></span>
- <span data-ttu-id="d8d1c-768">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-768">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16215"></a><span data-ttu-id="d8d1c-769">Build 16215</span><span class="sxs-lookup"><span data-stu-id="d8d1c-769">Build 16215</span></span>

<span data-ttu-id="d8d1c-770">Allgemeine Windows Informationen zum Build 16215 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-770">For general Windows information on build 16215 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-771">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-771">Fixed</span></span>
- <span data-ttu-id="d8d1c-772">WSL muss nicht mehr den Entwicklermodus.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-772">WSL no longer requires developer mode.</span></span>
- <span data-ttu-id="d8d1c-773">Verzeichnisverbindungen in Drvfs unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-773">Support directory junctions in drvfs.</span></span>
- <span data-ttu-id="d8d1c-774">Behandeln Sie die Deinstallation von WSL Verteilung Appx-Paketen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-774">Handle uninstalling of WSL distribution appx packages.</span></span>
- <span data-ttu-id="d8d1c-775">Update procfs anzuzeigenden private und freigegebene Zuordnungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-775">Update procfs to show private and shared mappings.</span></span>
- <span data-ttu-id="d8d1c-776">Fügen Sie die Möglichkeit wslconfig.exe zum Bereinigen von Verteilungen, die teilweise installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-776">Add ability for wslconfig.exe to clean up distributions that are partially installed or uninstalled.</span></span>
- <span data-ttu-id="d8d1c-777">Unterstützung für IP_MTU_DISCOVER für TCP-Sockets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-777">Added support for IP_MTU_DISCOVER for TCP sockets.</span></span> <span data-ttu-id="d8d1c-778">[GH 1639, 2115, 2205]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-778">[GH 1639, 2115, 2205]</span></span>
- <span data-ttu-id="d8d1c-779">Die Protokollfamilie für Routen, um AF_INADDR abgeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-779">Infer protocol family for routes to AF_INADDR.</span></span>
- <span data-ttu-id="d8d1c-780">Verbesserungen der seriellen Gerät [GH 1929].</span><span class="sxs-lookup"><span data-stu-id="d8d1c-780">Serial device improvements [GH 1929].</span></span>

</br>

## <a name="build-16199"></a><span data-ttu-id="d8d1c-781">Build 16199</span><span class="sxs-lookup"><span data-stu-id="d8d1c-781">Build 16199</span></span>

<span data-ttu-id="d8d1c-782">Allgemeine Windows Informationen zum Build 16199 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-782">For general Windows information on build 16199 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-783">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-783">Fixed</span></span>
- <span data-ttu-id="d8d1c-784">Keine WSL im Zusammenhang mit Änderungen in diesen Versionen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-784">No WSL related changes in these releases.</span></span>

</br>

## <a name="build-16193"></a><span data-ttu-id="d8d1c-785">Build 16193</span><span class="sxs-lookup"><span data-stu-id="d8d1c-785">Build 16193</span></span>

<span data-ttu-id="d8d1c-786">Allgemeine Windows Informationen zum Build 16193 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-786">For general Windows information on build 16193 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-787">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-787">Fixed</span></span>
- <span data-ttu-id="d8d1c-788">Racebedingung zwischen dem Senden der SIGCONT und eine Threadgroup beendet [GH 1973]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-788">Race condition between sending SIGCONT and a threadgroup terminating [GH 1973]</span></span>
- <span data-ttu-id="d8d1c-789">Ändern Sie die tty und Pty-Geräte in Bericht FILE_DEVICE_NAMED_PIPE statt FILE_DEVICE_CONSOLE [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-789">change tty and pty devices to report FILE_DEVICE_NAMED_PIPE instead of FILE_DEVICE_CONSOLE [GH 1840]</span></span>
- <span data-ttu-id="d8d1c-790">Beheben von SSH für IP_OPTIONS</span><span class="sxs-lookup"><span data-stu-id="d8d1c-790">SSH fix for IP_OPTIONS</span></span>
- <span data-ttu-id="d8d1c-791">Init-Daemon DrvFs Einbindung verschoben [GH 1862, 1968, 1767, 1933]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-791">Moved DrvFs mounting to init daemon [GH 1862, 1968, 1767, 1933]</span></span>
- <span data-ttu-id="d8d1c-792">Unterstützung in DrvFs für die folgenden NT symbolische Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-792">Added support in DrvFs for following NT symlinks.</span></span>

</br>

## <a name="build-16184"></a><span data-ttu-id="d8d1c-793">Build 16184</span><span class="sxs-lookup"><span data-stu-id="d8d1c-793">Build 16184</span></span>

<span data-ttu-id="d8d1c-794">Allgemeine Windows Informationen zum Build 16184 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-794">For general Windows information on build 16184 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-795">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-795">Fixed</span></span>
- <span data-ttu-id="d8d1c-796">Entfernt die Wartungstask "apt-Paket" (lxrun.exe/Update)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-796">Removed apt package maintenance task (lxrun.exe /update)</span></span>
- <span data-ttu-id="d8d1c-797">Ausgabe des festen nicht auftauchen von Windows-Prozessen in node.js [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-797">Fixed output not showing up in from Windows processes in node.js [GH 1840]</span></span>
- <span data-ttu-id="d8d1c-798">Lockern Sie ausrichtungsanforderungen in Lxcore [GH 1794]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-798">Relax alignment requirements in lxcore [GH 1794]</span></span>
- <span data-ttu-id="d8d1c-799">Korrektur der Verarbeitung des AT_EMPTY_PATH Flags in eine Anzahl von Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-799">Fixed handling of the AT_EMPTY_PATH flag in a numer of system calls.</span></span>
- <span data-ttu-id="d8d1c-800">Problem behoben, bei dem Datei, die nicht definierten Verhalten [GH 544,966,1357,1535,1615] verursacht wird DrvFs-Dateien mit offenen Handles zu löschen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-800">Fixed issue where deleting DrvFs files with open handles will cause the file to exhibit undefined behavior [GH 544,966,1357,1535,1615]</span></span>
- <span data-ttu-id="d8d1c-801">/ Etc/Hosts übernimmt jetzt Einträge aus der Windows-Hosts-Datei (% windir%\system32\drivers\etc\hosts) [GH 1495]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-801">/etc/hosts will now inherit entries from the Windows hosts file (%windir%\system32\drivers\etc\hosts) [GH 1495]</span></span>

</br>

## <a name="build-16179"></a><span data-ttu-id="d8d1c-802">Build 16179</span><span class="sxs-lookup"><span data-stu-id="d8d1c-802">Build 16179</span></span>

<span data-ttu-id="d8d1c-803">Allgemeine Windows Informationen zum Build 16179 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-803">For general Windows information on build 16179 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-804">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-804">Fixed</span></span>
- <span data-ttu-id="d8d1c-805">Keine Änderungen der WSL diese Woche.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-805">No WSL changes this week.</span></span>

</br>

## <a name="build-16176"></a><span data-ttu-id="d8d1c-806">Build 16176</span><span class="sxs-lookup"><span data-stu-id="d8d1c-806">Build 16176</span></span>

<span data-ttu-id="d8d1c-807">Allgemeine Windows Informationen zum Build 16176 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-807">For general Windows information on build 16176 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-808">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-808">Fixed</span></span>

- [<span data-ttu-id="d8d1c-809">Serielle Unterstützung aktiviert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-809">Enabled serial support</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- <span data-ttu-id="d8d1c-810">Zusätzliche IP-Socket-Option IP_OPTIONS [GH 1116]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-810">Added IP socket option IP_OPTIONS [GH 1116]</span></span>
- <span data-ttu-id="d8d1c-811">Pwritev-Funktion (während eine Datei hochladen, um Nginx/PHP-FPM) implementiert [GH 1506]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-811">Implemented pwritev function (while uploading file to nginx/PHP-FPM) [GH 1506]</span></span>
- <span data-ttu-id="d8d1c-812">Hinzugefügt von IP-Socket-Optionen IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-812">Added IP socket options IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span></span>
- <span data-ttu-id="d8d1c-813">Unterstützung für Socketoption IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-813">Support for socket option IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span></span>
- <span data-ttu-id="d8d1c-814">Hinzugefügte IP-(IPv6) _MTU Socketoption auf den Knoten "apps", "Traceroute", "informieren Sie sich", "Nslookup", "host</span><span class="sxs-lookup"><span data-stu-id="d8d1c-814">Added IP(V6)_MTU socket option for apps node, traceroute, dig, nslookup, host</span></span>
- <span data-ttu-id="d8d1c-815">Zusätzliche IP-Socket-Option IPV6_UNICAST_HOPS</span><span class="sxs-lookup"><span data-stu-id="d8d1c-815">Added IP socket option IPV6_UNICAST_HOPS</span></span>
- [<span data-ttu-id="d8d1c-816">Dateisystem-Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-816">Filesystem Improvements</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * <span data-ttu-id="d8d1c-817">Bereitstellen von UNC-Pfade zulassen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-817">Allow mounting of UNC paths</span></span>
    * <span data-ttu-id="d8d1c-818">CDFS-Unterstützung in Drvfs aktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-818">Enable CDFS support in drvfs</span></span>
    * <span data-ttu-id="d8d1c-819">Verarbeiten Sie Berechtigungen für die Netzwerk-Dateisysteme auf Drvfs ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="d8d1c-819">Correctly handle permissions for network file systems in drvfs</span></span>
    * <span data-ttu-id="d8d1c-820">Hinzufügen von Unterstützung für die remote-Laufwerke zu drvfs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-820">Add support for remote drives to drvfs</span></span>
    * <span data-ttu-id="d8d1c-821">Aktivieren von FAT-Unterstützung in Drvfs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-821">Enable FAT support in drvfs</span></span>
- <span data-ttu-id="d8d1c-822">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-822">Additional fixes and Improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-823">LTP Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="d8d1c-823">LTP Results</span></span>
<span data-ttu-id="d8d1c-824">Keine Änderungen seit der 15042</span><span class="sxs-lookup"><span data-stu-id="d8d1c-824">No changes since 15042</span></span>

</br>

## <a name="build-16170"></a><span data-ttu-id="d8d1c-825">Build 16170</span><span class="sxs-lookup"><span data-stu-id="d8d1c-825">Build 16170</span></span>

<span data-ttu-id="d8d1c-826">Allgemeine Windows Informationen zum Build 16170 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-826">For general Windows information on build 16170 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span></span><br/>

<span data-ttu-id="d8d1c-827">Veröffentlicht eine neue [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) erläutern unsere bemühungen um WSL zu testen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-827">We released a new [blog post](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) discussing our efforts to test WSL.</span></span>

### <a name="fixed"></a><span data-ttu-id="d8d1c-828">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-828">Fixed</span></span>

- <span data-ttu-id="d8d1c-829">Unterstützung für Socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-829">Support socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span></span>
- <span data-ttu-id="d8d1c-830">Hinzufügen von Unterstützung für PTRACE_OLDSETOPTIONS.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-830">Add support for PTRACE_OLDSETOPTIONS.</span></span> <span data-ttu-id="d8d1c-831">[GH 1692]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-831">[GH 1692]</span></span>
- <span data-ttu-id="d8d1c-832">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-832">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-833">LTP Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="d8d1c-833">LTP Results</span></span>
<span data-ttu-id="d8d1c-834">Keine Änderungen seit der 15042</span><span class="sxs-lookup"><span data-stu-id="d8d1c-834">No changes since 15042</span></span>

</br>

## <a name="build-15046-to-windows-10-creators-update"></a><span data-ttu-id="d8d1c-835">Erstellen 15046 zu Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="d8d1c-835">Build 15046 to Windows 10 Creators Update</span></span>
<span data-ttu-id="d8d1c-836">Es sind keine weiteren WSL Korrekturen oder Funktionen an, für die Aufnahme in die auf Windows 10 Creators Update.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-836">There are no more WSL fixes or features planned for inclusion in the Creators Update to Windows 10.</span></span> <span data-ttu-id="d8d1c-837">Anmerkungen zu dieser Version für WSL werden fortgesetzt, in den kommenden Wochen für Ergänzungen, die für das nächste größere Update für Windows.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-837">Release notes for WSL will resume in the coming weeks for additions targeting the next major Windows Update.</span></span> <span data-ttu-id="d8d1c-838">Für allgemeine Windows Informationen zu Builds 15046 und zukünftige Insider-Versionen finden Sie unter den [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-838">For general Windows information on build 15046 and future Insider releases visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span></span> <br/><br/>
 <br/>

## <a name="build-15042"></a><span data-ttu-id="d8d1c-839">Build 15042</span><span class="sxs-lookup"><span data-stu-id="d8d1c-839">Build 15042</span></span>

<span data-ttu-id="d8d1c-840">Allgemeine Windows Informationen zum Build 15042 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-840">For general Windows information on build 15042 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-841">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-841">Fixed</span></span>

- <span data-ttu-id="d8d1c-842">Für einen Deadlock zu beheben, entfernen Sie einen Pfad auf "..."</span><span class="sxs-lookup"><span data-stu-id="d8d1c-842">Fix for a deadlock when removing a path ending in ".."</span></span>
- <span data-ttu-id="d8d1c-843">Ein Problem wurde behoben, in denen FIONBIO keine 0 bei Erfolg [GH 1683] zurückgibt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-843">Fixed an issue where FIONBIO not returning 0 on success [GH 1683]</span></span>
- <span data-ttu-id="d8d1c-844">Korrigiert: Probleme mit der Zeichenfolge der Länge Null Lesevorgänge Inet Datagrammsockets</span><span class="sxs-lookup"><span data-stu-id="d8d1c-844">Fixed issue with zero-length reads of inet datagram sockets</span></span>
- <span data-ttu-id="d8d1c-845">Beheben Sie mögliches Deadlock aufgrund eines Race-Bedingung in Drvfs Inode Lookup [GH 1675]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-845">Fix possible deadlock due to race condition in drvfs inode lookup [GH 1675]</span></span>
- <span data-ttu-id="d8d1c-846">Erweiterte Unterstützung für Unix-Socket-Zusatzdaten; SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613 1326]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-846">Extended support for unix socket ancillary data; SCM_CREDENTIALS and SCM_RIGHTS [GH 514, 613, 1326]</span></span>
- <span data-ttu-id="d8d1c-847">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-847">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-848">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-848">LTP Results:</span></span>
<span data-ttu-id="d8d1c-849">Anzahl der bestandenen Test: 737</span><span class="sxs-lookup"><span data-stu-id="d8d1c-849">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="d8d1c-850">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255</span><span class="sxs-lookup"><span data-stu-id="d8d1c-850">Number of non-Passing (failing, skipped, etc…): 255</span></span>

</br>

## <a name="build-15031"></a><span data-ttu-id="d8d1c-851">Build 15031</span><span class="sxs-lookup"><span data-stu-id="d8d1c-851">Build 15031</span></span>

<span data-ttu-id="d8d1c-852">Allgemeine Windows Informationen zum Build 15031 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-852">For general Windows information on build 15031 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-853">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-853">Fixed</span></span>

- <span data-ttu-id="d8d1c-854">Korrektur eines Fehlers, in denen time(2) sporadisch problemereignis würde.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-854">Fixed a bug where time(2) would sporadically misbehave.</span></span>
- <span data-ttu-id="d8d1c-855">Behoben, und geben Sie die Where \* SIGPROCMASK Syscalls Signal-Maske kann beschädigt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-855">Fixed and issue where \*SIGPROCMASK syscalls could corrupt signal mask.</span></span>
- <span data-ttu-id="d8d1c-856">Nun gibt die vollständige Befehlszeilenlänge in WSL Benachrichtigung über Erstellung des Prozesses zurück.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-856">Now return full command line length in WSL process creation notification.</span></span> <span data-ttu-id="d8d1c-857">[GH 1632]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-857">[GH 1632]</span></span>
- <span data-ttu-id="d8d1c-858">WSL meldet jetzt Threadbeendigung über Ptrace für GDB Hängenbleiben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-858">WSL now reports thread exit through ptrace for GDB hangs.</span></span> <span data-ttu-id="d8d1c-859">[GH 1196]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-859">[GH 1196]</span></span>
- <span data-ttu-id="d8d1c-860">Korrektur von Bug, in denen Ptys nach hohe Tmux e/a hängen bleiben würde.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-860">Fixed bug where ptys would hang after heavy tmux IO.</span></span> <span data-ttu-id="d8d1c-861">[GH 1358]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-861">[GH 1358]</span></span>
- <span data-ttu-id="d8d1c-862">Feste Timeout-Validierung in viele Systemaufrufe (Futex, Semtimedop, Ppoll, Sigtimedwait, "itimer", Timer_create)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-862">Fixed timeout validation in many system calls (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span></span>
- <span data-ttu-id="d8d1c-863">Hinzugefügte Eventfd EFD_SEMAPHORE Unterstützung [GH 452]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-863">Added eventfd EFD_SEMAPHORE support [GH 452]</span></span>
- <span data-ttu-id="d8d1c-864">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-864">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-865">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-865">LTP Results:</span></span>
<span data-ttu-id="d8d1c-866">Anzahl der bestandenen Test: 737</span><span class="sxs-lookup"><span data-stu-id="d8d1c-866">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="d8d1c-867">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255</span><span class="sxs-lookup"><span data-stu-id="d8d1c-867">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="d8d1c-868">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-868">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a><span data-ttu-id="d8d1c-869">Build 15025</span><span class="sxs-lookup"><span data-stu-id="d8d1c-869">Build 15025</span></span>

<span data-ttu-id="d8d1c-870">Allgemeine Windows Informationen zum Build 15025 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-870">For general Windows information on build 15025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-871">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-871">Fixed</span></span>

- <span data-ttu-id="d8d1c-872">Korrektur für Fehler, kaputt Grep 2,27 [GH 1578]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-872">Fix for bug that broke grep 2.27 [GH 1578]</span></span>
- <span data-ttu-id="d8d1c-873">Implementierten EFD_SEMAPHORE-Flag für eventfd2 Syscall [GH 452]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-873">Implemented EFD_SEMAPHORE flag for eventfd2 syscall [GH 452]</span></span>
- <span data-ttu-id="d8d1c-874">Implementiert die /proc/ [ProzessID] / Net/ipv6_route [GH 1608]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-874">Implemented /proc/[pid]/net/ipv6_route [GH 1608]</span></span>
- <span data-ttu-id="d8d1c-875">Signal-driven e/a-Unterstützung für Unix-Streamsockets [GH 393, 68]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-875">Signal driven IO support for unix stream sockets [GH 393, 68]</span></span>
- <span data-ttu-id="d8d1c-876">Unterstützen Sie F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-876">Support F_GETPIPE_SZ and F_SETPIPE_SZ [GH 1012]</span></span>
- <span data-ttu-id="d8d1c-877">Implementieren von recvmmsg() Syscall [GH 1531]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-877">Implement recvmmsg() syscall [GH 1531]</span></span>
- <span data-ttu-id="d8d1c-878">Korrektur von Bug, in denen epoll_wait() [GH 1609] wartet, wurde nicht</span><span class="sxs-lookup"><span data-stu-id="d8d1c-878">Fixed bug where epoll_wait() wasn't waiting [GH 1609]</span></span>
- <span data-ttu-id="d8d1c-879">Implementieren von /proc/version_signature</span><span class="sxs-lookup"><span data-stu-id="d8d1c-879">Implement /proc/version_signature</span></span>
- <span data-ttu-id="d8d1c-880">Tee Syscall gibt jetzt Fehler, wenn beide Dateideskriptoren auf dieselbe Leitung verweisen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-880">Tee syscall now returns failure if both file descriptors refer to the same pipe</span></span>
- <span data-ttu-id="d8d1c-881">Richtige implementierte Verhalten für SO_PEERCRED für Unix-sockets</span><span class="sxs-lookup"><span data-stu-id="d8d1c-881">Implemented correct behavior for SO_PEERCRED for Unix sockets</span></span>
- <span data-ttu-id="d8d1c-882">Behandlung von festen Tkill Syscall ungültige parameter</span><span class="sxs-lookup"><span data-stu-id="d8d1c-882">Fixed tkill syscall invalid parameter handling</span></span>
- <span data-ttu-id="d8d1c-883">Änderungen an der Preformace von Drvfs erhöhen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-883">Changes to increase the preformace of drvfs</span></span>
- <span data-ttu-id="d8d1c-884">Kleinere Fehlerbehebung für Ruby e/a-Blockierung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-884">Minor fix for Ruby IO blocking</span></span>
- <span data-ttu-id="d8d1c-885">Feste recvmsg() EINVAL zurückgeben, für das Flag MSG_DONTWAIT für Inet-Sockets [GH 1296]</span><span class="sxs-lookup"><span data-stu-id="d8d1c-885">Fixed recvmsg() returning EINVAL for the MSG_DONTWAIT flag for inet sockets [GH 1296]</span></span>
- <span data-ttu-id="d8d1c-886">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-886">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-887">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-887">LTP Results:</span></span>
<span data-ttu-id="d8d1c-888">Anzahl der bestandenen Test: 732</span><span class="sxs-lookup"><span data-stu-id="d8d1c-888">Number of Passing Test: 732</span></span></br>
<span data-ttu-id="d8d1c-889">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255</span><span class="sxs-lookup"><span data-stu-id="d8d1c-889">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="d8d1c-890">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-890">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a><span data-ttu-id="d8d1c-891">Build 15019</span><span class="sxs-lookup"><span data-stu-id="d8d1c-891">Build 15019</span></span>

<span data-ttu-id="d8d1c-892">Allgemeine Windows Informationen zum Build 15019 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-892">For general Windows information on build 15019 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-893">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-893">Fixed</span></span>

- <span data-ttu-id="d8d1c-894">Der Fehler behoben, die falsch, CPU-Auslastung in gemeldet procfs für Tools wie Htop (GH 823, 945, 971)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-894">Fixed bug that incorrectly reported CPU usage in procfs for tools like htop (GH 823, 945, 971)</span></span>
- <span data-ttu-id="d8d1c-895">Beim Aufrufen von open() mit O_TRUNC auf einem vorhandenen generiert Datei Inotify jetzt IN_MODIFY vor IN_OPEN</span><span class="sxs-lookup"><span data-stu-id="d8d1c-895">When calling open() with O_TRUNC on an existing file inotify now generates IN_MODIFY before IN_OPEN</span></span>
- <span data-ttu-id="d8d1c-896">Fehlerbehebungen für Unix-Socket-Getsockopt SO_ERROR Postgress [GH-61, 1354] aktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-896">Fixes to unix socket getsockopt SO_ERROR to enable postgress [GH 61, 1354]</span></span>
- <span data-ttu-id="d8d1c-897">Implementieren von /proc/sys/net/core/somaxconn für die GO-Sprache</span><span class="sxs-lookup"><span data-stu-id="d8d1c-897">Implement /proc/sys/net/core/somaxconn for the GO language</span></span>
- <span data-ttu-id="d8d1c-898">Update-Hintergrundaufgabe Apt-Get-Paket wird nun ausgeführt ausgeblendeten aus der Ansicht</span><span class="sxs-lookup"><span data-stu-id="d8d1c-898">Apt-get package update background task now runs hidden from view</span></span>
- <span data-ttu-id="d8d1c-899">Klare Bereich für ipv6 "localhost" (Spring-Framework(Java) Fehler).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-899">Clear scope for ipv6 localhost (Spring-Framework(Java) failure).</span></span>
- <span data-ttu-id="d8d1c-900">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-900">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-901">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-901">LTP Results:</span></span>
<span data-ttu-id="d8d1c-902">Anzahl der bestandenen Test: 714</span><span class="sxs-lookup"><span data-stu-id="d8d1c-902">Number of Passing Test: 714</span></span> </br>
<span data-ttu-id="d8d1c-903">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 249</span><span class="sxs-lookup"><span data-stu-id="d8d1c-903">Number of non-Passing (failing, skipped, etc…): 249</span></span> </br>
[<span data-ttu-id="d8d1c-904">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-904">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a><span data-ttu-id="d8d1c-905">Build 15014</span><span class="sxs-lookup"><span data-stu-id="d8d1c-905">Build 15014</span></span>

<span data-ttu-id="d8d1c-906">Allgemeine Windows Informationen zum Build 15014 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-906">For general Windows information on build 15014 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-907">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-907">Fixed</span></span>

- <span data-ttu-id="d8d1c-908">STRG + C jetzt funktioniert wie vorgesehen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-908">Ctrl+C now works as intended</span></span>
- <span data-ttu-id="d8d1c-909">einfach und Ps Auxw jetzt richtig ressourcennutzung (GH #516)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-909">htop and ps auxw now show correct resource utilization (GH #516)</span></span>
- <span data-ttu-id="d8d1c-910">Einfache Übersetzung der NT-Ausnahmen auf Signale.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-910">Basic translation of NT exceptions to signals.</span></span> <span data-ttu-id="d8d1c-911">(GH #513)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-911">(GH #513)</span></span>
- <span data-ttu-id="d8d1c-912">Fallocate schlägt jetzt mit ENOSPC fehl, wenn nur noch wenig Speicherplatz statt EINVAL (GH #1571)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-912">fallocate now fails with ENOSPC  when running out of space instead of EINVAL (GH #1571)</span></span>
- <span data-ttu-id="d8d1c-913">Hinzugefügte /proc/sys/kernel/sem.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-913">Added /proc/sys/kernel/sem.</span></span>
- <span data-ttu-id="d8d1c-914">Implementierten Semop und Semtimedop Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="d8d1c-914">Implemented semop and semtimedop system calls</span></span>
- <span data-ttu-id="d8d1c-915">Feste Nslookup-Fehler mit IP_RECVTOS & IPV6_RECVTCLASS-Socketoption (GH 69)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-915">Fixed nslookup errors with IP_RECVTOS & IPV6_RECVTCLASS socket option (GH 69)</span></span>
- <span data-ttu-id="d8d1c-916">Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT</span><span class="sxs-lookup"><span data-stu-id="d8d1c-916">Support for socket options IP_RECVTTL and IPV6_RECVHOPLIMIT</span></span>
- <span data-ttu-id="d8d1c-917">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-917">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-918">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-918">LTP Results:</span></span>
<span data-ttu-id="d8d1c-919">Anzahl der bestandenen Test: 709</span><span class="sxs-lookup"><span data-stu-id="d8d1c-919">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="d8d1c-920">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255</span><span class="sxs-lookup"><span data-stu-id="d8d1c-920">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="d8d1c-921">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-921">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a><span data-ttu-id="d8d1c-922">Syscall-Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-922">Syscall Summary</span></span>
<span data-ttu-id="d8d1c-923">Insgesamt Syscalls: 384</span><span class="sxs-lookup"><span data-stu-id="d8d1c-923">Total Syscalls: 384</span></span> </br>
<span data-ttu-id="d8d1c-924">Die gesamte Implementierung: 235</span><span class="sxs-lookup"><span data-stu-id="d8d1c-924">Total Implemented: 235</span></span> </br>
<span data-ttu-id="d8d1c-925">Insgesamt, die ein Stub ausgeführt werden: 22</span><span class="sxs-lookup"><span data-stu-id="d8d1c-925">Total Stubbed: 22</span></span> </br>
<span data-ttu-id="d8d1c-926">Insgesamt, nicht implementiert: 127</span><span class="sxs-lookup"><span data-stu-id="d8d1c-926">Total Unimplemented: 127</span></span> </br>
[<span data-ttu-id="d8d1c-927">Detaillierte Aufschlüsselung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-927">Detailed Breakdown</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a><span data-ttu-id="d8d1c-928">Build 15007</span><span class="sxs-lookup"><span data-stu-id="d8d1c-928">Build 15007</span></span>

<span data-ttu-id="d8d1c-929">Allgemeine Windows Informationen zum Build 15007 finden Sie auf die [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-929">For general Windows information on build 15007 visit the [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="d8d1c-930">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="d8d1c-930">Known Issue</span></span>

- <span data-ttu-id="d8d1c-931">Es ist ein bekanntes Problem, das die Konsole, in denen keine einige STRG erkennt + <key> Eingabe.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-931">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="d8d1c-932">Dies schließt den Strg-c-Befehl die als eine normale "C" Keypress fungiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-932">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="d8d1c-933">Problemumgehung: Ordnen Sie einen alternativen Schlüssel STRG + C.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-933">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="d8d1c-934">Zuordnen beispielsweise STRG + K, STRG + C ausführen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-934">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="d8d1c-935">Diese Zuordnung erfolgt pro Terminal, und müssen erfolgen *jeder* Zeit Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-935">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="d8d1c-936">Benutzer können die Option zum Einschließen in untersuchen ihre</span><span class="sxs-lookup"><span data-stu-id="d8d1c-936">Users can explore the option to include this in their</span></span> `.bashrc`

### <a name="fixed"></a><span data-ttu-id="d8d1c-937">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-937">Fixed</span></span>

- <span data-ttu-id="d8d1c-938">Das Problem, in denen WSL mit 100 % der CPU-Kern beansprucht, korrigiert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-938">Corrected the issue where running WSL would consume 100% of a CPU core</span></span>
- <span data-ttu-id="d8d1c-939">Socketoption IP_PKTINFO, IPV6_RECVPKTINFO jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-939">Socket option IP_PKTINFO, IPV6_RECVPKTINFO now supported.</span></span> <span data-ttu-id="d8d1c-940">(GH #851, 987)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-940">(GH #851, 987)</span></span>
- <span data-ttu-id="d8d1c-941">Physische Adresse für die Netzwerkschnittstelle von 16 Bytes Lxcore Truncate (GH #1452, 1414, 1343, 468, 308)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-941">Truncate network interface physical address to 16 bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span></span>
- <span data-ttu-id="d8d1c-942">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-942">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-943">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-943">LTP Results:</span></span>
<span data-ttu-id="d8d1c-944">Anzahl der bestandenen Test: 709</span><span class="sxs-lookup"><span data-stu-id="d8d1c-944">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="d8d1c-945">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 255</span><span class="sxs-lookup"><span data-stu-id="d8d1c-945">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="d8d1c-946">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-946">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a><span data-ttu-id="d8d1c-947">Build 15002</span><span class="sxs-lookup"><span data-stu-id="d8d1c-947">Build 15002</span></span>

<span data-ttu-id="d8d1c-948">Allgemeine Windows Build 15002 Informationen finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-948">For general Windows information on build 15002 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="d8d1c-949">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="d8d1c-949">Known Issue</span></span>

<span data-ttu-id="d8d1c-950">Zwei bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-950">Two known issues:</span></span>
- <span data-ttu-id="d8d1c-951">Es ist ein bekanntes Problem, das die Konsole, in denen keine einige STRG erkennt + <key> Eingabe.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-951">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="d8d1c-952">Dies schließt den Strg-c-Befehl die als eine normale "C" Keypress fungiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-952">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="d8d1c-953">Problemumgehung: Ordnen Sie einen alternativen Schlüssel STRG + C.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-953">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="d8d1c-954">Zuordnen beispielsweise STRG + K, STRG + C ausführen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-954">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="d8d1c-955">Diese Zuordnung erfolgt pro Terminal, und müssen erfolgen *jeder* Zeit Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-955">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="d8d1c-956">Benutzer können die Option zum Einschließen in untersuchen ihre</span><span class="sxs-lookup"><span data-stu-id="d8d1c-956">Users can explore the option to include this in their</span></span> `.bashrc`

- <span data-ttu-id="d8d1c-957">Während der Ausführung WSL verbraucht Systemthread 100 % der CPU-Kern.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-957">While WSL is running a system thread will consume 100% of a CPU core.</span></span>  <span data-ttu-id="d8d1c-958">Die zugrunde liegende Ursache wurde behoben und intern behoben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-958">The root cause has been addressed and fixed internally.</span></span>

### <a name="fixed"></a><span data-ttu-id="d8d1c-959">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-959">Fixed</span></span>

- <span data-ttu-id="d8d1c-960">Alle Bash-Sitzungen müssen jetzt auf der gleichen Berechtigungsstufe erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-960">All bash sessions must now be created at the same permission level.</span></span>  <span data-ttu-id="d8d1c-961">Es wird versucht, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-961">Attempting to start a session at a different level will be blocked.</span></span>  <span data-ttu-id="d8d1c-962">Dies bedeutet, dass der Administrator als auch nicht-Administrator-Konsole zur gleichen Zeit ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-962">This means admin and non-admin consoles cannot run at the same time.</span></span> <span data-ttu-id="d8d1c-963">(GH #626)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-963">(GH #626)</span></span>
<br/>
- <span data-ttu-id="d8d1c-964">Implementiert die folgenden NETLINK_ROUTE-Meldungen (erfordert Windows-Administrator)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-964">Implemented the following NETLINK_ROUTE messages (requires Windows admin)</span></span>
     - <span data-ttu-id="d8d1c-965">RTM_NEWADDR (unterstützt `ip addr add`)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-965">RTM_NEWADDR (supports `ip addr add`)</span></span>
     - <span data-ttu-id="d8d1c-966">RTM_NEWROUTE (unterstützt `ip route add`)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-966">RTM_NEWROUTE (supports `ip route add`)</span></span>
     - <span data-ttu-id="d8d1c-967">RTM_DELADDR (unterstützt `ip addr del`)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-967">RTM_DELADDR (supports `ip addr del`)</span></span>
     - <span data-ttu-id="d8d1c-968">RTM_DELROUTE (unterstützt `ip route del`)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-968">RTM_DELROUTE (supports `ip route del`)</span></span>
- <span data-ttu-id="d8d1c-969">Geplante Aufgabe überprüfen zum Aktualisieren von Paketen werden einer getakteten Verbindung (GH #1371) nicht mehr ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-969">Scheduled task checking for packages to update will no longer run on a metered connection (GH #1371)</span></span>
- <span data-ttu-id="d8d1c-970">Fehler behoben wird, in denen hängen Pipeline ruft z. B. Bash - C "ls - AlR /" | bash -c "Cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-970">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="d8d1c-971">Implementierten TCP_KEEPCNT-Socketoption (GH #843)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-971">Implemented TCP_KEEPCNT socket option (GH #843)</span></span>
- <span data-ttu-id="d8d1c-972">Implementierten IP_MTU_DISCOVER INET-Socketoption (720 des GH #, 717, 170, 69)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-972">Implemented IP_MTU_DISCOVER INET socket option (GH #720, 717, 170, 69)</span></span>
- <span data-ttu-id="d8d1c-973">Entfernt die alte Funktion für die NT-Binärdateien von Init mit NT-Pfad-Suche ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-973">Removed legacy functionality to run NT binaries from init with NT path lookup.</span></span> <span data-ttu-id="d8d1c-974">(GH #1325)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-974">(GH #1325)</span></span>
- <span data-ttu-id="d8d1c-975">Modus der Kmsg/Dev/Gruppe / andere Lesezugriff (0644) (GH #1321) zu beheben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-975">Fix mode of /dev/kmsg to allow group / other read access (0644) (GH #1321)</span></span>
- <span data-ttu-id="d8d1c-976">Implementierten /proc/sys/kernel/random/uuid (GH #1092)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-976">Implemented /proc/sys/kernel/random/uuid  (GH #1092)</span></span>
- <span data-ttu-id="d8d1c-977">Fehler, in denen Startzeit des Prozesses als Jahr 2432 (GH #974) angezeigt wurden, behoben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-977">Corrected error where process start time was showing as year 2432 (GH #974)</span></span>
- <span data-ttu-id="d8d1c-978">Switched standardmäßige Begriff-Umgebungsvariable auf Xterm-256color (GH #1446)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-978">Switched default TERM environment variable to xterm-256color (GH #1446)</span></span>
- <span data-ttu-id="d8d1c-979">Die Möglichkeit, die Commits verarbeiten wird berechnet, während der Prozess Fork geändert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-979">Modified the way that process commit is calculated during process fork.</span></span> <span data-ttu-id="d8d1c-980">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-980">(GH #1286)</span></span>
- <span data-ttu-id="d8d1c-981">Implementierten /proc/sys/vm/overcommit_memory.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-981">Implemented /proc/sys/vm/overcommit_memory.</span></span> <span data-ttu-id="d8d1c-982">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-982">(GH #1286)</span></span>
- <span data-ttu-id="d8d1c-983">Implementierten /proc/net/route-Datei (GH #69)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-983">Implemented /proc/net/route file (GH #69)</span></span>
- <span data-ttu-id="d8d1c-984">Fehler wurde behoben, bei denen Verknüpfungsnamen falsch war, lokalisiert (GH #696)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-984">Fixed error where shortcut name was incorrectly localized (GH #696)</span></span>
- <span data-ttu-id="d8d1c-985">Feste Elf Analyselogik, die nicht ordnungsgemäß die Programm-Header überprüft muss kleiner als (oder gleich) PATH_MAX.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-985">Fixed elf parsing logic that is incorrectly validating the program headers must be less than (or equal to) PATH_MAX.</span></span> <span data-ttu-id="d8d1c-986">(GH #1048)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-986">(GH #1048)</span></span>
- <span data-ttu-id="d8d1c-987">Implementierten Statfs Rückruf für die procfs Sysfs Cgroupfs und Binfmtfs (GH #1378)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-987">Implemented statfs callback for procfs, sysfs, cgroupfs, and binfmtfs (GH #1378)</span></span>
- <span data-ttu-id="d8d1c-988">Feste AptPackageIndexUpdate Windows (GH #1184, auch in GH #1193 behandelt) wird nicht das Schließen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-988">Fixed AptPackageIndexUpdate windows that won’t close (GH #1184, also discussed in GH #1193)</span></span>
- <span data-ttu-id="d8d1c-989">ASLR-Persönlichkeit ADDR_NO_RANDOMIZE-Unterstützung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-989">Added ASLR personality  ADDR_NO_RANDOMIZE support.</span></span> <span data-ttu-id="d8d1c-990">(GH #1148, 1128)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-990">(GH #1148, 1128)</span></span>
- <span data-ttu-id="d8d1c-991">Verbesserte PTRACE_GETSIGINFO, SIGSEGV, für die ordnungsgemäße Gdb stapelüberwachungen während AV (GH #875)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-991">Improved PTRACE_GETSIGINFO, SIGSEGV, for proper gdb stack traces during AV (GH #875)</span></span>
- <span data-ttu-id="d8d1c-992">Elf nicht mehr analysieren, die für Patchelf Binärdateien schlägt fehl.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-992">Elf parsing no longer fails for patchelf binaries.</span></span> <span data-ttu-id="d8d1c-993">(GH #471)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-993">(GH #471)</span></span>
- <span data-ttu-id="d8d1c-994">VPN DNS weitergegeben wird, um /etc/resolv.conf (GH #416, 1350)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-994">VPN DNS propagated to /etc/resolv.conf (GH #416, 1350)</span></span>
- <span data-ttu-id="d8d1c-995">Verbesserungen bei TCP zuverlässiger Datenübertragungen schließen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-995">Improvements to TCP close for more reliable data transfer.</span></span> <span data-ttu-id="d8d1c-996">(GH #610, 616, 1025, 1335)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-996">(GH #610, 616, 1025, 1335)</span></span>
- <span data-ttu-id="d8d1c-997">Nun kehren richtigen Fehlercode, wenn zu viele Dateien sind geöffnet (EMFILE).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-997">Now return correct error code when too many files are opened (EMFILE).</span></span> <span data-ttu-id="d8d1c-998">(GH #1126, 2090)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-998">(GH #1126, 2090)</span></span>
- <span data-ttu-id="d8d1c-999">Windows Audit Log jetzt-Berichte nennen Sie das Image im Prozess erstellen, überwachen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-999">Windows Audit log now reports the image name in process create audit.</span></span>
- <span data-ttu-id="d8d1c-1000">Beim Starten von bash.exe aus in einer Bash-Fenster nun ordnungsgemäß abgebrochen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1000">Now gracefully fail when launching bash.exe from within a bash window</span></span>
- <span data-ttu-id="d8d1c-1001">Hinzugefügte Fehlermeldung beim Interop-kann nicht auf ein Arbeitsverzeichnis unter LxFs (z. B. notepad.exe bashrc) zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1001">Added error message when interop is unable to access a working directory under LxFs (i.e. notepad.exe .bashrc)</span></span>
- <span data-ttu-id="d8d1c-1002">Problem behoben, in denen Windows-Pfad in WSL abgeschnitten wurde</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1002">Fixed issue where Windows path was truncated in WSL</span></span>
- <span data-ttu-id="d8d1c-1003">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1003">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1004">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1004">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1005">Anzahl der bestandenen Test: 690</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1005">Number of Passing Test: 690</span></span> </br>
<span data-ttu-id="d8d1c-1006">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 274</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1006">Number of non-Passing (failing, skipped, etc…): 274</span></span> </br>
[<span data-ttu-id="d8d1c-1007">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1007">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1008">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1008">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1009">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1009">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1010">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1010">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a><span data-ttu-id="d8d1c-1011">Build 14986</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1011">Build 14986</span></span>

<span data-ttu-id="d8d1c-1012">Allgemeine Windows Informationen zum Build 14986 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1012">For general Windows information on build 14986 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1013">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1013">Fixed</span></span>

- <span data-ttu-id="d8d1c-1014">Feste Stoppfehler mit Netlink und Pty IOCTLs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1014">Fixed bugchecks with Netlink and Pty IOCTLs</span></span>
- <span data-ttu-id="d8d1c-1015">Kernel-Version meldet jetzt 4.4.0-43 für Konsistenz mit Xenial</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1015">Kernel version now reports 4.4.0-43 for consistency with Xenial</span></span>
- <span data-ttu-id="d8d1c-1016">Bash.exe aufrief, bei der Eingabe an geleitet ' Nul: "(GH #1259)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1016">Bash.exe now launches when input directed to 'nul:' (GH #1259)</span></span>
- <span data-ttu-id="d8d1c-1017">Thread-IDs jetzt korrekt gemeldet in procfs (GH #967)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1017">Thread IDs now reported correctly in procfs (GH #967)</span></span>
- <span data-ttu-id="d8d1c-1018">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR-Flags, die jetzt in inotify_add_watch() (GH #1280) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1018">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR flags now supported in inotify_add_watch() (GH #1280)</span></span>
- <span data-ttu-id="d8d1c-1019">Implementieren Timer_create und verwandte Systemaufrufe.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1019">Implement timer_create and related system calls.</span></span>  <span data-ttu-id="d8d1c-1020">Dies ermöglicht die GHC-Unterstützung (GH #307)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1020">This enables GHC support (GH #307)</span></span>
- <span data-ttu-id="d8d1c-1021">Problem behoben, in dem Ping für eine Zeit von 0.000ms (GH #1296) zurückgegeben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1021">Fixed issue where ping returned a time of 0.000ms (GH #1296)</span></span>
- <span data-ttu-id="d8d1c-1022">Geben Sie richtige Fehlercode zurück, wenn zu viele Dateien geöffnet sind.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1022">Return correct error code when too many files are opened.</span></span>
- <span data-ttu-id="d8d1c-1023">Korrigiert: Problem in WSL, in denen Netlink datenanforderung Netzwerk-Schnittstelle mit EINVAL fehlschlagen würde, ist die Adresse der Schnittstelle Hardware 32-Byte (z. B. die Teredo-Schnittstelle)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1023">Fixed issue in WSL where Netlink request for network interface data would fail with EINVAL if the interface's hardware address is 32-bytes (such as the Teredo interface)</span></span>
   - <span data-ttu-id="d8d1c-1024">Beachten Sie, dass das Hilfsprogramm "Linux"Ip"einen Fehler enthält, in dem er stürzt ab, wenn WSL eine 32-Byte-Hardwareadresse meldet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1024">Note that the Linux "ip" utility contains a bug where it will crash if WSL reports a 32-byte hardware address.</span></span> <span data-ttu-id="d8d1c-1025">Dies ist ein Fehler in "Ip", nicht WSL.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1025">This is a bug in "ip", not WSL.</span></span> <span data-ttu-id="d8d1c-1026">Die "Ip" Dienstprogramm hartcodierung die Länge des Zeichenfolgenpuffers verwendet, um die Hardwareadresse zu drucken, und diesen Puffer ist zu klein für eine 32-Byte-Hardwareadresse zu drucken.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1026">The “ip” utility hard-codes the length of the string buffer used to print the hardware address, and that buffer is too small to print a 32-byte hardware address.</span></span>
- <span data-ttu-id="d8d1c-1027">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1027">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1028">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1028">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1029">Anzahl der bestandenen Test: 669</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1029">Number of Passing Test: 669</span></span> </br>
<span data-ttu-id="d8d1c-1030">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 258</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1030">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="d8d1c-1031">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1031">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1032">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1032">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1033">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1033">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1034">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1034">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a><span data-ttu-id="d8d1c-1035">Build 14971</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1035">Build 14971</span></span>

<span data-ttu-id="d8d1c-1036">Allgemeine Windows Informationen zum Build 14971 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1036">For general Windows information on build 14971 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1037">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1037">Fixed</span></span>

 - <span data-ttu-id="d8d1c-1038">Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1038">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="d8d1c-1039">Regelmäßig geplanter Updates werden auf die nächste Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1039">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1040">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1040">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1041">14965 gegenüber</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1041">Unchanged from 14965</span></span> </br>
<span data-ttu-id="d8d1c-1042">Anzahl der bestandenen Test: 664</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1042">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="d8d1c-1043">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1043">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1044">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1044">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a><span data-ttu-id="d8d1c-1045">Build 14965</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1045">Build 14965</span></span>

<span data-ttu-id="d8d1c-1046">Allgemeine Windows Informationen zum Build 14965 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1046">For general Windows information on build 14965 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1047">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1047">Fixed</span></span>

- <span data-ttu-id="d8d1c-1048">Unterstützung für Netlink sockets des Protokolls NETLINK_ROUTE RTM_GETLINK und RTM_GETADDR (GH #468)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1048">Support for Netlink sockets NETLINK_ROUTE protocol's RTM_GETLINK and RTM_GETADDR (GH #468)</span></span>
  - <span data-ttu-id="d8d1c-1049">Ermöglicht die "ifconfig" und die IP-Befehlen für die Netzwerk-enumeration</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1049">Enables ifconfig and ip commands for network enumeration</span></span>
  - <span data-ttu-id="d8d1c-1050">Weitere Informationen finden Sie unserem [Blogbeitrag WSL Networking](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1050">More information can be found in our [WSL Networking blog post](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span></span>

- <span data-ttu-id="d8d1c-1051">einen befindet sich nun im Benutzerpfad standardmäßig</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1051">/sbin is now in the user's path by default</span></span>
- <span data-ttu-id="d8d1c-1052">NT-Benutzerrollen-Datenpfad jetzt auf den Pfad WSL angehängt, in der Standardeinstellung (d. h. Sie jetzt notepad.exe eingeben, ohne "System32" auf den Linux-Pfad hinzufügen)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1052">NT user path now appended to the WSL path by default (i.e. you can now type notepad.exe without adding System32 to the Linux path)</span></span>
- <span data-ttu-id="d8d1c-1053">Unterstützung für /proc/sys/kernel/cap_last_cap</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1053">Added support for /proc/sys/kernel/cap_last_cap</span></span>
- <span data-ttu-id="d8d1c-1054">NT-Binärdateien können jetzt über WSL gestartet werden, wenn das aktuelle Arbeitsverzeichnis nicht-Ansi-Zeichen (GH #1254) enthält</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1054">NT Binaries can now be launched from WSL when the current working directory contains non-ansi characters (GH #1254)</span></span>
- <span data-ttu-id="d8d1c-1055">Ermöglichen Sie Herunterfahren auf getrennten Unix-Stream-Socket.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1055">Allow shutdown on disconnected unix stream socket.</span></span>
- <span data-ttu-id="d8d1c-1056">Unterstützung für PR_GET_PDEATHSIG hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1056">Added support for PR_GET_PDEATHSIG.</span></span>
- <span data-ttu-id="d8d1c-1057">Unterstützung für CLONE_PARENT</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1057">Added support for CLONE_PARENT</span></span>
- <span data-ttu-id="d8d1c-1058">Fehler behoben wird, in denen hängen Pipeline ruft z. B. Bash - C "ls - AlR /" | bash -c "Cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1058">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="d8d1c-1059">Verarbeitung von Abfragen für die Verbindung zum aktuellen Terminal.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1059">Handle requests to connect to the current terminal.</span></span>
- <span data-ttu-id="d8d1c-1060">Markieren Sie /proc/<pid>/oom_score_adj als schreibbar.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1060">Mark /proc/<pid>/oom_score_adj as writable.</span></span>
- <span data-ttu-id="d8d1c-1061">Fügen Sie /sys/fs/cgroup-Ordner.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1061">Add /sys/fs/cgroup folder.</span></span>
- <span data-ttu-id="d8d1c-1062">Sched_setaffinity sollte die Anzahl der Bits-Affinitätsmaske zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1062">sched_setaffinity should return number of affinity bits mask</span></span>
- <span data-ttu-id="d8d1c-1063">Beheben Sie ELF Validierungslogik für die fälschlicherweise angenommen, dass der Interpreter Pfade weniger als 64 Zeichen lang sein müssen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1063">Fix ELF validation logic which incorrectly assumes interpreter paths must be less than 64 characters long.</span></span> <span data-ttu-id="d8d1c-1064">(GH #743)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1064">(GH #743)</span></span>
- <span data-ttu-id="d8d1c-1065">Öffnen von Dateideskriptoren können Konsolenfenster geöffnet (GH #1187) beibehalten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1065">Open file descriptors can keep console window open (GH #1187)</span></span>
- <span data-ttu-id="d8d1c-1066">Fixeed Fehler, in denen Rename()"mit nachgestellten Schrägstrich Zielname (GH #1008)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1066">Fixeed error where rename() failed with trailing slash on target name (GH #1008)</span></span>
- <span data-ttu-id="d8d1c-1067">Implementieren von /proc/net/dev-Datei</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1067">Implement /proc/net/dev file</span></span>
- <span data-ttu-id="d8d1c-1068">Feste 0.000ms Pingt aufgrund der zeitgeberauflösung.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1068">Fixed 0.000ms pings due to timer resolution.</span></span>
- <span data-ttu-id="d8d1c-1069">Implementierten /proc/self/environ (GH #730)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1069">Implemented /proc/self/environ (GH #730)</span></span>
- <span data-ttu-id="d8d1c-1070">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1070">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1071">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1071">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1072">Anzahl der bestandenen Test: 664</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1072">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="d8d1c-1073">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1073">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1074">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1074">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a><span data-ttu-id="d8d1c-1075">Build 14959</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1075">Build 14959</span></span>

<span data-ttu-id="d8d1c-1076">Allgemeine Windows Informationen zum Build 14959 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1076">For general Windows information on build 14959 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1077">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1077">Fixed</span></span>

- <span data-ttu-id="d8d1c-1078">Verbesserte des Pico-Prozess-Benachrichtigung für Windows.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1078">Improved Pico Process notification for Windows.</span></span>  <span data-ttu-id="d8d1c-1079">Weitere Informationen finden Sie auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1079">Additional information found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span></span>
- <span data-ttu-id="d8d1c-1080">Verbesserte Stabilität, die mit Windows-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1080">Improved stability with Windows interoperability</span></span>
- <span data-ttu-id="d8d1c-1081">Korrigieren des Fehlers 0 x 80070057 beim bash.exe zu starten, wenn die Enterprise Data Protection (EDP) aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1081">Fixed error 0x80070057 when launching bash.exe when Enterprise Data Protection (EDP) is enabled</span></span>
- <span data-ttu-id="d8d1c-1082">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1082">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1083">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1083">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1084">Anzahl der bestandenen Test: 665</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1084">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="d8d1c-1085">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1085">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1086">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1086">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a><span data-ttu-id="d8d1c-1087">Erstellen von 14955</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1087">Build 14955</span></span>

<span data-ttu-id="d8d1c-1088">Allgemeine Windows Informationen zum Build 14955 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1088">For general Windows information on build 14955 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1089">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1089">Fixed</span></span>

 - <span data-ttu-id="d8d1c-1090">Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1090">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="d8d1c-1091">Regelmäßig geplanter Updates werden auf die nächste Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1091">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1092">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1092">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1093">Anzahl der bestandenen Test: 665</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1093">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="d8d1c-1094">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1094">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1095">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1095">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a><span data-ttu-id="d8d1c-1096">Build 14951</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1096">Build 14951</span></span>

<span data-ttu-id="d8d1c-1097">Allgemeine Windows Informationen zum Build 14951 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1097">For general Windows information on build 14951 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span></span><br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a><span data-ttu-id="d8d1c-1098">Neues Feature: Windows / Ubuntu Interoperability</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1098">New Feature: Windows / Ubuntu Interoperability</span></span>
<span data-ttu-id="d8d1c-1099">Windows-Binärdateien können jetzt direkt über die Befehlszeile WSL aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1099">Windows binaries can now be invoked directly from the WSL command line.</span></span>  <span data-ttu-id="d8d1c-1100">Dies ermöglicht Benutzern die Interaktion mit ihrer Windows-Umgebung und das System in einer Weise, die nicht möglich war.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1100">This gives users the ability to interact with their Windows environment and system in a way that has not been possible.</span></span>  <span data-ttu-id="d8d1c-1101">Als kurzes Beispiel ist es jetzt möglich, damit Benutzer die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1101">As a quick example, it is now possible for users to run the following commands:</span></span>

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

<span data-ttu-id="d8d1c-1102">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1102">More information can be found at:</span></span>

- [<span data-ttu-id="d8d1c-1103">WSL-Teamblog für Interop</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1103">WSL Team Blog for Interop</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [<span data-ttu-id="d8d1c-1104">Interop-MSDN-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1104">MSDN Interop Documentation</span></span>](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1105">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1105">Fixed</span></span>

- <span data-ttu-id="d8d1c-1106">Ubuntu 16.04 (Xenial) ist jetzt für alle neuen WSL-Instanzen installiert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1106">Ubuntu 16.04 (Xenial) is now installed for all new WSL instances.</span></span>  <span data-ttu-id="d8d1c-1107">Benutzer mit vorhandenen 14.04 (bewährte)-Instanzen werden nicht automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1107">Users with existing 14.04 (Trusty) instances will not be automatically upgraded.</span></span>
- <span data-ttu-id="d8d1c-1108">Während der Installation festgelegten Gebietsschema wird jetzt angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1108">Locale set during install is now displayed</span></span>
- <span data-ttu-id="d8d1c-1109">Der Terminalserver einschließlich Fehler, bei denen einen WSL-Prozess in eine Datei umleiten nicht immer ermöglicht, arbeiten</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1109">Terminal improvements including bug where redirecting a WSL process to a file does not always work</span></span>
- <span data-ttu-id="d8d1c-1110">Konsole Lebensdauer sollte bash.exe Lebensdauer gebunden werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1110">Console lifetime should be tied to bash.exe lifetime</span></span>
- <span data-ttu-id="d8d1c-1111">Konsolenfenster sollte sichtbar Größe, nicht die Puffergröße verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1111">Console window size should use visible size, not buffer size</span></span>
- <span data-ttu-id="d8d1c-1112">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1112">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1113">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1113">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1114">Anzahl der bestandenen Test: 665</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1114">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="d8d1c-1115">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1115">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1116">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1116">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a><span data-ttu-id="d8d1c-1117">Build 14946</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1117">Build 14946</span></span>

<span data-ttu-id="d8d1c-1118">Allgemeine Windows Informationen zum Build 14946 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1118">For general Windows information on build 14946 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1119">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1119">Fixed</span></span>

- <span data-ttu-id="d8d1c-1120">Ein Problem wurde behoben, die verhindert, Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen, die Leerzeichen oder Anführungszeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1120">Fixed an issue that prevented creating WSL user accounts for users with NT usernames that contain spaces or quotes.</span></span> 
- <span data-ttu-id="d8d1c-1121">Ändern Sie VolFs und DrvFs damit 0 für die Anzahl von des Verzeichnisses links im Stat zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1121">Change VolFs and DrvFs to return 0 for directory's link count in stat</span></span>
- <span data-ttu-id="d8d1c-1122">IPV6_MULTICAST_HOPS-Socketoption zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1122">Support IPV6_MULTICAST_HOPS socket option.</span></span>
- <span data-ttu-id="d8d1c-1123">Eine einzige Konsole e/a-Schleife pro tty begrenzt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1123">Limit to a single console I/O loop per tty.</span></span> <span data-ttu-id="d8d1c-1124">Beispiel: der folgende Befehl ist möglich:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1124">Example: the following command is possible:</span></span>
  - <span data-ttu-id="d8d1c-1125">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1125">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span></span>

- <span data-ttu-id="d8d1c-1126">Ersetzen Sie Leerzeichen mit Tabstopps in /proc/cpuinfo (GH #1115)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1126">replace spaces with tabs in /proc/cpuinfo (GH #1115)</span></span>
- <span data-ttu-id="d8d1c-1127">DrvFs wird nun in Mountinfo mit einem Namen, der bereitgestelltes Windows Volume entspricht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1127">DrvFs now appears in mountinfo with a name that matches mounted Windows volume</span></span>
- <span data-ttu-id="d8d1c-1128">/ Home erscheinen/Root nun und in Mountinfo mit den richtigen Namen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1128">/home and /root now appear in mountinfo with correct names</span></span>
- <span data-ttu-id="d8d1c-1129">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1129">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1130">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1130">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1131">Anzahl der bestandenen Test: 665</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1131">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="d8d1c-1132">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1132">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1133">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1133">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a><span data-ttu-id="d8d1c-1134">Build 14942</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1134">Build 14942</span></span>

<span data-ttu-id="d8d1c-1135">Allgemeine Windows Informationen zum Build 14942 finden Sie auf die [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1135">For general Windows information on build 14942 visit the [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1136">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1136">Fixed</span></span>

- <span data-ttu-id="d8d1c-1137">Eine Anzahl von Stoppfehler behoben, einschließlich des "versucht Ausführen von"keinausführen "Speichers" networking Absturz die SSH blockiert wurde</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1137">A number of bugchecks addressed, including the “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY” networking crash which was blocking SSH</span></span>
- <span data-ttu-id="d8d1c-1138">Unterstützung von Windows-Anwendungen auf DrvFs generierten Benachrichtigungen Inotifiy ist jetzt in</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1138">inotifiy support for notifications generated from Windows applications on DrvFs is now in</span></span>
- <span data-ttu-id="d8d1c-1139">Implementieren Sie TCP_KEEPIDLE und TCP_KEEPINTVL für "mongod" ein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1139">Implement TCP_KEEPIDLE and TCP_KEEPINTVL for mongod.</span></span> <span data-ttu-id="d8d1c-1140">(GH #695)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1140">(GH #695)</span></span>
- <span data-ttu-id="d8d1c-1141">Implementieren von Pivot_root Systemaufruf</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1141">Implement the pivot_root system call</span></span>
- <span data-ttu-id="d8d1c-1142">Implementieren der Socketoption auf den SO_DONTROUTE</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1142">Implement socket option for SO_DONTROUTE</span></span>
- <span data-ttu-id="d8d1c-1143">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1143">Additional bugfixes and improvements</span></span>


### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1144">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1144">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1145">Anzahl der bestandenen Test: 665</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1145">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="d8d1c-1146">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 263</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1146">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="d8d1c-1147">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1147">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1148">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1148">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1149">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1149">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1150">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1150">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a><span data-ttu-id="d8d1c-1151">Build 14936</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1151">Build 14936</span></span>

<span data-ttu-id="d8d1c-1152">Allgemeine Windows Informationen zum Build 14936 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1152">For general Windows information on build 14936 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span></span><br/>


<span data-ttu-id="d8d1c-1153">Hinweis: WSL wird Ubuntu Version 16.04 (Xenial) anstelle von Ubuntu 14.04 (treuen) in einer zukünftigen Version installiert werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1153">Note: WSL will install Ubuntu version 16.04 (Xenial) instead of Ubuntu 14.04 (Trusty) in an upcoming release.</span></span>  <span data-ttu-id="d8d1c-1154">Diese Änderung gilt für Insider neue Instanzen (lxrun.exe/install oder erste Ausführung des bash.exe) installieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1154">This change will apply to Insiders installing new instances (lxrun.exe /install or first run of bash.exe).</span></span>  <span data-ttu-id="d8d1c-1155">Vorhandene Instanzen mit treuen werden nicht automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1155">Existing instances with Trusty will not be upgraded automatically.</span></span> <span data-ttu-id="d8d1c-1156">Benutzer können ihr Softwareverwaltungssystem-Image auf Xenial mithilfe des Befehls-Release-Upgrade aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1156">Users can upgrade their Trusty image to Xenial using the do-release-upgrade command.</span></span>

### <a name="known-issue"></a><span data-ttu-id="d8d1c-1157">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1157">Known Issue</span></span>
<span data-ttu-id="d8d1c-1158">WSL ist ein Problem mit einigen Socketimplementierungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1158">WSL is experiencing an issue with some socket implementations.</span></span>  <span data-ttu-id="d8d1c-1159">Die fehlerüberprüfung manifestiert sich selbst als ein Absturz mit dem Fehler "Es wurde versucht Ausführen von"keinausführen "Arbeitsspeicher".</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1159">The bugcheck manifests itself as a crash with the error “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY”.</span></span>  <span data-ttu-id="d8d1c-1160">Die am häufigsten verwendeten Manifestation dieses Problems ist ein Absturz auf, wenn ssh verwenden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1160">The most common manifestation of this issue is a crash when using ssh.</span></span>  <span data-ttu-id="d8d1c-1161">Die zugrunde liegende Ursache ist für interne Builds festgelegt und wird bei nächstmöglicher Gelegenheit für Insider übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1161">The root cause is fixed on internal builds and will be pushed to Insiders at the earliest opportunity.</span></span>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1162">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1162">Fixed</span></span>

- <span data-ttu-id="d8d1c-1163">Implementiert die Chroot Systemaufruf</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1163">Implemented the chroot system call</span></span>
- <span data-ttu-id="d8d1c-1164">Verbesserungen bei der Inotify ~~einschließlich der Unterstützung von Windows-Anwendungen auf DrvFs generierten Benachrichtigungen~~</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1164">Improvements in inotify ~~including support for notifications generated from Windows applications on DrvFs~~</span></span>
  - <span data-ttu-id="d8d1c-1165">Korrektur: Inotify Unterstützung für Änderungen, die von Windows-Anwendungen, die zu diesem Zeitpunkt nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1165">Correction: Inotify support for changes originating from Windows applications not available at this time.</span></span>
- <span data-ttu-id="d8d1c-1166">Socket-Bindung zu IPV6::<port n> unterstützt jetzt IPV6_V6ONLY (68 des GH #, #157 "," #393 "," #460 "," #674 "," #740 "," #982 "," #996)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1166">Socket binding to IPV6::<port n> now supports IPV6_V6ONLY  (GH #68, #157, #393, #460, #674, #740, #982, #996)</span></span>
- <span data-ttu-id="d8d1c-1167">WNOWAIT Waitid Systemcall implementiert (GH #638)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1167">WNOWAIT behavior for waitid systemcall implemented (GH #638)</span></span>
- <span data-ttu-id="d8d1c-1168">Unterstützung für IP-Socket-Optionen IP_HDRINCL und IP_TTL</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1168">Support for IP socket options IP_HDRINCL and IP_TTL</span></span>
- <span data-ttu-id="d8d1c-1169">Mit der Länge Null read() sollte sofort zurückgeben (GH #975)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1169">Zero-length read() should return immediately (GH #975)</span></span>
- <span data-ttu-id="d8d1c-1170">Ordnungsgemäß verarbeiten Sie, Dateinamen und den Dateinamen Präfixe, die einen NULL-Terminator in einer TAR-Datei enthalten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1170">Correctly handle filenames and filename prefixes that don't include a NULL terminator in a .tar file.</span></span>
- <span data-ttu-id="d8d1c-1171">Epoll-Unterstützung für/dev/null</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1171">epoll support for /dev/null</span></span>
- <span data-ttu-id="d8d1c-1172">Beheben von /dev/alarm Zeitquelle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1172">Fix /dev/alarm time source</span></span>
- <span data-ttu-id="d8d1c-1173">Bash -c kann nun in eine Datei umleiten</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1173">Bash -c now able to redirect to a file</span></span>
- <span data-ttu-id="d8d1c-1174">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1174">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1175">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1175">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1176">Anzahl der bestandenen Test: 664</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1176">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="d8d1c-1177">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 264</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1177">Number of non-Passing (failing, skipped, etc…): 264</span></span> </br>
[<span data-ttu-id="d8d1c-1178">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1178">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1179">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1179">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1180">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1180">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1181">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1181">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`chroot`<br/>
<br/>

## <a name="build-14931"></a><span data-ttu-id="d8d1c-1182">Build 14931</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1182">Build 14931</span></span>

<span data-ttu-id="d8d1c-1183">Allgemeine Windows Informationen zum Build 14931 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1183">For general Windows information on build 14931 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1184">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1184">Fixed</span></span>

 - <span data-ttu-id="d8d1c-1185">Aufgrund von Umständen außerhalb unserer Kontrolle sind keine Updates in diesem Build für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1185">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="d8d1c-1186">Geplante regelmäßige Updates werden in der nächsten Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1186">Regularly scheduled updates will resume in the next release.</span></span>

<br/>

## <a name="build-14926"></a><span data-ttu-id="d8d1c-1187">Build 14926</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1187">Build 14926</span></span>

<span data-ttu-id="d8d1c-1188">Allgemeine Windows Informationen zum Build 14926 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1188">For general Windows information on build 14926 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1189">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1189">Fixed</span></span>

- <span data-ttu-id="d8d1c-1190">Ping funktioniert jetzt in der Konsolen, die nicht über Administratorberechtigungen verfügen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1190">Ping now works in consoles which do not have administrator privileges</span></span>
- <span data-ttu-id="d8d1c-1191">Nun unterstützt, auch ohne Administratorrechte ping6</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1191">Ping6 now supported, also without administrator privileges</span></span>
- <span data-ttu-id="d8d1c-1192">Inotify-Unterstützung für Dateien, die über WSL geändert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1192">Inotify support for files modified through WSL.</span></span> <span data-ttu-id="d8d1c-1193">(GH #216)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1193">(GH #216)</span></span>
  - <span data-ttu-id="d8d1c-1194">Flags, die unterstützt werden:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1194">Flags supported:</span></span>
    - <span data-ttu-id="d8d1c-1195">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1195">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span></span>
    - <span data-ttu-id="d8d1c-1196">Inotify_add_watch-Ereignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1196">inotify_add_watch events: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span></span>
    - <span data-ttu-id="d8d1c-1197">Inotify_add_watch Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1197">inotify_add_watch attributes: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span></span>
    - <span data-ttu-id="d8d1c-1198">Lesen Sie die Ausgabe: LX_IN_ISDIR, LX_IN_IGNORED</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1198">read output: LX_IN_ISDIR, LX_IN_IGNORED</span></span>
  - <span data-ttu-id="d8d1c-1199">Bekanntes Problem: Ändern von Dateien aus Windows-Anwendungen keine Ereignisse generiert keine</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1199">Known issue: Modifying files from Windows applications does not generate any events</span></span>
- <span data-ttu-id="d8d1c-1200">UNIX-Socket unterstützt jetzt SCM_CREDENTIALS</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1200">Unix socket now supports SCM_CREDENTIALS</span></span>

### <a name="ltp-results"></a><span data-ttu-id="d8d1c-1201">LTP Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1201">LTP Results:</span></span>
<span data-ttu-id="d8d1c-1202">Anzahl der bestandenen Test: 651</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1202">Number of Passing Test: 651</span></span> </br>
<span data-ttu-id="d8d1c-1203">Anzahl der nicht bestandenen (fehlgeschlagenen, ausgelassenen usw....): 258</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1203">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="d8d1c-1204">LTP Testlauf-Protokolle</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1204">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a><span data-ttu-id="d8d1c-1205">Build 14915</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1205">Build 14915</span></span>

<span data-ttu-id="d8d1c-1206">Allgemeine Windows Informationen zum Build 14915 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1206">For general Windows information on build 14915 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1207">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1207">Fixed</span></span>
-  <span data-ttu-id="d8d1c-1208">Socketpair für Unix-Datagrammsockets (GH #262)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1208">Socketpair for unix datagram sockets (GH #262)</span></span>
- <span data-ttu-id="d8d1c-1209">UNIX-Socket-Unterstützung für SO_REUSEADDR</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1209">Unix socket support for SO_REUSEADDR</span></span>
- <span data-ttu-id="d8d1c-1210">UNIX-Socket-Unterstützung für SO_BROADCAST (GH #568)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1210">UNIX socket support for SO_BROADCAST (GH #568)</span></span>
- <span data-ttu-id="d8d1c-1211">UNIX-Socket-Unterstützung für SOCK_SEQPACKET (GH #758, #546)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1211">Unix socket support for SOCK_SEQPACKET (GH #758, #546)</span></span>
- <span data-ttu-id="d8d1c-1212">Hinzufügen von Unterstützung für Unix-Datagramm Socket senden, empfangen und Herunterfahren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1212">Adding support for unix datagram socket send, recv and shutdown</span></span>
- <span data-ttu-id="d8d1c-1213">Beheben Sie die fehlerprüfung aufgrund ungültiger "mmap" parametervalidierung für Adressen nicht festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1213">Fix bugcheck due to invalid mmap parameter validation for non-fixed addresses.</span></span> <span data-ttu-id="d8d1c-1214">(GH #847)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1214">(GH #847)</span></span>
- <span data-ttu-id="d8d1c-1215">Unterstützung für das Anhalten / Fortsetzen von Terminaldienste-Status</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1215">Support for suspend / resume of terminal states</span></span>
- <span data-ttu-id="d8d1c-1216">Unterstützung für TIOCPKT Ioctl zum Entsperren des Bildschirms-Dienstprogramms (GH #774)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1216">Support for TIOCPKT ioctl to unblock the Screen utility (GH #774)</span></span>
    - <span data-ttu-id="d8d1c-1217">Bekanntes Problem: Funktionstasten nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1217">Known issue: Function keys not operational</span></span>
- <span data-ttu-id="d8d1c-1218">Korrigiert ein Race in TimerFd, die einen freigegebenen Member 'ReaderReady' für den Zugriff durch LxpTimerFdWorkerRoutine (GH #814) verursachen können</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1218">Corrected a race in TimerFd that could cause a freed member 'ReaderReady' to be accessed by LxpTimerFdWorkerRoutine (GH #814)</span></span>
- <span data-ttu-id="d8d1c-1219">Aktivieren Sie neu startbares Aufruf systemunterstützung für Futex, abrufen und clock_nanosleep</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1219">Enable restartable system call support for futex, poll, and clock_nanosleep</span></span>
- <span data-ttu-id="d8d1c-1220">Hinzugefügte Bindung Mount-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1220">Added bind mount support</span></span>
- <span data-ttu-id="d8d1c-1221">Aufheben der Freigabe für Mount-Namespace-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1221">unshare for mount namespace support</span></span>
    - <span data-ttu-id="d8d1c-1222">Bekanntes Problem: Beim Erstellen einer neuen Bereitstellung-Namespace mit `unshare(CLONE_NEWNS)` weiterhin das aktuelle Arbeitsverzeichnis auf den alten Namespace zu verweisen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1222">Known issue: When creating a new mount namespace with `unshare(CLONE_NEWNS)` the current working directory will continue to point to the old namespace</span></span>
- <span data-ttu-id="d8d1c-1223">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1223">Additional improvements and bug fixes</span></span>

<br/>

## <a name="build-14905"></a><span data-ttu-id="d8d1c-1224">Erstellen von 14905</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1224">Build 14905</span></span>

<span data-ttu-id="d8d1c-1225">Allgemeine Windows Informationen zum Build 14905 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1225">For general Windows information on build 14905 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1226">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1226">Fixed</span></span>
- <span data-ttu-id="d8d1c-1227">Neu startbares System jetzt in Aufrufe werden unterstützt (GH #349, GH #520)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1227">Restartable system calls are now supported (GH #349, GH #520)</span></span>
- <span data-ttu-id="d8d1c-1228">Symbolische Verknüpfungen zu Verzeichnissen im / jetzt operative endet (GH #650)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1228">Symlinks to directories ending in / now operational (GH #650)</span></span>
- <span data-ttu-id="d8d1c-1229">Implementierten RNDGETENTCNT Ioctl für/dev/Random</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1229">Implemented RNDGETENTCNT ioctl for /dev/random</span></span>
- <span data-ttu-id="d8d1c-1230">Implementiert die /proc/ [ProzessID] / durchführte, /proc/ [ProzessID] / Mountinfo und /proc/ [ProzessID] / Mountstats-Dateien</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1230">Implemented the /proc/[pid]/mounts, /proc/[pid]/mountinfo and /proc/[pid]/mountstats files</span></span>
- <span data-ttu-id="d8d1c-1231">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1231">Additional bugfixes and improvements</span></span>

</br>

## <a name="build-14901"></a><span data-ttu-id="d8d1c-1232">Build 14901</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1232">Build 14901</span></span>
<span data-ttu-id="d8d1c-1233">Erste Insider-build für den Post-Version von Windows 10 Anniversary Update.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1233">First Insider build for the post Windows 10 Anniversary Update release.</span></span>

<span data-ttu-id="d8d1c-1234">Allgemeine Windows Informationen zum Build 14901 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1234">For general Windows information on build 14901 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1235">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1235">Fixed</span></span>
- <span data-ttu-id="d8d1c-1236">Nachgestellten Schrägstrich behoben</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1236">Fixed trailing slash issue</span></span>
    - <span data-ttu-id="d8d1c-1237">Befehle wie `$ mv a/c/ a/b/` funktioniert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1237">Commands such as `$ mv a/c/ a/b/` now work</span></span>
- <span data-ttu-id="d8d1c-1238">Installieren von jetzt aufgefordert, wenn es sich bei Ubuntu-Gebietsschema auf Windows-Gebietsschema festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1238">Installing now prompts if Ubuntu locale should be set to Windows locale</span></span>
- <span data-ttu-id="d8d1c-1239">Procfs Unterstützung für Ordner "ns"</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1239">Procfs support for ns folder</span></span>
- <span data-ttu-id="d8d1c-1240">Hinzugefügt bereitstellen und Aufheben der Bereitstellung für Tmpfs, procfs und Dateisysteme Sysfs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1240">Added mount and unmount for tmpfs, procfs and sysfs file systems</span></span>
- <span data-ttu-id="d8d1c-1241">Beheben von Mknod [at] 32-Bit-ABI-Signatur</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1241">Fix mknod[at] 32-bit ABI signature</span></span>
- <span data-ttu-id="d8d1c-1242">UNIX-Sockets verschoben wird, um Modell zu senden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1242">Unix sockets moved to dispatch model</span></span>
- <span data-ttu-id="d8d1c-1243">INET Socket empfangene Puffergröße festgelegt wird, verwenden die Setsockopt sollten berücksichtigt werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1243">INET socket recv buffer size set using the setsockopt should be honored</span></span>
- <span data-ttu-id="d8d1c-1244">Implementieren MSG_CMSG_CLOEXEC-Unix-Socket empfängt Nachricht kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1244">Implement MSG_CMSG_CLOEXEC unix socket receive message flag</span></span>
- <span data-ttu-id="d8d1c-1245">Linux-Prozess "Stdin/stdout" Pipe Umleitung (GH #2)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1245">Linux process stdin/stdout pipe redirection (GH #2)</span></span>
    - <span data-ttu-id="d8d1c-1246">Ermöglicht das Weiterleiten der Bash - C-Befehle in cmd ein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1246">Allows for piping of bash -c commands in CMD.</span></span>  <span data-ttu-id="d8d1c-1247">Beispiel: > Dir | bash -c "Foo" Grep"</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1247">Example:  >dir | bash -c "grep foo"</span></span>
- <span data-ttu-id="d8d1c-1248">Bash kann auf Systemen mit mehreren Auslagerungsdateien (GH #538, #358) jetzt installiert werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1248">Bash can now be installed on systems with multiple pagefiles (GH #538, #358)</span></span>
- <span data-ttu-id="d8d1c-1249">INET-Socket-Standardpuffergröße sollte mit der Standard-Ubuntu-Setup übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1249">Default INET Socket buffer size should match that of default Ubuntu setup</span></span>
- <span data-ttu-id="d8d1c-1250">Xattr Syscalls zu Listxattr ausrichten</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1250">Align xattr syscalls to listxattr</span></span>
- <span data-ttu-id="d8d1c-1251">Nur Schnittstellen mit einer gültigen IPv4-Adresse von SIOCGIFCONF zurück</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1251">Only return interfaces with a valid IPv4 address from SIOCGIFCONF</span></span>
- <span data-ttu-id="d8d1c-1252">Beheben von Signal Standardaktion, wenn durch Ptrace eingefügt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1252">Fix signal default action when injected by ptrace</span></span>
- <span data-ttu-id="d8d1c-1253">Implementieren von /proc/sys/vm/min_free_kbytes</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1253">implement /proc/sys/vm/min_free_kbytes</span></span>
- <span data-ttu-id="d8d1c-1254">Verwenden Sie Computer registrieren Kontextwerte, beim Wiederherstellen der Kontext in sigreturn</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1254">Use machine context register values when restoring context in sigreturn</span></span>
    - <span data-ttu-id="d8d1c-1255">Dadurch wird das Problem behoben, in denen wurden Java- und Javac für einige Benutzer hängende</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1255">This resolves the issue where java and javac were hanging for some users</span></span>
- <span data-ttu-id="d8d1c-1256">Implementieren von /proc/sys/kernel/hostname</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1256">Implement /proc/sys/kernel/hostname</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1257">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1257">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1258">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1258">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1259">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1259">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a><span data-ttu-id="d8d1c-1260">Erstellen von 14388 auf Windows 10 Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1260">Build 14388 to Windows 10 Anniversary Update</span></span>
<span data-ttu-id="d8d1c-1261">Allgemeine Windows Informationen zum Build 14388 finden Sie auf die [Windows Blog](https://aka.ms/14388wip).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1261">For general Windows information on build 14388 visit the [Windows Blog](https://aka.ms/14388wip).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1262">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1262">Fixed</span></span>
- <span data-ttu-id="d8d1c-1263">Fehlerbehebungen für die Vorbereitung auf Windows 10 Anniversary Update auf 8/2</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1263">Fixes to prepare for the Windows 10 Anniversary Update on 8/2</span></span>
  - <span data-ttu-id="d8d1c-1264">Weitere Informationen zu WSL, in dem Anniversary-Update finden Sie auf unserer [Blog](https://blogs.msdn.microsoft.com/wsl/)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1264">More information about WSL in the Anniversary Update can be found on our [blog](https://blogs.msdn.microsoft.com/wsl/)</span></span>

<br/>

## <a name="build-14376"></a><span data-ttu-id="d8d1c-1265">Build 14376</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1265">Build 14376</span></span>
<span data-ttu-id="d8d1c-1266">Allgemeine Windows Informationen zum Build 14376 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1266">For general Windows information on build 14376 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1267">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1267">Fixed</span></span>
- <span data-ttu-id="d8d1c-1268">Einigen Fällen, in dem apt-Get (GH #493) hängt, entfernt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1268">Removed some instances where apt-get hangs (GH #493)</span></span>
- <span data-ttu-id="d8d1c-1269">Ein Problem wurde behoben, in denen leere Mounts nicht ordnungsgemäß verarbeitet wurden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1269">Fixed an issue where empty mounts were not handled correctly</span></span>
- <span data-ttu-id="d8d1c-1270">Ein Problem wurde behoben, von dem Ramdisks nicht ordnungsgemäß bereitgestellt wurden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1270">Fixed an issue where ramdisks were not mounted correctly</span></span>
- <span data-ttu-id="d8d1c-1271">Änderung von Unix-Socket akzeptiert wird, zur Unterstützung von Flags (partielle GH #451)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1271">Change unix socket accept to support flags (partial GH #451)</span></span>
- <span data-ttu-id="d8d1c-1272">Feste allgemeine netzwerkbezogenen bluescreen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1272">Fixed common network related bluescreen</span></span>
- <span data-ttu-id="d8d1c-1273">Bluescreen behoben, wenn /proc/ [ProzessID] den Zugriff auf / task (GH #523)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1273">Fixed bluescreen when accessing /proc/[pid]/task (GH #523)</span></span>
- <span data-ttu-id="d8d1c-1274">Feste hohe CPU-Auslastung für einige Pty-Szenarien (GH #488, #504)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1274">Fixed high CPU utilization for some pty scenarios (GH #488, #504)</span></span>
- <span data-ttu-id="d8d1c-1275">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1275">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14371"></a><span data-ttu-id="d8d1c-1276">Build 14371</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1276">Build 14371</span></span>
<span data-ttu-id="d8d1c-1277">Allgemeine Windows Informationen zum Build 14371 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1277">For general Windows information on build 14371 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1278">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1278">Fixed</span></span>
- <span data-ttu-id="d8d1c-1279">Timing Race mit SIGCHLD und wait() korrigiert, wenn Sie Ptrace verwenden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1279">Corrected timing race with SIGCHLD and wait() when using ptrace</span></span>
- <span data-ttu-id="d8d1c-1280">Einige Verhalten korrigiert, wenn ein nachstehender-Pfade verfügen. / (GH #432)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1280">Corrected some behavior when paths have a trailing /  (GH #432)</span></span>
- <span data-ttu-id="d8d1c-1281">Korrigiert: beim Umbenennen und Aufheben der Verknüpfung Fehler aufgrund eines offenen Handles zu untergeordneten Elementen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1281">Fixed issue with rename/unlink failing due to open handles to children</span></span>
- <span data-ttu-id="d8d1c-1282">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1282">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14366"></a><span data-ttu-id="d8d1c-1283">Build 14366</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1283">Build 14366</span></span>
<span data-ttu-id="d8d1c-1284">Allgemeine Windows Informationen zum Build 14366 finden Sie auf die [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1284">For general Windows information on build 14366 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1285">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1285">Fixed</span></span>
- <span data-ttu-id="d8d1c-1286">Beheben Sie im dateierstellung bis hin zur symbolische Verknüpfungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1286">Fix in file creation through symlinks</span></span>
-   <span data-ttu-id="d8d1c-1287">Hinzugefügte Listxattr für Python (GH 385)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1287">Added listxattr for Python (GH 385)</span></span>
-   <span data-ttu-id="d8d1c-1288">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1288">Additional bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1289">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1289">Syscall Support</span></span>
-   <span data-ttu-id="d8d1c-1290">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1290">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1291">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1291">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`listxattr`<br/>
<br/>

## <a name="build-14361"></a><span data-ttu-id="d8d1c-1292">Build 14361</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1292">Build 14361</span></span>
<span data-ttu-id="d8d1c-1293">Allgemeine Windows Informationen zum Build 14361 finden Sie auf die [Windows Blog](https://aka.ms/wip14361).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1293">For general Windows information on build 14361 visit the [Windows Blog](https://aka.ms/wip14361).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1294">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1294">Fixed</span></span>
- <span data-ttu-id="d8d1c-1295">DrvFs ist jetzt Groß-/Kleinschreibung beachtet, wenn in Bash auf Ubuntu unter Windows ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1295">DrvFs is now case sensitive when running in Bash on Ubuntu on Windows.</span></span>
  - <span data-ttu-id="d8d1c-1296">Benutzer Mai case.txt und Groß-/KLEINSCHREIBUNG. TXT, auf die c/Mnt/Laufwerke</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1296">Users may case.txt and CASE.TXT on their /mnt/c drives</span></span>
  - <span data-ttu-id="d8d1c-1297">Groß-/Kleinschreibung wird nur in Bash auf Ubuntu unter Windows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1297">Case sensitivity is only supported within Bash on Ubuntu on Windows.</span></span> <span data-ttu-id="d8d1c-1298">Wenn außerhalb der Bash-NTFS-Dateien ordnungsgemäß gemeldet wird, aber kann unerwartetes Verhalten auftreten, interagieren mit den Dateien von Windows.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1298">When outside of Bash NTFS will report the files correctly, but unexpected behavior may occur interacting with the files from Windows.</span></span>
  - <span data-ttu-id="d8d1c-1299">Der Stamm des jedes Volume (d. h. /mnt/c) ist keine Groß-/Kleinschreibung beachten</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1299">The root of each volume (i.e. /mnt/c) is not case sensitive</span></span>
  - <span data-ttu-id="d8d1c-1300">Weitere Informationen zur Behandlung dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1300">More information on handling these files in Windows can be found [here](https://support.microsoft.com/en-us/kb/100625).</span></span>
- <span data-ttu-id="d8d1c-1301">Verbesserte Pty / tty unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1301">Greatly enhanced pty / tty support.</span></span>  <span data-ttu-id="d8d1c-1302">Anwendungen wie TMUX jetzt unterstützt (GH #-40).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1302">Applications like TMUX now supported (GH #40)</span></span>
- <span data-ttu-id="d8d1c-1303">Problem mit der festen Installation, in denen Benutzerkonten nicht immer erstellt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1303">Fixed install issue where user accounts not always created</span></span>
- <span data-ttu-id="d8d1c-1304">Optimiert die Befehlszeile Arg-Struktur, die sehr lange Argumentliste ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1304">Optimized command line arg structure allowing for extremely long argument list.</span></span> <span data-ttu-id="d8d1c-1305">(GH #153)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1305">(GH #153)</span></span>
- <span data-ttu-id="d8d1c-1306">Kann nun zum Löschen und Chmod-Dateien Read_only DrvFs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1306">Now able to delete and chmod read_only files from DrvFs</span></span>
- <span data-ttu-id="d8d1c-1307">Feste einigen Fällen, in dem der Terminaldienste Systemstillstand auf (GH #43) trennen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1307">Fixed some instances where the terminal hangs on disconnect (GH #43)</span></span>
- <span data-ttu-id="d8d1c-1308">Chmod und Chown sind jetzt für tty-Geräte</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1308">chmod and chown now work on tty devices</span></span>
- <span data-ttu-id="d8d1c-1309">Lassen Sie die Verbindung auf "0.0.0.0" und:: als "localhost" (GH #388)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1309">Allow connection to 0.0.0.0 and :: as localhost (GH #388)</span></span>
- <span data-ttu-id="d8d1c-1310">Sendmsg/Recvmsg jetzt eine e/a-Vektor-Länge des behandeln > 1 (partielle GH #376)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1310">Sendmsg/recvmsg now handle an IO vector length of >1 (partial GH #376)</span></span>
- <span data-ttu-id="d8d1c-1311">Benutzer können nun automatisch generierte Datei "Hosts" (GH #398) deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1311">Users can now opt-out of auto-generated hosts file (GH #398)</span></span>
- <span data-ttu-id="d8d1c-1312">Entsprechen Sie, Linux-Gebietsschema, das das NT-Gebietsschema automatisch während der Installation (GH #11)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1312">Automatically match Linux locale to the NT locale during install (GH #11)</span></span>
- <span data-ttu-id="d8d1c-1313">Die Datei /proc/sys/vm/swappiness (GH #306) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1313">Added the /proc/sys/vm/swappiness file (GH #306)</span></span>
- <span data-ttu-id="d8d1c-1314">"strace" wird jetzt beendet ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1314">strace now exits correctly</span></span>
- <span data-ttu-id="d8d1c-1315">Zulassen von Pipes, um über /proc/self/fd (GH #222) erneut geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1315">Allow pipes to be reopened through /proc/self/fd (GH #222)</span></span>
- <span data-ttu-id="d8d1c-1316">Blenden Sie die Verzeichnisse unter %LOCALAPPDATA%\lxss aus DrvFs (GH #270)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1316">Hide directories under %LOCALAPPDATA%\lxss from DrvFs (GH #270)</span></span>
- <span data-ttu-id="d8d1c-1317">Bessere Verarbeitung von bash.exe ~.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1317">Better handling of bash.exe ~.</span></span>  <span data-ttu-id="d8d1c-1318">Befehle wie "bash ~ - C ls" unterstützt jetzt (GH #467)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1318">Commands like “bash ~ -c ls” now supported (GH #467)</span></span>
- <span data-ttu-id="d8d1c-1319">Sockets benachrichtigen jetzt Epoll lesen, die während des Herunterfahrens (GH #271) zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1319">Sockets now notify epoll read available during shutdown (GH #271)</span></span>
- <span data-ttu-id="d8d1c-1320">Lxrun / uninstall ist besser Löschen von Dateien und Ordner</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1320">lxrun /uninstall does a better job of deleting the files and folders</span></span>
- <span data-ttu-id="d8d1c-1321">Korrigierte Ps -f (GH #246)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1321">Corrected ps -f (GH #246)</span></span>
- <span data-ttu-id="d8d1c-1322">Verbesserte Unterstützung für X11 apps wie xEmacs (GH #481)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1322">Improved support for x11 apps such as xEmacs (GH #481)</span></span>
- <span data-ttu-id="d8d1c-1323">Anfängliche Thread Stapelgröße Ubuntu-Standardeinstellung und die Größe ordnungsgemäß an die Get_rlimit Syscall (GH #172, #258) Berichten entsprechend aktualisiert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1323">Updated initial thread stack size to match default Ubuntu setting and reporting the size correctly to the get_rlimit syscall (GH #172, #258)</span></span>
- <span data-ttu-id="d8d1c-1324">Verbesserte berichterstellung mit Pico-Prozess-imagenamen (z. B. für die Überwachung)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1324">Improved reporting of pico process image names (e.g., for auditing)</span></span>
- <span data-ttu-id="d8d1c-1325">Implementierten /proc/mountinfo für df-Befehl</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1325">Implemented /proc/mountinfo for df command</span></span>
- <span data-ttu-id="d8d1c-1326">Festen "Symlink" den Fehlercode für den Namen fest.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1326">Fixed symlink error code for child name .</span></span> <span data-ttu-id="d8d1c-1327">und...</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1327">and ..</span></span>
- <span data-ttu-id="d8d1c-1328">Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1328">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1329">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1329">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1330">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1330">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1331">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1331">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a><span data-ttu-id="d8d1c-1332">Build 14352</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1332">Build 14352</span></span>
<span data-ttu-id="d8d1c-1333">Allgemeine Windows Informationen zum Build 14352 finden Sie auf die [Windows Blog](https://aka.ms/wip14352).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1333">For general Windows information on build 14352 visit the [Windows Blog](https://aka.ms/wip14352).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1334">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1334">Fixed</span></span>
- <span data-ttu-id="d8d1c-1335">Korrigiert: Problem, in dem große Dateien wurden heruntergeladen / nicht ordnungsgemäß erstellt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1335">Fixed issue where large files were not downloaded / created correctly.</span></span>  <span data-ttu-id="d8d1c-1336">Dies sollte Npm und andere Szenarien (GH-3, GH #313) zulassen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1336">This should unblock npm and other scenarios (GH #3, GH #313)</span></span>
- <span data-ttu-id="d8d1c-1337">Entfernt einige Instanzen, in denen Sockets hängen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1337">Removed some instances where sockets hang</span></span>
- <span data-ttu-id="d8d1c-1338">Einige Ptrace Fehler korrigiert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1338">Corrected some ptrace errors</span></span>
- <span data-ttu-id="d8d1c-1339">Korrigiert: Probleme mit WSL Dateinamen, die länger als 255 Zeichen zulassen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1339">Fixed issue with WSL allowing filenames longer than 255 characters</span></span>
- <span data-ttu-id="d8d1c-1340">Verbesserte Unterstützung für nicht-englische Zeichen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1340">Improved support for non-English characters</span></span>
- <span data-ttu-id="d8d1c-1341">Aktuelle Windows-Timezone-Daten hinzufügen und als Standard festlegen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1341">Add current Windows timezone data and set as default</span></span>
- <span data-ttu-id="d8d1c-1342">Eindeutige Geräte-Id für die einzelnen einbindungspunkt (Jre-Fix: GH Nr. 49)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1342">Unique device id’s for each mount point (jre fix – GH #49)</span></span>
- <span data-ttu-id="d8d1c-1343">Beheben Sie Fehler mit Pfaden, die mit "."</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1343">Correct issue with paths containing “.”</span></span> <span data-ttu-id="d8d1c-1344">und ".."</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1344">and “..”</span></span>
- <span data-ttu-id="d8d1c-1345">Fifo-Unterstützung (GH #71)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1345">Added Fifo support (GH #71)</span></span>
- <span data-ttu-id="d8d1c-1346">Aktualisierte Format von "resolv.conf" muss entsprechend der systemeigenen Ubuntu-format</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1346">Updated format of resolv.conf to match native Ubuntu format</span></span>
- <span data-ttu-id="d8d1c-1347">Einige Bereinigungsschritte procfs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1347">Some procfs cleanup</span></span>
- <span data-ttu-id="d8d1c-1348">Aktivierte Ping für Administratorkonsolen (GH Nr. 18)</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1348">Enabled ping for Administrator consoles (GH #18)</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1349">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1349">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1350">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1350">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1351">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1351">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a><span data-ttu-id="d8d1c-1352">Build 14342</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1352">Build 14342</span></span>
<span data-ttu-id="d8d1c-1353">Informationen zum Erstellen für allgemeine Windows 14342 der [Windows Blog](https://aka.ms/wip14342).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1353">For general Windows information on build 14342 the [Windows Blog](https://aka.ms/wip14342).</span></span> <br/>

<span data-ttu-id="d8d1c-1354">Informationen zu VolFs und DriveFs finden Sie auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1354">Information on VolFs and DriveFs can be found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1355">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1355">Fixed</span></span>
- <span data-ttu-id="d8d1c-1356">Install-Problem wurde behoben, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen hat.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1356">Fixed install issue when the Windows user had Unicode characters in the username</span></span>
- <span data-ttu-id="d8d1c-1357">Die Updates von apt-Get-Udev-problemumgehung in den häufig gestellten Fragen wird nun standardmäßig bei der ersten Ausführung bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1357">The apt-get update udev workaround in the FAQ is now provided by default on first run</span></span>
- <span data-ttu-id="d8d1c-1358">Symbolische Verknüpfungen in DriveFs aktiviert (/mnt/<drive>) Verzeichnisse</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1358">Enabled symlinks in DriveFs (/mnt/<drive>) directories</span></span>
- <span data-ttu-id="d8d1c-1359">Symbolische Verknüpfungen funktionieren jetzt zwischen DriveFs und VolFs</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1359">Symlinks now work between DriveFs and VolFs</span></span>
- <span data-ttu-id="d8d1c-1360">Adressierte Top Level Pfad Problem analysieren: ls. / / funktioniert nun wie erwartet</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1360">Addressed top level path parsing issue: ls .// will now work as expected</span></span>
- <span data-ttu-id="d8d1c-1361">Npm installieren, auf DriveFs und die -g-Optionen sind jetzt funktionsfähig.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1361">npm install on DriveFs and the -g options are now working</span></span>
- <span data-ttu-id="d8d1c-1362">Problem behoben, die verhindert, dass PHP-Server starten</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1362">Fixed issue preventing PHP server from launching</span></span>
- <span data-ttu-id="d8d1c-1363">Aktualisierte Umgebung Standardwerte, z. B. $PATH näher übereinstimmen der native Ubuntu</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1363">Updated default environment values, such as $PATH to closer match native Ubuntu</span></span>
- <span data-ttu-id="d8d1c-1364">Eine wöchentliche Wartungsaufgabe hinzugefügt, in Windows den apt-Paketcache aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1364">Added a weekly maintenance task in Windows to update the apt package cache</span></span>
- <span data-ttu-id="d8d1c-1365">Problem mit ELF headerüberprüfung wurde behoben, unterstützt die WSL jetzt alle Melkor-Optionen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1365">Fixed issue with ELF header validation, WSL now supports all Melkor options</span></span>
- <span data-ttu-id="d8d1c-1366">Zsh Shell funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1366">Zsh shell is functional</span></span>
- <span data-ttu-id="d8d1c-1367">Vorkompilierte Go-Binärdateien werden jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1367">Precompiled Go binaries are now supported</span></span>
- <span data-ttu-id="d8d1c-1368">Aufforderung für den anpassungs-Bash.exe ist jetzt ordnungsgemäß lokalisiert</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1368">Prompting on Bash.exe first run is now localized correctly</span></span>
- <span data-ttu-id="d8d1c-1369">/proc/meminfo gibt jetzt Informationen zurück.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1369">/proc/meminfo now returns correct information</span></span>
- <span data-ttu-id="d8d1c-1370">Sockets, die jetzt im virtuellen Dateisystem unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1370">Sockets now supported in VFS</span></span>
- <span data-ttu-id="d8d1c-1371">können jetzt als Tempfs eingebunden.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1371">/dev now mounted as tempfs</span></span>
- <span data-ttu-id="d8d1c-1372">FIFO-Prinzip jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1372">Fifo now supported</span></span>
- <span data-ttu-id="d8d1c-1373">Multicore-Systeme, die nun ordnungsgemäß angezeigt werden, in dem/Proc/cpuinfo</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1373">Multi-core systems now showing correctly in /proc/cpuinfo</span></span>
- <span data-ttu-id="d8d1c-1374">Weitere Verbesserungen und Fehlermeldungen, die während der ersten Ausführung herunterladen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1374">Additional improvements and error messages downloading during first run</span></span>
- <span data-ttu-id="d8d1c-1375">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1375">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="d8d1c-1376">Unterstützt Syscall-Liste unten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1376">Supported syscall list below.</span></span>
- <span data-ttu-id="d8d1c-1377">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1377">Additional bugfixes and improvements</span></span>

### <a name="known-issues"></a><span data-ttu-id="d8d1c-1378">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1378">Known Issues</span></span>
- <span data-ttu-id="d8d1c-1379">Nicht auflösen '..'</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1379">Not resolving ‘..’</span></span> <span data-ttu-id="d8d1c-1380">ordnungsgemäß auf DriveFs in einigen Fällen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1380">correctly on DriveFs in some cases</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1381">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1381">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1382">Im folgenden finden Sie eine Liste der neuen oder verbesserten Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1382">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1383">Die Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1383">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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

## <a name="build-14332"></a><span data-ttu-id="d8d1c-1384">Build 14332</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1384">Build 14332</span></span>

<span data-ttu-id="d8d1c-1385">Allgemeine Windows Informationen zum Build 14332 finden Sie auf die [Windows Blog](https://aka.ms/wip14332).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1385">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14332).</span></span> <br/>


### <a name="fixed"></a><span data-ttu-id="d8d1c-1386">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1386">Fixed</span></span>
- <span data-ttu-id="d8d1c-1387">Eine bessere "resolv.conf" Generation einschließlich Priorisieren von DNS-Einträge</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1387">Better resolv.conf generation including prioritizing DNS entries</span></span>
- <span data-ttu-id="d8d1c-1388">Problem beim Verschieben von Dateien und Verzeichnisse zwischen enthaltenen und nicht- / Mnt-Laufwerke</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1388">Issue with moving files and directories between /mnt and non-/mnt drives</span></span>
- <span data-ttu-id="d8d1c-1389">TAR-Dateien können jetzt mit symbolische Verknüpfungen erstellt werden</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1389">Tar files can now be created with symlinks</span></span>
- <span data-ttu-id="d8d1c-1390">Hinzugefügte /run/lock Standardverzeichnis für die instanzerstellung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1390">Added default /run/lock directory on instance creation</span></span>
- <span data-ttu-id="d8d1c-1391">Update/dev/NULL zurückzugebenden richtigen Stat-Informationen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1391">Update /dev/null to return proper stat info</span></span>
- <span data-ttu-id="d8d1c-1392">Weitere Fehler beim Herunterladen von während der ersten Ausführung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1392">Additional errors when downloading during first run</span></span>
- <span data-ttu-id="d8d1c-1393">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1393">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="d8d1c-1394">Unterstützt Syscall-Liste unten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1394">Supported syscall list below.</span></span>
- <span data-ttu-id="d8d1c-1395">Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1395">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1396">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1396">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1397">Im folgenden finden Sie die neue Syscall, die eine Implementierung in WSL aufweist.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1397">Below is the new syscall that has some implementation in WSL.</span></span> <span data-ttu-id="d8d1c-1398">Die Syscall in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise nicht, dass alle Parameter eine unterstützte zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1398">The syscall on this list is supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a><span data-ttu-id="d8d1c-1399">Build 14328</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1399">Build 14328</span></span>

<span data-ttu-id="d8d1c-1400">Allgemeine Windows Informationen zum Build 14332 finden Sie auf die [Windows Blog](https://aka.ms/wip14328).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1400">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14328).</span></span> <br/>


### <a name="new-features"></a><span data-ttu-id="d8d1c-1401">Neue Features</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1401">New Features</span></span>
* <span data-ttu-id="d8d1c-1402">Unterstützt nun Linux-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1402">Now support Linux users.</span></span>  <span data-ttu-id="d8d1c-1403">Installieren von Bash unter Ubuntu unter Windows werden für die Erstellung eines Linux-Benutzers aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1403">Installing Bash on Ubuntu on Windows will prompt for creation of a Linux user.</span></span>  <span data-ttu-id="d8d1c-1404">Weitere Informationen finden Sie unter https://aka.ms/wslusers</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1404">For more information, visit https://aka.ms/wslusers</span></span>
* <span data-ttu-id="d8d1c-1405">Hostname wird jetzt auf den Namen des Windows-Computers nicht mehr festgelegt @localhost</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1405">Hostname is now set to the Windows computer name, no more @localhost</span></span>
* <span data-ttu-id="d8d1c-1406">Weitere Informationen zum Erstellen von 14328 unterstützen, finden Sie unter: https://aka.ms/wip14328</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1406">For more information on build 14328, visit: https://aka.ms/wip14328</span></span>

### <a name="fixed"></a><span data-ttu-id="d8d1c-1407">Fest</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1407">Fixed</span></span>
* <span data-ttu-id="d8d1c-1408">Verbesserungen des "Symlink" für nicht /mnt/<drive> Dateien</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1408">Symlink improvements for non /mnt/<drive> files</span></span>
    * <span data-ttu-id="d8d1c-1409">die Installation funktioniert nun npm</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1409">npm install now works</span></span>
    * <span data-ttu-id="d8d1c-1410">JDK / Jre jetzt installierbare anhand der Anweisungen [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1410">jdk / jre now installable using instructions found [here](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span></span>
    * <span data-ttu-id="d8d1c-1411">bekanntes Problem: symbolische Links funktionieren nicht für Windows bindet.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1411">known issue: symlinks do not work for Windows mounts.</span></span>  <span data-ttu-id="d8d1c-1412">Funktionen werden in eine höhere Version verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1412">Functionality will be available in a later build</span></span>
* <span data-ttu-id="d8d1c-1413">Top und einfach zeigen jetzt</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1413">top and htop now display</span></span>
* <span data-ttu-id="d8d1c-1414">Installieren Sie weitere Fehlermeldungen für einige Fehler</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1414">Additional error messages for some install failures</span></span>
* <span data-ttu-id="d8d1c-1415">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1415">Syscall improvements and bugfixes.</span></span>  <span data-ttu-id="d8d1c-1416">Unterstützt Syscall-Liste unten.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1416">Supported syscall list below.</span></span>
* <span data-ttu-id="d8d1c-1417">Weitere Verbesserungen, Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1417">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="d8d1c-1418">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1418">Syscall Support</span></span>
<span data-ttu-id="d8d1c-1419">Es folgt eine Liste der Syscalls, die eine Implementierung in WSL zu haben.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1419">Below is a list of syscalls that have some implementation in WSL.</span></span>  <span data-ttu-id="d8d1c-1420">Syscalls in dieser Liste werden in mindestens ein Szenario unterstützt, aber möglicherweise nicht verfügen alle Parameter unterstützt zu diesem Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d8d1c-1420">Syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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
