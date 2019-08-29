---
title: Versions Hinweise für das Windows-Subsystem für Linux
description: Versions Hinweise für das Windows-Subsystem für Linux.  Wöchentlich aktualisiert.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu
author: benhillis
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 36ea641e-4d49-4881-84eb-a9ca85b1cdf4
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 56a596c39b0d07e75d0beb381b80af5a14612e00
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122754"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a><span data-ttu-id="19ca1-105">Versions Hinweise für das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="19ca1-105">Release Notes for Windows Subsystem for Linux</span></span>


## <a name="build-18945"></a><span data-ttu-id="19ca1-106">Build 18945</span><span class="sxs-lookup"><span data-stu-id="19ca1-106">Build 18945</span></span>
<span data-ttu-id="19ca1-107">Allgemeine Windows-Informationen zu Build 18945 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-107">For general Windows information on build 18945 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-108">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-108">WSL</span></span>
* <span data-ttu-id="19ca1-109">[WSL2] Ermöglicht den Zugriff auf das lauschen von TCP-Sockets in WSL2 über den Host mithilfe von "localhost: Port".</span><span class="sxs-lookup"><span data-stu-id="19ca1-109">[WSL2] Allow listening tcp sockets in WSL2 to be accessible from the host by using localhost:port</span></span>
* <span data-ttu-id="19ca1-110">[WSL2] Fehlerbehebungen für Installations-und Konvertierungs Fehler und zusätzliche Diagnose zur Verfolgung zukünftiger Probleme [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="19ca1-110">[WSL2] Fixes for install / conversion failures and additional diagnostics to track down future issues [GH 4105]</span></span> 
* <span data-ttu-id="19ca1-111">[WSL2] Verbessern der Diagnose von Netzwerkproblemen WSL2</span><span class="sxs-lookup"><span data-stu-id="19ca1-111">[WSL2] Improve diagnosability of WSL2 network issues</span></span>
* <span data-ttu-id="19ca1-112">[WSL2] Kernel Version auf 4.19.55 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="19ca1-112">[WSL2] Update kernel version to 4.19.55</span></span>
* <span data-ttu-id="19ca1-113">[WSL2] Aktualisieren des Kernels mit Konfigurationsoptionen, die für docker erforderlich sind [GH 4165]</span><span class="sxs-lookup"><span data-stu-id="19ca1-113">[WSL2] Update kernel with config options required for docker [GH 4165]</span></span>
* <span data-ttu-id="19ca1-114">[WSL2] Erhöhen Sie die Anzahl der CPUs, die dem Lightweight-Hilfsprogramm-VM zugewiesen sind, damit Sie mit dem Host identisch ist (zuvor auf 8 durch CONFIG_NR_CPUS in der Kernelkonfiguration begrenzt) [GH 4137]</span><span class="sxs-lookup"><span data-stu-id="19ca1-114">[WSL2] Increase the number of CPUs assigned to the lightweight utility VM to be the same as the host (was previously capped at 8 by CONFIG_NR_CPUS in the kernel config) [GH 4137]</span></span>
* <span data-ttu-id="19ca1-115">[WSL2] Erstellen einer Auslagerungs Datei für die WSL2-Lightweight-VM</span><span class="sxs-lookup"><span data-stu-id="19ca1-115">[WSL2] Create a swap file for the WSL2 lightweight VM</span></span>
* <span data-ttu-id="19ca1-116">[WSL2] Zulassen, dass Benutzer Bereitstellungen über \\ \\WSL $\\Distribution (z. b. sshfs) sichtbar sind [GH 4172]</span><span class="sxs-lookup"><span data-stu-id="19ca1-116">[WSL2] Allow user mounts to be visible via \\\\wsl$\\distro (for example sshfs) [GH 4172]</span></span>
* <span data-ttu-id="19ca1-117">[WSL2] Verbessern der Systemleistung von 9P</span><span class="sxs-lookup"><span data-stu-id="19ca1-117">[WSL2] Improve 9p filesystem performance</span></span>
* <span data-ttu-id="19ca1-118">[WSL2] Sicherstellen, dass die VHD-ACL nicht unbegrenzt wächst [GH 4126]</span><span class="sxs-lookup"><span data-stu-id="19ca1-118">[WSL2] Ensure vhd ACL does not grow unbounded [GH 4126]</span></span>
* <span data-ttu-id="19ca1-119">[WSL2] Aktualisieren der Kernelkonfiguration zur Unterstützung von "squashfs" und "xt_conntrack" [GH 4107, 4123]</span><span class="sxs-lookup"><span data-stu-id="19ca1-119">[WSL2] Update kernel config to support squashfs and xt_conntrack [GH 4107, 4123]</span></span>
* <span data-ttu-id="19ca1-120">[WSL2] Behebung für Interop. aktivierte/etc/WSL.conf Option [GH 4140]</span><span class="sxs-lookup"><span data-stu-id="19ca1-120">[WSL2] Fix for interop.enabled /etc/wsl.conf option [GH 4140]</span></span>
* <span data-ttu-id="19ca1-121">[WSL2] Rückgabe von "umotsup", wenn das Dateisystem EAS nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19ca1-121">[WSL2] Return ENOTSUP if the file system does not support EAs</span></span>
* <span data-ttu-id="19ca1-122">[WSL2] Korrigieren von CopyFile- \\hängen mit \\WSL $</span><span class="sxs-lookup"><span data-stu-id="19ca1-122">[WSL2] Fix CopyFile hang with \\\\wsl$</span></span>
* <span data-ttu-id="19ca1-123">Standard umask in 0022 umschalten und File System. umask-Einstellung zu/etc/WSL.conf hinzufügen</span><span class="sxs-lookup"><span data-stu-id="19ca1-123">Switch default umask to 0022 and add filesystem.umask setting to /etc/wsl.conf</span></span>
* <span data-ttu-id="19ca1-124">Korrigieren von wslpath, um symlinks ordnungsgemäß aufzulösen, dies wurde in 19h1 zurückgegangen [GH 4078]</span><span class="sxs-lookup"><span data-stu-id="19ca1-124">Fix wslpath to properly resolve symlinks, this was regressed in 19h1 [GH 4078]</span></span>
* <span data-ttu-id="19ca1-125">Führen Sie die Datei "\\% User Profile%. wslconfig" für die Optimierung der WSL2-Einstellungen ein.</span><span class="sxs-lookup"><span data-stu-id="19ca1-125">Introduce %UserProfile%\\.wslconfig file for tweaking WSL2 settings</span></span>
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

## <a name="build-18917"></a><span data-ttu-id="19ca1-126">Build 18917</span><span class="sxs-lookup"><span data-stu-id="19ca1-126">Build 18917</span></span>
<span data-ttu-id="19ca1-127">Allgemeine Windows-Informationen zu Build 18917 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-127">For general Windows information on build 18917 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-128">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-128">WSL</span></span>
* <span data-ttu-id="19ca1-129">WSL 2 ist jetzt verfügbar!</span><span class="sxs-lookup"><span data-stu-id="19ca1-129">WSL 2 is now available!</span></span> <span data-ttu-id="19ca1-130">Weitere Informationen finden Sie im [Blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) .</span><span class="sxs-lookup"><span data-stu-id="19ca1-130">Please see [blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) for more details.</span></span>
* <span data-ttu-id="19ca1-131">Korrektur einer Regression, bei der das Starten von Windows-Prozessen über symlinks nicht ordnungsgemäß funktioniert hat [GH 3999]</span><span class="sxs-lookup"><span data-stu-id="19ca1-131">Fix a regression where launching Windows processes via symlinks did not work correctly [GH 3999]</span></span>
* <span data-ttu-id="19ca1-132">Fügen Sie die Optionen "WSL. exe--list--Verbose", "WSL. exe--list--quiet" und "WSL. exe--Import--Version" zu "WSL. exe" hinzu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-132">Add wsl.exe --list --verbose, wsl.exe --list --quiet, and wsl.exe --import --version options to wsl.exe</span></span>
* <span data-ttu-id="19ca1-133">Add WSL. exe--Option zum Herunterfahren</span><span class="sxs-lookup"><span data-stu-id="19ca1-133">Add wsl.exe --shutdown option</span></span>
* <span data-ttu-id="19ca1-134">Plan 9: Das Öffnen eines Verzeichnisses für einen erfolgreichen Schreibvorgang zulassen</span><span class="sxs-lookup"><span data-stu-id="19ca1-134">Plan 9: Allow opening a directory for write to succeed</span></span>

## <a name="build-18890"></a><span data-ttu-id="19ca1-135">Build 18890</span><span class="sxs-lookup"><span data-stu-id="19ca1-135">Build 18890</span></span>
<span data-ttu-id="19ca1-136">Allgemeine Windows-Informationen zu Build 18890 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-136">For general Windows information on build 18890 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-137">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-137">WSL</span></span>
* <span data-ttu-id="19ca1-138">Nicht blockierender socketleck [GH 2913]</span><span class="sxs-lookup"><span data-stu-id="19ca1-138">Non-blocking socket leak [GH 2913]</span></span>
* <span data-ttu-id="19ca1-139">EOF-Eingabe zum Terminal kann nachfolgende Lesevorgänge blockieren [GH 3421]</span><span class="sxs-lookup"><span data-stu-id="19ca1-139">EOF input to terminal can block subsequent reads [GH 3421]</span></span>
* <span data-ttu-id="19ca1-140">Aktualisieren Sie den resolv. conf-Header so, dass er auf WSL. conf verweist [in GH 3928 erläutert].</span><span class="sxs-lookup"><span data-stu-id="19ca1-140">Update resolv.conf header to refer to wsl.conf [discussed in GH 3928]</span></span>
* <span data-ttu-id="19ca1-141">Deadlock im epoll-Lösch Code [GH 3922]</span><span class="sxs-lookup"><span data-stu-id="19ca1-141">Deadlock in epoll delete code [GH 3922]</span></span>
* <span data-ttu-id="19ca1-142">Behandeln von Leerzeichen in Argumenten für "--Import" und "– Export" [GH 3932]</span><span class="sxs-lookup"><span data-stu-id="19ca1-142">Handle spaces in arguments to --import and –export [GH 3932]</span></span>
* <span data-ttu-id="19ca1-143">Erweitern von mmap-'d-Dateien funktioniert nicht ordnungsgemäß [GH 3939]</span><span class="sxs-lookup"><span data-stu-id="19ca1-143">Extending mmap’d files does not work properly [GH 3939]</span></span>
* <span data-ttu-id="19ca1-144">Beheben von Problemen mit \\ARM64 WSL $ Access funktioniert nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="19ca1-144">Fix issue with ARM64 \\wsl$ access not working properly</span></span>
* <span data-ttu-id="19ca1-145">Besseres Standard Symbol für "WSL. exe" hinzufügen</span><span class="sxs-lookup"><span data-stu-id="19ca1-145">Add better default icon for wsl.exe</span></span>

## <a name="build-18342"></a><span data-ttu-id="19ca1-146">Build 18342</span><span class="sxs-lookup"><span data-stu-id="19ca1-146">Build 18342</span></span>
<span data-ttu-id="19ca1-147">Allgemeine Windows-Informationen zu Build 18342 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-147">For general Windows information on build 18342 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-148">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-148">WSL</span></span>
* <span data-ttu-id="19ca1-149">Wir haben Benutzern die Möglichkeit hinzugefügt, auf Linux-Dateien in einer WSL-Distribution von Windows zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-149">We've added the ability for users to access Linux files in a WSL distro from Windows.</span></span> <span data-ttu-id="19ca1-150">Auf diese Dateien kann über die Befehlszeile zugegriffen werden. Außerdem können Windows-apps wie der Datei-Explorer, vscode usw. mit diesen Dateien interagieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-150">These files can be accessed through the command line, and also Windows apps, like file explorer, VSCode, etc. can interact with these files.</span></span> <span data-ttu-id="19ca1-151">Greifen Sie auf Ihre Dateien zu \\, indem Sie\\zu \\WSL $ < distro_name > navigieren, oder zeigen Sie eine Liste \\der laufenden Distributionen an, indem Sie zu \\WSL $ navigieren</span><span class="sxs-lookup"><span data-stu-id="19ca1-151">Access your files by navigating to \\\\wsl$\\<distro_name>, or see a list of running distributions by navigating to \\\\wsl$</span></span>
* <span data-ttu-id="19ca1-152">Hinzufügen zusätzlicher CPU-Infotags und korrigieren der Cpus_allowed [_list]-Werte [GH 2234]</span><span class="sxs-lookup"><span data-stu-id="19ca1-152">Add additional CPU info tags and fix Cpus_allowed[_list] values [GH 2234]</span></span>
* <span data-ttu-id="19ca1-153">Unterstützung von exec von einem nicht-führenden Thread [GH 3800]</span><span class="sxs-lookup"><span data-stu-id="19ca1-153">Support exec from non-leader thread [GH 3800]</span></span>
* <span data-ttu-id="19ca1-154">Behandeln von Fehlern bei der Konfigurations Aktualisierung als nicht schwerwiegend [GH 3785]</span><span class="sxs-lookup"><span data-stu-id="19ca1-154">Treat configuration update failures as non-fatal [GH 3785]</span></span>
* <span data-ttu-id="19ca1-155">Aktualisieren von binfmt, damit Offsets ordnungsgemäß behandelt werden [GH 3768]</span><span class="sxs-lookup"><span data-stu-id="19ca1-155">Update binfmt to properly handle offsets [GH 3768]</span></span>
* <span data-ttu-id="19ca1-156">Aktivieren der Zuordnung von Netzwerklaufwerken für Plan 9 [GH 3854]</span><span class="sxs-lookup"><span data-stu-id="19ca1-156">Enable mapping network drives for Plan 9 [GH 3854]</span></span>
* <span data-ttu-id="19ca1-157">Unterstützung von Windows-> Linux-und Linux-> Windows-Pfad Übersetzung für Bindungs Zustellungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-157">Support Windows -> Linux and Linux -> Windows path translation for bind mounts</span></span>
* <span data-ttu-id="19ca1-158">Erstellen Sie schreibgeschützte Abschnitte für Zuordnungen in Dateien, die schreibgeschützt geöffnet sind.</span><span class="sxs-lookup"><span data-stu-id="19ca1-158">Create read-only sections for mappings on files opened read-only</span></span>

## <a name="build-18334"></a><span data-ttu-id="19ca1-159">Build 18334</span><span class="sxs-lookup"><span data-stu-id="19ca1-159">Build 18334</span></span>
<span data-ttu-id="19ca1-160">Allgemeine Windows-Informationen zu Build 18334 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-160">For general Windows information on build 18334 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-161">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-161">WSL</span></span>
* <span data-ttu-id="19ca1-162">Umgestalten der Art und Weise, in der die Windows-Zeitzone einer Linux-Zeitzone zugeordnet ist [GH 3747]</span><span class="sxs-lookup"><span data-stu-id="19ca1-162">Redesign the way that Windows time zone is mapped to a  Linux time zone [GH 3747]</span></span>
* <span data-ttu-id="19ca1-163">Beheben von Speicher Verlusten und Hinzufügen neuer Zeichen folgen Übersetzungsfunktionen [GH 3746]</span><span class="sxs-lookup"><span data-stu-id="19ca1-163">Fix memory leaks and add new string translation functions [GH 3746]</span></span>
* <span data-ttu-id="19ca1-164">Sigmt für eine Thread Gruppe ohne Threads ist ein No-op [GH 3741]</span><span class="sxs-lookup"><span data-stu-id="19ca1-164">SIGCONT on a threadgroup with no threads is a no-op [GH 3741]</span></span> 
* <span data-ttu-id="19ca1-165">Korrekter Anzeige von Socket-und epoll-Dateideskriptoren in/proc/self/fd</span><span class="sxs-lookup"><span data-stu-id="19ca1-165">Correctly display socket and epoll file descriptors in /proc/self/fd</span></span>

## <a name="build-18305"></a><span data-ttu-id="19ca1-166">Build 18305</span><span class="sxs-lookup"><span data-stu-id="19ca1-166">Build 18305</span></span>
<span data-ttu-id="19ca1-167">Allgemeine Windows-Informationen zu Build 18305 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-167">For general Windows information on build 18305 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-168">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-168">WSL</span></span>
* <span data-ttu-id="19ca1-169">pthreads verlieren den Zugriff auf Dateien, wenn der primäre Thread beendet wird [GH 3589]</span><span class="sxs-lookup"><span data-stu-id="19ca1-169">pthreads lose access to files when the primary thread exits [GH 3589]</span></span>
* <span data-ttu-id="19ca1-170">"Tiocsctty" sollte den "Force"-Parameter ignorieren, es sei denn, er ist erforderlich [GH 3652]</span><span class="sxs-lookup"><span data-stu-id="19ca1-170">TIOCSCTTY should ignore the “force” parameter unless it is required [GH 3652]</span></span>
* <span data-ttu-id="19ca1-171">Verbesserungen an der Befehlszeile von WSL. exe und zusätzliche Import-/Exportfunktionen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-171">wsl.exe command line improvements and addition of import / export functionality.</span></span>
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

## <a name="build-18277"></a><span data-ttu-id="19ca1-172">Build 18277</span><span class="sxs-lookup"><span data-stu-id="19ca1-172">Build 18277</span></span>
<span data-ttu-id="19ca1-173">Allgemeine Windows-Informationen zu Build 18277 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-173">For general Windows information on build 18277 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-174">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-174">WSL</span></span>
* <span data-ttu-id="19ca1-175">Fehlerbehebung "keine solche Schnittstelle unterstützt" in Build 18272 [GH 3645] eingeführt</span><span class="sxs-lookup"><span data-stu-id="19ca1-175">Fix "no such interface supported" error introduced in build 18272 [GH 3645]</span></span>
* <span data-ttu-id="19ca1-176">MNT_FORCE-Flag für aufheben syscall ignorieren [GH 3605]</span><span class="sxs-lookup"><span data-stu-id="19ca1-176">Ignore the MNT_FORCE flag for umount syscall [GH 3605]</span></span>
* <span data-ttu-id="19ca1-177">Wechseln von WSL-Interop zur Verwendung der offiziellen "deepseudoconsole"-API</span><span class="sxs-lookup"><span data-stu-id="19ca1-177">Switch WSL interop to use the official CreatePseudoConsole API</span></span>
* <span data-ttu-id="19ca1-178">Keinen Timeout Wert beibehalten, wenn FUTEX_WAIT neu gestartet wird</span><span class="sxs-lookup"><span data-stu-id="19ca1-178">Maintain no timeout value when FUTEX_WAIT restarts</span></span>

## <a name="build-18272"></a><span data-ttu-id="19ca1-179">Build 18272</span><span class="sxs-lookup"><span data-stu-id="19ca1-179">Build 18272</span></span>
<span data-ttu-id="19ca1-180">Allgemeine Windows-Informationen zu Build 18272 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-180">For general Windows information on build 18272 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-181">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-181">WSL</span></span>
* <span data-ttu-id="19ca1-182">**DAVOR** In diesem Build ist ein Problem aufgetreten, das WSL als nicht funktionsfähig macht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-182">**WARNING:** There is an issue in this build that makes WSL inoperable.</span></span> <span data-ttu-id="19ca1-183">Wenn Sie versuchen, die Distribution zu starten, wird die Fehlermeldung "Es wird keine solche Schnittstelle unterstützt" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-183">When trying to launch your distribution you will see a “No such interface supported” error.</span></span> <span data-ttu-id="19ca1-184">Das Problem wurde behoben und ist der Insider-schnell Build der nächsten Woche.</span><span class="sxs-lookup"><span data-stu-id="19ca1-184">The issue has been fixed and will be in next week's Insider Fast build.</span></span> <span data-ttu-id="19ca1-185">Wenn Sie diesen Build installiert haben, können Sie ein Rollback auf den vorherigen Windows-Build durchführen, indem Sie unter "Einstellungen-> Update & Sicherheit > Wiederherstellung" zurück zur vorherigen Version von Windows 10 wechseln.</span><span class="sxs-lookup"><span data-stu-id="19ca1-185">If you've installed this build you can roll back to the previous Windows build using “Go back to the previous version of Windows 10” in Settings->Update & Security->Recovery.</span></span>

## <a name="build-18267"></a><span data-ttu-id="19ca1-186">Build 18267</span><span class="sxs-lookup"><span data-stu-id="19ca1-186">Build 18267</span></span>
<span data-ttu-id="19ca1-187">Allgemeine Windows-Informationen zu Build 18267 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-187">For general Windows information on build 18267 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-188">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-188">WSL</span></span>
* <span data-ttu-id="19ca1-189">Behebung eines Problems, bei dem der Zombie Prozess möglicherweise nicht wiederholt wird und unbegrenzt bleibt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-189">Fix issue where zombie process may not be reaped and remain indefinitely.</span></span>
* <span data-ttu-id="19ca1-190">Wslregisterdistribution hängt ab, wenn die Fehlermeldung die maximale Länge überschreitet [GH 3592]</span><span class="sxs-lookup"><span data-stu-id="19ca1-190">WslRegisterDistribution hangs if error message exceeds max length [GH 3592]</span></span>
* <span data-ttu-id="19ca1-191">Zulassen der erfolgreichen Ausführung von fsync für schreibgeschützte Dateien auf drvfs [GH 3556]</span><span class="sxs-lookup"><span data-stu-id="19ca1-191">Allow fsync to succeed for read-only files on DrvFs [GH 3556]</span></span>
* <span data-ttu-id="19ca1-192">Stellen Sie sicher, dass die Verzeichnisse "/bin" und/sbin vorhanden sind, bevor Sie symlinks in [GH 3584] erstellen</span><span class="sxs-lookup"><span data-stu-id="19ca1-192">Ensure that /bin and /sbin directories exist before creating symlinks inside [GH 3584]</span></span>
* <span data-ttu-id="19ca1-193">Es wurde ein Timeout Mechanismus für Instanzen Beendigung für WSL-Instanzen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-193">Added an instance termination timeout mechanism for WSL instances.</span></span> <span data-ttu-id="19ca1-194">Der Timeout Wert ist derzeit auf 15 Sekunden festgelegt. das bedeutet, dass die Instanz 15 Sekunden nach Beendigung des letzten WSL-Prozesses beendet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-194">The timeout is currently set to 15 seconds, meaning the instance will terminate 15 seconds after the last WSL process exits.</span></span> <span data-ttu-id="19ca1-195">Um eine Verteilung sofort zu beenden, verwenden Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="19ca1-195">To terminate a distribution immediately, use:</span></span>
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a><span data-ttu-id="19ca1-196">Build 17763 (1809)</span><span class="sxs-lookup"><span data-stu-id="19ca1-196">Build 17763 (1809)</span></span>
<span data-ttu-id="19ca1-197">Allgemeine Windows-Informationen zu Build 17763 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-197">For general Windows information on build 17763 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-198">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-198">WSL</span></span>
* <span data-ttu-id="19ca1-199">Die SetPriority-syscall-Berechtigung zum Ändern der gleichen Thread Priorität ist zu streng. [GH 1838]</span><span class="sxs-lookup"><span data-stu-id="19ca1-199">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="19ca1-200">Stellen Sie sicher, dass eine unausgewogene Interruptzeit für die Startzeit verwendet wird, um die Rückgabe negativer Werte für clock_gettime (CLOCK_BOOTTIME) zu vermeiden. [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="19ca1-200">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="19ca1-201">Behandeln von Symlinks im WSL binf-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="19ca1-201">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="19ca1-202">Bessere Behandlung der Bereinigung der Thread Gruppen-Dateideskriptoren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-202">Better handling of threadgroup leader file descriptor cleanup.</span></span>
* <span data-ttu-id="19ca1-203">Wechseln von WSL zur Verwendung von kequeryinterrupttimepräzisen anstelle von KeQueryPerformanceCounter, um einen Überlauf zu vermeiden [GH 3252]</span><span class="sxs-lookup"><span data-stu-id="19ca1-203">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="19ca1-204">Ptrace-Anfüge Vorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="19ca1-204">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="19ca1-205">Beheben mehrerer AF_UNIX bezogener Probleme [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="19ca1-205">Fix several AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="19ca1-206">Behebung eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="19ca1-206">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>
* <span data-ttu-id="19ca1-207">Vermeiden einer Sekunde verzögert fehlerhafte Loopback Verbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="19ca1-207">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="19ca1-208">/Proc/sys/FS/File-Max Stub-Datei hinzufügen [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="19ca1-208">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="19ca1-209">Genauere IPv6-Bereichs Informationen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-209">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="19ca1-210">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="19ca1-210">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="19ca1-211">Pipe-Dateisystem versehentlich Löschen eines Edge-ausgelösten epoll-Ereignisses [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="19ca1-211">Pipe filesystem inadvertently clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="19ca1-212">Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen</span><span class="sxs-lookup"><span data-stu-id="19ca1-212">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>
* <span data-ttu-id="19ca1-213">Verbesserte Zombie Unterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="19ca1-213">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="19ca1-214">Hinzufügen von WSL. conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="19ca1-214">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="19ca1-215">Behebung für "getsockname" gibt nicht immer den UNIX-socketfamilientyp [GH 1774] zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-215">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="19ca1-216">Hinzufügen von Unterstützung für tiocsti [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="19ca1-216">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="19ca1-217">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche "eagain" zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="19ca1-217">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="19ca1-218">Unterstützung von Interop auf bereitgestellten VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="19ca1-218">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="19ca1-219">Beheben von Problemen mit der Berechtigungsüberprüfung im Stamm Ordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="19ca1-219">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="19ca1-220">Eingeschränkte Unterstützung für die TTY-Tastatur IOCTLs kdgkbtype, kdgkbmode und kdskbmode.</span><span class="sxs-lookup"><span data-stu-id="19ca1-220">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="19ca1-221">Windows-Benutzeroberflächen-apps sollten ausgeführt werden, auch wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-221">Windows UI apps should execute even when launched in the background.</span></span>
* <span data-ttu-id="19ca1-222">Add WSL-u oder--User-Option [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="19ca1-222">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="19ca1-223">Beheben von WSL-Startproblemen, wenn der schnelle Start aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="19ca1-223">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="19ca1-224">Unix-Sockets müssen getrennte Peer-Anmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="19ca1-224">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="19ca1-225">Nicht blockierende Unix-Sockets, die unbegrenzt mit eagain auftreten [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="19ca1-225">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="19ca1-226">Case = off ist der neue standardmäßige drvfs-Einstellungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="19ca1-226">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="19ca1-227">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) .</span><span class="sxs-lookup"><span data-stu-id="19ca1-227">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="19ca1-228">Fügen Sie wslconfig/Terminate hinzu, um die Ausführung von Verteilungen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="19ca1-228">Add wslconfig /terminate to stop running distributions.</span></span>
* <span data-ttu-id="19ca1-229">Beheben Sie das Problem mit den Kontextmenü Einträgen von WSL Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="19ca1-229">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="19ca1-230">Stellen Sie die Groß-/Kleinschreibung nach Verzeichnis als erweitertes Attribut bereit.</span><span class="sxs-lookup"><span data-stu-id="19ca1-230">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="19ca1-231">ARM64 Emulieren von Cache Wartungs Vorgängen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-231">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="19ca1-232">Beheben von [dotnet-Problemen](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="19ca1-232">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="19ca1-233">Drvfs: nur Escapezeichen im privaten Bereich, die einem Escapezeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-233">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>
* <span data-ttu-id="19ca1-234">Fehlerbehebung bei einem Fehler in der Überprüfung der Länge des elf-parserinterpreters [GH 3154]</span><span class="sxs-lookup"><span data-stu-id="19ca1-234">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="19ca1-235">Absolute WSL-Timer mit einer Zeit in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="19ca1-235">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="19ca1-236">Stellen Sie sicher, dass neu erstellte Analyse Punkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-236">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="19ca1-237">Erstellen Sie in drvfs atomarisch Fälle mit Berücksichtigung von Groß-und klein</span><span class="sxs-lookup"><span data-stu-id="19ca1-237">Atomically create case sensitive directories in DrvFs.</span></span>
* <span data-ttu-id="19ca1-238">Es wurde ein zusätzliches Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-238">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="19ca1-239">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="19ca1-239">[GH 2712]</span></span>
* <span data-ttu-id="19ca1-240">Fehler beim Starten des WSL-Starts, wenn die Option "-Konfigurations-</span><span class="sxs-lookup"><span data-stu-id="19ca1-240">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="19ca1-241">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="19ca1-241">[GH 3020]</span></span>
* <span data-ttu-id="19ca1-242">Fügen Sie den Explorer-Kontextmenü zum Starten von WSL [GH 437, 603, 1836] hinzu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-242">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="19ca1-243">Halten Sie die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, wenn Sie in einem Explorer-Fenster</span><span class="sxs-lookup"><span data-stu-id="19ca1-243">To use, hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="19ca1-244">Korrigieren des nicht blockierenden UNIX-socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="19ca1-244">Fix Unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="19ca1-245">Korrigieren Sie den hängenden NetLink-Befehl, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-245">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="19ca1-246">Unterstützung für einstellungsweitergabeflags [GH 2911] hinzufügen</span><span class="sxs-lookup"><span data-stu-id="19ca1-246">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="19ca1-247">Beheben von Problemen mit TRUNCATE, die keine inotify-Ereignisse verursachen [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="19ca1-247">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="19ca1-248">Fügen Sie die Option "--exec" für WSL. exe ein, um eine einzelne Binärdatei ohne Shell aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-248">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="19ca1-249">Fügen Sie die Option "--Distribution" für "WSL. exe" hinzu, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-249">Add --distribution option for wsl.exe to select a specific distro.</span></span>
* <span data-ttu-id="19ca1-250">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="19ca1-250">Limited support for dmesg.</span></span> <span data-ttu-id="19ca1-251">Anwendungen können sich jetzt an dmesg anmelden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-251">Applications can now log to dmesg.</span></span> <span data-ttu-id="19ca1-252">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="19ca1-252">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="19ca1-253">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnosen vom Treiber übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-253">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="19ca1-254">Hinweis: dmesg wird derzeit über die `/dev/kmsg` Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-254">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="19ca1-255">`syslog`Die syscall-Schnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-255">`syslog` syscall interface is not yet supported.</span></span> <span data-ttu-id="19ca1-256">Und daher funktionieren einige `dmesg` der Befehlszeilenoptionen `-S`, wie z. b `-C` ., nicht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-256">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="19ca1-257">Ändern der Standard-gid und des Modus von seriellen Geräten entsprechend der systemeigenen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="19ca1-257">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="19ca1-258">Drvfs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="19ca1-258">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="19ca1-259">Hinweis: Bei drvfs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="19ca1-259">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="19ca1-260">Einige Zeichen (z. b. "/", ":\*" und "") sind nicht zulässig, und erweiterte Attributnamen werden bei drvfs nicht groß-und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-260">Some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-18252-skip-ahead"></a><span data-ttu-id="19ca1-261">Build 18252 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-261">Build 18252 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-262">Allgemeine Windows-Informationen zu Build 18252 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-262">For general Windows information on build 18252 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-263">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-263">WSL</span></span>
* <span data-ttu-id="19ca1-264">Verschieben von init-und bsdtar-Binärdateien aus der lxssmanager-dll und in einen separaten Tool Ordner</span><span class="sxs-lookup"><span data-stu-id="19ca1-264">Move init and bsdtar binaries out of lxssmanager dll and into a separate tools folder</span></span>
* <span data-ttu-id="19ca1-265">Korrektur des raceumschließens des Datei Deskriptors bei Verwendung von CLONE_FILES</span><span class="sxs-lookup"><span data-stu-id="19ca1-265">Fix race around closing file descriptor when using CLONE_FILES</span></span>
* <span data-ttu-id="19ca1-266">Behandeln optionaler Felder in/proc/PID/mountinfo bei der Übersetzung von drvfs-Pfaden</span><span class="sxs-lookup"><span data-stu-id="19ca1-266">Handle optional fields in /proc/pid/mountinfo when translating DrvFs paths</span></span>
* <span data-ttu-id="19ca1-267">Zulassen, dass drvfs-mklod ohne Metadatenunterstützung für S_IFREG erfolgreich ist</span><span class="sxs-lookup"><span data-stu-id="19ca1-267">Allow DrvFs mknod to succeed without metadata support for S_IFREG</span></span>
* <span data-ttu-id="19ca1-268">Für schreibgeschützte Dateien, die auf drvfs erstellt wurden, muss das schreibgeschützte Attribut festgelegt werden [GH 3411]</span><span class="sxs-lookup"><span data-stu-id="19ca1-268">Readonly files created on DrvFs should have the readonly attribute set [GH 3411]</span></span>
* <span data-ttu-id="19ca1-269">Hinzufügen von/sbin/mount.drvfs Helper zur Behandlung der drvfs-Einbindung</span><span class="sxs-lookup"><span data-stu-id="19ca1-269">Add /sbin/mount.drvfs helper to handle DrvFs mounting</span></span>
* <span data-ttu-id="19ca1-270">Verwenden Sie die POSIX-Umbenennung in drvfs.</span><span class="sxs-lookup"><span data-stu-id="19ca1-270">Use POSIX rename in DrvFs.</span></span>
* <span data-ttu-id="19ca1-271">Ermöglicht die Pfad Übersetzung auf Volumes ohne Volume-GUID.</span><span class="sxs-lookup"><span data-stu-id="19ca1-271">Allow path translation on volumes without a volume GUID.</span></span>

## <a name="build-17738-fast"></a><span data-ttu-id="19ca1-272">Build 17738 (fast)</span><span class="sxs-lookup"><span data-stu-id="19ca1-272">Build 17738 (Fast)</span></span>
<span data-ttu-id="19ca1-273">Allgemeine Windows-Informationen zu Build 17738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-273">For general Windows information on build 17738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-274">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-274">WSL</span></span>
* <span data-ttu-id="19ca1-275">Die SetPriority-syscall-Berechtigung zum Ändern der gleichen Thread Priorität ist zu streng. [GH 1838]</span><span class="sxs-lookup"><span data-stu-id="19ca1-275">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="19ca1-276">Stellen Sie sicher, dass eine unausgewogene Interruptzeit für die Startzeit verwendet wird, um die Rückgabe negativer Werte für clock_gettime (CLOCK_BOOTTIME) zu vermeiden. [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="19ca1-276">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="19ca1-277">Behandeln von Symlinks im WSL binf-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="19ca1-277">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="19ca1-278">Bessere Behandlung der Bereinigung der Thread Gruppen-Dateideskriptoren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-278">Better handling of threadgroup leader file descriptor cleanup.</span></span>

## <a name="build-17728-fast"></a><span data-ttu-id="19ca1-279">Build 17728 (fast)</span><span class="sxs-lookup"><span data-stu-id="19ca1-279">Build 17728 (Fast)</span></span>
<span data-ttu-id="19ca1-280">Allgemeine Windows-Informationen zu Build 17728 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-280">For general Windows information on build 17728 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-281">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-281">WSL</span></span>
* <span data-ttu-id="19ca1-282">Wechseln von WSL zur Verwendung von kequeryinterrupttimepräzisen anstelle von KeQueryPerformanceCounter, um einen Überlauf zu vermeiden [GH 3252]</span><span class="sxs-lookup"><span data-stu-id="19ca1-282">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="19ca1-283">Ptrace-Anfüge Vorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="19ca1-283">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="19ca1-284">Beheben einer Reihe von AF_UNIX-bezogenen Problemen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="19ca1-284">Fix a number of AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="19ca1-285">Behebung eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="19ca1-285">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>

## <a name="build-18204-skip-ahead"></a><span data-ttu-id="19ca1-286">Build 18204 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-286">Build 18204 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-287">Allgemeine Windows-Informationen zu Build 18204 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-287">For general Windows information on build 18204 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-288">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-288">WSL</span></span>
* <span data-ttu-id="19ca1-289">Pipe-Dateisystem versehentlich löschen von Edge-ausgelösten epoll-Ereignissen [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="19ca1-289">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="19ca1-290">Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen</span><span class="sxs-lookup"><span data-stu-id="19ca1-290">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17723-fast"></a><span data-ttu-id="19ca1-291">Build 17723 (fast)</span><span class="sxs-lookup"><span data-stu-id="19ca1-291">Build 17723 (Fast)</span></span>
<span data-ttu-id="19ca1-292">Allgemeine Windows-Informationen zu Build 17723 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-292">For general Windows information on build 17723 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-293">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-293">WSL</span></span>
* <span data-ttu-id="19ca1-294">Vermeiden einer Sekunde verzögert fehlerhafte Loopback Verbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="19ca1-294">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="19ca1-295">/Proc/sys/FS/File-Max Stub-Datei hinzufügen [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="19ca1-295">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="19ca1-296">Genauere IPv6-Bereichs Informationen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-296">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="19ca1-297">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="19ca1-297">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="19ca1-298">Pipe-Dateisystem versehentlich löschen von Edge-ausgelösten epoll-Ereignissen [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="19ca1-298">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="19ca1-299">Die ausführbare Win32-Datei, die über den NTFS-Symlink gestartet wurde, respektiert den symlink2909 Namen</span><span class="sxs-lookup"><span data-stu-id="19ca1-299">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17713"></a><span data-ttu-id="19ca1-300">Build 17713</span><span class="sxs-lookup"><span data-stu-id="19ca1-300">Build 17713</span></span>
<span data-ttu-id="19ca1-301">Allgemeine Windows-Informationen zu Build 17713 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-301">For general Windows information on build 17713 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-302">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-302">WSL</span></span>
* <span data-ttu-id="19ca1-303">Verbesserte Zombie Unterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="19ca1-303">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="19ca1-304">Hinzufügen von WSL. conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="19ca1-304">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="19ca1-305">Behebung für "getsockname" gibt nicht immer den UNIX-socketfamilientyp [GH 1774] zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-305">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="19ca1-306">Hinzufügen von Unterstützung für tiocsti [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="19ca1-306">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="19ca1-307">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche "eagain" zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="19ca1-307">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="19ca1-308">Unterstützung von Interop auf bereitgestellten VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="19ca1-308">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="19ca1-309">Beheben von Problemen mit der Berechtigungsüberprüfung im Stamm Ordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="19ca1-309">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="19ca1-310">Eingeschränkte Unterstützung für die TTY-Tastatur IOCTLs kdgkbtype, kdgkbmode und kdskbmode.</span><span class="sxs-lookup"><span data-stu-id="19ca1-310">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="19ca1-311">Windows-Benutzeroberflächen-apps sollten ausgeführt werden, auch wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-311">Windows UI apps should execute even when launched in the background.</span></span>

## <a name="build-17704"></a><span data-ttu-id="19ca1-312">Build 17704</span><span class="sxs-lookup"><span data-stu-id="19ca1-312">Build 17704</span></span>
<span data-ttu-id="19ca1-313">Allgemeine Windows-Informationen zu Build 17704 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-313">For general Windows information on build 17704 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-314">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-314">WSL</span></span>
* <span data-ttu-id="19ca1-315">Add WSL-u oder--User-Option [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="19ca1-315">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="19ca1-316">Beheben von WSL-Startproblemen, wenn der schnelle Start aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="19ca1-316">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="19ca1-317">Unix-Sockets müssen getrennte Peer-Anmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="19ca1-317">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="19ca1-318">Nicht blockierende Unix-Sockets, die unbegrenzt mit eagain auftreten [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="19ca1-318">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="19ca1-319">Case = off ist der neue standardmäßige drvfs-Einstellungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="19ca1-319">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="19ca1-320">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) .</span><span class="sxs-lookup"><span data-stu-id="19ca1-320">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="19ca1-321">Fügen Sie wslconfig/Terminate hinzu, um die Ausführung von Verteilungen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="19ca1-321">Add wslconfig /terminate to stop running distributions.</span></span>

## <a name="build-17692"></a><span data-ttu-id="19ca1-322">Build 17692</span><span class="sxs-lookup"><span data-stu-id="19ca1-322">Build 17692</span></span>
<span data-ttu-id="19ca1-323">Allgemeine Windows-Informationen zu Build 17692 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span><span class="sxs-lookup"><span data-stu-id="19ca1-323">For general Windows information on build 17692 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-324">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-324">WSL</span></span>
* <span data-ttu-id="19ca1-325">Beheben Sie das Problem mit den Kontextmenü Einträgen von WSL Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="19ca1-325">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="19ca1-326">Stellen Sie die Groß-/Kleinschreibung nach Verzeichnis als erweitertes Attribut bereit.</span><span class="sxs-lookup"><span data-stu-id="19ca1-326">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="19ca1-327">ARM64 Emulieren von Cache Wartungs Vorgängen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-327">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="19ca1-328">Beheben von [dotnet-Problemen](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="19ca1-328">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="19ca1-329">Drvfs: nur Escapezeichen im privaten Bereich, die einem Escapezeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-329">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>

## <a name="build-17686"></a><span data-ttu-id="19ca1-330">Build 17686</span><span class="sxs-lookup"><span data-stu-id="19ca1-330">Build 17686</span></span>
<span data-ttu-id="19ca1-331">Allgemeine Windows-Informationen zu Build 17686 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span><span class="sxs-lookup"><span data-stu-id="19ca1-331">For general Windows information on build 17686 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-332">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-332">WSL</span></span>
* <span data-ttu-id="19ca1-333">Fehlerbehebung bei einem Fehler in der Überprüfung der Länge des elf-parserinterpreters [GH 3154]</span><span class="sxs-lookup"><span data-stu-id="19ca1-333">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="19ca1-334">Absolute WSL-Timer mit einer Zeit in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="19ca1-334">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="19ca1-335">Stellen Sie sicher, dass neu erstellte Analyse Punkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-335">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="19ca1-336">Erstellen Sie in drvfs atomarisch Fälle mit Berücksichtigung von Groß-und klein</span><span class="sxs-lookup"><span data-stu-id="19ca1-336">Atomically create case sensitive directories in DrvFs.</span></span>

## <a name="build-17677"></a><span data-ttu-id="19ca1-337">Build 17677</span><span class="sxs-lookup"><span data-stu-id="19ca1-337">Build 17677</span></span>
<span data-ttu-id="19ca1-338">Allgemeine Windows-Informationen zu Build 17677 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-338">For general Windows information on build 17677 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-339">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-339">WSL</span></span>
* <span data-ttu-id="19ca1-340">Es wurde ein zusätzliches Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-340">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="19ca1-341">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="19ca1-341">[GH 2712]</span></span>
* <span data-ttu-id="19ca1-342">Fehler beim Starten des WSL-Starts, wenn die Option "-Konfigurations-</span><span class="sxs-lookup"><span data-stu-id="19ca1-342">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="19ca1-343">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="19ca1-343">[GH 3020]</span></span>

## <a name="build-17666"></a><span data-ttu-id="19ca1-344">Build 17666</span><span class="sxs-lookup"><span data-stu-id="19ca1-344">Build 17666</span></span>
<span data-ttu-id="19ca1-345">Allgemeine Windows-Informationen zu Build 17666 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-345">For general Windows information on build 17666 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-346">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-346">WSL</span></span>
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a><span data-ttu-id="19ca1-347">WARNUNG: Es gibt ein Problem, das das Ausführen von WSL in einigen AMD-Chipsätzen [GH 3134] verhindert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-347">WARNING: There is an issue preventing WSL from running on some AMD chipsets [GH 3134].</span></span> <span data-ttu-id="19ca1-348">Ein Fix ist bereit und stellt den Insider-Build-Branch dar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-348">A fix is ready and making its way to the Insider Build branch.</span></span>
* <span data-ttu-id="19ca1-349">Fügen Sie den Explorer-Kontextmenü zum Starten von WSL [GH 437, 603, 1836] hinzu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-349">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="19ca1-350">, Wenn Sie die Halt-Umschalttaste verwenden möchten, und klicken Sie mit der rechten Maustaste auf den</span><span class="sxs-lookup"><span data-stu-id="19ca1-350">To use hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="19ca1-351">Korrigieren des nicht blockierenden UNIX-socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="19ca1-351">Fix unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="19ca1-352">Korrigieren Sie den hängenden NetLink-Befehl, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-352">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="19ca1-353">Unterstützung für einstellungsweitergabeflags [GH 2911] hinzufügen</span><span class="sxs-lookup"><span data-stu-id="19ca1-353">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="19ca1-354">Beheben von Problemen mit TRUNCATE, die keine inotify-Ereignisse verursachen [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="19ca1-354">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="19ca1-355">Fügen Sie die Option "--exec" für WSL. exe ein, um eine einzelne Binärdatei ohne Shell aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-355">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="19ca1-356">Fügen Sie die Option "--Distribution" für "WSL. exe" hinzu, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-356">Add --distribution option for wsl.exe to select a specific distro.</span></span>

## <a name="build-17655-skip-ahead"></a><span data-ttu-id="19ca1-357">Build 17655 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-357">Build 17655 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-358">Allgemeine Windows-Informationen zu Build 17655 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-358">For general Windows information on build 17655 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-359">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-359">WSL</span></span>
* <span data-ttu-id="19ca1-360">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="19ca1-360">Limited support for dmesg.</span></span> <span data-ttu-id="19ca1-361">Anwendungen können sich jetzt an dmesg anmelden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-361">Applications can now log to dmesg.</span></span> <span data-ttu-id="19ca1-362">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="19ca1-362">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="19ca1-363">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnosen vom Treiber übertragen werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-363">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="19ca1-364">Hinweis: dmesg wird derzeit über die `/dev/kmsg` Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-364">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="19ca1-365">`syslog`die sycallcenter-Schnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-365">`syslog` sycall interface is not yet supported.</span></span> <span data-ttu-id="19ca1-366">Und daher funktionieren einige `dmesg` der Befehlszeilenoptionen `-S`, wie z. b `-C` ., nicht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-366">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="19ca1-367">Es wurde ein Problem behoben, bei dem Multithread-Vorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-367">Fixed an issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="19ca1-368">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="19ca1-368">[GH 2712]</span></span>

## <a name="build-17639-skip-ahead"></a><span data-ttu-id="19ca1-369">Build 17639 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-369">Build 17639 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-370">Allgemeine Windows-Informationen zu Build 17639 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-370">For general Windows information on build 17639 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-371">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-371">WSL</span></span>
* <span data-ttu-id="19ca1-372">Ändern der Standard-gid und des Modus von seriellen Geräten entsprechend der systemeigenen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="19ca1-372">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="19ca1-373">Drvfs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="19ca1-373">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="19ca1-374">Hinweis: Bei drvfs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="19ca1-374">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="19ca1-375">Bestimmte Zeichen (z. b. "/", ":" und "\*") sind nicht zulässig, und erweiterte Attributnamen werden bei drvfs nicht Groß-/Kleinschreibung unterschieden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-375">In particular, some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-17133-fast"></a><span data-ttu-id="19ca1-376">Build 17133 (fast)</span><span class="sxs-lookup"><span data-stu-id="19ca1-376">Build 17133 (Fast)</span></span>
<span data-ttu-id="19ca1-377">Allgemeine Windows-Informationen zu Build 17133 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-377">For general Windows information on build 17133 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-378">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-378">WSL</span></span>
* <span data-ttu-id="19ca1-379">Fehlerbehebung für den Absturz in WSL.</span><span class="sxs-lookup"><span data-stu-id="19ca1-379">Fix for hang in WSL.</span></span> <span data-ttu-id="19ca1-380">[GH 3039, 3034]</span><span class="sxs-lookup"><span data-stu-id="19ca1-380">[GH 3039, 3034]</span></span>

## <a name="build-17128-fast"></a><span data-ttu-id="19ca1-381">Build 17128 (fast)</span><span class="sxs-lookup"><span data-stu-id="19ca1-381">Build 17128 (Fast)</span></span>
<span data-ttu-id="19ca1-382">Allgemeine Windows-Informationen zu Build 17128 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-382">For general Windows information on build 17128 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-383">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-383">WSL</span></span>
* <span data-ttu-id="19ca1-384">None</span><span class="sxs-lookup"><span data-stu-id="19ca1-384">None</span></span>

## <a name="build-17627-skip-ahead"></a><span data-ttu-id="19ca1-385">Build 17627 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-385">Build 17627 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-386">Allgemeine Windows-Informationen zu Build 17627 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-386">For general Windows information on build 17627 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-387">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-387">WSL</span></span>
* <span data-ttu-id="19ca1-388">Unterstützung für die Futex-Pi-fähigen Vorgänge hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-388">Add support for the futex pi-aware operations.</span></span> <span data-ttu-id="19ca1-389">[GH 1006]</span><span class="sxs-lookup"><span data-stu-id="19ca1-389">[GH 1006]</span></span>
    * <span data-ttu-id="19ca1-390">Beachten Sie, dass es sich bei den Prioritäten derzeit nicht um eine unterstützte WSL-Funktion handelt, sodass die Blockierung der Standard Auslastung aufgehoben werden muss.</span><span class="sxs-lookup"><span data-stu-id="19ca1-390">Note that priorities are not currently a supported WSL feature so there are limitations, but standard usage should be unblocked.</span></span>
* <span data-ttu-id="19ca1-391">Windows-Firewall-Unterstützung für WSL-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="19ca1-391">Windows firewall support for WSL processes.</span></span> <span data-ttu-id="19ca1-392">[GH 1852]</span><span class="sxs-lookup"><span data-stu-id="19ca1-392">[GH 1852]</span></span>
    * <span data-ttu-id="19ca1-393">Um beispielsweise zuzulassen, dass der WSL-python-Prozess an einem beliebigen Port lauschen kann, verwenden Sie das Windows-cmd mit erhöhten Rechten:```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span><span class="sxs-lookup"><span data-stu-id="19ca1-393">For example, to allow the WSL python process to listen on any port, use the elevated Windows cmd: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span></span>
    * <span data-ttu-id="19ca1-394">Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span><span class="sxs-lookup"><span data-stu-id="19ca1-394">For additional details on how to add firewall rules, see [link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span></span>
* <span data-ttu-id="19ca1-395">Beachten Sie die Standardshell des Benutzers bei der Verwendung von WSL. exe.</span><span class="sxs-lookup"><span data-stu-id="19ca1-395">Respect user's default shell when using wsl.exe.</span></span> <span data-ttu-id="19ca1-396">[GH 2372]</span><span class="sxs-lookup"><span data-stu-id="19ca1-396">[GH 2372]</span></span>
* <span data-ttu-id="19ca1-397">Alle Netzwerkschnittstellen als Ethernet melden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-397">Report all network interfaces as ethernet.</span></span> <span data-ttu-id="19ca1-398">[GH 2996]</span><span class="sxs-lookup"><span data-stu-id="19ca1-398">[GH 2996]</span></span>
* <span data-ttu-id="19ca1-399">Bessere Behandlung von beschädigten "/etc/passwd"-Dateien.</span><span class="sxs-lookup"><span data-stu-id="19ca1-399">Better handling of corrupt /etc/passwd file.</span></span> <span data-ttu-id="19ca1-400">[GH 3001]</span><span class="sxs-lookup"><span data-stu-id="19ca1-400">[GH 3001]</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-401">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-401">Console</span></span>
* <span data-ttu-id="19ca1-402">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-402">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-403">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-403">LTP Results:</span></span>
<span data-ttu-id="19ca1-404">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-404">Testing in progress.</span></span>

## <a name="build-17618-skip-ahead"></a><span data-ttu-id="19ca1-405">Build 17618 (überspringen)</span><span class="sxs-lookup"><span data-stu-id="19ca1-405">Build 17618 (Skip Ahead)</span></span>
<span data-ttu-id="19ca1-406">Allgemeine Windows-Informationen zu Build 17618 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-406">For general Windows information on build 17618 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-407">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-407">WSL</span></span>
* <span data-ttu-id="19ca1-408">Einführung in pseudoconsole-Funktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span><span class="sxs-lookup"><span data-stu-id="19ca1-408">Introduce pseudoconsole functionality for NT interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span></span>
* <span data-ttu-id="19ca1-409">Der Legacy Installationsmechanismus (lxrun. exe) ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-409">The legacy install mechanism (lxrun.exe) has been deprecated.</span></span> <span data-ttu-id="19ca1-410">Der unterstützte Mechanismus zum Installieren von Verteilungen ist die Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="19ca1-410">The supported mechanism for installing distributions is through the Microsoft Store.</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-411">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-411">Console</span></span>
* <span data-ttu-id="19ca1-412">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-412">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-413">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-413">LTP Results:</span></span>
<span data-ttu-id="19ca1-414">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-414">Testing in progress.</span></span>

## <a name="build-17110"></a><span data-ttu-id="19ca1-415">Build 17110</span><span class="sxs-lookup"><span data-stu-id="19ca1-415">Build 17110</span></span>
<span data-ttu-id="19ca1-416">Allgemeine Windows-Informationen zu Build 17110 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-416">For general Windows information on build 17110 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-417">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-417">WSL</span></span>
* <span data-ttu-id="19ca1-418">Zulassen, dass/init von Windows [GH 2928] beendet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-418">Allow /init to be terminated from Windows [GH 2928].</span></span>
* <span data-ttu-id="19ca1-419">Drvfs verwendet standardmäßig die Groß-/Kleinschreibung nach Groß-/Kleinschreibung (entspricht der Bereitstellungsoption "Case = dir").</span><span class="sxs-lookup"><span data-stu-id="19ca1-419">DrvFs now uses per-directory case sensitivity by default (equivalent to the “case=dir” mount option).</span></span>
    * <span data-ttu-id="19ca1-420">Wenn Sie "Case = Force" verwenden (das alte Verhalten), muss ein Registrierungsschlüssel festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-420">Using “case=force” (the old behavior) requires setting a registry key.</span></span> <span data-ttu-id="19ca1-421">Führen Sie den folgenden Befehl aus, um "Case = Force" zu aktivieren, wenn Sie ihn verwenden müssen: reg Add hklm\system\currentcontrolset\services\lxss/v drvfsallowforcecasesensitivity/t REG_DWORD/d 1</span><span class="sxs-lookup"><span data-stu-id="19ca1-421">Run the following command to enable “case=force” if you need to use it: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span></span>
    * <span data-ttu-id="19ca1-422">Wenn Sie über vorhandene Verzeichnisse verfügen, die in einer älteren Version von Windows mit WSL erstellt wurden, bei denen die Groß-/Kleinschreibung beachtet werden muss, verwenden Sie "fsutil. exe", um Sie als Unterscheidung <path> nach Groß-/Kleinschreibung zu kennzeichnen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-422">If you have existing directories created with WSL in older version of Windows which need to be case sensitive, use fsutil.exe to mark them as case sensitive: fsutil.exe file setcasesensitiveinfo <path> enable</span></span>
* <span data-ttu-id="19ca1-423">NULL-Beendigungs Zeichenfolgen werden von uname syscall zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-423">NULL terminate strings returned from the uname syscall.</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-424">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-424">Console</span></span>
* <span data-ttu-id="19ca1-425">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-425">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-426">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-426">LTP Results:</span></span>
<span data-ttu-id="19ca1-427">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-427">Testing in progress.</span></span>

## <a name="build-17107"></a><span data-ttu-id="19ca1-428">Build 17107</span><span class="sxs-lookup"><span data-stu-id="19ca1-428">Build 17107</span></span>
<span data-ttu-id="19ca1-429">Allgemeine Windows-Informationen zu Build 17107 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-429">For general Windows information on build 17107 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-430">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-430">WSL</span></span>
* <span data-ttu-id="19ca1-431">Unterstützung von tcot TSF und tccot auf den Master-Pty-Endpunkten [GH 2552].</span><span class="sxs-lookup"><span data-stu-id="19ca1-431">Support TCSETSF and TCSETSW on master pty endpoints [GH 2552].</span></span>
* <span data-ttu-id="19ca1-432">Das Starten von gleichzeitigen Interop-Prozessen kann zu "Inval [GH 2813]" führen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-432">Starting simultaneous interop processes can result in EINVAL [GH 2813].</span></span>
* <span data-ttu-id="19ca1-433">Korrigieren Sie PTRACE_ATTACH, um den richtigen Ablauf verfolgungsstatus in/proc/PID/Status. anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-433">Fix PTRACE_ATTACH to show proper tracing status in /proc/pid/status.</span></span>
* <span data-ttu-id="19ca1-434">Korrektur des Race, bei dem kurzlebige Prozesse, die mit dem cleartid-und dem Abgleich-Flags geklont wurden, ohne Löschen der TID-Adresse beendet werden könnten</span><span class="sxs-lookup"><span data-stu-id="19ca1-434">Fix race where short-lived processes cloned with both the CLEARTID and SETTID flags could exit without clearing the TID address.</span></span>
* <span data-ttu-id="19ca1-435">Anzeigen einer Meldung beim Aktualisieren der Linux-Dateisystem Verzeichnisse beim Umstieg von einem Pre-17093-Build.</span><span class="sxs-lookup"><span data-stu-id="19ca1-435">Display a message when upgrading the Linux file system directories when moving from a pre-17093 build.</span></span> <span data-ttu-id="19ca1-436">Weitere Informationen zu den Änderungen des 17093-Dateisystems finden Sie in den Anmerkungen zu dieser Version von [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span><span class="sxs-lookup"><span data-stu-id="19ca1-436">For more details on the 17093 file system changes, see the release notes for [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-437">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-437">Console</span></span>
* <span data-ttu-id="19ca1-438">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-438">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-439">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-439">LTP Results:</span></span>
<span data-ttu-id="19ca1-440">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-440">Testing in progress.</span></span>

## <a name="build-17101"></a><span data-ttu-id="19ca1-441">Build 17101</span><span class="sxs-lookup"><span data-stu-id="19ca1-441">Build 17101</span></span>
<span data-ttu-id="19ca1-442">Allgemeine Windows-Informationen zu Build 17101 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-442">For general Windows information on build 17101 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-443">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-443">WSL</span></span>
* <span data-ttu-id="19ca1-444">Unterstützung für signalfd.</span><span class="sxs-lookup"><span data-stu-id="19ca1-444">Support for signalfd.</span></span> <span data-ttu-id="19ca1-445">[GH 129]</span><span class="sxs-lookup"><span data-stu-id="19ca1-445">[GH 129]</span></span>
* <span data-ttu-id="19ca1-446">Unterstützung von Dateinamen, die ungültige NTFS-Zeichen enthalten, durch Codieren als private Unicode-Zeichen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-446">Support file-names containing illegal NTFS characters by encoding them as private Unicode characters.</span></span> <span data-ttu-id="19ca1-447">[GH 1514]</span><span class="sxs-lookup"><span data-stu-id="19ca1-447">[GH 1514]</span></span>
* <span data-ttu-id="19ca1-448">Das automatische einbinden wird auf schreibgeschützt zurückgreifen, wenn Schreibvorgänge nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-448">Auto mount will fallback to read-only when write is not supported.</span></span> <span data-ttu-id="19ca1-449">[GH 2603]</span><span class="sxs-lookup"><span data-stu-id="19ca1-449">[GH 2603]</span></span>
* <span data-ttu-id="19ca1-450">Ermöglicht das Einfügen von Unicode-Ersatz Zeichen Paaren (z. b. Emoji-Zeichen).</span><span class="sxs-lookup"><span data-stu-id="19ca1-450">Allow pasting of Unicode surrogate pairs (like emoji characters).</span></span> <span data-ttu-id="19ca1-451">[GH 2765]</span><span class="sxs-lookup"><span data-stu-id="19ca1-451">[GH 2765]</span></span>
* <span data-ttu-id="19ca1-452">Pseudo Dateien in/proc und/sys sollten Lese-und Schreibvorgänge aus SELECT, Abruf, epoll, et al. [GH 2838] zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-452">Pseudo-files in /proc and /sys should return read and write ready from select, poll, epoll, et al. [GH 2838]</span></span>
* <span data-ttu-id="19ca1-453">Beheben Sie Probleme, die dazu führen könnten, dass der Dienst in eine Endlosschleife wechselt, wenn die Registrierung manipuliert wurde oder beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-453">Fix issue that could cause service to go into infinite loop when the registry has been tampered with or is corrupt.</span></span>
* <span data-ttu-id="19ca1-454">Korrigieren Sie Netlink-Nachrichten, sodass Sie mit neueren Versionen von iproute2 (Upstream 4,14) funktionieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-454">Fix netlink messages to work with newer (upstream 4.14) version of iproute2.</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-455">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-455">Console</span></span>
* <span data-ttu-id="19ca1-456">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-456">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-457">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-457">LTP Results:</span></span>
<span data-ttu-id="19ca1-458">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-458">Testing in progress.</span></span>

## <a name="build-17093"></a><span data-ttu-id="19ca1-459">Build 17093</span><span class="sxs-lookup"><span data-stu-id="19ca1-459">Build 17093</span></span>
<span data-ttu-id="19ca1-460">Allgemeine Windows-Informationen zu Build 17093 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-460">For general Windows information on build 17093 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span></span>

#### <a name="important"></a><span data-ttu-id="19ca1-461">Wichtig:</span><span class="sxs-lookup"><span data-stu-id="19ca1-461">Important:</span></span>
<span data-ttu-id="19ca1-462">Wenn Sie WSL zum ersten Mal nach dem Upgrade auf diesen Build starten, müssen Sie einige Aufgaben durchführen, um die Linux-Dateisystem Verzeichnisse zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-462">When starting WSL for the first time after upgrading to this build, it needs to perform some work upgrading the Linux file system directories.</span></span> <span data-ttu-id="19ca1-463">Dieser Vorgang kann einige Minuten in Anspruch nehmen, sodass WSL möglicherweise langsam gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-463">This may take up to several minutes, so WSL may appear to start slowly.</span></span> <span data-ttu-id="19ca1-464">Dies sollte nur einmal für jede Distribution erfolgen, die Sie aus dem Speicher installiert haben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-464">This should only happen once for each distribution you have installed from the store.</span></span>
* <span data-ttu-id="19ca1-465">Verbesserte Unterscheidung nach Groß-/Kleinschreibung in drvfs.</span><span class="sxs-lookup"><span data-stu-id="19ca1-465">Improved case sensitivity support in DrvFs.</span></span>
    * <span data-ttu-id="19ca1-466">Drvfs unterstützt jetzt die Berücksichtigung der Groß-/Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="19ca1-466">DrvFs now supports per-directory case sensitivity.</span></span> <span data-ttu-id="19ca1-467">Dies ist ein neues Flag, das für Verzeichnisse festgelegt werden kann, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen als Unterscheidung nach Groß-/Kleinschreibung behandelt werden sollen, sodass sogar Windows-Anwendungen Dateien ordnungsgemäß öffnen können</span><span class="sxs-lookup"><span data-stu-id="19ca1-467">This is a new flag that can be set on directories to indicate all operations in those directories should be treated as case sensitive, which allows even Windows applications to correctly open files that differ only by case.</span></span>
    * <span data-ttu-id="19ca1-468">Drvfs verfügt über neue Bereitstellungs Optionen, die die Berücksichtigung der Groß-/Kleinschreibung pro Verzeichnis steuern.</span><span class="sxs-lookup"><span data-stu-id="19ca1-468">DrvFs has new mount options controlling case sensitivity on a per-directory basis</span></span>
        * <span data-ttu-id="19ca1-469">Case = Force: alle Verzeichnisse werden unter Berücksichtigung der Groß-/Kleinschreibung behandelt (mit Ausnahme des Laufwerks Stamms).</span><span class="sxs-lookup"><span data-stu-id="19ca1-469">case=force: all directories are treated as case sensitive (except for the drive root).</span></span> <span data-ttu-id="19ca1-470">Neue Verzeichnisse, die mit WSL erstellt werden, werden als Groß-/Kleinschreibung beachtet</span><span class="sxs-lookup"><span data-stu-id="19ca1-470">New directories created with WSL are marked as case sensitive.</span></span> <span data-ttu-id="19ca1-471">Dies ist das Legacy Verhalten, außer wenn die Groß-/Kleinschreibung neuer Verzeichnisse gekennzeichnet wird</span><span class="sxs-lookup"><span data-stu-id="19ca1-471">This is the legacy behavior except for marking new directories case sensitive.</span></span>
        * <span data-ttu-id="19ca1-472">Case = dir: nur Verzeichnisse mit der Unterscheidung nach Groß-/Kleinschreibung werden bei der Groß-/Kleinschreibung beachtet. bei anderen Verzeichnissen wird die Groß-/Kleinschreibung</span><span class="sxs-lookup"><span data-stu-id="19ca1-472">case=dir: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="19ca1-473">Neue Verzeichnisse, die mit WSL erstellt werden, werden als Groß-/Kleinschreibung beachtet</span><span class="sxs-lookup"><span data-stu-id="19ca1-473">New directories created with WSL are marked as case sensitive.</span></span>
        * <span data-ttu-id="19ca1-474">Case = off: nur Verzeichnisse mit der Unterscheidung nach Groß-/Kleinschreibung werden bei der Groß-/Kleinschreibung beachtet. bei anderen Verzeichnissen wird die Groß-/Kleinschreibung</span><span class="sxs-lookup"><span data-stu-id="19ca1-474">case=off: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="19ca1-475">Neue Verzeichnisse, die mit WSL erstellt werden, werden als groß-und Kleinschreibung markiert</span><span class="sxs-lookup"><span data-stu-id="19ca1-475">New directories created with WSL are marked as case insensitive.</span></span>
    * <span data-ttu-id="19ca1-476">Hinweis: bei Verzeichnissen, die in früheren Versionen von WSL erstellt wurden, ist dieses Flag nicht festgelegt, sodass bei Verwendung der Option "Case = dir" nicht die Groß-/Kleinschreibung beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-476">Note: directories created by WSL in previous releases do not have this flag set, so will not be treated as case sensitive if you use the “case=dir” option.</span></span> <span data-ttu-id="19ca1-477">Eine Möglichkeit, dieses Flag für vorhandene Verzeichnisse festzulegen, ist in Kürze verfügbar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-477">A way to set this flag on existing directories is coming soon.</span></span>
    * <span data-ttu-id="19ca1-478">Beispiel für die Bereitstellung mit diesen Optionen (für vorhandene Laufwerke müssen Sie zuerst die Bereitstellung aufheben, bevor Sie die Bereitstellung mit anderen Optionen ausführen können): sudo mount-t drvfs C:/mnt/c-o Case = dir</span><span class="sxs-lookup"><span data-stu-id="19ca1-478">Example of mounting with these options (for existing drives, you must first unmount before you can mount with different options): sudo mount -t drvfs C: /mnt/c -o case=dir</span></span>
    * <span data-ttu-id="19ca1-479">Für den Moment ist Case = Force immer noch die Standardoption.</span><span class="sxs-lookup"><span data-stu-id="19ca1-479">For now, case=force is still the default option.</span></span> <span data-ttu-id="19ca1-480">Dies wird in der Zukunft in Case = dir geändert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-480">This will be changed to case=dir in the future.</span></span>
* <span data-ttu-id="19ca1-481">Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, wenn Sie drvfs einbinden, z. b.: sudo mount-t drvfs//Server/Share/mnt/Share</span><span class="sxs-lookup"><span data-stu-id="19ca1-481">You can now use forward slashes in Windows paths when mounting DrvFs, e.g.: sudo mount -t drvfs //server/share /mnt/share</span></span>
* <span data-ttu-id="19ca1-482">WSL verarbeitet nun die "/etc/fstab"-Datei während des instanzstarts [GH 2636].</span><span class="sxs-lookup"><span data-stu-id="19ca1-482">WSL now processes the /etc/fstab file during instance start [GH 2636].</span></span>
    * <span data-ttu-id="19ca1-483">Dies erfolgt vor der automatischen Einbindung von drvfs-Laufwerken. alle Laufwerke, die bereits von fstab bereitgestellt wurden, werden nicht automatisch erneut bereitgestellt, sodass Sie den Einstellungspunkt für bestimmte Laufwerke ändern können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-483">This is done prior to automatically mounting DrvFs drives; any drives that were already mounted by fstab will not be remounted automatically, allowing you to change the mount point for specific drives.</span></span>
    * <span data-ttu-id="19ca1-484">Dieses Verhalten kann mithilfe von "WSL. conf" ausgeschaltet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-484">This behavior can be turned off using wsl.conf.</span></span>
* <span data-ttu-id="19ca1-485">Die Dateien Mount, mountinfo und mountstats in/proc haben Sonderzeichen wie umgekehrte Schrägstriche und Leerzeichen ordnungsgemäß Escapezeichen [GH 2799]</span><span class="sxs-lookup"><span data-stu-id="19ca1-485">The mount, mountinfo and mountstats files in /proc properly escape special characters like backslashes and spaces [GH 2799]</span></span>
* <span data-ttu-id="19ca1-486">Sonderdateien, die mit drvfs erstellt wurden, z. b. symbolische Verknüpfungen von WSL oder bei aktivierter Metadaten, können nun aus Windows kopiert und verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-486">Special files created with DrvFs such as WSL symbolic links, or fifos and sockets when metadata is enabled, can now be copied and moved from Windows.</span></span>

#### <a name="wsl-is-more-configurable-with-wslconf"></a><span data-ttu-id="19ca1-487">WSL ist mit "WSL. conf" konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-487">WSL is more configurable with wsl.conf</span></span>
<span data-ttu-id="19ca1-488">Wir haben eine Methode hinzugefügt, mit der Sie bestimmte Funktionen in WSL automatisch konfigurieren können, die bei jedem Start des Subsystems angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-488">We added a method for you to automatically configure certain functionality in WSL that will be applied every time you launch the subsystem.</span></span> <span data-ttu-id="19ca1-489">Dies umfasst die automatischen Optionen und die Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="19ca1-489">This includes automount options and network configuration.</span></span> <span data-ttu-id="19ca1-490">Weitere Informationen hierzu finden Sie in unserem Blogbeitrag unter: https://aka.ms/wslconf</span><span class="sxs-lookup"><span data-stu-id="19ca1-490">Learn more about it in our blog post at: https://aka.ms/wslconf</span></span>

#### <a name="af_unix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a><span data-ttu-id="19ca1-491">AF_UNIX ermöglicht Socketverbindungen zwischen Linux-Prozessen auf WSL-und nativen Windows-Prozessen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-491">AF_UNIX allows socket connections between Linux processes on WSL and Windows native processes</span></span>
<span data-ttu-id="19ca1-492">WSL-und Windows-Anwendungen können nun über Unix-Sockets miteinander kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-492">WSL and Windows applications can now communicate with each other over Unix sockets.</span></span> <span data-ttu-id="19ca1-493">Stellen Sie sich vor, Sie möchten einen Dienst in Windows ausführen und sowohl für Windows-als auch für WSL-apps verfügbar machen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-493">Imagine you want to run a service in Windows and make it available to both Windows and WSL apps.</span></span> <span data-ttu-id="19ca1-494">Das ist mit UNIX-Sockets möglich.</span><span class="sxs-lookup"><span data-stu-id="19ca1-494">Now, that’s possible with Unix sockets.</span></span> <span data-ttu-id="19ca1-495">Weitere Informationen finden Sie in unserem Blogbeitrag unter https://aka.ms/afunixinterop</span><span class="sxs-lookup"><span data-stu-id="19ca1-495">Read more in our blog post at https://aka.ms/afunixinterop</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-496">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-496">WSL</span></span>
* <span data-ttu-id="19ca1-497">Unterstützung von mmap () mit MAP_NORESERVE [GH 121, 2784]</span><span class="sxs-lookup"><span data-stu-id="19ca1-497">Support mmap() with MAP_NORESERVE [GH 121, 2784]</span></span>
* <span data-ttu-id="19ca1-498">Support CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="19ca1-498">Support CLONE_PTRACE and CLONE_UNTRACED [GH 121, 2781]</span></span>
* <span data-ttu-id="19ca1-499">Behandeln von nicht-SIGCHLD-Beendigungs Signalen im Klon [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="19ca1-499">Handle non-SIGCHLD termination signal in clone [GH 121, 2781]</span></span>
* <span data-ttu-id="19ca1-500">Stub/proc/sys/fs/inotify/max_user_instances und/proc/sys/fs/inotify/max_user_watches [GH 1705]</span><span class="sxs-lookup"><span data-stu-id="19ca1-500">Stub /proc/sys/fs/inotify/max_user_instances and /proc/sys/fs/inotify/max_user_watches [GH 1705]</span></span>
* <span data-ttu-id="19ca1-501">Fehler beim Laden von elf Binärdateien, die Lade Header mit nicht-NULL-Offsets enthalten [GH 1884]</span><span class="sxs-lookup"><span data-stu-id="19ca1-501">Error loading ELF binaries that contain load headers with non-zero offsets [GH 1884]</span></span>
* <span data-ttu-id="19ca1-502">Beim Laden von Bildern werden keine nachfolgenden Seiten Bytes angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-502">Zero out trailing page bytes when loading images.</span></span>
* <span data-ttu-id="19ca1-503">Fälle reduzieren, in denen execve den Prozess unbeaufsichtigt beendet</span><span class="sxs-lookup"><span data-stu-id="19ca1-503">Reduce cases where execve silently terminates process</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-504">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-504">Console</span></span>
* <span data-ttu-id="19ca1-505">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-505">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-506">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-506">LTP Results:</span></span>
<span data-ttu-id="19ca1-507">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-507">Testing in progress.</span></span>

## <a name="build-17083"></a><span data-ttu-id="19ca1-508">Build 17083</span><span class="sxs-lookup"><span data-stu-id="19ca1-508">Build 17083</span></span>
<span data-ttu-id="19ca1-509">Allgemeine Windows-Informationen zu Build 17083 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-509">For general Windows information on build 17083 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-510">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-510">WSL</span></span>
* <span data-ttu-id="19ca1-511">Korrigiert Fehlercode im Zusammenhang mit epoll [GH 2798, 2801, 2857]</span><span class="sxs-lookup"><span data-stu-id="19ca1-511">Fixed bugcheck related to epoll [GH 2798, 2801, 2857]</span></span>
* <span data-ttu-id="19ca1-512">Beim Ausschalten von ASLR festgelegte Abstürze [GH 1185, 2870]</span><span class="sxs-lookup"><span data-stu-id="19ca1-512">Fixed hangs when turning off ASLR [GH 1185, 2870]</span></span>
* <span data-ttu-id="19ca1-513">Sicherstellen, dass mmap-Vorgänge atomarisch erscheinen [GH 2732]</span><span class="sxs-lookup"><span data-stu-id="19ca1-513">Ensure mmap operations appear atomic [GH 2732]</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-514">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-514">Console</span></span>
* <span data-ttu-id="19ca1-515">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-515">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-516">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-516">LTP Results:</span></span>
<span data-ttu-id="19ca1-517">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-517">Testing in progress.</span></span>

## <a name="build-17074"></a><span data-ttu-id="19ca1-518">Build 17074</span><span class="sxs-lookup"><span data-stu-id="19ca1-518">Build 17074</span></span>
<span data-ttu-id="19ca1-519">Allgemeine Windows-Informationen zu Build 17074 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-519">For general Windows information on build 17074 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-520">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-520">WSL</span></span>
* <span data-ttu-id="19ca1-521">Festes Speicherformat der drvfs-Metadaten [GH 2777]</span><span class="sxs-lookup"><span data-stu-id="19ca1-521">Fixed storage format of DrvFs metadata [GH 2777]</span></span> </br>
<span data-ttu-id="19ca1-522">**Wichtig:** Die vor diesem Build erstellten drvfs-Metadaten werden falsch oder überhaupt nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-522">**Important:** DrvFs metadata created before this build will show up incorrectly or not at all.</span></span> <span data-ttu-id="19ca1-523">Um betroffene Dateien zu beheben, verwenden Sie chmod und chown zum erneuten Anwenden der Metadaten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-523">To fix affected files, use chmod and chown to re-apply the metadata.</span></span>
* <span data-ttu-id="19ca1-524">Problem mit mehreren Signalen und neu startbaren syscalls behoben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-524">Fixed issue with multiple signals and restartable syscalls.</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-525">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-525">Console</span></span>
* <span data-ttu-id="19ca1-526">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-526">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-527">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-527">LTP Results:</span></span>
<span data-ttu-id="19ca1-528">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-528">Testing in progress.</span></span>

## <a name="build-17063"></a><span data-ttu-id="19ca1-529">Build 17063</span><span class="sxs-lookup"><span data-stu-id="19ca1-529">Build 17063</span></span>
<span data-ttu-id="19ca1-530">Allgemeine Windows-Informationen zu Build 17063 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-530">For general Windows information on build 17063 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="19ca1-531">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-531">WSL</span></span>
* <span data-ttu-id="19ca1-532">Drvfs unterstützt zusätzliche Linux-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-532">DrvFs supports additional Linux metadata.</span></span> <span data-ttu-id="19ca1-533">Dies ermöglicht das Festlegen des Besitzers und des Dateimodus mit chmod/chown sowie das Erstellen spezieller Dateien, z. b. von der Erstellung von Dateien, Unix-Sockets und Gerätedateien.</span><span class="sxs-lookup"><span data-stu-id="19ca1-533">This allows setting the owner and mode of files using chmod/chown, and also the creation of special files such as fifos, unix sockets and device files.</span></span> <span data-ttu-id="19ca1-534">Diese Option ist standardmäßig deaktiviert, da Sie noch experimentell ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-534">This is disabled by default for now since it's still experimental.</span></span>
<span data-ttu-id="19ca1-535">**Hinweis**:  Wir haben einen Fehler im Metadatenformat behoben, das von drvfs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-535">**Note:**  We fixed a bug in the metadata format used by DrvFs.</span></span> <span data-ttu-id="19ca1-536">Obwohl Metadaten in diesem Build für Experimente funktionieren, lesen zukünftige Builds die von diesem Build erstellten Metadaten nicht ordnungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="19ca1-536">While metadata works on this build for experimentation, future builds will not correctly read metadata created by this build.</span></span>  <span data-ttu-id="19ca1-537">Möglicherweise müssen Sie den Besitzer für geänderte Dateien manuell aktualisieren, und Geräte mit einer benutzerdefinierten Geräte-ID müssen neu erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-537">You might need to manually update owner for modified files and devices with a custom device ID will have to be recreated.</span></span>

  <span data-ttu-id="19ca1-538">Um dies zu aktivieren, einbinden Sie drvfs mit der Metadatenoption (um Sie für eine vorhandene Bereitstellung zu aktivieren):</span><span class="sxs-lookup"><span data-stu-id="19ca1-538">To enable, mount DrvFs with the metadata option (to enable it on an existing mount, you must first unmount it):</span></span>

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  <span data-ttu-id="19ca1-539">Linux-Berechtigungen werden der Datei als zusätzliche Metadaten hinzugefügt. Sie wirken sich nicht auf die Windows-Berechtigungen aus.</span><span class="sxs-lookup"><span data-stu-id="19ca1-539">Linux permissions are added as additional metadata to the file; they do not affect the Windows permissions.</span></span>  <span data-ttu-id="19ca1-540">Beachten Sie, dass beim Bearbeiten einer Datei mithilfe eines Windows-Editors die Metadaten möglicherweise entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-540">Remember, editing a file using a Windows editor may remove the metadata.</span></span> <span data-ttu-id="19ca1-541">In diesem Fall wird die Datei auf die Standard Berechtigungen zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-541">In this case, the file will revert to its default permissions.</span></span>

* <span data-ttu-id="19ca1-542">Der drvfs wurden Bereitstellungsoptionen hinzugefügt, um Dateien ohne Metadaten zu steuern.</span><span class="sxs-lookup"><span data-stu-id="19ca1-542">Added mount options to DrvFs to control files without metadata.</span></span>
  * <span data-ttu-id="19ca1-543">UID: die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-543">uid: the user ID used for the owner of all files.</span></span>
  * <span data-ttu-id="19ca1-544">gid: die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-544">gid: the group ID used for the owner of all files.</span></span>
  * <span data-ttu-id="19ca1-545">"um Ask": eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-545">umask: an octal mask of permissions to exclude for all files and directories.</span></span>
  * <span data-ttu-id="19ca1-546">fmask: eine oktale Maske von Berechtigungen, die für alle regulären Dateien ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-546">fmask: an octal mask of permissions to exclude for all regular files.</span></span>
  * <span data-ttu-id="19ca1-547">dmask: eine oktale Maske von Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-547">dmask: an octal mask of permissions to exclude for all directories.</span></span>

  <span data-ttu-id="19ca1-548">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="19ca1-548">For example:</span></span>
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  <span data-ttu-id="19ca1-549">Kombinieren Sie mit der Option Metadata, um Standard Berechtigungen für Dateien ohne Metadaten anzugeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-549">Combine with the metadata option to specify default permissions for files without metadata.</span></span>

* <span data-ttu-id="19ca1-550">In wurde eine neue Umgebungsvariable `WSLENV`,, eingeführt, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32 fließen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-550">Introduced a new environment variable, `WSLENV`, to configure how environment variables flow between WSL and Win32.</span></span>

  <span data-ttu-id="19ca1-551">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="19ca1-551">For example:</span></span>

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  <span data-ttu-id="19ca1-552">`WSLENV`eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozessen von Win32-oder Win32-Prozessen von WSL eingeschlossen werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-552">`WSLENV` is a colon-delimited list of environment variables that can be included when launching WSL processes from Win32 or Win32 processes from WSL.</span></span>  <span data-ttu-id="19ca1-553">Jeder Variablen kann ein Schrägstrich gefolgt von Flags angehängt werden, um anzugeben, wie Sie übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="19ca1-553">Each variable can be suffixed with a slash followed by flags to specify how it is translated.</span></span>
  * <span data-ttu-id="19ca1-554">cker Der Wert ist ein Pfad, der zwischen WSL-Pfaden und Win32-Pfaden übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="19ca1-554">p: The value is a path that should be translated between WSL paths and Win32 paths.</span></span>
  * <span data-ttu-id="19ca1-555">int Der Wert ist eine Liste von Pfaden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-555">l: The value is a list of paths.</span></span> <span data-ttu-id="19ca1-556">In WSL ist es eine durch Doppelpunkte getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="19ca1-556">In WSL, it is a colon-delimited list.</span></span> <span data-ttu-id="19ca1-557">In Win32 ist es eine durch Semikolons getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="19ca1-557">In Win32, it is a semicolon-delimited list.</span></span>
  * <span data-ttu-id="19ca1-558">u Der Wert sollte nur beim Aufrufen von WSL aus Win32 eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-558">u: The value should only be included when invoking WSL from Win32</span></span>
  * <span data-ttu-id="19ca1-559">Löw Der Wert sollte nur eingeschlossen werden, wenn Win32 von WSL aus aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-559">w: The value should only be included when invoking Win32 from WSL</span></span>

  <span data-ttu-id="19ca1-560">Sie können in `WSLENV` . bashrc oder für Ihren Benutzer in der benutzerdefinierten Windows-Umgebung festlegen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-560">You can set `WSLENV` in .bashrc or in the custom Windows environment for your user.</span></span>

* <span data-ttu-id="19ca1-561">drvfs-bereit Stellungen speichert Zeitstempel ordnungsgemäß aus tar, CP-p (GH 1939)</span><span class="sxs-lookup"><span data-stu-id="19ca1-561">drvfs mounts correctly preserves timestamps from tar, cp -p (GH 1939)</span></span>
* <span data-ttu-id="19ca1-562">drvfs-symlinks melden die richtige Größe (GH 2641)</span><span class="sxs-lookup"><span data-stu-id="19ca1-562">drvfs symlinks report the correct size (GH 2641)</span></span>
* <span data-ttu-id="19ca1-563">Lese-/Schreibvorgänge funktionieren für sehr große e/a-Größen (GH 2653)</span><span class="sxs-lookup"><span data-stu-id="19ca1-563">read/write works for very large IO sizes (GH 2653)</span></span>
* <span data-ttu-id="19ca1-564">waitpid funktioniert mit Prozessgruppen-IDs (GH 2534)</span><span class="sxs-lookup"><span data-stu-id="19ca1-564">waitpid works with process group IDs (GH 2534)</span></span>
* <span data-ttu-id="19ca1-565">erheblich verbesserte mmap-Leistung für große Reserve Regionen; Verbesserung der Leistung von GHC (GH 1671)</span><span class="sxs-lookup"><span data-stu-id="19ca1-565">significantly improved mmap performance for large reserve regions; improves ghc performance (GH 1671)</span></span>
* <span data-ttu-id="19ca1-566">"Personality" unterstützt für READ_IMPLIES_EXEC; korrigiert von Maxima und clisp (GH 1185)</span><span class="sxs-lookup"><span data-stu-id="19ca1-566">personality supports for READ_IMPLIES_EXEC; fixes maxima and clisp (GH 1185)</span></span>
* <span data-ttu-id="19ca1-567">mprotect unterstützt PROT_GROWSDOWN; Fixes clisp (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="19ca1-567">mprotect supports PROT_GROWSDOWN; fixes clisp (GH 1128)</span></span>
* <span data-ttu-id="19ca1-568">Seiten Fehlerbehebungen im übercommitmodus; Fixes sbcl (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="19ca1-568">page fault fixes in overcommit mode; fixes sbcl (GH 1128)</span></span>
* <span data-ttu-id="19ca1-569">Klon unterstützt weitere Flags-Kombinationen</span><span class="sxs-lookup"><span data-stu-id="19ca1-569">clone supports more flags combinations</span></span>
* <span data-ttu-id="19ca1-570">Unterstützung von SELECT/epoll von epoll-Dateien (zuvor ein No-op-Vorgang).</span><span class="sxs-lookup"><span data-stu-id="19ca1-570">Support select/epoll of epoll files (previously a no-op).</span></span>
* <span data-ttu-id="19ca1-571">Ptrace über nicht implementierte syscalls benachrichtigen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-571">Notify ptrace of unimplemented syscalls.</span></span>
* <span data-ttu-id="19ca1-572">Beim Erstellen von resolv. conf-Namen Server nicht Aufforderungs Schnittstellen ignorieren [GH 2694]</span><span class="sxs-lookup"><span data-stu-id="19ca1-572">Ignore interfaces that are not up when generating resolv.conf nameservers [GH 2694]</span></span>
* <span data-ttu-id="19ca1-573">Listet Netzwerkschnittstellen ohne physische Adresse auf.</span><span class="sxs-lookup"><span data-stu-id="19ca1-573">Enumerate network interfaces with no physical address.</span></span> <span data-ttu-id="19ca1-574">[GH 2685]</span><span class="sxs-lookup"><span data-stu-id="19ca1-574">[GH 2685]</span></span>
* <span data-ttu-id="19ca1-575">Zusätzliche Fehlerbehebungen und Verbesserungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-575">Additional bug fixes and improvements.</span></span>

### <a name="linux-tools-available-to-developers-on-windows"></a><span data-ttu-id="19ca1-576">Linux-Tools für Entwickler unter Windows</span><span class="sxs-lookup"><span data-stu-id="19ca1-576">Linux tools available to developers on Windows</span></span>

* <span data-ttu-id="19ca1-577">Die Windows-Befehlszeilen-Toolkette enthält bsdtar (tar) und curl.</span><span class="sxs-lookup"><span data-stu-id="19ca1-577">Windows Command line Toolchain includes bsdtar (tar) and curl.</span></span>
  <span data-ttu-id="19ca1-578">Lesen Sie [diesen Blog](https://aka.ms/tarcurlwindows) , um mehr über das Hinzufügen dieser beiden neuen Tools zu erfahren, und erfahren Sie, wie Sie die Entwickler Darstellung unter Windows strukturieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-578">Read [this blog](https://aka.ms/tarcurlwindows) to learn more about the addition of these two new tools and see how they’re shaping the developer experience on Windows.</span></span>

*   <span data-ttu-id="19ca1-579">`AF_UNIX`ist im Windows Insider SDK (17061 +) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-579">`AF_UNIX` is available in the Windows Insider SDK (17061+).</span></span>
  <span data-ttu-id="19ca1-580">Lesen Sie [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) , um mehr `AF_UNIX` darüber zu erfahren, wie Entwickler in Windows ihn verwenden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-580">Read [this blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) to learn more about `AF_UNIX` and how developers on Windows can use it.</span></span>

### <a name="console"></a><span data-ttu-id="19ca1-581">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-581">Console</span></span>
* <span data-ttu-id="19ca1-582">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-582">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-583">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-583">LTP Results:</span></span>
<span data-ttu-id="19ca1-584">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-584">Testing in progress.</span></span>


## <a name="build-17046"></a><span data-ttu-id="19ca1-585">Build 17046</span><span class="sxs-lookup"><span data-stu-id="19ca1-585">Build 17046</span></span>

<span data-ttu-id="19ca1-586">Allgemeine Windows-Informationen zu Build 17046 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span><span class="sxs-lookup"><span data-stu-id="19ca1-586">For general Windows information on build 17046 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-587">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-587">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-588">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-588">WSL</span></span>
- <span data-ttu-id="19ca1-589">Ermöglicht das Ausführen von Prozessen ohne ein aktives Terminal.</span><span class="sxs-lookup"><span data-stu-id="19ca1-589">Allow processes to run without an active terminal.</span></span> <span data-ttu-id="19ca1-590">[GH 709, 1007, 1511, 2252, 2391, et al.]</span><span class="sxs-lookup"><span data-stu-id="19ca1-590">[GH 709, 1007, 1511, 2252, 2391, et al.]</span></span>
- <span data-ttu-id="19ca1-591">Bessere Unterstützung von CLONE_VFORK und CLONE_VM.</span><span class="sxs-lookup"><span data-stu-id="19ca1-591">Better support of CLONE_VFORK and CLONE_VM.</span></span> <span data-ttu-id="19ca1-592">[GH 1878, 2615]</span><span class="sxs-lookup"><span data-stu-id="19ca1-592">[GH 1878, 2615]</span></span>
- <span data-ttu-id="19ca1-593">Überspringen Sie die TDI-Filtertreiber für WSL-Netzwerk Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="19ca1-593">Skip TDI filter drivers for WSL networking operations.</span></span> <span data-ttu-id="19ca1-594">[GH 1554]</span><span class="sxs-lookup"><span data-stu-id="19ca1-594">[GH 1554]</span></span>
- <span data-ttu-id="19ca1-595">Drvfs erstellt NT-Symlinks, wenn bestimmte Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="19ca1-595">DrvFs creates NT symlinks when certain conditions are met.</span></span> <span data-ttu-id="19ca1-596">[GH 353, 1475, 2602]</span><span class="sxs-lookup"><span data-stu-id="19ca1-596">[GH 353, 1475, 2602]</span></span>
    - <span data-ttu-id="19ca1-597">Das Linkziel muss relativ sein, darf keine Bereitstellungs Punkte oder symlinks überschreiten und muss vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="19ca1-597">The link target must be relative, must not cross any mount points or symlinks, and must exist.</span></span>
    - <span data-ttu-id="19ca1-598">Der Benutzer muss über SE_CREATE_SYMBOLIC_LINK_PRIVILEGE verfügen (Dies erfordert normalerweise, dass Sie "WSL. exe" mit erhöhten Rechten starten), sofern der Entwicklermodus nicht aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-598">The user must have SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (this normally requires you to launch wsl.exe elevated), unless Developer Mode is turned on.</span></span>
    - <span data-ttu-id="19ca1-599">In allen anderen Situationen erstellt drvfs weiterhin WSL-symlinks.</span><span class="sxs-lookup"><span data-stu-id="19ca1-599">In all other situations, DrvFs still creates WSL symlinks.</span></span>
- <span data-ttu-id="19ca1-600">Ermöglicht das gleichzeitige Ausführen von erweiterten und nicht erhöhten WSL-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-600">Allow running elevated and non-elevated WSL instances simultaneously.</span></span>
- <span data-ttu-id="19ca1-601">Support/proc/sys/kernel/Yama/ptrace_scope</span><span class="sxs-lookup"><span data-stu-id="19ca1-601">Support /proc/sys/kernel/yama/ptrace_scope</span></span>
- <span data-ttu-id="19ca1-602">Fügen Sie wslpath zum Durchführen von WSL-< > Windows-Pfad Konvertierungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-602">Add wslpath to do WSL<->Windows path conversions.</span></span> <span data-ttu-id="19ca1-603">[GH 522, 1243, 1834, 2327, et al.]</span><span class="sxs-lookup"><span data-stu-id="19ca1-603">[GH 522, 1243, 1834, 2327, et al.]</span></span>
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a><span data-ttu-id="19ca1-604">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-604">Console</span></span>
- <span data-ttu-id="19ca1-605">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-605">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-606">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-606">LTP Results:</span></span>
<span data-ttu-id="19ca1-607">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-607">Testing in progress.</span></span>


## <a name="build-17040"></a><span data-ttu-id="19ca1-608">Build 17040</span><span class="sxs-lookup"><span data-stu-id="19ca1-608">Build 17040</span></span>

<span data-ttu-id="19ca1-609">Allgemeine Windows-Informationen zu Build 17040 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span><span class="sxs-lookup"><span data-stu-id="19ca1-609">For general Windows information on build 17040 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-610">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-610">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-611">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-611">WSL</span></span>
- <span data-ttu-id="19ca1-612">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="19ca1-612">No fixes since 17035.</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-613">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-613">Console</span></span>
- <span data-ttu-id="19ca1-614">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="19ca1-614">No fixes since 17035.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-615">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-615">LTP Results:</span></span>
<span data-ttu-id="19ca1-616">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-616">Testing in progress.</span></span>

## <a name="build-17035"></a><span data-ttu-id="19ca1-617">Build 17035</span><span class="sxs-lookup"><span data-stu-id="19ca1-617">Build 17035</span></span>

<span data-ttu-id="19ca1-618">Allgemeine Windows-Informationen zu Build 17035 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span><span class="sxs-lookup"><span data-stu-id="19ca1-618">For general Windows information on build 17035 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-619">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-619">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-620">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-620">WSL</span></span>
- <span data-ttu-id="19ca1-621">Der Zugriff auf Dateien auf drvfs kann gelegentlich mit EINVAL fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-621">Accessing files on DrvFs could occasionally fail with EINVAL.</span></span> <span data-ttu-id="19ca1-622">[GH 2448]</span><span class="sxs-lookup"><span data-stu-id="19ca1-622">[GH 2448]</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-623">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-623">Console</span></span>
- <span data-ttu-id="19ca1-624">Ein Farbverlust beim Einfügen/Löschen von Zeilen im VT-Modus.</span><span class="sxs-lookup"><span data-stu-id="19ca1-624">Some color loss when inserting/deleting lines in VT mode.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-625">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-625">LTP Results:</span></span>
<span data-ttu-id="19ca1-626">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-626">Testing in progress.</span></span>

## <a name="build-17025"></a><span data-ttu-id="19ca1-627">Build 17025</span><span class="sxs-lookup"><span data-stu-id="19ca1-627">Build 17025</span></span>

<span data-ttu-id="19ca1-628">Allgemeine Windows-Informationen zu Build 17025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span><span class="sxs-lookup"><span data-stu-id="19ca1-628">For general Windows information on build 17025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-629">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-629">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-630">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-630">WSL</span></span>
- <span data-ttu-id="19ca1-631">Starten Sie anfängliche Prozesse in einer neuen Vordergrund-Prozessgruppe [GH 1653, 2510].</span><span class="sxs-lookup"><span data-stu-id="19ca1-631">Start initial processes in a new foreground process group [GH 1653, 2510].</span></span>
- <span data-ttu-id="19ca1-632">Problem Behebungen für die Übermittlung [GH 2496]</span><span class="sxs-lookup"><span data-stu-id="19ca1-632">SIGHUP delivery fixes [GH 2496].</span></span>
- <span data-ttu-id="19ca1-633">Standardname für virtuelle Bridge generieren, wenn keine Angabe erfolgt [GH 2497].</span><span class="sxs-lookup"><span data-stu-id="19ca1-633">Generate default virtual bridge name if none provided [GH 2497].</span></span>
- <span data-ttu-id="19ca1-634">Implementieren Sie/proc/sys/kernel/Random/boot_id [GH 2518].</span><span class="sxs-lookup"><span data-stu-id="19ca1-634">Implement /proc/sys/kernel/random/boot_id [GH 2518].</span></span>
- <span data-ttu-id="19ca1-635">Weitere Interop stdout/stderr-pipekorrekturen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-635">More interop stdout/stderr pipe fixes.</span></span>
- <span data-ttu-id="19ca1-636">Der Stub-syncfs-System Aufruf.</span><span class="sxs-lookup"><span data-stu-id="19ca1-636">Stub syncfs system call.</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-637">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-637">Console</span></span>
- <span data-ttu-id="19ca1-638">Korrigieren der Eingabe-VT-Übersetzung für Drittanbieter Konsolen [GH 111]</span><span class="sxs-lookup"><span data-stu-id="19ca1-638">Fix input VT translation for third party consoles [GH 111]</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-639">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-639">LTP Results:</span></span>
<span data-ttu-id="19ca1-640">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-640">Testing in progress.</span></span>

## <a name="build-17017"></a><span data-ttu-id="19ca1-641">Build 17017</span><span class="sxs-lookup"><span data-stu-id="19ca1-641">Build 17017</span></span>

<span data-ttu-id="19ca1-642">Allgemeine Windows-Informationen zu Build 17017 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span><span class="sxs-lookup"><span data-stu-id="19ca1-642">For general Windows information on build 17017 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-643">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-643">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-644">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-644">WSL</span></span>
- <span data-ttu-id="19ca1-645">Ignoriert leere elf-Programm Header [GH 330].</span><span class="sxs-lookup"><span data-stu-id="19ca1-645">Ignore empty ELF program headers [GH 330].</span></span>
- <span data-ttu-id="19ca1-646">Ermöglicht lxssmanager das Erstellen von WSL-Instanzen für nicht interaktive Benutzer (Unterstützung für SSH-und geplante Aufgaben) [GH 777, 1602].</span><span class="sxs-lookup"><span data-stu-id="19ca1-646">Allow LxssManager to create WSL instances for non-interactive users (ssh and scheduled task support) [GH 777, 1602].</span></span>
- <span data-ttu-id="19ca1-647">Unterstützung von WSL-> Win32-> WSL-Szenarios ("Inception") [GH 1228].</span><span class="sxs-lookup"><span data-stu-id="19ca1-647">Support WSL->Win32->WSL ("inception") scenarios [GH 1228].</span></span>
- <span data-ttu-id="19ca1-648">Eingeschränkte Unterstützung für das Beenden von Konsolen-apps, die über Interop [GH 1614] aufgerufen wurden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-648">Limited support for termination of console apps invoked via interop [GH 1614].</span></span>
- <span data-ttu-id="19ca1-649">Unterstützung von Einstellungsoptionen für devpts [GH 1948].</span><span class="sxs-lookup"><span data-stu-id="19ca1-649">Support mount options for devpts [GH 1948].</span></span>
- <span data-ttu-id="19ca1-650">Ptrace blockiert den untergeordneten Start [GH 2333].</span><span class="sxs-lookup"><span data-stu-id="19ca1-650">Ptrace blocking child startup [GH 2333].</span></span>
- <span data-ttu-id="19ca1-651">Im epollet fehlen einige Ereignisse [GH 2462].</span><span class="sxs-lookup"><span data-stu-id="19ca1-651">EPOLLET missing some events [GH 2462].</span></span>
- <span data-ttu-id="19ca1-652">Gibt weitere Daten für PTRACE_GETSIGINFO zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-652">Return more data for PTRACE_GETSIGINFO.</span></span>
- <span data-ttu-id="19ca1-653">Getdents mit lseek haben falsche Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="19ca1-653">Getdents with lseek gives incorrect results.</span></span>
- <span data-ttu-id="19ca1-654">Beheben Sie einige Win32-Interop-apps, die auf Eingaben in einer Pipe warten, die keine weiteren Daten enthält.</span><span class="sxs-lookup"><span data-stu-id="19ca1-654">Fix some Win32 interop app hangs, waiting for input on a pipe that has no more data.</span></span>
- <span data-ttu-id="19ca1-655">O_ASYNC Unterstützung für TTY/Pty-Dateien.</span><span class="sxs-lookup"><span data-stu-id="19ca1-655">O_ASYNC support for tty/pty files.</span></span>
- <span data-ttu-id="19ca1-656">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-656">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-657">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-657">Console</span></span>
- <span data-ttu-id="19ca1-658">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-658">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-659">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-659">LTP Results:</span></span>
<span data-ttu-id="19ca1-660">Tests werden ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-660">Testing in progress.</span></span>

## <a name="fall-creators-update"></a><span data-ttu-id="19ca1-661">Fall Creators Update</span><span class="sxs-lookup"><span data-stu-id="19ca1-661">Fall Creators Update</span></span>

## <a name="build-16288"></a><span data-ttu-id="19ca1-662">Build 16288</span><span class="sxs-lookup"><span data-stu-id="19ca1-662">Build 16288</span></span>

<span data-ttu-id="19ca1-663">Allgemeine Windows-Informationen zu Build 16288 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-663">For general Windows information on build 16288 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-664">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-664">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-665">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-665">WSL</span></span>
- <span data-ttu-id="19ca1-666">Ordnungsgemäße Initialisierung und Berichts-UID, gid und Modus für socketdateideskriptoren [GH 2490]</span><span class="sxs-lookup"><span data-stu-id="19ca1-666">Correctly initialize and report uid, gid, and mode for socket file descriptors [GH 2490]</span></span>
- <span data-ttu-id="19ca1-667">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-667">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-668">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-668">Console</span></span>
- <span data-ttu-id="19ca1-669">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-669">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-670">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-670">LTP Results:</span></span>
<span data-ttu-id="19ca1-671">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="19ca1-671">No change since 16273</span></span>

## <a name="build-16278"></a><span data-ttu-id="19ca1-672">Build 16278</span><span class="sxs-lookup"><span data-stu-id="19ca1-672">Build 16278</span></span>

<span data-ttu-id="19ca1-673">Allgemeine Windows-Informationen zu Build 162738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-673">For general Windows information on build 162738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-674">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-674">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-675">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-675">WSL</span></span>
- <span data-ttu-id="19ca1-676">Zuordnung zugeordneter Sichten von Datei gestützten Abschnitten explizit aufheben, wenn der LX mm-Status beendet wird [GH 2415]</span><span class="sxs-lookup"><span data-stu-id="19ca1-676">Explicitly unmap mapped views of file backed sections when tearing down LX MM state [GH 2415]</span></span>
- <span data-ttu-id="19ca1-677">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-677">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-678">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-678">Console</span></span>
- <span data-ttu-id="19ca1-679">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-679">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-680">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-680">LTP Results:</span></span>
<span data-ttu-id="19ca1-681">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="19ca1-681">No change since 16273</span></span>

## <a name="build-16275"></a><span data-ttu-id="19ca1-682">Build 16275</span><span class="sxs-lookup"><span data-stu-id="19ca1-682">Build 16275</span></span>

<span data-ttu-id="19ca1-683">Allgemeine Windows-Informationen zu Build 162735 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-683">For general Windows information on build 162735 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-684">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-684">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-685">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-685">WSL</span></span>
- <span data-ttu-id="19ca1-686">In dieser Version gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-686">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-687">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-687">Console</span></span>
- <span data-ttu-id="19ca1-688">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-688">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-689">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-689">LTP Results:</span></span>
<span data-ttu-id="19ca1-690">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="19ca1-690">No change since 16273</span></span>

## <a name="build-16273"></a><span data-ttu-id="19ca1-691">Build 16273</span><span class="sxs-lookup"><span data-stu-id="19ca1-691">Build 16273</span></span>

<span data-ttu-id="19ca1-692">Allgemeine Windows-Informationen zu Build 16273 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-692">For general Windows information on build 16273 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-693">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-693">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-694">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-694">WSL</span></span>
- <span data-ttu-id="19ca1-695">Es wurde ein Problem behoben, bei dem drvfs manchmal den falschen Dateityp für Verzeichnisse gemeldet hat [GH 2392]</span><span class="sxs-lookup"><span data-stu-id="19ca1-695">Fixed an issue where DrvFs sometimes reported the wrong file type for directories [GH 2392]</span></span>
- <span data-ttu-id="19ca1-696">Erstellung von NETLINK_KOBJECT_UEVENT Sockets zum Entsperren von Programmen zulassen, die uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span><span class="sxs-lookup"><span data-stu-id="19ca1-696">Allow creation of NETLINK_KOBJECT_UEVENT sockets to unblock programs that use uevent [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span></span>
- <span data-ttu-id="19ca1-697">Unterstützung für nicht blockierende Verbindung hinzufügen [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span><span class="sxs-lookup"><span data-stu-id="19ca1-697">Add support for non-blocking connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span></span>
- <span data-ttu-id="19ca1-698">Implementierende CLONE_FS Clone System-aufrufsflag [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="19ca1-698">Implement CLONE_FS clone system call flag [GH 2242]</span></span>
- <span data-ttu-id="19ca1-699">Beheben von Problemen im Zusammenhang mit der korrekten Behandlung von Registerkarten oder Anführungszeichen in NT-Interop [GH 1625, 2164]</span><span class="sxs-lookup"><span data-stu-id="19ca1-699">Fix issues around not handling tabs or quotes correctly in NT interop [GH 1625, 2164]</span></span>
- <span data-ttu-id="19ca1-700">Beheben des Fehlers "Zugriff verweigert" beim erneuten Starten von WSL-Instanzen [GH 651, 2095]</span><span class="sxs-lookup"><span data-stu-id="19ca1-700">Resolve access denied error when trying to re-launch WSL instances [GH 651, 2095]</span></span>
- <span data-ttu-id="19ca1-701">Implementieren von Futex-FUTEX_REQUEUE und FUTEX_CMP_REQUEUE-Vorgängen [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="19ca1-701">Implement futex FUTEX_REQUEUE and FUTEX_CMP_REQUEUE operations [GH 2242]</span></span>
- <span data-ttu-id="19ca1-702">Korrigieren von Berechtigungen für verschiedene sysfs-Dateien [GH 2214]</span><span class="sxs-lookup"><span data-stu-id="19ca1-702">Fix permissions for various SysFs files [GH 2214]</span></span>
- <span data-ttu-id="19ca1-703">Korrigieren des haskell-Stapel Staus während des Setups [GH 2290]</span><span class="sxs-lookup"><span data-stu-id="19ca1-703">Fix Haskell stack hang during setup [GH 2290]</span></span>
- <span data-ttu-id="19ca1-704">Implementieren der binfmt_misc-Flags "C", "O" und "P" [GH 2103]</span><span class="sxs-lookup"><span data-stu-id="19ca1-704">Implement binfmt_misc 'C' 'O' and 'P' flags [GH 2103]</span></span>
- <span data-ttu-id="19ca1-705">Add/proc/sys/kernel/SHMMAX/shmmni &/Threads-Max [GH 1753]</span><span class="sxs-lookup"><span data-stu-id="19ca1-705">Add /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span></span>
- <span data-ttu-id="19ca1-706">Hinzufügen partieller Unterstützung für ioprio_set-Systemaufrufe [GH 498]</span><span class="sxs-lookup"><span data-stu-id="19ca1-706">Add partial support for ioprio_set system call [GH 498]</span></span>
- <span data-ttu-id="19ca1-707">Stub SO_REUSEPORT & Hinzufügen von Unterstützung für SO_PASSCRED für netLINK-Sockets [GH 69]</span><span class="sxs-lookup"><span data-stu-id="19ca1-707">Stub SO_REUSEPORT & adding support for SO_PASSCRED for netlink sockets [GH 69]</span></span>
- <span data-ttu-id="19ca1-708">Gibt andere Fehlercodes von registerdistribuiton zurück, wenn derzeit eine Distribution installiert oder deinstalliert wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-708">Return different error codes from RegisterDistribuiton if a distribution is currently being installed or uninstalled.</span></span>
- <span data-ttu-id="19ca1-709">Aufheben der Registrierung von teilweise installierten WSL-Verteilungen über "wslconfig. exe" zulassen</span><span class="sxs-lookup"><span data-stu-id="19ca1-709">Allow unregistration of partially installed WSL distributions via wslconfig.exe</span></span>
- <span data-ttu-id="19ca1-710">Korrigieren Sie den python-sockettestabsturz von UDP:: msg_peek</span><span class="sxs-lookup"><span data-stu-id="19ca1-710">Fix python socket test hang from udp::msg_peek</span></span>
- <span data-ttu-id="19ca1-711">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-711">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-712">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-712">Console</span></span>
- <span data-ttu-id="19ca1-713">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-713">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-714">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-714">LTP Results:</span></span>
<span data-ttu-id="19ca1-715">Tests gesamt: 1904</span><span class="sxs-lookup"><span data-stu-id="19ca1-715">Total Tests: 1904</span></span><br/>
<span data-ttu-id="19ca1-716">Übersprungene Tests insgesamt: 209</span><span class="sxs-lookup"><span data-stu-id="19ca1-716">Total Skipped Tests: 209</span></span><br/>
<span data-ttu-id="19ca1-717">Gesamtanzahl der Fehler: 229</span><span class="sxs-lookup"><span data-stu-id="19ca1-717">Total Failures: 229</span></span><br/>
[<span data-ttu-id="19ca1-718">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-718">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a><span data-ttu-id="19ca1-719">Build 16257</span><span class="sxs-lookup"><span data-stu-id="19ca1-719">Build 16257</span></span>

<span data-ttu-id="19ca1-720">Allgemeine Windows-Informationen zu Build 16257 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-720">For general Windows information on build 16257 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-721">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-721">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-722">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-722">WSL</span></span>
- <span data-ttu-id="19ca1-723">Prlimit64-Systemaufrufe implementieren</span><span class="sxs-lookup"><span data-stu-id="19ca1-723">Implement prlimit64 system call</span></span>
- <span data-ttu-id="19ca1-724">Hinzufügen von Unterstützung für ulimit-n (RLIMIT_NOFILE Limit) [GH 1688]</span><span class="sxs-lookup"><span data-stu-id="19ca1-724">Add support for ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span></span>
- <span data-ttu-id="19ca1-725">Stub MSG_MORE für TCP-Sockets [GH 2351]</span><span class="sxs-lookup"><span data-stu-id="19ca1-725">Stub MSG_MORE for TCP sockets [GH 2351]</span></span>
- <span data-ttu-id="19ca1-726">Korrigieren von ungültigem AT_EXECFN-Hilfsvektor Verhalten [GH 2133]</span><span class="sxs-lookup"><span data-stu-id="19ca1-726">Fix invalid AT_EXECFN auxiliary vector behavior [GH 2133]</span></span>
- <span data-ttu-id="19ca1-727">Korrigieren von Kopier-/Einfügeverhalten für Konsole/TTY und Hinzufügen einer besseren vollständigen Puffer Verarbeitung [GH 2204, 2131]</span><span class="sxs-lookup"><span data-stu-id="19ca1-727">Fix copy/paste behavior for console/tty, and add better full buffer handling [GH 2204, 2131]</span></span>
- <span data-ttu-id="19ca1-728">Set AT_SECURE im Hilfsvektor für Set-User-ID und Set-Group-ID-Programme [GH 2031]</span><span class="sxs-lookup"><span data-stu-id="19ca1-728">Set AT_SECURE in auxiliary vector for set-user-ID and set-group-ID programs [GH 2031]</span></span>
- <span data-ttu-id="19ca1-729">Psuedo-Terminal Master Endpunkt behandelt nicht tiocpgrp [GH 1063]</span><span class="sxs-lookup"><span data-stu-id="19ca1-729">Psuedo-terminal master endpoint not handling TIOCPGRP [GH 1063]</span></span>
- <span data-ttu-id="19ca1-730">Korrigieren von lseek zum Zurückspulen von Verzeichnissen in lxfs [GH 2310]</span><span class="sxs-lookup"><span data-stu-id="19ca1-730">Fix lseek does to rewind directories in LxFs [GH 2310]</span></span>
- <span data-ttu-id="19ca1-731">/dev/ptmx sperrt nach hoher Auslastung [GH 1882]</span><span class="sxs-lookup"><span data-stu-id="19ca1-731">/dev/ptmx locks up after heavy usage [GH 1882]</span></span>
- <span data-ttu-id="19ca1-732">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-732">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-733">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-733">Console</span></span>
- <span data-ttu-id="19ca1-734">Behebung für horizontale Linien/Unterstriche überall [GH 2168]</span><span class="sxs-lookup"><span data-stu-id="19ca1-734">Fix for horizontal Lines/Underscores Everywhere [GH 2168]</span></span>
- <span data-ttu-id="19ca1-735">Behebung von Änderungen an der Prozess Reihenfolge, die das Schließen von NPM erschwert [GH 2170]</span><span class="sxs-lookup"><span data-stu-id="19ca1-735">Fix for process order changed making NPM harder to close [GH 2170]</span></span>
- <span data-ttu-id="19ca1-736">Neues Farbschema hinzugefügt: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span><span class="sxs-lookup"><span data-stu-id="19ca1-736">Added our new color scheme: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-737">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-737">LTP Results:</span></span>
<span data-ttu-id="19ca1-738">Keine Änderung seit 16251</span><span class="sxs-lookup"><span data-stu-id="19ca1-738">No change since 16251</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-739">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-739">Syscall Support</span></span>
<span data-ttu-id="19ca1-740">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-740">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-741">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-741">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`prlimit64`<br/>

### <a name="known-issues"></a><span data-ttu-id="19ca1-742">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="19ca1-742">Known Issues</span></span>
#### <a name="github-issue-2392-windows-folders-not-recognized-by-wsl-httpsgithubcommicrosoftbashonwindowsissues2392"></a>[<span data-ttu-id="19ca1-743">GitHub-Problem 2392: Windows-Ordner, die nicht von WSL erkannt werden...</span><span class="sxs-lookup"><span data-stu-id="19ca1-743">GitHub Issue 2392: Windows Folders not recognized by WSL ...</span></span>](https://github.com/Microsoft/BashOnWindows/issues/2392)
<span data-ttu-id="19ca1-744">In Build 16257 hat WSL Probleme, wenn Windows-Dateien/-Ordner über `/mnt/c/...`aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-744">In build 16257, WSL has issues when enumerating Windows files/folders via `/mnt/c/...`.</span></span>
<span data-ttu-id="19ca1-745">Dieses Problem wurde behoben und sollte in Insider-Builds in der Woche ab 8/14/2017 veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-745">This issue has been fixed and should be released in Insiders build during week commencing 8/14/2017.</span></span>

<br/>

## <a name="build-16251"></a><span data-ttu-id="19ca1-746">Build 16251</span><span class="sxs-lookup"><span data-stu-id="19ca1-746">Build 16251</span></span>

<span data-ttu-id="19ca1-747">Allgemeine Windows-Informationen zu Build 16251 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-747">For general Windows information on build 16251 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-748">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-748">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-749">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-749">WSL</span></span>
- <span data-ttu-id="19ca1-750">Entfernen Sie das Beta-Tag aus der optionalen WSL-Komponente. Weitere Informationen finden Sie im [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) .</span><span class="sxs-lookup"><span data-stu-id="19ca1-750">Remove beta tag from WSL optional component, see [blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) for details.</span></span>
- <span data-ttu-id="19ca1-751">Ordnungsgemäße Initialisierung der gespeicherten Set-UID und GID für die Binärdateien "Set-User-ID" und "Set-Group-ID" bei EXEC [GH 962, 1415, 2072]</span><span class="sxs-lookup"><span data-stu-id="19ca1-751">Correctly initialize saved-set uid and gid for set-user-ID and set-group-ID binaries on exec [GH 962, 1415, 2072]</span></span>
- <span data-ttu-id="19ca1-752">Hinzugefügte Unterstützung für ptrace PTRACE_O_TRACEEXIT [GH 555]</span><span class="sxs-lookup"><span data-stu-id="19ca1-752">Added support for ptrace PTRACE_O_TRACEEXIT [GH 555]</span></span>
- <span data-ttu-id="19ca1-753">Unterstützung für ptrace PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555] wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-753">Added support for ptrace PTRACE_GETFPREGS and PTRACE_GETREGSET with NT_FPREGSET [GH 555]</span></span>
- <span data-ttu-id="19ca1-754">Ptrace korrigiert, um bei ignorierten Signalen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="19ca1-754">Fixed ptrace to stop on ignored signals</span></span>
- <span data-ttu-id="19ca1-755">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-755">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-756">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-756">Console</span></span>
- <span data-ttu-id="19ca1-757">Keine Konsolen bezogenen Änderungen in dieser Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-757">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-758">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-758">LTP Results:</span></span>
<span data-ttu-id="19ca1-759">Anzahl der bestandenen Tests: 768</span><span class="sxs-lookup"><span data-stu-id="19ca1-759">Number of Passing Tests: 768</span></span></br>
<span data-ttu-id="19ca1-760">Anzahl der fehlgeschlagenen Tests: 244</span><span class="sxs-lookup"><span data-stu-id="19ca1-760">Number of Failing Tests: 244</span></span></br>
<span data-ttu-id="19ca1-761">Anzahl übersprungener Tests: 96</span><span class="sxs-lookup"><span data-stu-id="19ca1-761">Number of Skipped Tests: 96</span></span></br>
[<span data-ttu-id="19ca1-762">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-762">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a><span data-ttu-id="19ca1-763">Build 16241</span><span class="sxs-lookup"><span data-stu-id="19ca1-763">Build 16241</span></span>

<span data-ttu-id="19ca1-764">Allgemeine Windows-Informationen zu Build 16241 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-764">For general Windows information on build 16241 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-765">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-765">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="19ca1-766">WSL</span><span class="sxs-lookup"><span data-stu-id="19ca1-766">WSL</span></span>
- <span data-ttu-id="19ca1-767">In dieser Version gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-767">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="19ca1-768">Console</span><span class="sxs-lookup"><span data-stu-id="19ca1-768">Console</span></span>
- <span data-ttu-id="19ca1-769">Korrektur für die Ausgabe des falschen Zeichens für die Übergänge, die ursprünglich [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/) gemeldet wurden</span><span class="sxs-lookup"><span data-stu-id="19ca1-769">Fix for outputting the wrong character for the crossing-lines DEC, originally reported [here](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span></span>
- <span data-ttu-id="19ca1-770">Behebung, dass kein Ausgabetext in Codepage 65001 (UTF8) angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="19ca1-770">Fix for no output text being displayed in codepage 65001 (utf8)</span></span>
- <span data-ttu-id="19ca1-771">Übertragen Sie an den RGB-Werten einer Farbe vorgenommene Änderungen nicht an andere Teile der Palette bei Auswahl Änderungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-771">Do not transfer changes made to one color's RGB values to other parts of the palette on selection change.</span></span> <span data-ttu-id="19ca1-772">Dadurch wird die Verwendung des Konsolen Eigenschaften Blatts erheblich vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-772">This will make the console properties sheet a lot easier to use.</span></span>
- <span data-ttu-id="19ca1-773">STRG + S funktioniert anscheinend nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="19ca1-773">Ctrl+S doesn't appear to work correctly</span></span>
- <span data-ttu-id="19ca1-774">Unbold/-Dim in ANSI-Escapecodes vollständig nicht vorhanden [GH 2174]</span><span class="sxs-lookup"><span data-stu-id="19ca1-774">Un-Bold/-Dim completely absent from ANSI escape codes [GH 2174]</span></span>
- <span data-ttu-id="19ca1-775">Die Konsole unterstützt vim Color-Designs nicht ordnungsgemäß [GH 1706]</span><span class="sxs-lookup"><span data-stu-id="19ca1-775">Console doesn't correctly support Vim color themes [GH 1706]</span></span>
- <span data-ttu-id="19ca1-776">Bestimmte Zeichen können nicht eingefügt werden [GH 2149]</span><span class="sxs-lookup"><span data-stu-id="19ca1-776">Cannot paste particular characters [GH 2149]</span></span>
- <span data-ttu-id="19ca1-777">Die Größenänderung von reflows interagiert seltsam mit der Größenänderung eines bash-Fensters, wenn sich die Inhalte in der Bearbeitungs-/Befehlszeile befinden [GH-Verbindung 1123]</span><span class="sxs-lookup"><span data-stu-id="19ca1-777">Reflow resize interacts strangely with resizing a bash window when stuff is on the edit/command line [GH ConEmu 1123]</span></span>
- <span data-ttu-id="19ca1-778">STRG + L lässt den Bildschirm nicht geändert [GH 1978]</span><span class="sxs-lookup"><span data-stu-id="19ca1-778">Ctrl-L leaves the screen dirty [GH 1978]</span></span>
- <span data-ttu-id="19ca1-779">Fehler beim Rendern der Konsole beim Anzeigen von VT auf hdpi [GH 1907]</span><span class="sxs-lookup"><span data-stu-id="19ca1-779">Console rendering bug when displaying VT on HDPI [GH 1907]</span></span>
- <span data-ttu-id="19ca1-780">Japansese-Zeichen sehen seltsam mit Unicode-Zeichen U + 30FB [GH 2146]</span><span class="sxs-lookup"><span data-stu-id="19ca1-780">Japansese characters look strange with Unicode Character U+30FB [GH 2146]</span></span>
- <span data-ttu-id="19ca1-781">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-781">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16237"></a><span data-ttu-id="19ca1-782">Build 16237</span><span class="sxs-lookup"><span data-stu-id="19ca1-782">Build 16237</span></span>

<span data-ttu-id="19ca1-783">Allgemeine Windows-Informationen zu Build 16237 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-783">For general Windows information on build 16237 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-784">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-784">Fixed</span></span>
- <span data-ttu-id="19ca1-785">Standard Attribute für Dateien ohne EAS in lxfs verwenden (root, root, 0000)</span><span class="sxs-lookup"><span data-stu-id="19ca1-785">Use default attributes for files without EAs in lxfs (root, root, 0000)</span></span>
- <span data-ttu-id="19ca1-786">Unterstützung für Verteilungen mit erweiterten Attributen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-786">Added support for distributions that use extended attributes</span></span>
- <span data-ttu-id="19ca1-787">Korrigieren der Auffüll Zeichen für von getdents und getdents64 zurückgegebene Einträge</span><span class="sxs-lookup"><span data-stu-id="19ca1-787">Fix padding for entries returned by getdents and getdents64</span></span>
- <span data-ttu-id="19ca1-788">Korrektur der Berechtigungsüberprüfung für den shmctl SHM_STAT-Systembefehl [GH 2068]</span><span class="sxs-lookup"><span data-stu-id="19ca1-788">Fix permissions check for the shmctl SHM_STAT system call [GH 2068]</span></span>
- <span data-ttu-id="19ca1-789">Korrigiert falscher ursprünglicher epoll-Status für Schreib Telefone [GH 2231]</span><span class="sxs-lookup"><span data-stu-id="19ca1-789">Fixed incorrect initial epoll state for ttys [GH 2231]</span></span>
- <span data-ttu-id="19ca1-790">Korrigiert drvfs-Fehler beim Zurückgeben aller Einträge [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="19ca1-790">Fix DrvFs readdir not returning all entries [GH 2077]</span></span>
- <span data-ttu-id="19ca1-791">Korrigieren von lxfs-Nachrichten, wenn Dateien nicht verknüpft sind [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="19ca1-791">Fix LxFs readdir when files are unlinked [GH 2077]</span></span>
- <span data-ttu-id="19ca1-792">Wieder öffnen nicht verknüpfter drvfs-Dateien über procfs zulassen</span><span class="sxs-lookup"><span data-stu-id="19ca1-792">Allow unlinked drvfs files to be reopened through procfs</span></span>
- <span data-ttu-id="19ca1-793">Außer Kraft setzung des globalen Registrierungsschlüssels zum Deaktivieren von WSL-Features (Interop/Laufwerk Einbindung) wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-793">Added global registry key override for disabling WSL features (interop / drive mounting)</span></span>
- <span data-ttu-id="19ca1-794">Korrektur falscher Block Anzahl in "stat" für drvfs (und lxfs) [GH 1894]</span><span class="sxs-lookup"><span data-stu-id="19ca1-794">Fix incorrect block count in "stat" for DrvFs (and LxFs) [GH 1894]</span></span>
- <span data-ttu-id="19ca1-795">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-795">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16232"></a><span data-ttu-id="19ca1-796">Build 16232</span><span class="sxs-lookup"><span data-stu-id="19ca1-796">Build 16232</span></span>

<span data-ttu-id="19ca1-797">Allgemeine Windows-Informationen zu Build 16232 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-797">For general Windows information on build 16232 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-798">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-798">Fixed</span></span>
- <span data-ttu-id="19ca1-799">In dieser Version gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-799">No WSL related changes in this release.</span></span>

</br>

## <a name="build-16226"></a><span data-ttu-id="19ca1-800">Build 16226</span><span class="sxs-lookup"><span data-stu-id="19ca1-800">Build 16226</span></span>

<span data-ttu-id="19ca1-801">Allgemeine Windows-Informationen zu Build 16226 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-801">For general Windows information on build 16226 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-802">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-802">Fixed</span></span>
- <span data-ttu-id="19ca1-803">Unterstützung von xattr-bezogenen syscalls (getxattr, setxattr, listxattr, removexattr).</span><span class="sxs-lookup"><span data-stu-id="19ca1-803">xattr related syscalls support (getxattr, setxattr, listxattr, removexattr).</span></span>
- <span data-ttu-id="19ca1-804">Security. capablity xattr-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="19ca1-804">security.capablity xattr support.</span></span>
- <span data-ttu-id="19ca1-805">Verbesserte Kompatibilität mit bestimmten Dateisystemen und Filtern, einschließlich nicht-MS-SMB-Servern.</span><span class="sxs-lookup"><span data-stu-id="19ca1-805">Improved compatibility with certain file systems and filters, including non-MS SMB servers.</span></span> <span data-ttu-id="19ca1-806">[GH #1952]</span><span class="sxs-lookup"><span data-stu-id="19ca1-806">[GH #1952]</span></span>
- <span data-ttu-id="19ca1-807">Verbesserte Unterstützung für onedrive-Platzhalter, gvfs-Platzhalter und komprimierte Compact OS-Dateien.</span><span class="sxs-lookup"><span data-stu-id="19ca1-807">Improved support for OneDrive placeholders, GVFS placeholders, and Compact OS compressed files.</span></span>
- <span data-ttu-id="19ca1-808">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-808">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16215"></a><span data-ttu-id="19ca1-809">Build 16215</span><span class="sxs-lookup"><span data-stu-id="19ca1-809">Build 16215</span></span>

<span data-ttu-id="19ca1-810">Allgemeine Windows-Informationen zu Build 16215 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-810">For general Windows information on build 16215 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-811">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-811">Fixed</span></span>
- <span data-ttu-id="19ca1-812">Für WSL ist der Entwicklermodus nicht mehr erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19ca1-812">WSL no longer requires developer mode.</span></span>
- <span data-ttu-id="19ca1-813">Unterstützung von Verzeichnis Verbindungen in drvfs.</span><span class="sxs-lookup"><span data-stu-id="19ca1-813">Support directory junctions in drvfs.</span></span>
- <span data-ttu-id="19ca1-814">Die Installation von AppX-Paketen der WSL-Verteilung wird durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-814">Handle uninstalling of WSL distribution appx packages.</span></span>
- <span data-ttu-id="19ca1-815">Aktualisieren Sie procfs, um private und freigegebene Zuordnungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-815">Update procfs to show private and shared mappings.</span></span>
- <span data-ttu-id="19ca1-816">Fügen Sie "wslconfig. exe" die Möglichkeit hinzu, Verteilungen zu bereinigen, die teilweise installiert oder deinstalliert wurden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-816">Add ability for wslconfig.exe to clean up distributions that are partially installed or uninstalled.</span></span>
- <span data-ttu-id="19ca1-817">Unterstützung für IP_MTU_DISCOVER für TCP-Sockets hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-817">Added support for IP_MTU_DISCOVER for TCP sockets.</span></span> <span data-ttu-id="19ca1-818">[GH 1639, 2115, 2205]</span><span class="sxs-lookup"><span data-stu-id="19ca1-818">[GH 1639, 2115, 2205]</span></span>
- <span data-ttu-id="19ca1-819">Leiten Sie die Protokollfamilie für Routen zu AF_INADDR ein.</span><span class="sxs-lookup"><span data-stu-id="19ca1-819">Infer protocol family for routes to AF_INADDR.</span></span>
- <span data-ttu-id="19ca1-820">Verbesserungen an seriellen Geräten [GH 1929].</span><span class="sxs-lookup"><span data-stu-id="19ca1-820">Serial device improvements [GH 1929].</span></span>

</br>

## <a name="build-16199"></a><span data-ttu-id="19ca1-821">Build 16199</span><span class="sxs-lookup"><span data-stu-id="19ca1-821">Build 16199</span></span>

<span data-ttu-id="19ca1-822">Allgemeine Windows-Informationen zu Build 16199 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-822">For general Windows information on build 16199 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-823">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-823">Fixed</span></span>
- <span data-ttu-id="19ca1-824">Keine WSL-bezogenen Änderungen in diesen Releases.</span><span class="sxs-lookup"><span data-stu-id="19ca1-824">No WSL related changes in these releases.</span></span>

</br>

## <a name="build-16193"></a><span data-ttu-id="19ca1-825">Build 16193</span><span class="sxs-lookup"><span data-stu-id="19ca1-825">Build 16193</span></span>

<span data-ttu-id="19ca1-826">Allgemeine Windows-Informationen zu Build 16193 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-826">For general Windows information on build 16193 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-827">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-827">Fixed</span></span>
- <span data-ttu-id="19ca1-828">Racebedingung zwischen dem Senden von sigtt und einer Thread Gruppe, die beendet wird [GH 1973]</span><span class="sxs-lookup"><span data-stu-id="19ca1-828">Race condition between sending SIGCONT and a threadgroup terminating [GH 1973]</span></span>
- <span data-ttu-id="19ca1-829">Ändern von TTY-und Pty-Geräten in Report FILE_DEVICE_NAMED_PIPE anstelle von FILE_DEVICE_CONSOLE [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="19ca1-829">change tty and pty devices to report FILE_DEVICE_NAMED_PIPE instead of FILE_DEVICE_CONSOLE [GH 1840]</span></span>
- <span data-ttu-id="19ca1-830">SSH-Fix für IP_OPTIONS</span><span class="sxs-lookup"><span data-stu-id="19ca1-830">SSH fix for IP_OPTIONS</span></span>
- <span data-ttu-id="19ca1-831">Verschieben der drvfs-Einbindung in den init-Daemon [GH 1862, 1968, 1767, 1933]</span><span class="sxs-lookup"><span data-stu-id="19ca1-831">Moved DrvFs mounting to init daemon [GH 1862, 1968, 1767, 1933]</span></span>
- <span data-ttu-id="19ca1-832">Unterstützung in drvfs wurde für die folgenden NT-symlinks hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-832">Added support in DrvFs for following NT symlinks.</span></span>

</br>

## <a name="build-16184"></a><span data-ttu-id="19ca1-833">Build 16184</span><span class="sxs-lookup"><span data-stu-id="19ca1-833">Build 16184</span></span>

<span data-ttu-id="19ca1-834">Allgemeine Windows-Informationen zu Build 16184 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-834">For general Windows information on build 16184 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-835">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-835">Fixed</span></span>
- <span data-ttu-id="19ca1-836">Der Task "apt Package Maintenance" (lxrun. exe/Update) wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-836">Removed apt package maintenance task (lxrun.exe /update)</span></span>
- <span data-ttu-id="19ca1-837">In "Node. js" wird eine Fehlerausgabe, die von Windows-Prozessen in Node. 1840 js nicht angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="19ca1-837">Fixed output not showing up in from Windows processes in node.js [GH 1840]</span></span>
- <span data-ttu-id="19ca1-838">Lockern der Ausrichtungs Anforderungen in lxcore [GH 1794]</span><span class="sxs-lookup"><span data-stu-id="19ca1-838">Relax alignment requirements in lxcore [GH 1794]</span></span>
- <span data-ttu-id="19ca1-839">Korrigiert der Behandlung des AT_EMPTY_PATH-Flags in einem Zahl von Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-839">Fixed handling of the AT_EMPTY_PATH flag in a numer of system calls.</span></span>
- <span data-ttu-id="19ca1-840">Problem behoben, bei dem das Löschen von drvfs-Dateien mit geöffneten Handles bewirkt, dass die Datei nicht definiertes Verhalten aufweist [GH 544, 966, 1357, 1535, 1615]</span><span class="sxs-lookup"><span data-stu-id="19ca1-840">Fixed issue where deleting DrvFs files with open handles will cause the file to exhibit undefined behavior [GH 544,966,1357,1535,1615]</span></span>
- <span data-ttu-id="19ca1-841">"/etc/hosts" erbt nun Einträge von der Windows-Hostdatei (%windir%\system32\drivers\etc\hosts) [GH 1495]</span><span class="sxs-lookup"><span data-stu-id="19ca1-841">/etc/hosts will now inherit entries from the Windows hosts file (%windir%\system32\drivers\etc\hosts) [GH 1495]</span></span>

</br>

## <a name="build-16179"></a><span data-ttu-id="19ca1-842">Build 16179</span><span class="sxs-lookup"><span data-stu-id="19ca1-842">Build 16179</span></span>

<span data-ttu-id="19ca1-843">Allgemeine Windows-Informationen zu Build 16179 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-843">For general Windows information on build 16179 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-844">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-844">Fixed</span></span>
- <span data-ttu-id="19ca1-845">In dieser Woche ändert sich keine WSL-Datei.</span><span class="sxs-lookup"><span data-stu-id="19ca1-845">No WSL changes this week.</span></span>

</br>

## <a name="build-16176"></a><span data-ttu-id="19ca1-846">Build 16176</span><span class="sxs-lookup"><span data-stu-id="19ca1-846">Build 16176</span></span>

<span data-ttu-id="19ca1-847">Allgemeine Windows-Informationen zu Build 16176 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-847">For general Windows information on build 16176 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-848">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-848">Fixed</span></span>

- [<span data-ttu-id="19ca1-849">Aktivierte serielle Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-849">Enabled serial support</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- <span data-ttu-id="19ca1-850">Hinzugefügte IP-Socketoption IP_OPTIONS [GH 1116]</span><span class="sxs-lookup"><span data-stu-id="19ca1-850">Added IP socket option IP_OPTIONS [GH 1116]</span></span>
- <span data-ttu-id="19ca1-851">Implementierte pschreitev-Funktion (beim Hochladen der Datei nach nginx/php-FPM) [GH 1506]</span><span class="sxs-lookup"><span data-stu-id="19ca1-851">Implemented pwritev function (while uploading file to nginx/PHP-FPM) [GH 1506]</span></span>
- <span data-ttu-id="19ca1-852">Hinzugefügte IP-Socket-Optionen IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span><span class="sxs-lookup"><span data-stu-id="19ca1-852">Added IP socket options IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span></span>
- <span data-ttu-id="19ca1-853">Unterstützung für Socketoption IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="19ca1-853">Support for socket option IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span></span>
- <span data-ttu-id="19ca1-854">Added IP (V6) _MTU Socketoption für den Knoten apps, traceroute, Dig, nslookup, Host</span><span class="sxs-lookup"><span data-stu-id="19ca1-854">Added IP(V6)_MTU socket option for apps node, traceroute, dig, nslookup, host</span></span>
- <span data-ttu-id="19ca1-855">IP-Socketoption IPV6_UNICAST_HOPS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-855">Added IP socket option IPV6_UNICAST_HOPS</span></span>
- [<span data-ttu-id="19ca1-856">Dateisystem Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-856">Filesystem Improvements</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * <span data-ttu-id="19ca1-857">Einbinden von UNC-Pfaden zulassen</span><span class="sxs-lookup"><span data-stu-id="19ca1-857">Allow mounting of UNC paths</span></span>
    * <span data-ttu-id="19ca1-858">Aktivieren der CDFS-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="19ca1-858">Enable CDFS support in drvfs</span></span>
    * <span data-ttu-id="19ca1-859">Ordnungsgemäße Handhabung von Berechtigungen für Netzwerkdatei Systeme in drvfs</span><span class="sxs-lookup"><span data-stu-id="19ca1-859">Correctly handle permissions for network file systems in drvfs</span></span>
    * <span data-ttu-id="19ca1-860">Unterstützung für Remote Laufwerke zu drvfs hinzufügen</span><span class="sxs-lookup"><span data-stu-id="19ca1-860">Add support for remote drives to drvfs</span></span>
    * <span data-ttu-id="19ca1-861">Aktivieren der FAT-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="19ca1-861">Enable FAT support in drvfs</span></span>
- <span data-ttu-id="19ca1-862">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-862">Additional fixes and Improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-863">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="19ca1-863">LTP Results</span></span>
<span data-ttu-id="19ca1-864">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="19ca1-864">No changes since 15042</span></span>

</br>

## <a name="build-16170"></a><span data-ttu-id="19ca1-865">Build 16170</span><span class="sxs-lookup"><span data-stu-id="19ca1-865">Build 16170</span></span>

<span data-ttu-id="19ca1-866">Allgemeine Windows-Informationen zu Build 16170 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-866">For general Windows information on build 16170 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span></span><br/>

<span data-ttu-id="19ca1-867">Wir haben einen neuen [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) veröffentlicht, der unsere Anstrengungen zum Testen von WSL erörtert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-867">We released a new [blog post](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) discussing our efforts to test WSL.</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-868">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-868">Fixed</span></span>

- <span data-ttu-id="19ca1-869">Support Socketoption IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="19ca1-869">Support socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span></span>
- <span data-ttu-id="19ca1-870">Unterstützung für PTRACE_OLDSETOPTIONS hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-870">Add support for PTRACE_OLDSETOPTIONS.</span></span> <span data-ttu-id="19ca1-871">[GH 1692]</span><span class="sxs-lookup"><span data-stu-id="19ca1-871">[GH 1692]</span></span>
- <span data-ttu-id="19ca1-872">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-872">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-873">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="19ca1-873">LTP Results</span></span>
<span data-ttu-id="19ca1-874">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="19ca1-874">No changes since 15042</span></span>

</br>

## <a name="build-15046-to-windows-10-creators-update"></a><span data-ttu-id="19ca1-875">Build 15046 mit Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="19ca1-875">Build 15046 to Windows 10 Creators Update</span></span>
<span data-ttu-id="19ca1-876">Es gibt keine weiteren WSL-Korrekturen oder-Funktionen, die für die Einbindung in das Creators Update in Windows 10 geplant sind.</span><span class="sxs-lookup"><span data-stu-id="19ca1-876">There are no more WSL fixes or features planned for inclusion in the Creators Update to Windows 10.</span></span> <span data-ttu-id="19ca1-877">Die Anmerkungen zu dieser Version von WSL werden in den kommenden Wochen fortgesetzt, um Ergänzungen für die nächsten Haupt Windows Update zu Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-877">Release notes for WSL will resume in the coming weeks for additions targeting the next major Windows Update.</span></span> <span data-ttu-id="19ca1-878">Allgemeine Windows-Informationen zu Build 15046 und zukünftigen Insider Releases finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-878">For general Windows information on build 15046 and future Insider releases visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span></span> <br/><br/>
 <br/>

## <a name="build-15042"></a><span data-ttu-id="19ca1-879">Build 15042</span><span class="sxs-lookup"><span data-stu-id="19ca1-879">Build 15042</span></span>

<span data-ttu-id="19ca1-880">Allgemeine Windows-Informationen zu Build 15042 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-880">For general Windows information on build 15042 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-881">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-881">Fixed</span></span>

- <span data-ttu-id="19ca1-882">Behebung eines Deadlocks beim Entfernen eines Pfades, der in ".." endet</span><span class="sxs-lookup"><span data-stu-id="19ca1-882">Fix for a deadlock when removing a path ending in ".."</span></span>
- <span data-ttu-id="19ca1-883">Es wurde ein Problem behoben, bei dem "fonbio" bei 1683 Erfolg "0" nicht zurückgibt</span><span class="sxs-lookup"><span data-stu-id="19ca1-883">Fixed an issue where FIONBIO not returning 0 on success [GH 1683]</span></span>
- <span data-ttu-id="19ca1-884">Problem bei Lesevorgängen mit einer Länge von inet-Datagramm-Sockets</span><span class="sxs-lookup"><span data-stu-id="19ca1-884">Fixed issue with zero-length reads of inet datagram sockets</span></span>
- <span data-ttu-id="19ca1-885">Behebung eines möglichen Deadlocks aufgrund einer Racebedingung in der drvfs-tatsächliche-Suche [GH 1675]</span><span class="sxs-lookup"><span data-stu-id="19ca1-885">Fix possible deadlock due to race condition in drvfs inode lookup [GH 1675]</span></span>
- <span data-ttu-id="19ca1-886">Erweiterte Unterstützung für UNIX-sockethilfdaten; SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613, 1326]</span><span class="sxs-lookup"><span data-stu-id="19ca1-886">Extended support for unix socket ancillary data; SCM_CREDENTIALS and SCM_RIGHTS [GH 514, 613, 1326]</span></span>
- <span data-ttu-id="19ca1-887">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-887">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-888">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-888">LTP Results:</span></span>
<span data-ttu-id="19ca1-889">Anzahl der bestandenen Tests: 737</span><span class="sxs-lookup"><span data-stu-id="19ca1-889">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="19ca1-890">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="19ca1-890">Number of non-Passing (failing, skipped, etc…): 255</span></span>

</br>

## <a name="build-15031"></a><span data-ttu-id="19ca1-891">Build 15031</span><span class="sxs-lookup"><span data-stu-id="19ca1-891">Build 15031</span></span>

<span data-ttu-id="19ca1-892">Allgemeine Windows-Informationen zu Build 15031 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-892">For general Windows information on build 15031 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-893">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-893">Fixed</span></span>

- <span data-ttu-id="19ca1-894">Es wurde ein Fehler behoben, bei dem sich die Zeit (2) sporadisch nicht verhält.</span><span class="sxs-lookup"><span data-stu-id="19ca1-894">Fixed a bug where time(2) would sporadically misbehave.</span></span>
- <span data-ttu-id="19ca1-895">Korrigiert und Problem, dass die Signal Maske von \* sigprocmask-syscalls beschädigt werden konnte.</span><span class="sxs-lookup"><span data-stu-id="19ca1-895">Fixed and issue where \*SIGPROCMASK syscalls could corrupt signal mask.</span></span>
- <span data-ttu-id="19ca1-896">Gibt jetzt die vollständige Befehlszeilen Länge in der WSL-Prozess Erstellungs Benachrichtigung zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-896">Now return full command line length in WSL process creation notification.</span></span> <span data-ttu-id="19ca1-897">[GH 1632]</span><span class="sxs-lookup"><span data-stu-id="19ca1-897">[GH 1632]</span></span>
- <span data-ttu-id="19ca1-898">WSL meldet jetzt die Thread Exit-über-ptrace für gdb-Abstürze.</span><span class="sxs-lookup"><span data-stu-id="19ca1-898">WSL now reports thread exit through ptrace for GDB hangs.</span></span> <span data-ttu-id="19ca1-899">[GH 1196]</span><span class="sxs-lookup"><span data-stu-id="19ca1-899">[GH 1196]</span></span>
- <span data-ttu-id="19ca1-900">Es wurde ein Fehler behoben, bei dem PTYs nach hoher tmux-e/a hängen</span><span class="sxs-lookup"><span data-stu-id="19ca1-900">Fixed bug where ptys would hang after heavy tmux IO.</span></span> <span data-ttu-id="19ca1-901">[GH 1358]</span><span class="sxs-lookup"><span data-stu-id="19ca1-901">[GH 1358]</span></span>
- <span data-ttu-id="19ca1-902">Korrigieren der Timeout Validierung in vielen Systemaufrufen (Futex, SEMTIMEDOP, ppoll, sigtimedwait, itimer, timer_create)</span><span class="sxs-lookup"><span data-stu-id="19ca1-902">Fixed timeout validation in many system calls (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span></span>
- <span data-ttu-id="19ca1-903">Hinzugefügte eventfd EFD_SEMAPHORE-Unterstützung [GH 452]</span><span class="sxs-lookup"><span data-stu-id="19ca1-903">Added eventfd EFD_SEMAPHORE support [GH 452]</span></span>
- <span data-ttu-id="19ca1-904">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-904">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-905">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-905">LTP Results:</span></span>
<span data-ttu-id="19ca1-906">Anzahl der bestandenen Tests: 737</span><span class="sxs-lookup"><span data-stu-id="19ca1-906">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="19ca1-907">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="19ca1-907">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="19ca1-908">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-908">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a><span data-ttu-id="19ca1-909">Build 15025</span><span class="sxs-lookup"><span data-stu-id="19ca1-909">Build 15025</span></span>

<span data-ttu-id="19ca1-910">Allgemeine Windows-Informationen zu Build 15025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-910">For general Windows information on build 15025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-911">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-911">Fixed</span></span>

- <span data-ttu-id="19ca1-912">Behebung von Fehlern, bei denen die grep 2,27 [GH 1578] abgebrochen wurde</span><span class="sxs-lookup"><span data-stu-id="19ca1-912">Fix for bug that broke grep 2.27 [GH 1578]</span></span>
- <span data-ttu-id="19ca1-913">Implementiertes EFD_SEMAPHORE-Flag für eventfd2 syscall [GH 452]</span><span class="sxs-lookup"><span data-stu-id="19ca1-913">Implemented EFD_SEMAPHORE flag for eventfd2 syscall [GH 452]</span></span>
- <span data-ttu-id="19ca1-914">Implementiertes/proc/[PID]/NET/ipv6_route [GH 1608]</span><span class="sxs-lookup"><span data-stu-id="19ca1-914">Implemented /proc/[pid]/net/ipv6_route [GH 1608]</span></span>
- <span data-ttu-id="19ca1-915">Signal gestützte IO-Unterstützung für UNIX-Streamsockets [GH 393, 68]</span><span class="sxs-lookup"><span data-stu-id="19ca1-915">Signal driven IO support for unix stream sockets [GH 393, 68]</span></span>
- <span data-ttu-id="19ca1-916">Support F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]</span><span class="sxs-lookup"><span data-stu-id="19ca1-916">Support F_GETPIPE_SZ and F_SETPIPE_SZ [GH 1012]</span></span>
- <span data-ttu-id="19ca1-917">Implementieren von recvmmsg () syscall [GH 1531]</span><span class="sxs-lookup"><span data-stu-id="19ca1-917">Implement recvmmsg() syscall [GH 1531]</span></span>
- <span data-ttu-id="19ca1-918">Fehler behoben, bei dem epoll_wait () nicht gewartet hat [GH 1609]</span><span class="sxs-lookup"><span data-stu-id="19ca1-918">Fixed bug where epoll_wait() wasn't waiting [GH 1609]</span></span>
- <span data-ttu-id="19ca1-919">Implementieren von/proc/version_signature</span><span class="sxs-lookup"><span data-stu-id="19ca1-919">Implement /proc/version_signature</span></span>
- <span data-ttu-id="19ca1-920">Tee syscall gibt jetzt einen Fehler zurück, wenn beide Dateideskriptoren auf dieselbe Pipe verweisen</span><span class="sxs-lookup"><span data-stu-id="19ca1-920">Tee syscall now returns failure if both file descriptors refer to the same pipe</span></span>
- <span data-ttu-id="19ca1-921">Implementiertes korrektes Verhalten für SO_PEERCRED für UNIX-Sockets</span><span class="sxs-lookup"><span data-stu-id="19ca1-921">Implemented correct behavior for SO_PEERCRED for Unix sockets</span></span>
- <span data-ttu-id="19ca1-922">Korrigieren der Behandlung von ungültigen tkill syscall-Parametern</span><span class="sxs-lookup"><span data-stu-id="19ca1-922">Fixed tkill syscall invalid parameter handling</span></span>
- <span data-ttu-id="19ca1-923">Änderungen zum Vergrößern des vorformace von drvfs</span><span class="sxs-lookup"><span data-stu-id="19ca1-923">Changes to increase the preformace of drvfs</span></span>
- <span data-ttu-id="19ca1-924">Kleinere Behebung für Ruby IO-Blockierung</span><span class="sxs-lookup"><span data-stu-id="19ca1-924">Minor fix for Ruby IO blocking</span></span>
- <span data-ttu-id="19ca1-925">Korrigieren von recvmsg () beim Zurückgeben von EINVAL für das MSG_DONTWAIT-Flag für inet Sockets [GH 1296]</span><span class="sxs-lookup"><span data-stu-id="19ca1-925">Fixed recvmsg() returning EINVAL for the MSG_DONTWAIT flag for inet sockets [GH 1296]</span></span>
- <span data-ttu-id="19ca1-926">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-926">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-927">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-927">LTP Results:</span></span>
<span data-ttu-id="19ca1-928">Anzahl der bestandenen Tests: 732</span><span class="sxs-lookup"><span data-stu-id="19ca1-928">Number of Passing Test: 732</span></span></br>
<span data-ttu-id="19ca1-929">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="19ca1-929">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="19ca1-930">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-930">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a><span data-ttu-id="19ca1-931">Build 15019</span><span class="sxs-lookup"><span data-stu-id="19ca1-931">Build 15019</span></span>

<span data-ttu-id="19ca1-932">Allgemeine Windows-Informationen zu Build 15019 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-932">For general Windows information on build 15019 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-933">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-933">Fixed</span></span>

- <span data-ttu-id="19ca1-934">Es wurde ein Fehler behoben, der fälschlicherweise die CPU-Auslastung in procfs für Tools wie htop (GH 823, 945, 971) gemeldet hat.</span><span class="sxs-lookup"><span data-stu-id="19ca1-934">Fixed bug that incorrectly reported CPU usage in procfs for tools like htop (GH 823, 945, 971)</span></span>
- <span data-ttu-id="19ca1-935">Beim Aufrufen von "Open () with O_TRUNC" für eine vorhandene Datei "inotify" generiert nun IN_MODIFY vor IN_OPEN</span><span class="sxs-lookup"><span data-stu-id="19ca1-935">When calling open() with O_TRUNC on an existing file inotify now generates IN_MODIFY before IN_OPEN</span></span>
- <span data-ttu-id="19ca1-936">Fehlerbehebungen für den UNIX-Socket getsockopt SO_ERROR zum Aktivieren des Postgress [GH 61, 1354]</span><span class="sxs-lookup"><span data-stu-id="19ca1-936">Fixes to unix socket getsockopt SO_ERROR to enable postgress [GH 61, 1354]</span></span>
- <span data-ttu-id="19ca1-937">Implementieren von/proc/sys/net/Core/somaxconn für die Sprache go</span><span class="sxs-lookup"><span data-stu-id="19ca1-937">Implement /proc/sys/net/core/somaxconn for the GO language</span></span>
- <span data-ttu-id="19ca1-938">Apt-get Package Update background-Task wird jetzt ausgeblendet aus der Ansicht</span><span class="sxs-lookup"><span data-stu-id="19ca1-938">Apt-get package update background task now runs hidden from view</span></span>
- <span data-ttu-id="19ca1-939">Löschen Sie den Bereich für IPv6 localhost (Spring-Framework (Java)-Fehler).</span><span class="sxs-lookup"><span data-stu-id="19ca1-939">Clear scope for ipv6 localhost (Spring-Framework(Java) failure).</span></span>
- <span data-ttu-id="19ca1-940">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-940">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-941">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-941">LTP Results:</span></span>
<span data-ttu-id="19ca1-942">Anzahl der bestandenen Tests: 714</span><span class="sxs-lookup"><span data-stu-id="19ca1-942">Number of Passing Test: 714</span></span> </br>
<span data-ttu-id="19ca1-943">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 249</span><span class="sxs-lookup"><span data-stu-id="19ca1-943">Number of non-Passing (failing, skipped, etc…): 249</span></span> </br>
[<span data-ttu-id="19ca1-944">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-944">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a><span data-ttu-id="19ca1-945">Build 15014</span><span class="sxs-lookup"><span data-stu-id="19ca1-945">Build 15014</span></span>

<span data-ttu-id="19ca1-946">Allgemeine Windows-Informationen zu Build 15014 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="19ca1-946">For general Windows information on build 15014 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-947">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-947">Fixed</span></span>

- <span data-ttu-id="19ca1-948">STRG + C funktioniert nun wie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="19ca1-948">Ctrl+C now works as intended</span></span>
- <span data-ttu-id="19ca1-949">htop und PS-Lösung zeigen jetzt die korrekte Ressourcenverwendung an (GH #516)</span><span class="sxs-lookup"><span data-stu-id="19ca1-949">htop and ps auxw now show correct resource utilization (GH #516)</span></span>
- <span data-ttu-id="19ca1-950">Grundlegende Übersetzung von NT-Ausnahmen in Signale.</span><span class="sxs-lookup"><span data-stu-id="19ca1-950">Basic translation of NT exceptions to signals.</span></span> <span data-ttu-id="19ca1-951">(GH #513)</span><span class="sxs-lookup"><span data-stu-id="19ca1-951">(GH #513)</span></span>
- <span data-ttu-id="19ca1-952">bei der Aufhebung der Speicherplatz Ausführung von "ENOSPC" tritt nun ein Fehler auf, wenn nicht mehr als EINVAL (GH #1571)</span><span class="sxs-lookup"><span data-stu-id="19ca1-952">fallocate now fails with ENOSPC  when running out of space instead of EINVAL (GH #1571)</span></span>
- <span data-ttu-id="19ca1-953">/Proc/sys/kernel/SEM. hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-953">Added /proc/sys/kernel/sem.</span></span>
- <span data-ttu-id="19ca1-954">Implementierte semop-und SEMTIMEDOP-Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="19ca1-954">Implemented semop and semtimedop system calls</span></span>
- <span data-ttu-id="19ca1-955">Korrigiert nslookup-Fehler mit der Option IP_RECVTOS & IPV6_RECVTCLASS Socket (GH 69)</span><span class="sxs-lookup"><span data-stu-id="19ca1-955">Fixed nslookup errors with IP_RECVTOS & IPV6_RECVTCLASS socket option (GH 69)</span></span>
- <span data-ttu-id="19ca1-956">Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT</span><span class="sxs-lookup"><span data-stu-id="19ca1-956">Support for socket options IP_RECVTTL and IPV6_RECVHOPLIMIT</span></span>
- <span data-ttu-id="19ca1-957">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-957">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-958">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-958">LTP Results:</span></span>
<span data-ttu-id="19ca1-959">Anzahl der bestandenen Tests: 709</span><span class="sxs-lookup"><span data-stu-id="19ca1-959">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="19ca1-960">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="19ca1-960">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="19ca1-961">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-961">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a><span data-ttu-id="19ca1-962">Syscall-Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="19ca1-962">Syscall Summary</span></span>
<span data-ttu-id="19ca1-963">Gesamtanzahl der syscalls: 384</span><span class="sxs-lookup"><span data-stu-id="19ca1-963">Total Syscalls: 384</span></span> </br>
<span data-ttu-id="19ca1-964">Implementiertes gesamt: 235</span><span class="sxs-lookup"><span data-stu-id="19ca1-964">Total Implemented: 235</span></span> </br>
<span data-ttu-id="19ca1-965">Stub gesamt: 22</span><span class="sxs-lookup"><span data-stu-id="19ca1-965">Total Stubbed: 22</span></span> </br>
<span data-ttu-id="19ca1-966">Nicht implementiert gesamt: 127</span><span class="sxs-lookup"><span data-stu-id="19ca1-966">Total Unimplemented: 127</span></span> </br>
[<span data-ttu-id="19ca1-967">Ausführliche Aufschlüsselung</span><span class="sxs-lookup"><span data-stu-id="19ca1-967">Detailed Breakdown</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a><span data-ttu-id="19ca1-968">Build 15007</span><span class="sxs-lookup"><span data-stu-id="19ca1-968">Build 15007</span></span>

<span data-ttu-id="19ca1-969">Allgemeine Windows-Informationen zu Build 15007 finden Sie im [Windows-Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span><span class="sxs-lookup"><span data-stu-id="19ca1-969">For general Windows information on build 15007 visit the [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="19ca1-970">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="19ca1-970">Known Issue</span></span>

- <span data-ttu-id="19ca1-971">Es gibt einen bekannten Fehler, bei dem die Konsole eine STRG + <key> Eingabe nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-971">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="19ca1-972">Dies schließt den Strg-c-Befehl ein, der als normales ' c '-KeyPress fungiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-972">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="19ca1-973">Problemumgehung: Ordnen Sie einen alternativen Schlüssel zu STRG + C zu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-973">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="19ca1-974">Um z. b. STRG + K zu STRG + C zuzuordnen, `stty intr \^k`führen Sie Folgendes aus:.</span><span class="sxs-lookup"><span data-stu-id="19ca1-974">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="19ca1-975">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-975">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="19ca1-976">Benutzer können die Option zum Einbeziehen der`.bashrc`</span><span class="sxs-lookup"><span data-stu-id="19ca1-976">Users can explore the option to include this in their `.bashrc`</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-977">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-977">Fixed</span></span>

- <span data-ttu-id="19ca1-978">Das Problem wurde behoben, bei dem die Ausführung von WSL 100% eines CPU-Kerns verbraucht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-978">Corrected the issue where running WSL would consume 100% of a CPU core</span></span>
- <span data-ttu-id="19ca1-979">Socketoption IP_PKTINFO, IPV6_RECVPKTINFO wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-979">Socket option IP_PKTINFO, IPV6_RECVPKTINFO now supported.</span></span> <span data-ttu-id="19ca1-980">(GH #851, 987)</span><span class="sxs-lookup"><span data-stu-id="19ca1-980">(GH #851, 987)</span></span>
- <span data-ttu-id="19ca1-981">Die physische Adresse der Netzwerkschnittstelle wird in lxcore (GH #1452, 1414, 1343, 468, 308) auf 16 Bytes abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-981">Truncate network interface physical address to 16 bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span></span>
- <span data-ttu-id="19ca1-982">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-982">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-983">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-983">LTP Results:</span></span>
<span data-ttu-id="19ca1-984">Anzahl der bestandenen Tests: 709</span><span class="sxs-lookup"><span data-stu-id="19ca1-984">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="19ca1-985">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="19ca1-985">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="19ca1-986">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-986">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a><span data-ttu-id="19ca1-987">Build 15002</span><span class="sxs-lookup"><span data-stu-id="19ca1-987">Build 15002</span></span>

<span data-ttu-id="19ca1-988">Allgemeine Windows-Informationen zu Build 15002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-988">For general Windows information on build 15002 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="19ca1-989">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="19ca1-989">Known Issue</span></span>

<span data-ttu-id="19ca1-990">Zwei bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="19ca1-990">Two known issues:</span></span>
- <span data-ttu-id="19ca1-991">Es gibt einen bekannten Fehler, bei dem die Konsole eine STRG + <key> Eingabe nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-991">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="19ca1-992">Dies schließt den Strg-c-Befehl ein, der als normales ' c '-KeyPress fungiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-992">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="19ca1-993">Problemumgehung: Ordnen Sie einen alternativen Schlüssel zu STRG + C zu.</span><span class="sxs-lookup"><span data-stu-id="19ca1-993">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="19ca1-994">Um z. b. STRG + K zu STRG + C zuzuordnen, `stty intr \^k`führen Sie Folgendes aus:.</span><span class="sxs-lookup"><span data-stu-id="19ca1-994">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="19ca1-995">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-995">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="19ca1-996">Benutzer können die Option zum Einbeziehen der`.bashrc`</span><span class="sxs-lookup"><span data-stu-id="19ca1-996">Users can explore the option to include this in their `.bashrc`</span></span>

- <span data-ttu-id="19ca1-997">Während der Ausführung von WSL werden von einem System Thread 100% eines CPU-Kerns beansprucht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-997">While WSL is running a system thread will consume 100% of a CPU core.</span></span>  <span data-ttu-id="19ca1-998">Die Ursache wurde intern behoben und behoben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-998">The root cause has been addressed and fixed internally.</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-999">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-999">Fixed</span></span>

- <span data-ttu-id="19ca1-1000">Alle bash-Sitzungen müssen jetzt auf derselben Berechtigungsebene erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1000">All bash sessions must now be created at the same permission level.</span></span>  <span data-ttu-id="19ca1-1001">Der Versuch, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1001">Attempting to start a session at a different level will be blocked.</span></span>  <span data-ttu-id="19ca1-1002">Dies bedeutet, dass Administrator-und nicht-Administrator Konsolen nicht gleichzeitig ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1002">This means admin and non-admin consoles cannot run at the same time.</span></span> <span data-ttu-id="19ca1-1003">(GH #626)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1003">(GH #626)</span></span>
<br/>
- <span data-ttu-id="19ca1-1004">Die folgenden NETLINK_ROUTE-Nachrichten wurden implementiert (erfordert Windows-Administrator).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1004">Implemented the following NETLINK_ROUTE messages (requires Windows admin)</span></span>
     - <span data-ttu-id="19ca1-1005">RTM_NEWADDR (unter `ip addr add`stützt)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1005">RTM_NEWADDR (supports `ip addr add`)</span></span>
     - <span data-ttu-id="19ca1-1006">RTM_NEWROUTE (unter `ip route add`stützt)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1006">RTM_NEWROUTE (supports `ip route add`)</span></span>
     - <span data-ttu-id="19ca1-1007">RTM_DELADDR (unter `ip addr del`stützt)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1007">RTM_DELADDR (supports `ip addr del`)</span></span>
     - <span data-ttu-id="19ca1-1008">RTM_DELROUTE (unter `ip route del`stützt)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1008">RTM_DELROUTE (supports `ip route del`)</span></span>
- <span data-ttu-id="19ca1-1009">Die geplante Task Überprüfung für zu Aktualisier Ende Pakete wird nicht mehr über eine getaktete Verbindung (GH #1371) ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1009">Scheduled task checking for packages to update will no longer run on a metered connection (GH #1371)</span></span>
- <span data-ttu-id="19ca1-1010">Es wurde ein Fehler behoben, bei dem die Weiterleitung unterbrochen wird, d.h. bash-c "ls-ALR/" | bash-c "Cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1010">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="19ca1-1011">Implementierte TCP_KEEPCNT-Socketoption (GH #843)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1011">Implemented TCP_KEEPCNT socket option (GH #843)</span></span>
- <span data-ttu-id="19ca1-1012">Implementierte IP_MTU_DISCOVER inet-Socketoption (GH #720, 717, 170, 69)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1012">Implemented IP_MTU_DISCOVER INET socket option (GH #720, 717, 170, 69)</span></span>
- <span data-ttu-id="19ca1-1013">Ältere Funktionalität zum Ausführen von NT-Binärdateien aus init mit NT-Pfad Suche entfernt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1013">Removed legacy functionality to run NT binaries from init with NT path lookup.</span></span> <span data-ttu-id="19ca1-1014">(GH #1325)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1014">(GH #1325)</span></span>
- <span data-ttu-id="19ca1-1015">Korrekturmodus von/dev/Kmsg zum Zulassen von Gruppen-/sonstigen Lesezugriff (0644) (GH #1321)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1015">Fix mode of /dev/kmsg to allow group / other read access (0644) (GH #1321)</span></span>
- <span data-ttu-id="19ca1-1016">Implementiertes/proc/sys/kernel/Random/UUID (GH #1092)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1016">Implemented /proc/sys/kernel/random/uuid  (GH #1092)</span></span>
- <span data-ttu-id="19ca1-1017">Der Fehler wurde behoben, bei dem die Startzeit des Prozesses als Jahr 2432 (GH #974) angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1017">Corrected error where process start time was showing as year 2432 (GH #974)</span></span>
- <span data-ttu-id="19ca1-1018">Der Standardbegriff "Umgebungsvariable" wird in "xterm-256 Color" (GH #1446) gewechselt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1018">Switched default TERM environment variable to xterm-256color (GH #1446)</span></span>
- <span data-ttu-id="19ca1-1019">Änderung der Art und Weise, in der der prozesscommit während der Prozess Verzweigung berechnet wird</span><span class="sxs-lookup"><span data-stu-id="19ca1-1019">Modified the way that process commit is calculated during process fork.</span></span> <span data-ttu-id="19ca1-1020">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1020">(GH #1286)</span></span>
- <span data-ttu-id="19ca1-1021">Implementiertes/proc/sys/VM/overcommit_memory.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1021">Implemented /proc/sys/vm/overcommit_memory.</span></span> <span data-ttu-id="19ca1-1022">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1022">(GH #1286)</span></span>
- <span data-ttu-id="19ca1-1023">Implementierte/proc/net/Route-Datei (GH #69)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1023">Implemented /proc/net/route file (GH #69)</span></span>
- <span data-ttu-id="19ca1-1024">Fehler behoben, bei dem der Verknüpfungs Name falsch lokalisiert wurde (GH #696)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1024">Fixed error where shortcut name was incorrectly localized (GH #696)</span></span>
- <span data-ttu-id="19ca1-1025">Eine fehlerhafte ELF-Verarbeitungslogik, die die Programm Header nicht ordnungsgemäß überprüft, muss kleiner als (oder gleich) PATH_MAX sein.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1025">Fixed elf parsing logic that is incorrectly validating the program headers must be less than (or equal to) PATH_MAX.</span></span> <span data-ttu-id="19ca1-1026">(GH #1048)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1026">(GH #1048)</span></span>
- <span data-ttu-id="19ca1-1027">Implementierter Status von "procfs", "sysfs", "cgroupfs" und "binf" (#1378)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1027">Implemented statfs callback for procfs, sysfs, cgroupfs, and binfmtfs (GH #1378)</span></span>
- <span data-ttu-id="19ca1-1028">Korrigieren von aptpackageindexupdate-Fenstern, die nicht geschlossen werden (GH #1184, auch in GH #1193 erläutert)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1028">Fixed AptPackageIndexUpdate windows that won’t close (GH #1184, also discussed in GH #1193)</span></span>
- <span data-ttu-id="19ca1-1029">ASLR-Persönlichkeit ADDR_NO_RANDOMIZE-Unterstützung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1029">Added ASLR personality  ADDR_NO_RANDOMIZE support.</span></span> <span data-ttu-id="19ca1-1030">(GH #1148, 1128)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1030">(GH #1148, 1128)</span></span>
- <span data-ttu-id="19ca1-1031">Verbessertes PTRACE_GETSIGINFO, Signatur Segment v, für ordnungsgemäße gdb-Stapel Überwachungen während der AV (GH #875)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1031">Improved PTRACE_GETSIGINFO, SIGSEGV, for proper gdb stack traces during AV (GH #875)</span></span>
- <span data-ttu-id="19ca1-1032">Die elf-Verarbeitung schlägt für patchelf-Binärdateien nicht mehr fehl.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1032">Elf parsing no longer fails for patchelf binaries.</span></span> <span data-ttu-id="19ca1-1033">(GH #471)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1033">(GH #471)</span></span>
- <span data-ttu-id="19ca1-1034">VPN-DNS-Weitergabe an/etc/resolv.conf (GH #416, 1350)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1034">VPN DNS propagated to /etc/resolv.conf (GH #416, 1350)</span></span>
- <span data-ttu-id="19ca1-1035">Verbesserungen an TCP Close für eine zuverlässigere Datenübertragung.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1035">Improvements to TCP close for more reliable data transfer.</span></span> <span data-ttu-id="19ca1-1036">(GH #610, 616, 1025, 1335)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1036">(GH #610, 616, 1025, 1335)</span></span>
- <span data-ttu-id="19ca1-1037">Geben Sie nun den richtigen Fehlercode zurück, wenn zu viele Dateien (EMFILE) geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1037">Now return correct error code when too many files are opened (EMFILE).</span></span> <span data-ttu-id="19ca1-1038">(GH #1126, 2090)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1038">(GH #1126, 2090)</span></span>
- <span data-ttu-id="19ca1-1039">Windows Audit Log meldet jetzt den Image Namen in Process create Audit.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1039">Windows Audit log now reports the image name in process create audit.</span></span>
- <span data-ttu-id="19ca1-1040">Fehler beim Starten von bash. exe in einem bash-Fenster ordnungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1040">Now gracefully fail when launching bash.exe from within a bash window</span></span>
- <span data-ttu-id="19ca1-1041">Es wurde eine Fehlermeldung hinzugefügt, wenn Interop nicht auf ein Arbeitsverzeichnis unter lxfs zugreifen kann (z.b. "Notepad. exe. bashrc").</span><span class="sxs-lookup"><span data-stu-id="19ca1-1041">Added error message when interop is unable to access a working directory under LxFs (i.e. notepad.exe .bashrc)</span></span>
- <span data-ttu-id="19ca1-1042">Problem behoben, bei dem der Windows-Pfad in WSL abgeschnitten wurde</span><span class="sxs-lookup"><span data-stu-id="19ca1-1042">Fixed issue where Windows path was truncated in WSL</span></span>
- <span data-ttu-id="19ca1-1043">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1043">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1044">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1044">LTP Results:</span></span>
<span data-ttu-id="19ca1-1045">Anzahl der bestandenen Tests: 690</span><span class="sxs-lookup"><span data-stu-id="19ca1-1045">Number of Passing Test: 690</span></span> </br>
<span data-ttu-id="19ca1-1046">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 274</span><span class="sxs-lookup"><span data-stu-id="19ca1-1046">Number of non-Passing (failing, skipped, etc…): 274</span></span> </br>
[<span data-ttu-id="19ca1-1047">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1047">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1048">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1048">Syscall Support</span></span>
<span data-ttu-id="19ca1-1049">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1049">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1050">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1050">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a><span data-ttu-id="19ca1-1051">Build 14986</span><span class="sxs-lookup"><span data-stu-id="19ca1-1051">Build 14986</span></span>

<span data-ttu-id="19ca1-1052">Allgemeine Windows-Informationen zu Build 14986 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1052">For general Windows information on build 14986 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1053">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1053">Fixed</span></span>

- <span data-ttu-id="19ca1-1054">Bugprüfungen mit NetLink und Pty IOCTLs korrigiert</span><span class="sxs-lookup"><span data-stu-id="19ca1-1054">Fixed bugchecks with Netlink and Pty IOCTLs</span></span>
- <span data-ttu-id="19ca1-1055">Nun meldet die Kernel Version 4.4.0-43 aus Gründen der Konsistenz mit xenial.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1055">Kernel version now reports 4.4.0-43 for consistency with Xenial</span></span>
- <span data-ttu-id="19ca1-1056">Bash. exe wird jetzt gestartet, wenn die Eingabe an "NUL:" (GH #1259) gerichtet ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1056">Bash.exe now launches when input directed to 'nul:' (GH #1259)</span></span>
- <span data-ttu-id="19ca1-1057">Thread-IDs werden nun ordnungsgemäß in procfs gemeldet (GH #967)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1057">Thread IDs now reported correctly in procfs (GH #967)</span></span>
- <span data-ttu-id="19ca1-1058">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR-Flags werden jetzt in inotify_add_watch () (GH #1280) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1058">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR flags now supported in inotify_add_watch() (GH #1280)</span></span>
- <span data-ttu-id="19ca1-1059">Implementieren Sie timer_create und verwandte Systemaufrufe.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1059">Implement timer_create and related system calls.</span></span>  <span data-ttu-id="19ca1-1060">Dies ermöglicht die Unterstützung von GHC (GH #307).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1060">This enables GHC support (GH #307)</span></span>
- <span data-ttu-id="19ca1-1061">Problem behoben, bei dem Ping eine Zeit von 0.000 ms zurück gab (GH #1296)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1061">Fixed issue where ping returned a time of 0.000ms (GH #1296)</span></span>
- <span data-ttu-id="19ca1-1062">Geben Sie den richtigen Fehlercode zurück, wenn zu viele Dateien geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1062">Return correct error code when too many files are opened.</span></span>
- <span data-ttu-id="19ca1-1063">Es wurde ein Problem in WSL behoben, bei dem die NETLink-Anforderung für Netzwerkschnittstellen Daten mit EINVAL fehlgeschlagen ist, wenn die Hardwareadresse der Schnittstelle 32 Bytes (z. b. die Teredo-Schnittstelle</span><span class="sxs-lookup"><span data-stu-id="19ca1-1063">Fixed issue in WSL where Netlink request for network interface data would fail with EINVAL if the interface's hardware address is 32-bytes (such as the Teredo interface)</span></span>
   - <span data-ttu-id="19ca1-1064">Beachten Sie, dass das Linux-Hilfsprogramm "IP" einen Fehler enthält, bei dem ein Absturz erfolgt, wenn WSL eine 32-Byte-Hardwareadresse meldet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1064">Note that the Linux "ip" utility contains a bug where it will crash if WSL reports a 32-byte hardware address.</span></span> <span data-ttu-id="19ca1-1065">Dies ist ein Fehler in "IP", nicht bei WSL.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1065">This is a bug in "ip", not WSL.</span></span> <span data-ttu-id="19ca1-1066">Mit dem Hilfsprogramm "IP" wird die Länge des Zeichen folgen Puffers fest codiert, der zum Drucken der Hardwareadresse verwendet wird, und dieser Puffer ist zu klein, um eine 32-Byte-Hardwareadresse auszugeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1066">The “ip” utility hard-codes the length of the string buffer used to print the hardware address, and that buffer is too small to print a 32-byte hardware address.</span></span>
- <span data-ttu-id="19ca1-1067">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1067">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1068">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1068">LTP Results:</span></span>
<span data-ttu-id="19ca1-1069">Anzahl der bestandenen Tests: 669</span><span class="sxs-lookup"><span data-stu-id="19ca1-1069">Number of Passing Test: 669</span></span> </br>
<span data-ttu-id="19ca1-1070">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="19ca1-1070">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="19ca1-1071">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1071">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1072">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1072">Syscall Support</span></span>
<span data-ttu-id="19ca1-1073">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1073">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1074">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1074">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a><span data-ttu-id="19ca1-1075">Build 14971</span><span class="sxs-lookup"><span data-stu-id="19ca1-1075">Build 14971</span></span>

<span data-ttu-id="19ca1-1076">Allgemeine Windows-Informationen zu Build 14971 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1076">For general Windows information on build 14971 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1077">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1077">Fixed</span></span>

 - <span data-ttu-id="19ca1-1078">Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1078">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="19ca1-1079">Regelmäßig geplante Updates werden bei der nächsten Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1079">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1080">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1080">LTP Results:</span></span>
<span data-ttu-id="19ca1-1081">Unverändert gegenüber 14965</span><span class="sxs-lookup"><span data-stu-id="19ca1-1081">Unchanged from 14965</span></span> </br>
<span data-ttu-id="19ca1-1082">Anzahl der bestandenen Tests: 664</span><span class="sxs-lookup"><span data-stu-id="19ca1-1082">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="19ca1-1083">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1083">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1084">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1084">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a><span data-ttu-id="19ca1-1085">Build 14965</span><span class="sxs-lookup"><span data-stu-id="19ca1-1085">Build 14965</span></span>

<span data-ttu-id="19ca1-1086">Allgemeine Windows-Informationen zu Build 14965 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1086">For general Windows information on build 14965 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1087">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1087">Fixed</span></span>

- <span data-ttu-id="19ca1-1088">Unterstützung für netLINK Sockets NETLINK_ROUTE Protocol RTM_GETLINK und RTM_GETADDR (GH #468)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1088">Support for Netlink sockets NETLINK_ROUTE protocol's RTM_GETLINK and RTM_GETADDR (GH #468)</span></span>
  - <span data-ttu-id="19ca1-1089">Aktiviert ifconfig-und IP-Befehle für die netzwerkenumeration.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1089">Enables ifconfig and ip commands for network enumeration</span></span>
  - <span data-ttu-id="19ca1-1090">Weitere Informationen finden Sie im [Blogbeitrag zu WSL-Netzwerken](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1090">More information can be found in our [WSL Networking blog post](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span></span>

- <span data-ttu-id="19ca1-1091">/sbin befindet sich jetzt standardmäßig im Pfad des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1091">/sbin is now in the user's path by default</span></span>
- <span data-ttu-id="19ca1-1092">Der NT-Benutzer Pfad wird jetzt standardmäßig an den WSL-Pfad angefügt (Sie können nun Notepad. exe eingeben, ohne dem Linux-Pfad System32 hinzuzufügen).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1092">NT user path now appended to the WSL path by default (i.e. you can now type notepad.exe without adding System32 to the Linux path)</span></span>
- <span data-ttu-id="19ca1-1093">Unterstützung für/proc/sys/kernel/cap_last_cap hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1093">Added support for /proc/sys/kernel/cap_last_cap</span></span>
- <span data-ttu-id="19ca1-1094">NT-Binärdateien können nun von WSL aus gestartet werden, wenn das aktuelle Arbeitsverzeichnis nicht-ANSI-Zeichen (GH #1254) enthält.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1094">NT Binaries can now be launched from WSL when the current working directory contains non-ansi characters (GH #1254)</span></span>
- <span data-ttu-id="19ca1-1095">Zulassen des herunter Fahrens auf einem nicht verbundenen UNIX-Streamsocket</span><span class="sxs-lookup"><span data-stu-id="19ca1-1095">Allow shutdown on disconnected unix stream socket.</span></span>
- <span data-ttu-id="19ca1-1096">Unterstützung für PR_GET_PDEATHSIG hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1096">Added support for PR_GET_PDEATHSIG.</span></span>
- <span data-ttu-id="19ca1-1097">Unterstützung für CLONE_PARENT hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1097">Added support for CLONE_PARENT</span></span>
- <span data-ttu-id="19ca1-1098">Es wurde ein Fehler behoben, bei dem die Weiterleitung unterbrochen wird, d.h. bash-c "ls-ALR/" | bash-c "Cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1098">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="19ca1-1099">Verarbeitet Anforderungen zum Herstellen einer Verbindung mit dem aktuellen Terminal.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1099">Handle requests to connect to the current terminal.</span></span>
- <span data-ttu-id="19ca1-1100">Markieren Sie<pid>/proc//oom_score_adj als beschreibbar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1100">Mark /proc/<pid>/oom_score_adj as writable.</span></span>
- <span data-ttu-id="19ca1-1101">/Sys/fs/CGroup Ordner hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1101">Add /sys/fs/cgroup folder.</span></span>
- <span data-ttu-id="19ca1-1102">sched_setaffinity sollte die Anzahl der Affinitäts Bits Mask zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1102">sched_setaffinity should return number of affinity bits mask</span></span>
- <span data-ttu-id="19ca1-1103">Korrektur der elf-Validierungs Logik, die fälschlicherweise annimmt, dass interpreterpfade weniger als 64 Zeichen lang sein müssen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1103">Fix ELF validation logic which incorrectly assumes interpreter paths must be less than 64 characters long.</span></span> <span data-ttu-id="19ca1-1104">(GH #743)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1104">(GH #743)</span></span>
- <span data-ttu-id="19ca1-1105">Dateideskriptoren öffnen können das Konsolenfenster geöffnet lassen (GH #1187)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1105">Open file descriptors can keep console window open (GH #1187)</span></span>
- <span data-ttu-id="19ca1-1106">Fixeed-Fehler, bei dem Rename () mit einem nachgestellten Schrägstrich am Zielnamen (GH #1008) fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1106">Fixeed error where rename() failed with trailing slash on target name (GH #1008)</span></span>
- <span data-ttu-id="19ca1-1107">Implementieren der/proc/net/dev-Datei</span><span class="sxs-lookup"><span data-stu-id="19ca1-1107">Implement /proc/net/dev file</span></span>
- <span data-ttu-id="19ca1-1108">Korrigiert 0.000 ms Pings aufgrund der Zeit Geber Auflösung.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1108">Fixed 0.000ms pings due to timer resolution.</span></span>
- <span data-ttu-id="19ca1-1109">Implementiertes/proc/self/Environ (GH #730)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1109">Implemented /proc/self/environ (GH #730)</span></span>
- <span data-ttu-id="19ca1-1110">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1110">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1111">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1111">LTP Results:</span></span>
<span data-ttu-id="19ca1-1112">Anzahl der bestandenen Tests: 664</span><span class="sxs-lookup"><span data-stu-id="19ca1-1112">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="19ca1-1113">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1113">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1114">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1114">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a><span data-ttu-id="19ca1-1115">Build 14959</span><span class="sxs-lookup"><span data-stu-id="19ca1-1115">Build 14959</span></span>

<span data-ttu-id="19ca1-1116">Allgemeine Windows-Informationen zu Build 14959 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1116">For general Windows information on build 14959 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1117">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1117">Fixed</span></span>

- <span data-ttu-id="19ca1-1118">Verbesserte Pico-Prozess Benachrichtigung für Windows.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1118">Improved Pico Process notification for Windows.</span></span>  <span data-ttu-id="19ca1-1119">Weitere Informationen finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1119">Additional information found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span></span>
- <span data-ttu-id="19ca1-1120">Verbesserte Stabilität durch Windows-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="19ca1-1120">Improved stability with Windows interoperability</span></span>
- <span data-ttu-id="19ca1-1121">Fehler 0x80070057 beim Starten von bash. exe behoben, wenn der Unternehmens Datenschutz (Enterprise Data Protection, EDP) aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="19ca1-1121">Fixed error 0x80070057 when launching bash.exe when Enterprise Data Protection (EDP) is enabled</span></span>
- <span data-ttu-id="19ca1-1122">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1122">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1123">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1123">LTP Results:</span></span>
<span data-ttu-id="19ca1-1124">Anzahl der bestandenen Tests: 665</span><span class="sxs-lookup"><span data-stu-id="19ca1-1124">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="19ca1-1125">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1125">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1126">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1126">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a><span data-ttu-id="19ca1-1127">Build 14955</span><span class="sxs-lookup"><span data-stu-id="19ca1-1127">Build 14955</span></span>

<span data-ttu-id="19ca1-1128">Allgemeine Windows-Informationen zu Build 14955 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1128">For general Windows information on build 14955 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1129">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1129">Fixed</span></span>

 - <span data-ttu-id="19ca1-1130">Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1130">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="19ca1-1131">Regelmäßig geplante Updates werden bei der nächsten Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1131">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1132">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1132">LTP Results:</span></span>
<span data-ttu-id="19ca1-1133">Anzahl der bestandenen Tests: 665</span><span class="sxs-lookup"><span data-stu-id="19ca1-1133">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="19ca1-1134">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1134">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1135">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1135">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a><span data-ttu-id="19ca1-1136">Build 14951</span><span class="sxs-lookup"><span data-stu-id="19ca1-1136">Build 14951</span></span>

<span data-ttu-id="19ca1-1137">Allgemeine Windows-Informationen zu Build 14951 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1137">For general Windows information on build 14951 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span></span><br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a><span data-ttu-id="19ca1-1138">Neues Feature: Interoperabilität von Windows/Ubuntu</span><span class="sxs-lookup"><span data-stu-id="19ca1-1138">New Feature: Windows / Ubuntu Interoperability</span></span>
<span data-ttu-id="19ca1-1139">Windows-Binärdateien können jetzt direkt über die WSL-Befehlszeile aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1139">Windows binaries can now be invoked directly from the WSL command line.</span></span>  <span data-ttu-id="19ca1-1140">Dadurch haben Benutzer die Möglichkeit, mit Ihrer Windows-Umgebung und dem System auf eine Weise zu interagieren, die nicht möglich war.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1140">This gives users the ability to interact with their Windows environment and system in a way that has not been possible.</span></span>  <span data-ttu-id="19ca1-1141">Als kurzes Beispiel können Benutzer nun die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1141">As a quick example, it is now possible for users to run the following commands:</span></span>

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

<span data-ttu-id="19ca1-1142">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1142">More information can be found at:</span></span>

- [<span data-ttu-id="19ca1-1143">WSL-Teamblog für Interop</span><span class="sxs-lookup"><span data-stu-id="19ca1-1143">WSL Team Blog for Interop</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [<span data-ttu-id="19ca1-1144">MSDN-Interop-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="19ca1-1144">MSDN Interop Documentation</span></span>](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1145">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1145">Fixed</span></span>

- <span data-ttu-id="19ca1-1146">Ubuntu 16,04 (xenial) ist jetzt für alle neuen WSL-Instanzen installiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1146">Ubuntu 16.04 (Xenial) is now installed for all new WSL instances.</span></span>  <span data-ttu-id="19ca1-1147">Benutzer mit vorhandenen 14,04-Instanzen (trusty) werden nicht automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1147">Users with existing 14.04 (Trusty) instances will not be automatically upgraded.</span></span>
- <span data-ttu-id="19ca1-1148">Das während der Installation festgelegte Gebiets Schema wird jetzt angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1148">Locale set during install is now displayed</span></span>
- <span data-ttu-id="19ca1-1149">Terminal Verbesserungen, einschließlich des Fehlers bei der Umleitung eines WSL-Prozesses an eine Datei, funktioniert nicht immer</span><span class="sxs-lookup"><span data-stu-id="19ca1-1149">Terminal improvements including bug where redirecting a WSL process to a file does not always work</span></span>
- <span data-ttu-id="19ca1-1150">Die Konsolen Lebensdauer muss an die Lebensdauer von bash. exe gebunden sein</span><span class="sxs-lookup"><span data-stu-id="19ca1-1150">Console lifetime should be tied to bash.exe lifetime</span></span>
- <span data-ttu-id="19ca1-1151">Die Größe des Konsolenfensters sollte die sichtbare Größe und nicht die Puffergröße verwenden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1151">Console window size should use visible size, not buffer size</span></span>
- <span data-ttu-id="19ca1-1152">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1152">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1153">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1153">LTP Results:</span></span>
<span data-ttu-id="19ca1-1154">Anzahl der bestandenen Tests: 665</span><span class="sxs-lookup"><span data-stu-id="19ca1-1154">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="19ca1-1155">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1155">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1156">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1156">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a><span data-ttu-id="19ca1-1157">Build 14946</span><span class="sxs-lookup"><span data-stu-id="19ca1-1157">Build 14946</span></span>

<span data-ttu-id="19ca1-1158">Allgemeine Windows-Informationen zu Build 14946 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1158">For general Windows information on build 14946 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1159">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1159">Fixed</span></span>

- <span data-ttu-id="19ca1-1160">Es wurde ein Problem behoben, das das Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen, die Leerzeichen oder Anführungszeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="19ca1-1160">Fixed an issue that prevented creating WSL user accounts for users with NT usernames that contain spaces or quotes.</span></span> 
- <span data-ttu-id="19ca1-1161">Ändern Sie "volfs" und "drvfs" so, dass für die Verknüpfungs Anzahl der Verzeichnisse in der</span><span class="sxs-lookup"><span data-stu-id="19ca1-1161">Change VolFs and DrvFs to return 0 for directory's link count in stat</span></span>
- <span data-ttu-id="19ca1-1162">Support IPV6_MULTICAST_HOPS Socketoption.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1162">Support IPV6_MULTICAST_HOPS socket option.</span></span>
- <span data-ttu-id="19ca1-1163">Beschränken auf eine einzige Konsolen-e/a-Schleife pro TTY.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1163">Limit to a single console I/O loop per tty.</span></span> <span data-ttu-id="19ca1-1164">Beispiel: der folgende Befehl ist möglich:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1164">Example: the following command is possible:</span></span>
  - <span data-ttu-id="19ca1-1165">bash-c "Echo Daten" | bash-c "SSH user@example.com " cat > foo. txt ""</span><span class="sxs-lookup"><span data-stu-id="19ca1-1165">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span></span>

- <span data-ttu-id="19ca1-1166">Ersetzen von Leerzeichen durch Registerkarten in/proc/cpuinfo (GH #1115)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1166">replace spaces with tabs in /proc/cpuinfo (GH #1115)</span></span>
- <span data-ttu-id="19ca1-1167">Drvfs wird jetzt in mountinfo mit einem Namen angezeigt, der dem bereitgestellten Windows-Volume entspricht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1167">DrvFs now appears in mountinfo with a name that matches mounted Windows volume</span></span>
- <span data-ttu-id="19ca1-1168">/Home und/root werden nun in mountinfo mit korrekten Namen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1168">/home and /root now appear in mountinfo with correct names</span></span>
- <span data-ttu-id="19ca1-1169">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1169">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1170">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1170">LTP Results:</span></span>
<span data-ttu-id="19ca1-1171">Anzahl der bestandenen Tests: 665</span><span class="sxs-lookup"><span data-stu-id="19ca1-1171">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="19ca1-1172">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1172">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1173">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1173">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a><span data-ttu-id="19ca1-1174">Build 14942</span><span class="sxs-lookup"><span data-stu-id="19ca1-1174">Build 14942</span></span>

<span data-ttu-id="19ca1-1175">Allgemeine Windows-Informationen zu Build 14942 finden Sie im [Windows-Blog](https://aka.ms/onefourninefourtwoooooo).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1175">For general Windows information on build 14942 visit the [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1176">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1176">Fixed</span></span>

- <span data-ttu-id="19ca1-1177">Eine Reihe von bugprüfungen, einschließlich des Netzwerk Absturzes "versuchte Ausführung des noexecute-Speichers", der SSH blockiert hat</span><span class="sxs-lookup"><span data-stu-id="19ca1-1177">A number of bugchecks addressed, including the “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY” networking crash which was blocking SSH</span></span>
- <span data-ttu-id="19ca1-1178">Unterstützung von Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf drvfs generiert werden, ist jetzt in</span><span class="sxs-lookup"><span data-stu-id="19ca1-1178">inotifiy support for notifications generated from Windows applications on DrvFs is now in</span></span>
- <span data-ttu-id="19ca1-1179">Implementieren Sie TCP_KEEPIDLE und TCP_KEEPINTVL für mongod.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1179">Implement TCP_KEEPIDLE and TCP_KEEPINTVL for mongod.</span></span> <span data-ttu-id="19ca1-1180">(GH #695)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1180">(GH #695)</span></span>
- <span data-ttu-id="19ca1-1181">Implementieren des pivot_root-System Aufrufes</span><span class="sxs-lookup"><span data-stu-id="19ca1-1181">Implement the pivot_root system call</span></span>
- <span data-ttu-id="19ca1-1182">Implementieren der Socketoption für SO_DONTROUTE</span><span class="sxs-lookup"><span data-stu-id="19ca1-1182">Implement socket option for SO_DONTROUTE</span></span>
- <span data-ttu-id="19ca1-1183">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1183">Additional bugfixes and improvements</span></span>


### <a name="ltp-results"></a><span data-ttu-id="19ca1-1184">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1184">LTP Results:</span></span>
<span data-ttu-id="19ca1-1185">Anzahl der bestandenen Tests: 665</span><span class="sxs-lookup"><span data-stu-id="19ca1-1185">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="19ca1-1186">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="19ca1-1186">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="19ca1-1187">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1187">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1188">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1188">Syscall Support</span></span>
<span data-ttu-id="19ca1-1189">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1189">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1190">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1190">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a><span data-ttu-id="19ca1-1191">Build 14936</span><span class="sxs-lookup"><span data-stu-id="19ca1-1191">Build 14936</span></span>

<span data-ttu-id="19ca1-1192">Allgemeine Windows-Informationen zu Build 14936 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1192">For general Windows information on build 14936 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span></span><br/>


<span data-ttu-id="19ca1-1193">Hinweis: WSL wird in einer zukünftigen Version Ubuntu-Version 16,04 (xenial) anstelle von Ubuntu 14,04 (trusty) installieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1193">Note: WSL will install Ubuntu version 16.04 (Xenial) instead of Ubuntu 14.04 (Trusty) in an upcoming release.</span></span>  <span data-ttu-id="19ca1-1194">Diese Änderung gilt für Insider, die neue Instanzen installieren (lxrun. exe/install oder die erste Ausführen von bash. exe).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1194">This change will apply to Insiders installing new instances (lxrun.exe /install or first run of bash.exe).</span></span>  <span data-ttu-id="19ca1-1195">Vorhandene Instanzen mit trusty werden nicht automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1195">Existing instances with Trusty will not be upgraded automatically.</span></span> <span data-ttu-id="19ca1-1196">Benutzer können mit dem Befehl "Do-Release-Upgrade" Ihr trusty-Bild auf "xenial" aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1196">Users can upgrade their Trusty image to Xenial using the do-release-upgrade command.</span></span>

### <a name="known-issue"></a><span data-ttu-id="19ca1-1197">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="19ca1-1197">Known Issue</span></span>
<span data-ttu-id="19ca1-1198">Bei WSL treten Probleme mit einigen Socketimplementierungen auf.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1198">WSL is experiencing an issue with some socket implementations.</span></span>  <span data-ttu-id="19ca1-1199">Der Fehlercode manifestiert sich selbst als Absturz mit dem Fehler "Es wurde versucht, den noexecute-Speicher auszuführen".</span><span class="sxs-lookup"><span data-stu-id="19ca1-1199">The bugcheck manifests itself as a crash with the error “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY”.</span></span>  <span data-ttu-id="19ca1-1200">Die häufigste Erscheinung dieses Problems ist ein Absturz bei der Verwendung von SSH.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1200">The most common manifestation of this issue is a crash when using ssh.</span></span>  <span data-ttu-id="19ca1-1201">Die Ursache ist bei internen Builds korrigiert und wird zu Beginn der frühesten Gelegenheit an Insider übermittelt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1201">The root cause is fixed on internal builds and will be pushed to Insiders at the earliest opportunity.</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-1202">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1202">Fixed</span></span>

- <span data-ttu-id="19ca1-1203">Der chroot-Systemaufrufe wurde implementiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1203">Implemented the chroot system call</span></span>
- <span data-ttu-id="19ca1-1204">Verbesserungen bei der inotifizierungen ~~einschließlich Unterstützung für von Windows-Anwendungen generierte Benachrichtigungen auf drvfs~~</span><span class="sxs-lookup"><span data-stu-id="19ca1-1204">Improvements in inotify ~~including support for notifications generated from Windows applications on DrvFs~~</span></span>
  - <span data-ttu-id="19ca1-1205">Berichtigungs Die Unterstützung von Änderungen, die von Windows-Anwendungen stammen, ist zurzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1205">Correction: Inotify support for changes originating from Windows applications not available at this time.</span></span>
- <span data-ttu-id="19ca1-1206">Socketbindung an IPv6:<port n> : unterstützt jetzt IPV6_V6ONLY (GH #68, #157, #393, #460, #674, #740, #982)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1206">Socket binding to IPV6::<port n> now supports IPV6_V6ONLY  (GH #68, #157, #393, #460, #674, #740, #982, #996)</span></span>
- <span data-ttu-id="19ca1-1207">Wnowait-Verhalten für waitid systemcallimplementiertes (GH #638)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1207">WNOWAIT behavior for waitid systemcall implemented (GH #638)</span></span>
- <span data-ttu-id="19ca1-1208">Unterstützung für IP-Socketoptionen IP_HDRINCL und IP_TTL</span><span class="sxs-lookup"><span data-stu-id="19ca1-1208">Support for IP socket options IP_HDRINCL and IP_TTL</span></span>
- <span data-ttu-id="19ca1-1209">Lesevorgänge () der Länge 0 (null) sollten sofort (GH #975) zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1209">Zero-length read() should return immediately (GH #975)</span></span>
- <span data-ttu-id="19ca1-1210">Ordnungsgemäße Behandlung von Dateinamen und Dateinamen Präfixen, die keinen null-Terminator in einer tar-Datei enthalten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1210">Correctly handle filenames and filename prefixes that don't include a NULL terminator in a .tar file.</span></span>
- <span data-ttu-id="19ca1-1211">epoll-Unterstützung für/dev/null</span><span class="sxs-lookup"><span data-stu-id="19ca1-1211">epoll support for /dev/null</span></span>
- <span data-ttu-id="19ca1-1212">Fix/dev/Alarm Zeit Quelle</span><span class="sxs-lookup"><span data-stu-id="19ca1-1212">Fix /dev/alarm time source</span></span>
- <span data-ttu-id="19ca1-1213">Bash-c kann nun zu einer Datei umgeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1213">Bash -c now able to redirect to a file</span></span>
- <span data-ttu-id="19ca1-1214">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1214">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1215">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1215">LTP Results:</span></span>
<span data-ttu-id="19ca1-1216">Anzahl der bestandenen Tests: 664</span><span class="sxs-lookup"><span data-stu-id="19ca1-1216">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="19ca1-1217">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 264</span><span class="sxs-lookup"><span data-stu-id="19ca1-1217">Number of non-Passing (failing, skipped, etc…): 264</span></span> </br>
[<span data-ttu-id="19ca1-1218">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1218">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1219">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1219">Syscall Support</span></span>
<span data-ttu-id="19ca1-1220">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1220">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1221">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1221">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`chroot`<br/>
<br/>

## <a name="build-14931"></a><span data-ttu-id="19ca1-1222">Build 14931</span><span class="sxs-lookup"><span data-stu-id="19ca1-1222">Build 14931</span></span>

<span data-ttu-id="19ca1-1223">Allgemeine Windows-Informationen zu Build 14931 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1223">For general Windows information on build 14931 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1224">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1224">Fixed</span></span>

 - <span data-ttu-id="19ca1-1225">Aufgrund von über unsere Kontrolle hinausgehende Umstände gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1225">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="19ca1-1226">Regelmäßig geplante Updates werden in der nächsten Version fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1226">Regularly scheduled updates will resume in the next release.</span></span>

<br/>

## <a name="build-14926"></a><span data-ttu-id="19ca1-1227">Build 14926</span><span class="sxs-lookup"><span data-stu-id="19ca1-1227">Build 14926</span></span>

<span data-ttu-id="19ca1-1228">Allgemeine Windows-Informationen zu Build 14926 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1228">For general Windows information on build 14926 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1229">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1229">Fixed</span></span>

- <span data-ttu-id="19ca1-1230">Ping funktioniert nun in-Konsolen, die nicht über Administratorrechte verfügen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1230">Ping now works in consoles which do not have administrator privileges</span></span>
- <span data-ttu-id="19ca1-1231">Ping6 wird jetzt auch ohne Administratorrechte unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1231">Ping6 now supported, also without administrator privileges</span></span>
- <span data-ttu-id="19ca1-1232">Unterstützung von Dateien, die über WSL geändert wurden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1232">Inotify support for files modified through WSL.</span></span> <span data-ttu-id="19ca1-1233">(GH #216)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1233">(GH #216)</span></span>
  - <span data-ttu-id="19ca1-1234">Unterstützte Flags:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1234">Flags supported:</span></span>
    - <span data-ttu-id="19ca1-1235">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span><span class="sxs-lookup"><span data-stu-id="19ca1-1235">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span></span>
    - <span data-ttu-id="19ca1-1236">inotify_add_watch-Ereignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span><span class="sxs-lookup"><span data-stu-id="19ca1-1236">inotify_add_watch events: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span></span>
    - <span data-ttu-id="19ca1-1237">inotify_add_watch-Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span><span class="sxs-lookup"><span data-stu-id="19ca1-1237">inotify_add_watch attributes: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span></span>
    - <span data-ttu-id="19ca1-1238">Ausgabe lesen: LX_IN_ISDIR, LX_IN_IGNORED</span><span class="sxs-lookup"><span data-stu-id="19ca1-1238">read output: LX_IN_ISDIR, LX_IN_IGNORED</span></span>
  - <span data-ttu-id="19ca1-1239">Bekanntes Problem: Durch das Ändern von Dateien aus Windows-Anwendungen werden keine Ereignisse generiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1239">Known issue: Modifying files from Windows applications does not generate any events</span></span>
- <span data-ttu-id="19ca1-1240">UNIX-Socket unterstützt jetzt SCM_CREDENTIALS</span><span class="sxs-lookup"><span data-stu-id="19ca1-1240">Unix socket now supports SCM_CREDENTIALS</span></span>

### <a name="ltp-results"></a><span data-ttu-id="19ca1-1241">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="19ca1-1241">LTP Results:</span></span>
<span data-ttu-id="19ca1-1242">Anzahl der bestandenen Tests: 651</span><span class="sxs-lookup"><span data-stu-id="19ca1-1242">Number of Passing Test: 651</span></span> </br>
<span data-ttu-id="19ca1-1243">Anzahl der nicht bestandenen (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="19ca1-1243">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="19ca1-1244">Test Laufprotokolle von LTP</span><span class="sxs-lookup"><span data-stu-id="19ca1-1244">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a><span data-ttu-id="19ca1-1245">Build 14915</span><span class="sxs-lookup"><span data-stu-id="19ca1-1245">Build 14915</span></span>

<span data-ttu-id="19ca1-1246">Allgemeine Windows-Informationen zu Build 14915 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1246">For general Windows information on build 14915 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1247">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1247">Fixed</span></span>
-  <span data-ttu-id="19ca1-1248">Socketpair für UNIX Datagramm-Sockets (GH #262)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1248">Socketpair for unix datagram sockets (GH #262)</span></span>
- <span data-ttu-id="19ca1-1249">Unterstützung für UNIX-Sockets für SO_REUSEADDR</span><span class="sxs-lookup"><span data-stu-id="19ca1-1249">Unix socket support for SO_REUSEADDR</span></span>
- <span data-ttu-id="19ca1-1250">Unterstützung von UNIX-Sockets für SO_BROADCAST (GH #568)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1250">UNIX socket support for SO_BROADCAST (GH #568)</span></span>
- <span data-ttu-id="19ca1-1251">Unterstützung für UNIX-Sockets für sock_seqpacket (GH #758 #546)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1251">Unix socket support for SOCK_SEQPACKET (GH #758, #546)</span></span>
- <span data-ttu-id="19ca1-1252">Hinzufügen von Unterstützung für UNIX Datagram Socket Send, empfangener und Shutdown</span><span class="sxs-lookup"><span data-stu-id="19ca1-1252">Adding support for unix datagram socket send, recv and shutdown</span></span>
- <span data-ttu-id="19ca1-1253">Korrigieren Sie Fehlercode aufgrund einer ungültigen Überprüfung des mmap-Parameters für nicht feste Adressen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1253">Fix bugcheck due to invalid mmap parameter validation for non-fixed addresses.</span></span> <span data-ttu-id="19ca1-1254">(GH #847)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1254">(GH #847)</span></span>
- <span data-ttu-id="19ca1-1255">Unterstützung für das aussetzen/fortsetzen von Terminal Zuständen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1255">Support for suspend / resume of terminal states</span></span>
- <span data-ttu-id="19ca1-1256">Unterstützung für tiocpkt ioctl zum Entsperren des Bildschirm Hilfsprogramms (GH #774)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1256">Support for TIOCPKT ioctl to unblock the Screen utility (GH #774)</span></span>
    - <span data-ttu-id="19ca1-1257">Bekanntes Problem: Funktionstasten sind nicht funktionsfähig.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1257">Known issue: Function keys not operational</span></span>
- <span data-ttu-id="19ca1-1258">Es wurde ein Race in timerfd korrigiert, das dazu führen kann, dass ein frei gegebener Member "readerready" von lxptimerfdworkerroutine (GH #814) aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1258">Corrected a race in TimerFd that could cause a freed member 'ReaderReady' to be accessed by LxpTimerFdWorkerRoutine (GH #814)</span></span>
- <span data-ttu-id="19ca1-1259">Aktivieren der Unterstützung für den erneuten Start baren System Abruf für Futex, Abruf und clock_nanosleep</span><span class="sxs-lookup"><span data-stu-id="19ca1-1259">Enable restartable system call support for futex, poll, and clock_nanosleep</span></span>
- <span data-ttu-id="19ca1-1260">Unterstützung für Bindungs einbinden hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1260">Added bind mount support</span></span>
- <span data-ttu-id="19ca1-1261">Freigabe für einstellungsnamespace-Unterstützung aufheben</span><span class="sxs-lookup"><span data-stu-id="19ca1-1261">unshare for mount namespace support</span></span>
    - <span data-ttu-id="19ca1-1262">Bekanntes Problem: Beim Erstellen eines neuen Mount-Namespace `unshare(CLONE_NEWNS)` mit dem aktuellen Arbeitsverzeichnis wird weiterhin auf den alten Namespace verweisen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1262">Known issue: When creating a new mount namespace with `unshare(CLONE_NEWNS)` the current working directory will continue to point to the old namespace</span></span>
- <span data-ttu-id="19ca1-1263">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1263">Additional improvements and bug fixes</span></span>

<br/>

## <a name="build-14905"></a><span data-ttu-id="19ca1-1264">Build 14905</span><span class="sxs-lookup"><span data-stu-id="19ca1-1264">Build 14905</span></span>

<span data-ttu-id="19ca1-1265">Allgemeine Windows-Informationen zu Build 14905 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1265">For general Windows information on build 14905 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1266">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1266">Fixed</span></span>
- <span data-ttu-id="19ca1-1267">Neu Start Bare Systemaufrufe werden jetzt unterstützt (GH #349, GH #520)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1267">Restartable system calls are now supported (GH #349, GH #520)</span></span>
- <span data-ttu-id="19ca1-1268">Symlinks zu Verzeichnissen, die mit/jetzt funktionstüchtig (GH #650) enden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1268">Symlinks to directories ending in / now operational (GH #650)</span></span>
- <span data-ttu-id="19ca1-1269">Implementierte rndgetentcnt ioctl für "/dev/random"</span><span class="sxs-lookup"><span data-stu-id="19ca1-1269">Implemented RNDGETENTCNT ioctl for /dev/random</span></span>
- <span data-ttu-id="19ca1-1270">Die/proc/[PID]/Mounts,/proc/[PID]/mountinfo und/proc/[PID]/mountstats-Dateien wurden implementiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1270">Implemented the /proc/[pid]/mounts, /proc/[pid]/mountinfo and /proc/[pid]/mountstats files</span></span>
- <span data-ttu-id="19ca1-1271">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1271">Additional bugfixes and improvements</span></span>

</br>

## <a name="build-14901"></a><span data-ttu-id="19ca1-1272">Build 14901</span><span class="sxs-lookup"><span data-stu-id="19ca1-1272">Build 14901</span></span>
<span data-ttu-id="19ca1-1273">Der erste Insider-Build für die Windows 10 Anniversary Update-Version.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1273">First Insider build for the post Windows 10 Anniversary Update release.</span></span>

<span data-ttu-id="19ca1-1274">Allgemeine Windows-Informationen zu Build 14901 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1274">For general Windows information on build 14901 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1275">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1275">Fixed</span></span>
- <span data-ttu-id="19ca1-1276">Korrigieren des nachfolgenden Schrägstrichs</span><span class="sxs-lookup"><span data-stu-id="19ca1-1276">Fixed trailing slash issue</span></span>
    - <span data-ttu-id="19ca1-1277">Befehle wie `$ mv a/c/ a/b/` jetzt funktionieren.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1277">Commands such as `$ mv a/c/ a/b/` now work</span></span>
- <span data-ttu-id="19ca1-1278">Bei der Installation werden jetzt Aufforderungen angezeigt, wenn Ubuntu-Gebiets Schema auf Windows</span><span class="sxs-lookup"><span data-stu-id="19ca1-1278">Installing now prompts if Ubuntu locale should be set to Windows locale</span></span>
- <span data-ttu-id="19ca1-1279">Procfs-Unterstützung für den NS-Ordner</span><span class="sxs-lookup"><span data-stu-id="19ca1-1279">Procfs support for ns folder</span></span>
- <span data-ttu-id="19ca1-1280">Hinzufügen und Entfernen von Bereitstellungs-, procfs-und sysfs-Dateisystemen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1280">Added mount and unmount for tmpfs, procfs and sysfs file systems</span></span>
- <span data-ttu-id="19ca1-1281">Korrigieren von mklod [at] 32-Bit-ABI-Signatur</span><span class="sxs-lookup"><span data-stu-id="19ca1-1281">Fix mknod[at] 32-bit ABI signature</span></span>
- <span data-ttu-id="19ca1-1282">In Dispatch-Modell verschobene Unix-Sockets</span><span class="sxs-lookup"><span data-stu-id="19ca1-1282">Unix sockets moved to dispatch model</span></span>
- <span data-ttu-id="19ca1-1283">Die mit setsockopt festgelegte inet-Socket-empfangener-Puffergröße muss berücksichtigt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1283">INET socket recv buffer size set using the setsockopt should be honored</span></span>
- <span data-ttu-id="19ca1-1284">MSG_CMSG_CLOEXEC UNIX-Socket-Empfangs Nachrichtenflag implementieren</span><span class="sxs-lookup"><span data-stu-id="19ca1-1284">Implement MSG_CMSG_CLOEXEC unix socket receive message flag</span></span>
- <span data-ttu-id="19ca1-1285">Linux-Prozess stdin/stdout-Pipe-Umleitung (GH #2)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1285">Linux process stdin/stdout pipe redirection (GH #2)</span></span>
    - <span data-ttu-id="19ca1-1286">Ermöglicht das Weiterleiten von bash-c-Befehlen in cmd.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1286">Allows for piping of bash -c commands in CMD.</span></span>  <span data-ttu-id="19ca1-1287">Beispiel: > dir | bash-c "grep foo"</span><span class="sxs-lookup"><span data-stu-id="19ca1-1287">Example:  >dir | bash -c "grep foo"</span></span>
- <span data-ttu-id="19ca1-1288">Bash kann nun auf Systemen mit mehreren Seiten Dateien (GH #538 #358) installiert werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1288">Bash can now be installed on systems with multiple pagefiles (GH #538, #358)</span></span>
- <span data-ttu-id="19ca1-1289">Die standardmäßige inet-socketpuffergröße sollte mit der standardmäßigen Ubuntu-Einrichtung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1289">Default INET Socket buffer size should match that of default Ubuntu setup</span></span>
- <span data-ttu-id="19ca1-1290">Ausrichten von xattr-syscalls an listxattr</span><span class="sxs-lookup"><span data-stu-id="19ca1-1290">Align xattr syscalls to listxattr</span></span>
- <span data-ttu-id="19ca1-1291">Gibt nur Schnittstellen mit einer gültigen IPv4-Adresse von siocgifconf zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1291">Only return interfaces with a valid IPv4 address from SIOCGIFCONF</span></span>
- <span data-ttu-id="19ca1-1292">Signal Standardaktion korrigieren, wenn von ptrace eingefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1292">Fix signal default action when injected by ptrace</span></span>
- <span data-ttu-id="19ca1-1293">Implementieren von/proc/sys/VM/min_free_kbytes</span><span class="sxs-lookup"><span data-stu-id="19ca1-1293">implement /proc/sys/vm/min_free_kbytes</span></span>
- <span data-ttu-id="19ca1-1294">Beim Wiederherstellen von Kontext in sigreturn Werte für den Computer Kontext Register verwenden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1294">Use machine context register values when restoring context in sigreturn</span></span>
    - <span data-ttu-id="19ca1-1295">Dadurch wird das Problem behoben, dass Java und javac für einige Benutzer hängen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1295">This resolves the issue where java and javac were hanging for some users</span></span>
- <span data-ttu-id="19ca1-1296">Implementieren von/proc/sys/kernel/Hostname</span><span class="sxs-lookup"><span data-stu-id="19ca1-1296">Implement /proc/sys/kernel/hostname</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1297">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1297">Syscall Support</span></span>
<span data-ttu-id="19ca1-1298">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1298">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1299">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1299">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a><span data-ttu-id="19ca1-1300">Build 14388 bis Windows 10 Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="19ca1-1300">Build 14388 to Windows 10 Anniversary Update</span></span>
<span data-ttu-id="19ca1-1301">Allgemeine Windows-Informationen zu Build 14388 finden Sie im [Windows-Blog](https://aka.ms/14388wip).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1301">For general Windows information on build 14388 visit the [Windows Blog](https://aka.ms/14388wip).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1302">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1302">Fixed</span></span>
- <span data-ttu-id="19ca1-1303">Korrekturen für die Vorbereitung auf das Windows 10 Anniversary Update auf 8/2</span><span class="sxs-lookup"><span data-stu-id="19ca1-1303">Fixes to prepare for the Windows 10 Anniversary Update on 8/2</span></span>
  - <span data-ttu-id="19ca1-1304">Weitere Informationen zu WSL im Anniversary Update finden Sie in unserem [Blog](https://blogs.msdn.microsoft.com/wsl/) .</span><span class="sxs-lookup"><span data-stu-id="19ca1-1304">More information about WSL in the Anniversary Update can be found on our [blog](https://blogs.msdn.microsoft.com/wsl/)</span></span>

<br/>

## <a name="build-14376"></a><span data-ttu-id="19ca1-1305">Build 14376</span><span class="sxs-lookup"><span data-stu-id="19ca1-1305">Build 14376</span></span>
<span data-ttu-id="19ca1-1306">Allgemeine Windows-Informationen zu Build 14376 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1306">For general Windows information on build 14376 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1307">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1307">Fixed</span></span>
- <span data-ttu-id="19ca1-1308">Einige Instanzen entfernt, bei denen apt-get nicht mehr reagiert (GH #493)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1308">Removed some instances where apt-get hangs (GH #493)</span></span>
- <span data-ttu-id="19ca1-1309">Ein Problem wurde behoben, bei dem leere bereit Stellungen nicht ordnungsgemäß behandelt wurden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1309">Fixed an issue where empty mounts were not handled correctly</span></span>
- <span data-ttu-id="19ca1-1310">Ein Problem wurde behoben, bei dem Ramdisks nicht ordnungsgemäß bereitgestellt wurde</span><span class="sxs-lookup"><span data-stu-id="19ca1-1310">Fixed an issue where ramdisks were not mounted correctly</span></span>
- <span data-ttu-id="19ca1-1311">Ändern der UNIX-Socket-Annahme zur Unterstützung von Flags (Teil-GH-#451</span><span class="sxs-lookup"><span data-stu-id="19ca1-1311">Change unix socket accept to support flags (partial GH #451)</span></span>
- <span data-ttu-id="19ca1-1312">Ein gängiger Netzwerk bezogener Bluescreen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1312">Fixed common network related bluescreen</span></span>
- <span data-ttu-id="19ca1-1313">Festes Bluescreen beim Zugriff auf/proc/[PID] > Task (GH #523)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1313">Fixed bluescreen when accessing /proc/[pid]/task (GH #523)</span></span>
- <span data-ttu-id="19ca1-1314">Hohe CPU-Auslastung für einige Pty-Szenarien (GH #488 #504) korrigiert</span><span class="sxs-lookup"><span data-stu-id="19ca1-1314">Fixed high CPU utilization for some pty scenarios (GH #488, #504)</span></span>
- <span data-ttu-id="19ca1-1315">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1315">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14371"></a><span data-ttu-id="19ca1-1316">Build 14371</span><span class="sxs-lookup"><span data-stu-id="19ca1-1316">Build 14371</span></span>
<span data-ttu-id="19ca1-1317">Allgemeine Windows-Informationen zu Build 14371 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1317">For general Windows information on build 14371 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1318">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1318">Fixed</span></span>
- <span data-ttu-id="19ca1-1319">Korrigiertes zeitlichen Rennen mit SIGCHLD und Wait () bei Verwendung von ptrace</span><span class="sxs-lookup"><span data-stu-id="19ca1-1319">Corrected timing race with SIGCHLD and wait() when using ptrace</span></span>
- <span data-ttu-id="19ca1-1320">Es wurde ein gewisses Verhalten korrigiert, wenn Pfade eine nachfolgende/(GH #432)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1320">Corrected some behavior when paths have a trailing /  (GH #432)</span></span>
- <span data-ttu-id="19ca1-1321">Problem mit Fehler beim Umbenennen/Aufheben der Verknüpfung aufgrund von geöffneten Handles für untergeordnete Elemente behoben</span><span class="sxs-lookup"><span data-stu-id="19ca1-1321">Fixed issue with rename/unlink failing due to open handles to children</span></span>
- <span data-ttu-id="19ca1-1322">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1322">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14366"></a><span data-ttu-id="19ca1-1323">Build 14366</span><span class="sxs-lookup"><span data-stu-id="19ca1-1323">Build 14366</span></span>
<span data-ttu-id="19ca1-1324">Allgemeine Windows-Informationen zu Build 14366 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1324">For general Windows information on build 14366 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1325">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1325">Fixed</span></span>
- <span data-ttu-id="19ca1-1326">Korrektur beim Erstellen von Dateien durch symlinks</span><span class="sxs-lookup"><span data-stu-id="19ca1-1326">Fix in file creation through symlinks</span></span>
-   <span data-ttu-id="19ca1-1327">Hinzugefügter listxattr für python (GH 385)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1327">Added listxattr for Python (GH 385)</span></span>
-   <span data-ttu-id="19ca1-1328">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1328">Additional bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1329">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1329">Syscall Support</span></span>
-   <span data-ttu-id="19ca1-1330">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1330">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1331">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1331">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`listxattr`<br/>
<br/>

## <a name="build-14361"></a><span data-ttu-id="19ca1-1332">Build 14361</span><span class="sxs-lookup"><span data-stu-id="19ca1-1332">Build 14361</span></span>
<span data-ttu-id="19ca1-1333">Allgemeine Windows-Informationen zu Build 14361 finden Sie im [Windows-Blog](https://aka.ms/wip14361).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1333">For general Windows information on build 14361 visit the [Windows Blog](https://aka.ms/wip14361).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1334">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1334">Fixed</span></span>
- <span data-ttu-id="19ca1-1335">Bei der Ausführung in bash unter Ubuntu unter Windows wird bei drvfs nun die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1335">DrvFs is now case sensitive when running in Bash on Ubuntu on Windows.</span></span>
  - <span data-ttu-id="19ca1-1336">Benutzer können Case. txt und Case. TXT auf Ihren/mnt/c-Laufwerken</span><span class="sxs-lookup"><span data-stu-id="19ca1-1336">Users may case.txt and CASE.TXT on their /mnt/c drives</span></span>
  - <span data-ttu-id="19ca1-1337">Die Groß-/Kleinschreibung wird nur in bash unter Ubuntu unter Windows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1337">Case sensitivity is only supported within Bash on Ubuntu on Windows.</span></span> <span data-ttu-id="19ca1-1338">Wenn die Dateien außerhalb von bash-NTFS korrekt gemeldet werden, kann es bei der Interaktion mit den Dateien von Windows zu unerwartetem Verhalten kommen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1338">When outside of Bash NTFS will report the files correctly, but unexpected behavior may occur interacting with the files from Windows.</span></span>
  - <span data-ttu-id="19ca1-1339">Beim Stamm der einzelnen Volumes (d.h./mnt/c) wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1339">The root of each volume (i.e. /mnt/c) is not case sensitive</span></span>
  - <span data-ttu-id="19ca1-1340">Weitere Informationen zum Verarbeiten dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1340">More information on handling these files in Windows can be found [here](https://support.microsoft.com/en-us/kb/100625).</span></span>
- <span data-ttu-id="19ca1-1341">Stark verbesserte Pty-/TTY-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1341">Greatly enhanced pty / tty support.</span></span>  <span data-ttu-id="19ca1-1342">Anwendungen wie tmux werden jetzt unterstützt (GH #40)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1342">Applications like TMUX now supported (GH #40)</span></span>
- <span data-ttu-id="19ca1-1343">Installationsproblem behoben, bei dem Benutzerkonten nicht immer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1343">Fixed install issue where user accounts not always created</span></span>
- <span data-ttu-id="19ca1-1344">Optimierte Befehlszeilen-arg-Struktur, die eine extrem lange Argumentliste zulässt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1344">Optimized command line arg structure allowing for extremely long argument list.</span></span> <span data-ttu-id="19ca1-1345">(GH #153)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1345">(GH #153)</span></span>
- <span data-ttu-id="19ca1-1346">Jetzt können READ_ONLY-Dateien und chmod-Dateien aus drvfs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1346">Now able to delete and chmod read_only files from DrvFs</span></span>
- <span data-ttu-id="19ca1-1347">Es wurden einige Instanzen behoben, bei denen das Terminal beim Trennen nicht mehr reagiert (GH #43)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1347">Fixed some instances where the terminal hangs on disconnect (GH #43)</span></span>
- <span data-ttu-id="19ca1-1348">chmod und chown funktionieren jetzt auf TTY-Geräten</span><span class="sxs-lookup"><span data-stu-id="19ca1-1348">chmod and chown now work on tty devices</span></span>
- <span data-ttu-id="19ca1-1349">Verbindung mit 0.0.0.0 und:: As localhost zulassen (GH #388)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1349">Allow connection to 0.0.0.0 and :: as localhost (GH #388)</span></span>
- <span data-ttu-id="19ca1-1350">Sendmsg/recvmsg behandelt nun eine IO-Vektor Länge von > 1 (partielle GH-#376)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1350">Sendmsg/recvmsg now handle an IO vector length of >1 (partial GH #376)</span></span>
- <span data-ttu-id="19ca1-1351">Benutzer können jetzt die automatisch generierte Hostdatei ablehnen (GH #398).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1351">Users can now opt-out of auto-generated hosts file (GH #398)</span></span>
- <span data-ttu-id="19ca1-1352">Automatisches Zuordnen von Linux-Gebiets Schemas zum NT-Gebiets Schema während der Installation (GH #11)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1352">Automatically match Linux locale to the NT locale during install (GH #11)</span></span>
- <span data-ttu-id="19ca1-1353">/Proc/sys/VM/swappiness-Datei hinzugefügt (GH #306)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1353">Added the /proc/sys/vm/swappiness file (GH #306)</span></span>
- <span data-ttu-id="19ca1-1354">"strace" wird jetzt ordnungsgemäß beendet.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1354">strace now exits correctly</span></span>
- <span data-ttu-id="19ca1-1355">Erneuten Öffnen von Pipes über/proc/self/fd (GH #222) zulassen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1355">Allow pipes to be reopened through /proc/self/fd (GH #222)</span></span>
- <span data-ttu-id="19ca1-1356">Ausblenden von Verzeichnissen unter "%LocalAppData%\lxss" aus drvfs (GH #270)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1356">Hide directories under %LOCALAPPDATA%\lxss from DrvFs (GH #270)</span></span>
- <span data-ttu-id="19ca1-1357">Bessere Behandlung von bash. exe ~.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1357">Better handling of bash.exe ~.</span></span>  <span data-ttu-id="19ca1-1358">Befehle wie "bash ~-c ls" werden jetzt unterstützt (GH #467).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1358">Commands like “bash ~ -c ls” now supported (GH #467)</span></span>
- <span data-ttu-id="19ca1-1359">Sockets Benachrichtigen, dass epoll beim Herunterfahren verfügbar ist (GH #271)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1359">Sockets now notify epoll read available during shutdown (GH #271)</span></span>
- <span data-ttu-id="19ca1-1360">lxrun/Uninstall bietet eine bessere Aufgabe zum Löschen der Dateien und Ordner.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1360">lxrun /uninstall does a better job of deleting the files and folders</span></span>
- <span data-ttu-id="19ca1-1361">Korrigierte PS-f (GH #246)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1361">Corrected ps -f (GH #246)</span></span>
- <span data-ttu-id="19ca1-1362">Verbesserte Unterstützung für X11-apps, z. b. XEmacs (GH #481)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1362">Improved support for x11 apps such as xEmacs (GH #481)</span></span>
- <span data-ttu-id="19ca1-1363">Aktualisierte anfängliche Thread Stapelgröße, um der standardmäßigen Ubuntu-Einstellung zu entsprechen und die Größe ordnungsgemäß an get_rlimit syscall (GH #172 #258) zu melden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1363">Updated initial thread stack size to match default Ubuntu setting and reporting the size correctly to the get_rlimit syscall (GH #172, #258)</span></span>
- <span data-ttu-id="19ca1-1364">Verbesserte Berichterstellung von Namen von Pico-Prozess Images (z. b. für die Überwachung)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1364">Improved reporting of pico process image names (e.g., for auditing)</span></span>
- <span data-ttu-id="19ca1-1365">Implementierter/proc/mountinfo for DF-Befehl</span><span class="sxs-lookup"><span data-stu-id="19ca1-1365">Implemented /proc/mountinfo for df command</span></span>
- <span data-ttu-id="19ca1-1366">Der Symlink-Fehlercode für den untergeordneten Namen wurde korrigiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1366">Fixed symlink error code for child name .</span></span> <span data-ttu-id="19ca1-1367">und..</span><span class="sxs-lookup"><span data-stu-id="19ca1-1367">and ..</span></span>
- <span data-ttu-id="19ca1-1368">Weitere Verbesserungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1368">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1369">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1369">Syscall Support</span></span>
<span data-ttu-id="19ca1-1370">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1370">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1371">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1371">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a><span data-ttu-id="19ca1-1372">Build 14352</span><span class="sxs-lookup"><span data-stu-id="19ca1-1372">Build 14352</span></span>
<span data-ttu-id="19ca1-1373">Allgemeine Windows-Informationen zu Build 14352 finden Sie im [Windows-Blog](https://aka.ms/wip14352).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1373">For general Windows information on build 14352 visit the [Windows Blog](https://aka.ms/wip14352).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1374">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1374">Fixed</span></span>
- <span data-ttu-id="19ca1-1375">Ein Problem wurde behoben, bei dem große Dateien nicht ordnungsgemäß heruntergeladen/erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1375">Fixed issue where large files were not downloaded / created correctly.</span></span>  <span data-ttu-id="19ca1-1376">Dadurch wird die Blockierung von NPM und anderen Szenarien (GH #3, GH #313) verhindert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1376">This should unblock npm and other scenarios (GH #3, GH #313)</span></span>
- <span data-ttu-id="19ca1-1377">Einige Instanzen entfernt, bei denen Sockets hängen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1377">Removed some instances where sockets hang</span></span>
- <span data-ttu-id="19ca1-1378">Einige ptrace-Fehler wurden korrigiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1378">Corrected some ptrace errors</span></span>
- <span data-ttu-id="19ca1-1379">Problem mit WSL behoben, das die Angabe von Dateinamen mit mehr als 255 Zeichen zulässt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1379">Fixed issue with WSL allowing filenames longer than 255 characters</span></span>
- <span data-ttu-id="19ca1-1380">Verbesserte Unterstützung für nicht englische Zeichen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1380">Improved support for non-English characters</span></span>
- <span data-ttu-id="19ca1-1381">Aktuelle Windows-Zeit Zonendaten hinzufügen und als Standard festlegen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1381">Add current Windows timezone data and set as default</span></span>
- <span data-ttu-id="19ca1-1382">Eindeutige Geräte-IDs für jeden Einstellungspunkt (JRE Fix – GH #49)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1382">Unique device id’s for each mount point (jre fix – GH #49)</span></span>
- <span data-ttu-id="19ca1-1383">Korrigieren eines Problems mit Pfaden, die "." enthalten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1383">Correct issue with paths containing “.”</span></span> <span data-ttu-id="19ca1-1384">und ".."</span><span class="sxs-lookup"><span data-stu-id="19ca1-1384">and “..”</span></span>
- <span data-ttu-id="19ca1-1385">Hinzugefügte FIFO-Unterstützung (GH #71)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1385">Added Fifo support (GH #71)</span></span>
- <span data-ttu-id="19ca1-1386">Aktualisiertes Format von "resolv. conf" entsprechend dem systemeigenen Ubuntu-Format</span><span class="sxs-lookup"><span data-stu-id="19ca1-1386">Updated format of resolv.conf to match native Ubuntu format</span></span>
- <span data-ttu-id="19ca1-1387">Einige procfs-Bereinigung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1387">Some procfs cleanup</span></span>
- <span data-ttu-id="19ca1-1388">Aktiviertes Ping für Administrator Konsolen (GH #18)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1388">Enabled ping for Administrator consoles (GH #18)</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1389">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1389">Syscall Support</span></span>
<span data-ttu-id="19ca1-1390">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1390">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1391">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1391">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a><span data-ttu-id="19ca1-1392">Build 14342</span><span class="sxs-lookup"><span data-stu-id="19ca1-1392">Build 14342</span></span>
<span data-ttu-id="19ca1-1393">Allgemeine Windows-Informationen zu Build 14342 im [Windows-Blog](https://aka.ms/wip14342).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1393">For general Windows information on build 14342 the [Windows Blog](https://aka.ms/wip14342).</span></span> <br/>

<span data-ttu-id="19ca1-1394">Informationen zu volfs und drivefs finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1394">Information on VolFs and DriveFs can be found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="19ca1-1395">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1395">Fixed</span></span>
- <span data-ttu-id="19ca1-1396">Installationsproblem behoben, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen enthielt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1396">Fixed install issue when the Windows user had Unicode characters in the username</span></span>
- <span data-ttu-id="19ca1-1397">Die Problem Umgehung "apt-get update udev" in den FAQ wird jetzt standardmäßig bei der ersten Ausführung bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1397">The apt-get update udev workaround in the FAQ is now provided by default on first run</span></span>
- <span data-ttu-id="19ca1-1398">Aktivierte symlinks in drivefs-<drive>Verzeichnissen (im)</span><span class="sxs-lookup"><span data-stu-id="19ca1-1398">Enabled symlinks in DriveFs (/mnt/<drive>) directories</span></span>
- <span data-ttu-id="19ca1-1399">Symlinks funktionieren nun zwischen drivefs und volfs</span><span class="sxs-lookup"><span data-stu-id="19ca1-1399">Symlinks now work between DriveFs and VolFs</span></span>
- <span data-ttu-id="19ca1-1400">Problem bei der übergeordneten Pfad Verarbeitung adressiert: ls.//funktioniert jetzt erwartungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1400">Addressed top level path parsing issue: ls .// will now work as expected</span></span>
- <span data-ttu-id="19ca1-1401">NPM-Installation auf drivefs und die-g-Optionen funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1401">npm install on DriveFs and the -g options are now working</span></span>
- <span data-ttu-id="19ca1-1402">Problem behoben, das den Start des PHP-Servers verhindert</span><span class="sxs-lookup"><span data-stu-id="19ca1-1402">Fixed issue preventing PHP server from launching</span></span>
- <span data-ttu-id="19ca1-1403">Aktualisierte Standard Umgebungs Werte, z. b. $Path, um System eigenes Ubuntu zu erreichen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1403">Updated default environment values, such as $PATH to closer match native Ubuntu</span></span>
- <span data-ttu-id="19ca1-1404">Ein wöchentlicher Wartungs Task in Windows zum Aktualisieren des APT-Paket Caches wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1404">Added a weekly maintenance task in Windows to update the apt package cache</span></span>
- <span data-ttu-id="19ca1-1405">Problem bei der Überprüfung elf Header behoben, WSL unterstützt jetzt alle Melkor-Optionen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1405">Fixed issue with ELF header validation, WSL now supports all Melkor options</span></span>
- <span data-ttu-id="19ca1-1406">Zsh Shell ist funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="19ca1-1406">Zsh shell is functional</span></span>
- <span data-ttu-id="19ca1-1407">Vorkompilierte go-Binärdateien werden jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1407">Precompiled Go binaries are now supported</span></span>
- <span data-ttu-id="19ca1-1408">Eingabeaufforderung für bash. exe: erste Testlauf ist nun ordnungsgemäß lokalisiert.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1408">Prompting on Bash.exe first run is now localized correctly</span></span>
- <span data-ttu-id="19ca1-1409">/proc/meminfo gibt jetzt korrekte Informationen zurück.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1409">/proc/meminfo now returns correct information</span></span>
- <span data-ttu-id="19ca1-1410">Sockets werden jetzt in VFS unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1410">Sockets now supported in VFS</span></span>
- <span data-ttu-id="19ca1-1411">/dev jetzt als tempfs eingebunden</span><span class="sxs-lookup"><span data-stu-id="19ca1-1411">/dev now mounted as tempfs</span></span>
- <span data-ttu-id="19ca1-1412">FIFO wird jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1412">Fifo now supported</span></span>
- <span data-ttu-id="19ca1-1413">Mehr Kernsysteme werden nun ordnungsgemäß in/proc/cpuinfo angezeigt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1413">Multi-core systems now showing correctly in /proc/cpuinfo</span></span>
- <span data-ttu-id="19ca1-1414">Weitere Verbesserungen und Fehlermeldungen, die während der ersten Testlauf</span><span class="sxs-lookup"><span data-stu-id="19ca1-1414">Additional improvements and error messages downloading during first run</span></span>
- <span data-ttu-id="19ca1-1415">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1415">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="19ca1-1416">Unterstützte syscall-Liste weiter unten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1416">Supported syscall list below.</span></span>
- <span data-ttu-id="19ca1-1417">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1417">Additional bugfixes and improvements</span></span>

### <a name="known-issues"></a><span data-ttu-id="19ca1-1418">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="19ca1-1418">Known Issues</span></span>
- <span data-ttu-id="19ca1-1419">".." Wird nicht aufgelöst.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1419">Not resolving ‘..’</span></span> <span data-ttu-id="19ca1-1420">in einigen Fällen ordnungsgemäß auf drivefs</span><span class="sxs-lookup"><span data-stu-id="19ca1-1420">correctly on DriveFs in some cases</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1421">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1421">Syscall Support</span></span>
<span data-ttu-id="19ca1-1422">Im folgenden finden Sie eine Liste der neuen oder verbesserten syscalls, die in WSL implementiert werden können.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1422">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1423">Die syscalls in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1423">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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

## <a name="build-14332"></a><span data-ttu-id="19ca1-1424">Build 14332</span><span class="sxs-lookup"><span data-stu-id="19ca1-1424">Build 14332</span></span>

<span data-ttu-id="19ca1-1425">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14332).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1425">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14332).</span></span> <br/>


### <a name="fixed"></a><span data-ttu-id="19ca1-1426">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1426">Fixed</span></span>
- <span data-ttu-id="19ca1-1427">Bessere resolv. conf-Generierung einschließlich Priorisieren von DNS-Einträgen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1427">Better resolv.conf generation including prioritizing DNS entries</span></span>
- <span data-ttu-id="19ca1-1428">Problem beim Verschieben von Dateien und Verzeichnissen zwischen/mnt-und nicht-/mnt-Laufwerken</span><span class="sxs-lookup"><span data-stu-id="19ca1-1428">Issue with moving files and directories between /mnt and non-/mnt drives</span></span>
- <span data-ttu-id="19ca1-1429">Tar-Dateien können jetzt mit symlinks erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1429">Tar files can now be created with symlinks</span></span>
- <span data-ttu-id="19ca1-1430">Standardmäßiges/Run/Lock-Verzeichnis bei der Instanzerstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1430">Added default /run/lock directory on instance creation</span></span>
- <span data-ttu-id="19ca1-1431">Aktualisieren von/dev/null, um die richtigen stat-Informationen zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="19ca1-1431">Update /dev/null to return proper stat info</span></span>
- <span data-ttu-id="19ca1-1432">Weitere Fehler beim Herunterladen während der ersten Testlauf</span><span class="sxs-lookup"><span data-stu-id="19ca1-1432">Additional errors when downloading during first run</span></span>
- <span data-ttu-id="19ca1-1433">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1433">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="19ca1-1434">Unterstützte syscall-Liste weiter unten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1434">Supported syscall list below.</span></span>
- <span data-ttu-id="19ca1-1435">Weitere Verbesserungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1435">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1436">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1436">Syscall Support</span></span>
<span data-ttu-id="19ca1-1437">Im folgenden finden Sie den neuen syscall-Wert, der in WSL implementiert ist.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1437">Below is the new syscall that has some implementation in WSL.</span></span> <span data-ttu-id="19ca1-1438">Der syscall in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1438">The syscall on this list is supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a><span data-ttu-id="19ca1-1439">Build 14328</span><span class="sxs-lookup"><span data-stu-id="19ca1-1439">Build 14328</span></span>

<span data-ttu-id="19ca1-1440">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14328).</span><span class="sxs-lookup"><span data-stu-id="19ca1-1440">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14328).</span></span> <br/>


### <a name="new-features"></a><span data-ttu-id="19ca1-1441">Neue Funktionen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1441">New Features</span></span>
* <span data-ttu-id="19ca1-1442">Unterstützt jetzt Linux-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1442">Now support Linux users.</span></span>  <span data-ttu-id="19ca1-1443">Wenn Sie bash unter Ubuntu unter Windows installieren, werden Sie aufgefordert, einen Linux-Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1443">Installing Bash on Ubuntu on Windows will prompt for creation of a Linux user.</span></span>  <span data-ttu-id="19ca1-1444">Weitere Informationen finden Sie unter https://aka.ms/wslusers</span><span class="sxs-lookup"><span data-stu-id="19ca1-1444">For more information, visit https://aka.ms/wslusers</span></span>
* <span data-ttu-id="19ca1-1445">Der Hostname ist jetzt auf den Windows-Computernamen festgelegt.@localhost</span><span class="sxs-lookup"><span data-stu-id="19ca1-1445">Hostname is now set to the Windows computer name, no more @localhost</span></span>
* <span data-ttu-id="19ca1-1446">Weitere Informationen zu Build 14328 finden Sie unter: https://aka.ms/wip14328</span><span class="sxs-lookup"><span data-stu-id="19ca1-1446">For more information on build 14328, visit: https://aka.ms/wip14328</span></span>

### <a name="fixed"></a><span data-ttu-id="19ca1-1447">Fest</span><span class="sxs-lookup"><span data-stu-id="19ca1-1447">Fixed</span></span>
* <span data-ttu-id="19ca1-1448">Symlink-Verbesserungen<drive> für nicht-im-Dateien</span><span class="sxs-lookup"><span data-stu-id="19ca1-1448">Symlink improvements for non /mnt/<drive> files</span></span>
    * <span data-ttu-id="19ca1-1449">NPM-Installation funktioniert jetzt</span><span class="sxs-lookup"><span data-stu-id="19ca1-1449">npm install now works</span></span>
    * <span data-ttu-id="19ca1-1450">JDK/JRE kann nun mithilfe der [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html)gefundenen Anweisungen installiert werden.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1450">jdk / jre now installable using instructions found [here](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span></span>
    * <span data-ttu-id="19ca1-1451">bekanntes Problem: symlinks funktionieren bei Windows-bereit Stellungen nicht.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1451">known issue: symlinks do not work for Windows mounts.</span></span>  <span data-ttu-id="19ca1-1452">Funktionen werden in einem späteren Build verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1452">Functionality will be available in a later build</span></span>
* <span data-ttu-id="19ca1-1453">Top und htop jetzt anzeigen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1453">top and htop now display</span></span>
* <span data-ttu-id="19ca1-1454">Zusätzliche Fehlermeldungen bei einigen Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="19ca1-1454">Additional error messages for some install failures</span></span>
* <span data-ttu-id="19ca1-1455">Syscall-Verbesserungen und Fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1455">Syscall improvements and bugfixes.</span></span>  <span data-ttu-id="19ca1-1456">Unterstützte syscall-Liste weiter unten.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1456">Supported syscall list below.</span></span>
* <span data-ttu-id="19ca1-1457">Weitere Verbesserungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="19ca1-1457">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="19ca1-1458">Syscall-Unterstützung</span><span class="sxs-lookup"><span data-stu-id="19ca1-1458">Syscall Support</span></span>
<span data-ttu-id="19ca1-1459">Im folgenden finden Sie eine Liste der syscalls, die eine Implementierung in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1459">Below is a list of syscalls that have some implementation in WSL.</span></span>  <span data-ttu-id="19ca1-1460">Syscalls für diese Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19ca1-1460">Syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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
