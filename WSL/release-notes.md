---
title: Anmerkungen zu dieser Version des Windows-Subsystems für Linux
description: Anmerkungen zu dieser Version des Windows-Subsystems für Linux  Wöchentlich aktualisiert.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu
author: benhillis
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 36ea641e-4d49-4881-84eb-a9ca85b1cdf4
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 0dcf4519877fac5b838d4542dfd088cb6d233353
ms.sourcegitcommit: 0fa3b02b36dc49779e165e689dfded4f3b727124
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71249186"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a><span data-ttu-id="02d0f-105">Anmerkungen zu dieser Version des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="02d0f-105">Release Notes for Windows Subsystem for Linux</span></span>

## <a name="build-18990"></a><span data-ttu-id="02d0f-106">Build 18990</span><span class="sxs-lookup"><span data-stu-id="02d0f-106">Build 18990</span></span>
<span data-ttu-id="02d0f-107">Allgemeine Windows-Informationen zu Build 18990 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-107">For general Windows information on build 18990 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span></span>

* <span data-ttu-id="02d0f-108">Verbessern der Leistung für Verzeichnisauflistungen in \\wsl$</span><span class="sxs-lookup"><span data-stu-id="02d0f-108">Improve the performance for directory listings in \\wsl$</span></span>
* <span data-ttu-id="02d0f-109">[WSL2] Einführen zusätzlicher Entropie beim Systemstart [GH 4416]</span><span class="sxs-lookup"><span data-stu-id="02d0f-109">[WSL2] Inject additional boot entropy [GH 4416]</span></span>
* <span data-ttu-id="02d0f-110">[WSL2] Problembehebung für Windows-Interop bei der Verwendung von „su“ / „sudo“ [GH 4465]</span><span class="sxs-lookup"><span data-stu-id="02d0f-110">[WSL2] Fix for Windows interop when using su / sudo [GH 4465]</span></span>


## <a name="build-18980"></a><span data-ttu-id="02d0f-111">Build 18980</span><span class="sxs-lookup"><span data-stu-id="02d0f-111">Build 18980</span></span>
<span data-ttu-id="02d0f-112">Allgemeine Windows-Informationen zu Build 18980 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-112">For general Windows information on build 18980 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span></span>

* <span data-ttu-id="02d0f-113">Korrektur des Lesen von symbolischen Verknüpfungen, die FILE_READ_DATA verweigern.</span><span class="sxs-lookup"><span data-stu-id="02d0f-113">Fix reading symlinks that deny FILE_READ_DATA.</span></span> <span data-ttu-id="02d0f-114">Dies umfasst alle symbolischen Verknüpfungen, die von Windows aus Gründen der Abwärtskompatibilität erstellt werden, z.B. „C:\Dokumente und Einstellungen“ und eine Reihe von symbolischen Verknüpfungen im Benutzerprofilverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="02d0f-114">This includes all the symlinks Windows creates for backwards compatibility such as "C:\Document and Settings" and a bunch of symlinks in the user profile directory</span></span>
* <span data-ttu-id="02d0f-115">Festlegen eines unerwarteten Dateisystemzustands als nicht schwerwiegend [GH 4334, 4305]</span><span class="sxs-lookup"><span data-stu-id="02d0f-115">Make unexpected filesystem state non-fatal [GH 4334, 4305]</span></span>
* <span data-ttu-id="02d0f-116">[WSL2] Hinzufügen von Unterstützung für arm64, wenn Ihre CPU/Firmware Virtualisierung unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d0f-116">[WSL2] Add support for arm64 if your CPU / firmware supports virtualization</span></span>
* <span data-ttu-id="02d0f-117">[WSL2] Zulassen der Anzeige von Kernelprotokollen durch nicht berechtigte Benutzer</span><span class="sxs-lookup"><span data-stu-id="02d0f-117">[WSL2] Allow unprivileged users to view kernel log</span></span>
* <span data-ttu-id="02d0f-118">[WSL2] Korrigieren des Ausgaberelays, wenn stdout/stderr-Sockets geschlossen wurden [GH 4375]</span><span class="sxs-lookup"><span data-stu-id="02d0f-118">[WSL2] Fix output relay when stdout / stderr sockets have been closed [GH 4375]</span></span>
* <span data-ttu-id="02d0f-119">[WSL2] Unterstützung von Akku- und AC-Adapter-Passthrough</span><span class="sxs-lookup"><span data-stu-id="02d0f-119">[WSL2] Support battery and AC adapter passthrough</span></span>
* <span data-ttu-id="02d0f-120">[WSL2] Aktualisieren des Linux-Kernels auf 4.19.67</span><span class="sxs-lookup"><span data-stu-id="02d0f-120">[WSL2] Update Linux kernel to 4.19.67</span></span>
* <span data-ttu-id="02d0f-121">Hinzufügen der Möglichkeit, den Standardbenutzernamen in „/etc/wsl.conf“ festzulegen:</span><span class="sxs-lookup"><span data-stu-id="02d0f-121">Add the ability to set default username in /etc/wsl.conf:</span></span>
```
[user]
default=root
```

## <a name="build-18975"></a><span data-ttu-id="02d0f-122">Build 18975</span><span class="sxs-lookup"><span data-stu-id="02d0f-122">Build 18975</span></span>
<span data-ttu-id="02d0f-123">Allgemeine Windows-Informationen zu Build 18975 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-123">For general Windows information on build 18975 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span></span>

* <span data-ttu-id="02d0f-124">[WSL2] Korrektur einer Reihe von Problemen mit der localhost-Zuverlässigkeit [GH 4340]</span><span class="sxs-lookup"><span data-stu-id="02d0f-124">[WSL2] Fixed a number of localhost reliability issues [GH 4340]</span></span>

## <a name="build-18970"></a><span data-ttu-id="02d0f-125">Build 18970</span><span class="sxs-lookup"><span data-stu-id="02d0f-125">Build 18970</span></span>
<span data-ttu-id="02d0f-126">Allgemeine Windows-Informationen zu Build 18970 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-126">For general Windows information on build 18970 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span></span>

* <span data-ttu-id="02d0f-127">[WSL2] Synchronisierung der Uhrzeit mit der Hostzeit, wenn das System nach dem Ruhezustand fortgesetzt wird [GH 4245]</span><span class="sxs-lookup"><span data-stu-id="02d0f-127">[WSL2] Sync time with host time when system resumes from sleep state [GH 4245]</span></span>
* <span data-ttu-id="02d0f-128">[WSL2] Nach Möglichkeit Erstellen symbolischer NT-Verknüpfungen auf den Windows-Volumes</span><span class="sxs-lookup"><span data-stu-id="02d0f-128">[WSL2] Create NT symlinks on the Windows volumes when possible.</span></span>
* <span data-ttu-id="02d0f-129">[WSL2] Erstellen von Distributionen in den UTS-, IPC-, PID- und Mount-Namespaces.</span><span class="sxs-lookup"><span data-stu-id="02d0f-129">[WSL2] Create distros in UTS, IPC, PID, and Mount namespaces.</span></span>
* <span data-ttu-id="02d0f-130">[WSL2] Korrigieren des localhost-Portrelays, wenn der Server direkt an localhost gebunden wird [GH 4353]</span><span class="sxs-lookup"><span data-stu-id="02d0f-130">[WSL2] Fix localhost port relay when server binds to localhost directly [GH 4353]</span></span>
* <span data-ttu-id="02d0f-131">[WSL2] Korrigieren von Interop, wenn die Ausgabe umgeleitet wird [GH 4337]</span><span class="sxs-lookup"><span data-stu-id="02d0f-131">[WSL2] Fix interop when output is redirected [GH 4337]</span></span>
* <span data-ttu-id="02d0f-132">[WSL2] Unterstützung der Übersetzung absoluter symbolischer NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-132">[WSL2] Support translating absolute NT symlinks.</span></span>
* <span data-ttu-id="02d0f-133">[WSL2] Aktualisieren des Kernels auf 4.19.59</span><span class="sxs-lookup"><span data-stu-id="02d0f-133">[WSL2] Update kernel to 4.19.59</span></span>
* <span data-ttu-id="02d0f-134">[WSL2] Ordnungsgemäße Festlegung der Subnetzmaske für eth0.</span><span class="sxs-lookup"><span data-stu-id="02d0f-134">[WSL2] Properly set subnet mask for eth0.</span></span>
* <span data-ttu-id="02d0f-135">[WSL2] Ändern der Logik, um die Konsolenworkerschleife zu verlassen, wenn das Beendigungsereignis signalisiert wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-135">[WSL2] Change logic to break out of console worker loop when exit event is signaled.</span></span>
* <span data-ttu-id="02d0f-136">[WSL2] Auswerfen der Distributions-VHD, wenn die Distribution nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-136">[WSL2] Eject distribution vhd when the distro is not running.</span></span>
* <span data-ttu-id="02d0f-137">[WSL2] Korrigieren der Analysebibliothek, um leere Werte ordnungsgemäß zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-137">[WSL2] Fix config parsing library to correctly handle empty values.</span></span>
* <span data-ttu-id="02d0f-138">[WSL2] Unterstützung von Docker Desktop durch Erstellen von distributionsübergreifenden Einbindungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-138">[WSL2] Support Docker Desktop by creating cross distro mounts.</span></span> <span data-ttu-id="02d0f-139">Dieses Verhalten kann durch eine Distribution übernommen werden, indem die folgende Zeile der Datei „/etc/wsl.conf“ hinzugefügt wird:</span><span class="sxs-lookup"><span data-stu-id="02d0f-139">A distro can opt-in to this behavior by adding the following line to the /etc/wsl.conf file:</span></span>
```
[automount]
crossDistro = true
```

## <a name="build-18945"></a><span data-ttu-id="02d0f-140">Build 18945</span><span class="sxs-lookup"><span data-stu-id="02d0f-140">Build 18945</span></span>
<span data-ttu-id="02d0f-141">Allgemeine Windows-Informationen zu Build 18945 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-141">For general Windows information on build 18945 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-142">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-142">WSL</span></span>
* <span data-ttu-id="02d0f-143">[WSL2] Zulassen, dass der Zugriff auf lauschende TCP-Sockets in WSL2 über „localhost:port“ vom Host erfolgen kann.</span><span class="sxs-lookup"><span data-stu-id="02d0f-143">[WSL2] Allow listening tcp sockets in WSL2 to be accessible from the host by using localhost:port</span></span>
* <span data-ttu-id="02d0f-144">[WSL2] Korrekturen für Installations- und Konvertierungsfehler und zusätzliche Diagnose zur Nachverfolgung zukünftiger Probleme [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="02d0f-144">[WSL2] Fixes for install / conversion failures and additional diagnostics to track down future issues [GH 4105]</span></span> 
* <span data-ttu-id="02d0f-145">[WSL2] Verbessern der Diagnose von WSL2-Netzwerkproblemen</span><span class="sxs-lookup"><span data-stu-id="02d0f-145">[WSL2] Improve diagnosability of WSL2 network issues</span></span>
* <span data-ttu-id="02d0f-146">[WSL2] Aktualisieren der Kernelversion auf 4.19.55</span><span class="sxs-lookup"><span data-stu-id="02d0f-146">[WSL2] Update kernel version to 4.19.55</span></span>
* <span data-ttu-id="02d0f-147">[WSL2] Aktualisieren des Kernels mit Konfigurationsoptionen, die für Docker erforderlich sind [GH 4165]</span><span class="sxs-lookup"><span data-stu-id="02d0f-147">[WSL2] Update kernel with config options required for docker [GH 4165]</span></span>
* <span data-ttu-id="02d0f-148">[WSL2] Erhöhen der Anzahl der CPUs, die der Lightweight Utility-VM zugeordnet sind, um eine mit dem Host identische Anzahl zu erreichen (wurde zuvor durch CONFIG_NR_CPUS in der Kernelkonfiguration auf 8 begrenzt) [GH 4137]</span><span class="sxs-lookup"><span data-stu-id="02d0f-148">[WSL2] Increase the number of CPUs assigned to the lightweight utility VM to be the same as the host (was previously capped at 8 by CONFIG_NR_CPUS in the kernel config) [GH 4137]</span></span>
* <span data-ttu-id="02d0f-149">[WSL2] Erstellen einer Auslagerungsdatei für die WSL2-Lightweight-VM</span><span class="sxs-lookup"><span data-stu-id="02d0f-149">[WSL2] Create a swap file for the WSL2 lightweight VM</span></span>
* <span data-ttu-id="02d0f-150">[WSL2] Zulassen, dass Benutzereinbindungen über die \\\\wsl$\\-Distribution (z.B. sshfs) sichtbar sind [GH 4172]</span><span class="sxs-lookup"><span data-stu-id="02d0f-150">[WSL2] Allow user mounts to be visible via \\\\wsl$\\distro (for example sshfs) [GH 4172]</span></span>
* <span data-ttu-id="02d0f-151">[WSL2] Verbessern der Leistung des 9P-Dateisystems</span><span class="sxs-lookup"><span data-stu-id="02d0f-151">[WSL2] Improve 9p filesystem performance</span></span>
* <span data-ttu-id="02d0f-152">[WSL2] Sicherstellen, dass die VHD-ACL nicht unbegrenzt anwächst [GH 4126]</span><span class="sxs-lookup"><span data-stu-id="02d0f-152">[WSL2] Ensure vhd ACL does not grow unbounded [GH 4126]</span></span>
* <span data-ttu-id="02d0f-153">[WSL2] Aktualisieren der Kernelkonfiguration für die Unterstützung von squashfs und xt_conntrack [GH 4107, 4123]</span><span class="sxs-lookup"><span data-stu-id="02d0f-153">[WSL2] Update kernel config to support squashfs and xt_conntrack [GH 4107, 4123]</span></span>
* <span data-ttu-id="02d0f-154">[WSL2] Korrektur für interopaktivierte „/etc/wsl.conf“-Option [GH 4140]</span><span class="sxs-lookup"><span data-stu-id="02d0f-154">[WSL2] Fix for interop.enabled /etc/wsl.conf option [GH 4140]</span></span>
* <span data-ttu-id="02d0f-155">[WSL2] Rückgabe von ENOTSUP, wenn das Dateisystem EAS nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d0f-155">[WSL2] Return ENOTSUP if the file system does not support EAs</span></span>
* <span data-ttu-id="02d0f-156">[WSL2] Korrigieren von CopyFile-Hänger mit \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="02d0f-156">[WSL2] Fix CopyFile hang with \\\\wsl$</span></span>
* <span data-ttu-id="02d0f-157">Umschalten von Standard-umask in 0022 und Hinzufügen der filesystem.umask-Einstellung zu „/etc/wsl.conf“</span><span class="sxs-lookup"><span data-stu-id="02d0f-157">Switch default umask to 0022 and add filesystem.umask setting to /etc/wsl.conf</span></span>
* <span data-ttu-id="02d0f-158">Korrigieren von wslpath, um symbolische Verknüpfungen ordnungsgemäß aufzulösen, dies wurde in 19h1 zurückgesetzt [GH 4078]</span><span class="sxs-lookup"><span data-stu-id="02d0f-158">Fix wslpath to properly resolve symlinks, this was regressed in 19h1 [GH 4078]</span></span>
* <span data-ttu-id="02d0f-159">Einführung der Datei „%UserProfile%\\.wslconfig“ für die Optimierung der WSL2-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-159">Introduce %UserProfile%\\.wslconfig file for tweaking WSL2 settings</span></span>
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

## <a name="build-18917"></a><span data-ttu-id="02d0f-160">Build 18917</span><span class="sxs-lookup"><span data-stu-id="02d0f-160">Build 18917</span></span>
<span data-ttu-id="02d0f-161">Allgemeine Windows-Informationen zu Build 18917 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-161">For general Windows information on build 18917 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-162">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-162">WSL</span></span>
* <span data-ttu-id="02d0f-163">WSL 2 ist Jetzt verfügbar!</span><span class="sxs-lookup"><span data-stu-id="02d0f-163">WSL 2 is now available!</span></span> <span data-ttu-id="02d0f-164">Weitere Informationen finden Sie im [Blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-164">Please see [blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) for more details.</span></span>
* <span data-ttu-id="02d0f-165">Korrektur einer Regression, bei der das Starten von Windows-Prozessen über symbolische Verknüpfungen nicht ordnungsgemäß funktioniert hat [GH 3999]</span><span class="sxs-lookup"><span data-stu-id="02d0f-165">Fix a regression where launching Windows processes via symlinks did not work correctly [GH 3999]</span></span>
* <span data-ttu-id="02d0f-166">Hinzufügen der Optionen wsl.exe --list --verbose, wsl.exe --list --quiet und wsl.exe --import --version zu „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="02d0f-166">Add wsl.exe --list --verbose, wsl.exe --list --quiet, and wsl.exe --import --version options to wsl.exe</span></span>
* <span data-ttu-id="02d0f-167">Hinzufügen der Option wsl.exe --shutdown</span><span class="sxs-lookup"><span data-stu-id="02d0f-167">Add wsl.exe --shutdown option</span></span>
* <span data-ttu-id="02d0f-168">Plan 9: Zulassen des Öffnend eines Verzeichnisses für einen erfolgreichen Schreibvorgang</span><span class="sxs-lookup"><span data-stu-id="02d0f-168">Plan 9: Allow opening a directory for write to succeed</span></span>

## <a name="build-18890"></a><span data-ttu-id="02d0f-169">Build 18890</span><span class="sxs-lookup"><span data-stu-id="02d0f-169">Build 18890</span></span>
<span data-ttu-id="02d0f-170">Allgemeine Windows-Informationen zu Build 18890 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-170">For general Windows information on build 18890 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-171">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-171">WSL</span></span>
* <span data-ttu-id="02d0f-172">Nicht blockierender Socketverlust [GH 2913]</span><span class="sxs-lookup"><span data-stu-id="02d0f-172">Non-blocking socket leak [GH 2913]</span></span>
* <span data-ttu-id="02d0f-173">EOF-Eingabe für Terminal kann nachfolgende Lesevorgänge blockieren [GH 3421]</span><span class="sxs-lookup"><span data-stu-id="02d0f-173">EOF input to terminal can block subsequent reads [GH 3421]</span></span>
* <span data-ttu-id="02d0f-174">Aktualisieren des resolv.conf-Headers, damit er auf „wsl.conf“ verweist [in GH 3928 beschrieben].</span><span class="sxs-lookup"><span data-stu-id="02d0f-174">Update resolv.conf header to refer to wsl.conf [discussed in GH 3928]</span></span>
* <span data-ttu-id="02d0f-175">Deadlock im epoll-Löschcode [GH 3922]</span><span class="sxs-lookup"><span data-stu-id="02d0f-175">Deadlock in epoll delete code [GH 3922]</span></span>
* <span data-ttu-id="02d0f-176">Verarbeiten von Leerzeichen in Argumenten für --import und --export [GH 3932]</span><span class="sxs-lookup"><span data-stu-id="02d0f-176">Handle spaces in arguments to --import and –export [GH 3932]</span></span>
* <span data-ttu-id="02d0f-177">Erweitern von mit mmap behandelten Dateien funktioniert nicht ordnungsgemäß [GH 3939]</span><span class="sxs-lookup"><span data-stu-id="02d0f-177">Extending mmap’d files does not work properly [GH 3939]</span></span>
* <span data-ttu-id="02d0f-178">Korrektur eines Problems mit ARM64 \\wsl$-Zugriff funktioniert nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="02d0f-178">Fix issue with ARM64 \\wsl$ access not working properly</span></span>
* <span data-ttu-id="02d0f-179">Hinzufügen eines besseren Standardsymbols für „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="02d0f-179">Add better default icon for wsl.exe</span></span>

## <a name="build-18342"></a><span data-ttu-id="02d0f-180">Build 18342</span><span class="sxs-lookup"><span data-stu-id="02d0f-180">Build 18342</span></span>
<span data-ttu-id="02d0f-181">Allgemeine Windows-Informationen zu Build 18342 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-181">For general Windows information on build 18342 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-182">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-182">WSL</span></span>
* <span data-ttu-id="02d0f-183">Wir haben für Benutzer die Möglichkeit hinzugefügt, auf Linux-Dateien in einer WSL-Distribution aus Windows zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-183">We've added the ability for users to access Linux files in a WSL distro from Windows.</span></span> <span data-ttu-id="02d0f-184">Auf diese Dateien kann über die Befehlszeile zugegriffen werden. Außerdem können Windows-Apps wie der Datei-Explorer, VSCode usw. mit diesen Dateien interagieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-184">These files can be accessed through the command line, and also Windows apps, like file explorer, VSCode, etc. can interact with these files.</span></span> <span data-ttu-id="02d0f-185">Greifen Sie auf Ihre Dateien zu, indem Sie zu \\\\wsl$\\<distributions_name> navigieren, oder zeigen Sie eine Liste der ausgeführten Distributionen an, indem Sie zu \\\\wsl$ navigieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-185">Access your files by navigating to \\\\wsl$\\<distro_name>, or see a list of running distributions by navigating to \\\\wsl$</span></span>
* <span data-ttu-id="02d0f-186">Hinzufügen zusätzlicher CPU-Infotags und Korrigieren der Cpus_allowed[_list]-Werte [GH 2234]</span><span class="sxs-lookup"><span data-stu-id="02d0f-186">Add additional CPU info tags and fix Cpus_allowed[_list] values [GH 2234]</span></span>
* <span data-ttu-id="02d0f-187">Unterstützung der Ausführung aus Nicht-Leaderthread [GH 3800]</span><span class="sxs-lookup"><span data-stu-id="02d0f-187">Support exec from non-leader thread [GH 3800]</span></span>
* <span data-ttu-id="02d0f-188">Behandeln von Konfigurationsupdatefehlern als nicht schwerwiegend [GH 3785]</span><span class="sxs-lookup"><span data-stu-id="02d0f-188">Treat configuration update failures as non-fatal [GH 3785]</span></span>
* <span data-ttu-id="02d0f-189">Aktualisieren von binfmt für die ordnungsgemäße Verarbeitung von Offsets [GH 3768]</span><span class="sxs-lookup"><span data-stu-id="02d0f-189">Update binfmt to properly handle offsets [GH 3768]</span></span>
* <span data-ttu-id="02d0f-190">Aktivieren der Zuordnung von Netzlaufwerken für Plan 9 [GH 3854]</span><span class="sxs-lookup"><span data-stu-id="02d0f-190">Enable mapping network drives for Plan 9 [GH 3854]</span></span>
* <span data-ttu-id="02d0f-191">Unterstützung von Windows -> Linux und Linux -> Windows-Pfadübersetzung für Bindungseinbindungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-191">Support Windows -> Linux and Linux -> Windows path translation for bind mounts</span></span>
* <span data-ttu-id="02d0f-192">Erstellen schreibgeschützter Abschnitte für Zuordnungen für Dateien, die schreibgeschützt geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="02d0f-192">Create read-only sections for mappings on files opened read-only</span></span>

## <a name="build-18334"></a><span data-ttu-id="02d0f-193">Build 18334</span><span class="sxs-lookup"><span data-stu-id="02d0f-193">Build 18334</span></span>
<span data-ttu-id="02d0f-194">Allgemeine Windows-Informationen zu Build 18334 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-194">For general Windows information on build 18334 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-195">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-195">WSL</span></span>
* <span data-ttu-id="02d0f-196">Umgestalten der Art und Weise, in der die Windows-Zeitzone einer Linux-Zeitzone zugeordnet wird [GH 3747]</span><span class="sxs-lookup"><span data-stu-id="02d0f-196">Redesign the way that Windows time zone is mapped to a  Linux time zone [GH 3747]</span></span>
* <span data-ttu-id="02d0f-197">Beheben von Speicherverlusten und Hinzufügen neuer Zeichenfolgenübersetzungsfunktionen [GH 3746]</span><span class="sxs-lookup"><span data-stu-id="02d0f-197">Fix memory leaks and add new string translation functions [GH 3746]</span></span>
* <span data-ttu-id="02d0f-198">SIGCONT für eine Threadgruppe ohne Threads ist eine Nulloperation [GH 3741]</span><span class="sxs-lookup"><span data-stu-id="02d0f-198">SIGCONT on a threadgroup with no threads is a no-op [GH 3741]</span></span> 
* <span data-ttu-id="02d0f-199">Richtige Anzeige von Socket- und Epoll-Dateideskriptoren in „/proc/self/fd“</span><span class="sxs-lookup"><span data-stu-id="02d0f-199">Correctly display socket and epoll file descriptors in /proc/self/fd</span></span>

## <a name="build-18305"></a><span data-ttu-id="02d0f-200">Build 18305</span><span class="sxs-lookup"><span data-stu-id="02d0f-200">Build 18305</span></span>
<span data-ttu-id="02d0f-201">Allgemeine Windows-Informationen zu Build 18305 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-201">For general Windows information on build 18305 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-202">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-202">WSL</span></span>
* <span data-ttu-id="02d0f-203">pthreads verlieren den Zugriff auf Dateien, wenn der primäre Thread beendet wird [GH 3589]</span><span class="sxs-lookup"><span data-stu-id="02d0f-203">pthreads lose access to files when the primary thread exits [GH 3589]</span></span>
* <span data-ttu-id="02d0f-204">TIOCSCTTY sollte den Parameter „force“ ignorieren, wenn er nicht erforderlich ist [GH 3652]</span><span class="sxs-lookup"><span data-stu-id="02d0f-204">TIOCSCTTY should ignore the “force” parameter unless it is required [GH 3652]</span></span>
* <span data-ttu-id="02d0f-205">Verbesserungen an der Befehlszeile von „wsl.exe“ und Hinzufügung von Import-/Exportfunktionen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-205">wsl.exe command line improvements and addition of import / export functionality.</span></span>
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

## <a name="build-18277"></a><span data-ttu-id="02d0f-206">Build 18277</span><span class="sxs-lookup"><span data-stu-id="02d0f-206">Build 18277</span></span>
<span data-ttu-id="02d0f-207">Allgemeine Windows-Informationen zu Build 18277 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-207">For general Windows information on build 18277 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-208">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-208">WSL</span></span>
* <span data-ttu-id="02d0f-209">Korrektur des Fehlers „no such interface supported“ in Build 18272 [GH 3645]</span><span class="sxs-lookup"><span data-stu-id="02d0f-209">Fix "no such interface supported" error introduced in build 18272 [GH 3645]</span></span>
* <span data-ttu-id="02d0f-210">Ignorieren des MNT_FORCE-Flags für Systemaufruf zum Aufheben der Einbindung [GH 3605]</span><span class="sxs-lookup"><span data-stu-id="02d0f-210">Ignore the MNT_FORCE flag for umount syscall [GH 3605]</span></span>
* <span data-ttu-id="02d0f-211">Umschalten von WSL-Interop für die Verwendung der offiziellen CreatePseudoConsole-API</span><span class="sxs-lookup"><span data-stu-id="02d0f-211">Switch WSL interop to use the official CreatePseudoConsole API</span></span>
* <span data-ttu-id="02d0f-212">Keinen Timeoutwert beibehalten, wenn FUTEX_WAIT neu gestartet wird</span><span class="sxs-lookup"><span data-stu-id="02d0f-212">Maintain no timeout value when FUTEX_WAIT restarts</span></span>

## <a name="build-18272"></a><span data-ttu-id="02d0f-213">Build 18272</span><span class="sxs-lookup"><span data-stu-id="02d0f-213">Build 18272</span></span>
<span data-ttu-id="02d0f-214">Allgemeine Windows-Informationen zu Build 18272 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-214">For general Windows information on build 18272 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-215">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-215">WSL</span></span>
* <span data-ttu-id="02d0f-216">**WARNUNG:** In diesem Build liegt ein Problem vor, durch das WSL nicht funktionsfähig wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-216">**WARNING:** There is an issue in this build that makes WSL inoperable.</span></span> <span data-ttu-id="02d0f-217">Wenn Sie versuchen, die Distribution zu starten, wird der Fehler „No such interface supported“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-217">When trying to launch your distribution you will see a “No such interface supported” error.</span></span> <span data-ttu-id="02d0f-218">Das Problem wurde behoben und ist im Insider Fast-Build der nächsten Woche nicht mehr enthalten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-218">The issue has been fixed and will be in next week's Insider Fast build.</span></span> <span data-ttu-id="02d0f-219">Wenn Sie diesen Build installiert haben, können Sie ein Rollback auf den vorherigen Windows-Build durchführen, indem Sie unter „Einstellungen > Update und Sicherheit > Wiederherstellung“ die Option „Zur vorherigen Version von Windows 10 zurückkehren“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-219">If you've installed this build you can roll back to the previous Windows build using “Go back to the previous version of Windows 10” in Settings->Update & Security->Recovery.</span></span>

## <a name="build-18267"></a><span data-ttu-id="02d0f-220">Build 18267</span><span class="sxs-lookup"><span data-stu-id="02d0f-220">Build 18267</span></span>
<span data-ttu-id="02d0f-221">Allgemeine Windows-Informationen zu Build 18267 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-221">For general Windows information on build 18267 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-222">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-222">WSL</span></span>
* <span data-ttu-id="02d0f-223">Korrektur eines Problems, bei dem der Zombieprozess möglicherweise nicht beendet und unbegrenzt ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-223">Fix issue where zombie process may not be reaped and remain indefinitely.</span></span>
* <span data-ttu-id="02d0f-224">WslRegisterDistribution hängt, wenn die Fehlermeldung die maximale Länge überschreitet [GH 3592]</span><span class="sxs-lookup"><span data-stu-id="02d0f-224">WslRegisterDistribution hangs if error message exceeds max length [GH 3592]</span></span>
* <span data-ttu-id="02d0f-225">Zulassen der erfolgreichen Ausführung von fsync für schreibgeschützte Dateien auf DrvFs [GH 3556]</span><span class="sxs-lookup"><span data-stu-id="02d0f-225">Allow fsync to succeed for read-only files on DrvFs [GH 3556]</span></span>
* <span data-ttu-id="02d0f-226">Sicherstellen, dass die Verzeichnisse „/bin“ und „/sbin“ vorhanden sind, bevor symbolische Verknüpfungen darin erstellt werden [GH 3584]</span><span class="sxs-lookup"><span data-stu-id="02d0f-226">Ensure that /bin and /sbin directories exist before creating symlinks inside [GH 3584]</span></span>
* <span data-ttu-id="02d0f-227">Hinzufügen eines Instanztimeoutmechanismus für WSL-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-227">Added an instance termination timeout mechanism for WSL instances.</span></span> <span data-ttu-id="02d0f-228">Der Timeoutwert ist derzeit auf 15 Sekunden festgelegt. Das bedeutet, dass die Instanz 15 Sekunden nach Beendigung des letzten WSL-Prozesses beendet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-228">The timeout is currently set to 15 seconds, meaning the instance will terminate 15 seconds after the last WSL process exits.</span></span> <span data-ttu-id="02d0f-229">Um eine Distribution sofort zu beenden, verwenden Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="02d0f-229">To terminate a distribution immediately, use:</span></span>
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a><span data-ttu-id="02d0f-230">Build 17763 (1809)</span><span class="sxs-lookup"><span data-stu-id="02d0f-230">Build 17763 (1809)</span></span>
<span data-ttu-id="02d0f-231">Allgemeine Windows-Informationen zu Build 17763 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-231">For general Windows information on build 17763 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-232">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-232">WSL</span></span>
* <span data-ttu-id="02d0f-233">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="02d0f-233">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="02d0f-234">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="02d0f-234">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="02d0f-235">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="02d0f-235">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="02d0f-236">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="02d0f-236">Better handling of threadgroup leader file descriptor cleanup.</span></span>
* <span data-ttu-id="02d0f-237">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="02d0f-237">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="02d0f-238">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="02d0f-238">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="02d0f-239">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="02d0f-239">Fix several AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="02d0f-240">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="02d0f-240">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>
* <span data-ttu-id="02d0f-241">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="02d0f-241">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="02d0f-242">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="02d0f-242">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="02d0f-243">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-243">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="02d0f-244">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="02d0f-244">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="02d0f-245">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="02d0f-245">Pipe filesystem inadvertently clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="02d0f-246">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="02d0f-246">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>
* <span data-ttu-id="02d0f-247">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="02d0f-247">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="02d0f-248">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="02d0f-248">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="02d0f-249">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="02d0f-249">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="02d0f-250">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="02d0f-250">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="02d0f-251">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="02d0f-251">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="02d0f-252">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="02d0f-252">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="02d0f-253">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="02d0f-253">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="02d0f-254">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="02d0f-254">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="02d0f-255">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-255">Windows UI apps should execute even when launched in the background.</span></span>
* <span data-ttu-id="02d0f-256">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="02d0f-256">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="02d0f-257">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="02d0f-257">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="02d0f-258">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="02d0f-258">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="02d0f-259">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="02d0f-259">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="02d0f-260">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="02d0f-260">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="02d0f-261">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-261">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="02d0f-262">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="02d0f-262">Add wslconfig /terminate to stop running distributions.</span></span>
* <span data-ttu-id="02d0f-263">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="02d0f-263">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="02d0f-264">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="02d0f-264">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="02d0f-265">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-265">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="02d0f-266">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="02d0f-266">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="02d0f-267">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-267">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>
* <span data-ttu-id="02d0f-268">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="02d0f-268">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="02d0f-269">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="02d0f-269">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="02d0f-270">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-270">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="02d0f-271">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="02d0f-271">Atomically create case sensitive directories in DrvFs.</span></span>
* <span data-ttu-id="02d0f-272">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-272">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="02d0f-273">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="02d0f-273">[GH 2712]</span></span>
* <span data-ttu-id="02d0f-274">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="02d0f-274">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="02d0f-275">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="02d0f-275">[GH 3020]</span></span>
* <span data-ttu-id="02d0f-276">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="02d0f-276">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="02d0f-277">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-277">To use, hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="02d0f-278">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="02d0f-278">Fix Unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="02d0f-279">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-279">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="02d0f-280">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="02d0f-280">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="02d0f-281">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="02d0f-281">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="02d0f-282">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="02d0f-282">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="02d0f-283">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-283">Add --distribution option for wsl.exe to select a specific distro.</span></span>
* <span data-ttu-id="02d0f-284">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="02d0f-284">Limited support for dmesg.</span></span> <span data-ttu-id="02d0f-285">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-285">Applications can now log to dmesg.</span></span> <span data-ttu-id="02d0f-286">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="02d0f-286">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="02d0f-287">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-287">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="02d0f-288">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-288">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="02d0f-289">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-289">`syslog` syscall interface is not yet supported.</span></span> <span data-ttu-id="02d0f-290">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-290">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="02d0f-291">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="02d0f-291">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="02d0f-292">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="02d0f-292">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="02d0f-293">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="02d0f-293">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="02d0f-294">Einige Zeichen (etwa „/“, „:“ und „\*“) sind unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-294">Some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-18252-skip-ahead"></a><span data-ttu-id="02d0f-295">Build 18252 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-295">Build 18252 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-296">Allgemeine Windows-Informationen zu Build 18252 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-296">For general Windows information on build 18252 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-297">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-297">WSL</span></span>
* <span data-ttu-id="02d0f-298">Verschieben von init- und bsdtar-Binärdateien aus der lxssmanager-DLL in einen separaten Toolsordner</span><span class="sxs-lookup"><span data-stu-id="02d0f-298">Move init and bsdtar binaries out of lxssmanager dll and into a separate tools folder</span></span>
* <span data-ttu-id="02d0f-299">Korrektur von Racebedingung um schließenden Dateideskriptor bei Verwendung von CLONE_FILES</span><span class="sxs-lookup"><span data-stu-id="02d0f-299">Fix race around closing file descriptor when using CLONE_FILES</span></span>
* <span data-ttu-id="02d0f-300">Verarbeiten optionaler Felder in „/proc/pid/mountinfo“ bei der Übersetzung von DrvFs-Pfaden</span><span class="sxs-lookup"><span data-stu-id="02d0f-300">Handle optional fields in /proc/pid/mountinfo when translating DrvFs paths</span></span>
* <span data-ttu-id="02d0f-301">Zulassen, dass DrvFs mklod ohne Metadatenunterstützung für S_IFREG erfolgreich ist</span><span class="sxs-lookup"><span data-stu-id="02d0f-301">Allow DrvFs mknod to succeed without metadata support for S_IFREG</span></span>
* <span data-ttu-id="02d0f-302">Für schreibgeschützte Dateien, die auf DrvFs erstellt wurden, muss das schreibgeschützte Attribut festgelegt werden [GH 3411]</span><span class="sxs-lookup"><span data-stu-id="02d0f-302">Readonly files created on DrvFs should have the readonly attribute set [GH 3411]</span></span>
* <span data-ttu-id="02d0f-303">Hinzufügen von /sbin/mount.drvfs-Hilfsprogramm zur Verarbeitung der DrvFs-Einbindung</span><span class="sxs-lookup"><span data-stu-id="02d0f-303">Add /sbin/mount.drvfs helper to handle DrvFs mounting</span></span>
* <span data-ttu-id="02d0f-304">Verwenden der POSIX-Umbenennung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="02d0f-304">Use POSIX rename in DrvFs.</span></span>
* <span data-ttu-id="02d0f-305">Ermöglichen der Pfadübersetzung für Volumes ohne Volume-GUID.</span><span class="sxs-lookup"><span data-stu-id="02d0f-305">Allow path translation on volumes without a volume GUID.</span></span>

## <a name="build-17738-fast"></a><span data-ttu-id="02d0f-306">Build 17738 (Fast)</span><span class="sxs-lookup"><span data-stu-id="02d0f-306">Build 17738 (Fast)</span></span>
<span data-ttu-id="02d0f-307">Allgemeine Windows-Informationen zu Build 17738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-307">For general Windows information on build 17738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-308">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-308">WSL</span></span>
* <span data-ttu-id="02d0f-309">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="02d0f-309">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="02d0f-310">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="02d0f-310">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="02d0f-311">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="02d0f-311">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="02d0f-312">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="02d0f-312">Better handling of threadgroup leader file descriptor cleanup.</span></span>

## <a name="build-17728-fast"></a><span data-ttu-id="02d0f-313">Build 17728 (Fast)</span><span class="sxs-lookup"><span data-stu-id="02d0f-313">Build 17728 (Fast)</span></span>
<span data-ttu-id="02d0f-314">Allgemeine Windows-Informationen zu Build 17728 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-314">For general Windows information on build 17728 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-315">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-315">WSL</span></span>
* <span data-ttu-id="02d0f-316">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="02d0f-316">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="02d0f-317">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="02d0f-317">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="02d0f-318">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="02d0f-318">Fix a number of AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="02d0f-319">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="02d0f-319">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>

## <a name="build-18204-skip-ahead"></a><span data-ttu-id="02d0f-320">Build 18204 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-320">Build 18204 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-321">Allgemeine Windows-Informationen zu Build 18204 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-321">For general Windows information on build 18204 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-322">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-322">WSL</span></span>
* <span data-ttu-id="02d0f-323">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="02d0f-323">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="02d0f-324">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="02d0f-324">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17723-fast"></a><span data-ttu-id="02d0f-325">Build 17723 (Fast)</span><span class="sxs-lookup"><span data-stu-id="02d0f-325">Build 17723 (Fast)</span></span>
<span data-ttu-id="02d0f-326">Allgemeine Windows-Informationen zu Build 17723 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-326">For general Windows information on build 17723 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-327">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-327">WSL</span></span>
* <span data-ttu-id="02d0f-328">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="02d0f-328">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="02d0f-329">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="02d0f-329">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="02d0f-330">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-330">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="02d0f-331">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="02d0f-331">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="02d0f-332">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="02d0f-332">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="02d0f-333">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="02d0f-333">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17713"></a><span data-ttu-id="02d0f-334">Build 17713</span><span class="sxs-lookup"><span data-stu-id="02d0f-334">Build 17713</span></span>
<span data-ttu-id="02d0f-335">Allgemeine Windows-Informationen zu Build 17713 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-335">For general Windows information on build 17713 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-336">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-336">WSL</span></span>
* <span data-ttu-id="02d0f-337">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="02d0f-337">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="02d0f-338">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="02d0f-338">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="02d0f-339">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="02d0f-339">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="02d0f-340">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="02d0f-340">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="02d0f-341">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="02d0f-341">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="02d0f-342">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="02d0f-342">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="02d0f-343">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="02d0f-343">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="02d0f-344">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="02d0f-344">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="02d0f-345">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-345">Windows UI apps should execute even when launched in the background.</span></span>

## <a name="build-17704"></a><span data-ttu-id="02d0f-346">Build 17704</span><span class="sxs-lookup"><span data-stu-id="02d0f-346">Build 17704</span></span>
<span data-ttu-id="02d0f-347">Allgemeine Windows-Informationen zu Build 17704 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-347">For general Windows information on build 17704 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-348">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-348">WSL</span></span>
* <span data-ttu-id="02d0f-349">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="02d0f-349">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="02d0f-350">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="02d0f-350">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="02d0f-351">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="02d0f-351">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="02d0f-352">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="02d0f-352">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="02d0f-353">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="02d0f-353">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="02d0f-354">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-354">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="02d0f-355">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="02d0f-355">Add wslconfig /terminate to stop running distributions.</span></span>

## <a name="build-17692"></a><span data-ttu-id="02d0f-356">Build 17692</span><span class="sxs-lookup"><span data-stu-id="02d0f-356">Build 17692</span></span>
<span data-ttu-id="02d0f-357">Allgemeine Windows-Informationen zu Build 17692 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span><span class="sxs-lookup"><span data-stu-id="02d0f-357">For general Windows information on build 17692 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-358">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-358">WSL</span></span>
* <span data-ttu-id="02d0f-359">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="02d0f-359">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="02d0f-360">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="02d0f-360">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="02d0f-361">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-361">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="02d0f-362">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="02d0f-362">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="02d0f-363">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-363">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>

## <a name="build-17686"></a><span data-ttu-id="02d0f-364">Build 17686</span><span class="sxs-lookup"><span data-stu-id="02d0f-364">Build 17686</span></span>
<span data-ttu-id="02d0f-365">Allgemeine Windows-Informationen zu Build 17686 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span><span class="sxs-lookup"><span data-stu-id="02d0f-365">For general Windows information on build 17686 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-366">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-366">WSL</span></span>
* <span data-ttu-id="02d0f-367">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="02d0f-367">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="02d0f-368">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="02d0f-368">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="02d0f-369">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-369">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="02d0f-370">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="02d0f-370">Atomically create case sensitive directories in DrvFs.</span></span>

## <a name="build-17677"></a><span data-ttu-id="02d0f-371">Build 17677</span><span class="sxs-lookup"><span data-stu-id="02d0f-371">Build 17677</span></span>
<span data-ttu-id="02d0f-372">Allgemeine Windows-Informationen zu Build 17677 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-372">For general Windows information on build 17677 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-373">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-373">WSL</span></span>
* <span data-ttu-id="02d0f-374">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-374">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="02d0f-375">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="02d0f-375">[GH 2712]</span></span>
* <span data-ttu-id="02d0f-376">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="02d0f-376">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="02d0f-377">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="02d0f-377">[GH 3020]</span></span>

## <a name="build-17666"></a><span data-ttu-id="02d0f-378">Build 17666</span><span class="sxs-lookup"><span data-stu-id="02d0f-378">Build 17666</span></span>
<span data-ttu-id="02d0f-379">Allgemeine Windows-Informationen zu Build 17666 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-379">For general Windows information on build 17666 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-380">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-380">WSL</span></span>
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a><span data-ttu-id="02d0f-381">WARNUNG: Es gibt ein Problem, das das Ausführen von WSL in einigen AMD-Chipsätzen verhindert [GH 3134].</span><span class="sxs-lookup"><span data-stu-id="02d0f-381">WARNING: There is an issue preventing WSL from running on some AMD chipsets [GH 3134].</span></span> <span data-ttu-id="02d0f-382">Eine Korrektur ist verfügbar und wird in den Insider Build-Branch integriert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-382">A fix is ready and making its way to the Insider Build branch.</span></span>
* <span data-ttu-id="02d0f-383">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="02d0f-383">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="02d0f-384">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-384">To use hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="02d0f-385">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="02d0f-385">Fix unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="02d0f-386">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-386">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="02d0f-387">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="02d0f-387">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="02d0f-388">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="02d0f-388">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="02d0f-389">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="02d0f-389">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="02d0f-390">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-390">Add --distribution option for wsl.exe to select a specific distro.</span></span>

## <a name="build-17655-skip-ahead"></a><span data-ttu-id="02d0f-391">Build 17655 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-391">Build 17655 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-392">Allgemeine Windows-Informationen zu Build 17655 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-392">For general Windows information on build 17655 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-393">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-393">WSL</span></span>
* <span data-ttu-id="02d0f-394">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="02d0f-394">Limited support for dmesg.</span></span> <span data-ttu-id="02d0f-395">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-395">Applications can now log to dmesg.</span></span> <span data-ttu-id="02d0f-396">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="02d0f-396">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="02d0f-397">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-397">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="02d0f-398">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-398">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="02d0f-399">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-399">`syslog` sycall interface is not yet supported.</span></span> <span data-ttu-id="02d0f-400">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-400">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="02d0f-401">Korrektur eines Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-401">Fixed an issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="02d0f-402">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="02d0f-402">[GH 2712]</span></span>

## <a name="build-17639-skip-ahead"></a><span data-ttu-id="02d0f-403">Build 17639 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-403">Build 17639 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-404">Allgemeine Windows-Informationen zu Build 17639 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-404">For general Windows information on build 17639 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-405">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-405">WSL</span></span>
* <span data-ttu-id="02d0f-406">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="02d0f-406">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="02d0f-407">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="02d0f-407">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="02d0f-408">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="02d0f-408">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="02d0f-409">Insbesondere sind einige Zeichen (etwa „/“, „:“ und „\*“) unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-409">In particular, some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-17133-fast"></a><span data-ttu-id="02d0f-410">Build 17133 (Fast)</span><span class="sxs-lookup"><span data-stu-id="02d0f-410">Build 17133 (Fast)</span></span>
<span data-ttu-id="02d0f-411">Allgemeine Windows-Informationen zu Build 17133 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-411">For general Windows information on build 17133 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-412">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-412">WSL</span></span>
* <span data-ttu-id="02d0f-413">Fehlerbehebung für Hängen in WSL.</span><span class="sxs-lookup"><span data-stu-id="02d0f-413">Fix for hang in WSL.</span></span> <span data-ttu-id="02d0f-414">[GH 3039, 3034]</span><span class="sxs-lookup"><span data-stu-id="02d0f-414">[GH 3039, 3034]</span></span>

## <a name="build-17128-fast"></a><span data-ttu-id="02d0f-415">Build 17128 (Fast)</span><span class="sxs-lookup"><span data-stu-id="02d0f-415">Build 17128 (Fast)</span></span>
<span data-ttu-id="02d0f-416">Allgemeine Windows-Informationen zu Build 17128 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-416">For general Windows information on build 17128 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-417">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-417">WSL</span></span>
* <span data-ttu-id="02d0f-418">Keine</span><span class="sxs-lookup"><span data-stu-id="02d0f-418">None</span></span>

## <a name="build-17627-skip-ahead"></a><span data-ttu-id="02d0f-419">Build 17627 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-419">Build 17627 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-420">Allgemeine Windows-Informationen zu Build 17627 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-420">For general Windows information on build 17627 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-421">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-421">WSL</span></span>
* <span data-ttu-id="02d0f-422">Hinzufügen von Unterstützung für futex-pi-fähige Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="02d0f-422">Add support for the futex pi-aware operations.</span></span> <span data-ttu-id="02d0f-423">[GH 1006]</span><span class="sxs-lookup"><span data-stu-id="02d0f-423">[GH 1006]</span></span>
    * <span data-ttu-id="02d0f-424">Beachten Sie, dass Prioritäten derzeit keine unterstützte WSL-Funktion sind, sodass Einschränkungen bestehen. Die Standardverwenund sollte jedoch aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-424">Note that priorities are not currently a supported WSL feature so there are limitations, but standard usage should be unblocked.</span></span>
* <span data-ttu-id="02d0f-425">Windows-Firewallunterstützung für WSL-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="02d0f-425">Windows firewall support for WSL processes.</span></span> <span data-ttu-id="02d0f-426">[GH 1852]</span><span class="sxs-lookup"><span data-stu-id="02d0f-426">[GH 1852]</span></span>
    * <span data-ttu-id="02d0f-427">Um beispielsweise zuzulassen, dass der WSL python-Prozess an einem beliebigen Port lauschen kann, verwenden Sie Windows-CMD mit erhöhten Rechten: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span><span class="sxs-lookup"><span data-stu-id="02d0f-427">For example, to allow the WSL python process to listen on any port, use the elevated Windows cmd: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span></span>
    * <span data-ttu-id="02d0f-428">Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link.](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span><span class="sxs-lookup"><span data-stu-id="02d0f-428">For additional details on how to add firewall rules, see [link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span></span>
* <span data-ttu-id="02d0f-429">Beachten der Standardshell des Benutzers bei der Verwendung von „wsl.exe“.</span><span class="sxs-lookup"><span data-stu-id="02d0f-429">Respect user's default shell when using wsl.exe.</span></span> <span data-ttu-id="02d0f-430">[GH 2372]</span><span class="sxs-lookup"><span data-stu-id="02d0f-430">[GH 2372]</span></span>
* <span data-ttu-id="02d0f-431">Melden aller Netzwerkschnittstellen als Ethernet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-431">Report all network interfaces as ethernet.</span></span> <span data-ttu-id="02d0f-432">[GH 2996]</span><span class="sxs-lookup"><span data-stu-id="02d0f-432">[GH 2996]</span></span>
* <span data-ttu-id="02d0f-433">Bessere Verarbeitung von beschädigten /etc/passwd-Dateien.</span><span class="sxs-lookup"><span data-stu-id="02d0f-433">Better handling of corrupt /etc/passwd file.</span></span> <span data-ttu-id="02d0f-434">[GH 3001]</span><span class="sxs-lookup"><span data-stu-id="02d0f-434">[GH 3001]</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-435">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-435">Console</span></span>
* <span data-ttu-id="02d0f-436">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-436">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-437">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-437">LTP Results:</span></span>
<span data-ttu-id="02d0f-438">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-438">Testing in progress.</span></span>

## <a name="build-17618-skip-ahead"></a><span data-ttu-id="02d0f-439">Build 17618 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="02d0f-439">Build 17618 (Skip Ahead)</span></span>
<span data-ttu-id="02d0f-440">Allgemeine Windows-Informationen zu Build 17618 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-440">For general Windows information on build 17618 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-441">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-441">WSL</span></span>
* <span data-ttu-id="02d0f-442">Einführung in Pseudoconsolenfunktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span><span class="sxs-lookup"><span data-stu-id="02d0f-442">Introduce pseudoconsole functionality for NT interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span></span>
* <span data-ttu-id="02d0f-443">Der Legacyinstallationsmechanismus („lxrun.exe“) ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-443">The legacy install mechanism (lxrun.exe) has been deprecated.</span></span> <span data-ttu-id="02d0f-444">Der unterstützte Mechanismus zum Installieren von Distributionen ist der Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="02d0f-444">The supported mechanism for installing distributions is through the Microsoft Store.</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-445">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-445">Console</span></span>
* <span data-ttu-id="02d0f-446">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-446">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-447">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-447">LTP Results:</span></span>
<span data-ttu-id="02d0f-448">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-448">Testing in progress.</span></span>

## <a name="build-17110"></a><span data-ttu-id="02d0f-449">Build 17110</span><span class="sxs-lookup"><span data-stu-id="02d0f-449">Build 17110</span></span>
<span data-ttu-id="02d0f-450">Allgemeine Windows-Informationen zu Build 17110 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-450">For general Windows information on build 17110 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-451">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-451">WSL</span></span>
* <span data-ttu-id="02d0f-452">Zulassen, dass /init aus Windows beendet wird [GH 2928].</span><span class="sxs-lookup"><span data-stu-id="02d0f-452">Allow /init to be terminated from Windows [GH 2928].</span></span>
* <span data-ttu-id="02d0f-453">DrvFs verwendet nun standardmäßig Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis (entspricht der Einbindungsoption „case=dir“).</span><span class="sxs-lookup"><span data-stu-id="02d0f-453">DrvFs now uses per-directory case sensitivity by default (equivalent to the “case=dir” mount option).</span></span>
    * <span data-ttu-id="02d0f-454">Wenn Sie „case=force“ verwenden (das alte Verhalten), muss ein Registrierungsschlüssel festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-454">Using “case=force” (the old behavior) requires setting a registry key.</span></span> <span data-ttu-id="02d0f-455">Führen Sie den folgenden Befehl aus, um „case=force“ zu aktivieren, wenn Sie diese Option verwenden müssen: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span><span class="sxs-lookup"><span data-stu-id="02d0f-455">Run the following command to enable “case=force” if you need to use it: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span></span>
    * <span data-ttu-id="02d0f-456">Wenn Sie über vorhandene Verzeichnisse verfügen, die mit WSL in einer älteren Version von Windows erstellt wurden, bei denen die Groß-/Kleinschreibung beachtet werden muss, verwenden Sie „fsutil.exe“, um sie für Unterscheidung von Groß-/Kleinschreibung zu markieren: fsutil.exe file setcasesensitiveinfo <path> enable</span><span class="sxs-lookup"><span data-stu-id="02d0f-456">If you have existing directories created with WSL in older version of Windows which need to be case sensitive, use fsutil.exe to mark them as case sensitive: fsutil.exe file setcasesensitiveinfo <path> enable</span></span>
* <span data-ttu-id="02d0f-457">NULL-Beendigungszeichenfolgen werden vom uname-Systemaufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-457">NULL terminate strings returned from the uname syscall.</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-458">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-458">Console</span></span>
* <span data-ttu-id="02d0f-459">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-459">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-460">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-460">LTP Results:</span></span>
<span data-ttu-id="02d0f-461">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-461">Testing in progress.</span></span>

## <a name="build-17107"></a><span data-ttu-id="02d0f-462">Build 17107</span><span class="sxs-lookup"><span data-stu-id="02d0f-462">Build 17107</span></span>
<span data-ttu-id="02d0f-463">Allgemeine Windows-Informationen zu Build 17107 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-463">For general Windows information on build 17107 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-464">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-464">WSL</span></span>
* <span data-ttu-id="02d0f-465">Unterstützung von TCSETSF und TCSETSW für pty-Masterendpunkte [GH 2552].</span><span class="sxs-lookup"><span data-stu-id="02d0f-465">Support TCSETSF and TCSETSW on master pty endpoints [GH 2552].</span></span>
* <span data-ttu-id="02d0f-466">Starten von gleichzeitigen Interop-Prozessen kann zu EINVAL führen [GH 2813].</span><span class="sxs-lookup"><span data-stu-id="02d0f-466">Starting simultaneous interop processes can result in EINVAL [GH 2813].</span></span>
* <span data-ttu-id="02d0f-467">Korrektur von PTRACE_ATTACH, um den richtigen Ablaufverfolgungsstatus in „/proc/pid/status“ anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-467">Fix PTRACE_ATTACH to show proper tracing status in /proc/pid/status.</span></span>
* <span data-ttu-id="02d0f-468">Korrektur der Racebedingung, bei der kurzlebige Prozesse, die mit den CLEARTID- und SETTID-Flags geklont wurden, ohne Löschen der TID-Adresse beendet werden konnten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-468">Fix race where short-lived processes cloned with both the CLEARTID and SETTID flags could exit without clearing the TID address.</span></span>
* <span data-ttu-id="02d0f-469">Anzeigen einer Meldung beim Aktualisieren der Linux-Dateisystemverzeichnisse beim Umstieg von einem Build vor 17093.</span><span class="sxs-lookup"><span data-stu-id="02d0f-469">Display a message when upgrading the Linux file system directories when moving from a pre-17093 build.</span></span> <span data-ttu-id="02d0f-470">Weitere Informationen zu den Änderungen für das 17093-Dateisystem finden Sie in den Anmerkungen zur Version für [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span><span class="sxs-lookup"><span data-stu-id="02d0f-470">For more details on the 17093 file system changes, see the release notes for [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-471">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-471">Console</span></span>
* <span data-ttu-id="02d0f-472">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-472">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-473">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-473">LTP Results:</span></span>
<span data-ttu-id="02d0f-474">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-474">Testing in progress.</span></span>

## <a name="build-17101"></a><span data-ttu-id="02d0f-475">Build 17101</span><span class="sxs-lookup"><span data-stu-id="02d0f-475">Build 17101</span></span>
<span data-ttu-id="02d0f-476">Allgemeine Windows-Informationen zu Build 17101 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-476">For general Windows information on build 17101 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-477">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-477">WSL</span></span>
* <span data-ttu-id="02d0f-478">Unterstützung für signalfd.</span><span class="sxs-lookup"><span data-stu-id="02d0f-478">Support for signalfd.</span></span> <span data-ttu-id="02d0f-479">[GH 129]</span><span class="sxs-lookup"><span data-stu-id="02d0f-479">[GH 129]</span></span>
* <span data-ttu-id="02d0f-480">Unterstützung von Dateinamen, die ungültige NTFS-Zeichen enthalten, durch Codieren als private Unicode-Zeichen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-480">Support file-names containing illegal NTFS characters by encoding them as private Unicode characters.</span></span> <span data-ttu-id="02d0f-481">[GH 1514]</span><span class="sxs-lookup"><span data-stu-id="02d0f-481">[GH 1514]</span></span>
* <span data-ttu-id="02d0f-482">Automatisches Einbinden greift auf den schreibgeschützten Modus zurück, wenn Schreibvorgänge nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-482">Auto mount will fallback to read-only when write is not supported.</span></span> <span data-ttu-id="02d0f-483">[GH 2603]</span><span class="sxs-lookup"><span data-stu-id="02d0f-483">[GH 2603]</span></span>
* <span data-ttu-id="02d0f-484">Ermöglichen des Einfügens von Unicode-Ersatzzeichenpaaren (z.B. Emojis).</span><span class="sxs-lookup"><span data-stu-id="02d0f-484">Allow pasting of Unicode surrogate pairs (like emoji characters).</span></span> <span data-ttu-id="02d0f-485">[GH 2765]</span><span class="sxs-lookup"><span data-stu-id="02d0f-485">[GH 2765]</span></span>
* <span data-ttu-id="02d0f-486">Pseudodateien in „/proc“ und „/sys“ sollten „read“ und „write ready“ aus select, poll, epoll, usw. zurückgeben [GH 2838].</span><span class="sxs-lookup"><span data-stu-id="02d0f-486">Pseudo-files in /proc and /sys should return read and write ready from select, poll, epoll, et al. [GH 2838]</span></span>
* <span data-ttu-id="02d0f-487">Korrektur eines Problems, das dazu führen kann, dass der Dienst in eine Endlosschleife übergeht, wenn die Registrierung manipuliert wurde oder beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-487">Fix issue that could cause service to go into infinite loop when the registry has been tampered with or is corrupt.</span></span>
* <span data-ttu-id="02d0f-488">Korrektur von Netlink-Nachrichten, sodass sie mit neueren Versionen von iproute2 (upstream 4.14) funktionieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-488">Fix netlink messages to work with newer (upstream 4.14) version of iproute2.</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-489">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-489">Console</span></span>
* <span data-ttu-id="02d0f-490">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-490">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-491">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-491">LTP Results:</span></span>
<span data-ttu-id="02d0f-492">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-492">Testing in progress.</span></span>

## <a name="build-17093"></a><span data-ttu-id="02d0f-493">Build 17093</span><span class="sxs-lookup"><span data-stu-id="02d0f-493">Build 17093</span></span>
<span data-ttu-id="02d0f-494">Allgemeine Windows-Informationen zu Build 17093 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-494">For general Windows information on build 17093 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span></span>

#### <a name="important"></a><span data-ttu-id="02d0f-495">Wichtig:</span><span class="sxs-lookup"><span data-stu-id="02d0f-495">Important:</span></span>
<span data-ttu-id="02d0f-496">Wenn Sie WSL zum ersten Mal nach dem Upgrade auf diesen Build starten, müssen Sie einige Aufgaben durchführen, um die Linux-Dateisystemverzeichnisse zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-496">When starting WSL for the first time after upgrading to this build, it needs to perform some work upgrading the Linux file system directories.</span></span> <span data-ttu-id="02d0f-497">Dieser Vorgang kann einige Minuten in Anspruch nehmen, sodass WSL möglicherweise langsam zu starten scheint.</span><span class="sxs-lookup"><span data-stu-id="02d0f-497">This may take up to several minutes, so WSL may appear to start slowly.</span></span> <span data-ttu-id="02d0f-498">Dies sollte nur ein Mal für jede Distribution erfolgen, die Sie aus dem Store installiert haben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-498">This should only happen once for each distribution you have installed from the store.</span></span>
* <span data-ttu-id="02d0f-499">Verbesserte Unterscheidung von Groß-/Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="02d0f-499">Improved case sensitivity support in DrvFs.</span></span>
    * <span data-ttu-id="02d0f-500">DrvFs unterstützt jetzt Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="02d0f-500">DrvFs now supports per-directory case sensitivity.</span></span> <span data-ttu-id="02d0f-501">Dies ist ein neues Flag, das für Verzeichnisse festgelegt werden kann, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen mit Unterscheidung zwischen Groß-/Kleinschreibung behandelt werden sollen, sodass sogar Windows-Anwendungen Dateien ordnungsgemäß öffnen können, bei denen sich nur die Groß-/Kleinschreibung unterscheidet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-501">This is a new flag that can be set on directories to indicate all operations in those directories should be treated as case sensitive, which allows even Windows applications to correctly open files that differ only by case.</span></span>
    * <span data-ttu-id="02d0f-502">DrvFs verfügt über neue Einbindungsoptionen, die die Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis steuern.</span><span class="sxs-lookup"><span data-stu-id="02d0f-502">DrvFs has new mount options controlling case sensitivity on a per-directory basis</span></span>
        * <span data-ttu-id="02d0f-503">case=force: Für alle Verzeichnisse wird zwischen Groß-/Kleinschreibung unterschieden (mit Ausnahme des Laufwerkstamms).</span><span class="sxs-lookup"><span data-stu-id="02d0f-503">case=force: all directories are treated as case sensitive (except for the drive root).</span></span> <span data-ttu-id="02d0f-504">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-504">New directories created with WSL are marked as case sensitive.</span></span> <span data-ttu-id="02d0f-505">Dies ist das Legacyverhalten (ausgenommen, wenn neue Verzeichnisse für Unterscheidung zwischen Groß-/Kleinschreibung markiert werden).</span><span class="sxs-lookup"><span data-stu-id="02d0f-505">This is the legacy behavior except for marking new directories case sensitive.</span></span>
        * <span data-ttu-id="02d0f-506">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-506">case=dir: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="02d0f-507">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-507">New directories created with WSL are marked as case sensitive.</span></span>
        * <span data-ttu-id="02d0f-508">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-508">case=off: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="02d0f-509">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-509">New directories created with WSL are marked as case insensitive.</span></span>
    * <span data-ttu-id="02d0f-510">Hinweis: Für Verzeichnisse, die in früheren Versionen von WSL erstellt wurden, ist dieses Flag nicht festgelegt, sodass bei Verwendung der Option „case=dir“ keine Groß-/Kleinschreibung beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-510">Note: directories created by WSL in previous releases do not have this flag set, so will not be treated as case sensitive if you use the “case=dir” option.</span></span> <span data-ttu-id="02d0f-511">Eine Möglichkeit, dieses Flag für vorhandene Verzeichnisse festzulegen, ist in Kürze verfügbar.</span><span class="sxs-lookup"><span data-stu-id="02d0f-511">A way to set this flag on existing directories is coming soon.</span></span>
    * <span data-ttu-id="02d0f-512">Beispiel für die Einbindung mit diesen Optionen (für vorhandene Laufwerke müssen Sie zuerst die Einbindung aufheben, bevor Sie die Einbindung mit anderen Optionen ausführen können): sudo mount -t drvfs C: /mnt/c -o case=dir</span><span class="sxs-lookup"><span data-stu-id="02d0f-512">Example of mounting with these options (for existing drives, you must first unmount before you can mount with different options): sudo mount -t drvfs C: /mnt/c -o case=dir</span></span>
    * <span data-ttu-id="02d0f-513">Momentan ist case=force immer noch die Standardoption.</span><span class="sxs-lookup"><span data-stu-id="02d0f-513">For now, case=force is still the default option.</span></span> <span data-ttu-id="02d0f-514">Dies wird in Zukunft in case=dir geändert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-514">This will be changed to case=dir in the future.</span></span>
* <span data-ttu-id="02d0f-515">Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, wenn Sie DrvFs einbinden, z.B. sudo mount -t drvfs //server/share /mnt/share</span><span class="sxs-lookup"><span data-stu-id="02d0f-515">You can now use forward slashes in Windows paths when mounting DrvFs, e.g.: sudo mount -t drvfs //server/share /mnt/share</span></span>
* <span data-ttu-id="02d0f-516">WSL verarbeitet nun die /etc/fstab-Datei während des Instanzstarts [GH 2636].</span><span class="sxs-lookup"><span data-stu-id="02d0f-516">WSL now processes the /etc/fstab file during instance start [GH 2636].</span></span>
    * <span data-ttu-id="02d0f-517">Dies erfolgt vor der automatischen Einbindung von DrvFs-Laufwerken. Alle Laufwerke, die bereits von fstab eingebunden wurden, werden nicht automatisch erneut eingebunden, sodass Sie den Einbindungspunkt für bestimmte Laufwerke ändern können.</span><span class="sxs-lookup"><span data-stu-id="02d0f-517">This is done prior to automatically mounting DrvFs drives; any drives that were already mounted by fstab will not be remounted automatically, allowing you to change the mount point for specific drives.</span></span>
    * <span data-ttu-id="02d0f-518">Dieses Verhalten kann mithilfe von „wsl.conf“ deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-518">This behavior can be turned off using wsl.conf.</span></span>
* <span data-ttu-id="02d0f-519">Die mount, mountinfo- und mountstats-Dateien in „/proc“ versehen Sonderzeichen wie umgekehrte Schrägstriche und Leerzeichen ordnungsgemäß mit Escapezeichen [GH 2799]</span><span class="sxs-lookup"><span data-stu-id="02d0f-519">The mount, mountinfo and mountstats files in /proc properly escape special characters like backslashes and spaces [GH 2799]</span></span>
* <span data-ttu-id="02d0f-520">Spezielle Dateien, die mit DrvFs erstellt werden (z.B. symbolische WSL-Verknüpfungen oder Fifos und Sockets, wenn Metadaten aktiviert sind), können nun aus Windows kopiert und verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-520">Special files created with DrvFs such as WSL symbolic links, or fifos and sockets when metadata is enabled, can now be copied and moved from Windows.</span></span>

#### <a name="wsl-is-more-configurable-with-wslconf"></a><span data-ttu-id="02d0f-521">WSL ist mit „wsl.conf“ besser konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="02d0f-521">WSL is more configurable with wsl.conf</span></span>
<span data-ttu-id="02d0f-522">Es wurde eine Methode zum automatischen Konfigurieren bestimmter Funktionen in WSL hinzugefügt, die jedes Mal angewendet wird, wenn Sie das Subsystem starten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-522">We added a method for you to automatically configure certain functionality in WSL that will be applied every time you launch the subsystem.</span></span> <span data-ttu-id="02d0f-523">Dies umfasst Optionen für die automatische Einbindung und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="02d0f-523">This includes automount options and network configuration.</span></span> <span data-ttu-id="02d0f-524">Weitere Informationen hierzu finden Sie in unserem Blogbeitrag unter: https://aka.ms/wslconf</span><span class="sxs-lookup"><span data-stu-id="02d0f-524">Learn more about it in our blog post at: https://aka.ms/wslconf</span></span>

#### <a name="af_unix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a><span data-ttu-id="02d0f-525">AF_UNIX ermöglicht Socketverbindungen zwischen Linux-Prozessen für WSL- und native Windows-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="02d0f-525">AF_UNIX allows socket connections between Linux processes on WSL and Windows native processes</span></span>
<span data-ttu-id="02d0f-526">WSL- und Windows-Anwendungen können nun über Unix-Sockets miteinander kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-526">WSL and Windows applications can now communicate with each other over Unix sockets.</span></span> <span data-ttu-id="02d0f-527">Stellen Sie sich vor, Sie möchten einen Dienst in Windows ausführen und sowohl für Windows- als auch für WSL-Apps verfügbar machen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-527">Imagine you want to run a service in Windows and make it available to both Windows and WSL apps.</span></span> <span data-ttu-id="02d0f-528">Das ist nun mit UNIX-Sockets möglich.</span><span class="sxs-lookup"><span data-stu-id="02d0f-528">Now, that’s possible with Unix sockets.</span></span> <span data-ttu-id="02d0f-529">Weitere Informationen finden Sie in unserem Blogbeitrag unter https://aka.ms/afunixinterop.</span><span class="sxs-lookup"><span data-stu-id="02d0f-529">Read more in our blog post at https://aka.ms/afunixinterop</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-530">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-530">WSL</span></span>
* <span data-ttu-id="02d0f-531">Unterstützung von mmap() mit MAP_NORESERVE [GH 121, 2784]</span><span class="sxs-lookup"><span data-stu-id="02d0f-531">Support mmap() with MAP_NORESERVE [GH 121, 2784]</span></span>
* <span data-ttu-id="02d0f-532">Unterstützung von CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="02d0f-532">Support CLONE_PTRACE and CLONE_UNTRACED [GH 121, 2781]</span></span>
* <span data-ttu-id="02d0f-533">Verarbeiten eines Nicht-SIGCHLD-Beendigungssignals im Klon [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="02d0f-533">Handle non-SIGCHLD termination signal in clone [GH 121, 2781]</span></span>
* <span data-ttu-id="02d0f-534">Stub für /proc/sys/fs/inotify/max_user_instances und /proc/sys/fs/inotify/max_user_watches [GH 1705]</span><span class="sxs-lookup"><span data-stu-id="02d0f-534">Stub /proc/sys/fs/inotify/max_user_instances and /proc/sys/fs/inotify/max_user_watches [GH 1705]</span></span>
* <span data-ttu-id="02d0f-535">Fehler beim Laden von ELF-Binärdateien, die Ladeheader mit Offsets ungleich NULL enthalten [GH 1884]</span><span class="sxs-lookup"><span data-stu-id="02d0f-535">Error loading ELF binaries that contain load headers with non-zero offsets [GH 1884]</span></span>
* <span data-ttu-id="02d0f-536">Eliminieren von nachfolgenden Seitenbytes beim Laden von Images.</span><span class="sxs-lookup"><span data-stu-id="02d0f-536">Zero out trailing page bytes when loading images.</span></span>
* <span data-ttu-id="02d0f-537">Verringern der Fälle, in denen execve den Prozess automatisch beendet</span><span class="sxs-lookup"><span data-stu-id="02d0f-537">Reduce cases where execve silently terminates process</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-538">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-538">Console</span></span>
* <span data-ttu-id="02d0f-539">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-539">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-540">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-540">LTP Results:</span></span>
<span data-ttu-id="02d0f-541">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-541">Testing in progress.</span></span>

## <a name="build-17083"></a><span data-ttu-id="02d0f-542">Build 17083</span><span class="sxs-lookup"><span data-stu-id="02d0f-542">Build 17083</span></span>
<span data-ttu-id="02d0f-543">Allgemeine Windows-Informationen zu Build 17083 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-543">For general Windows information on build 17083 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-544">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-544">WSL</span></span>
* <span data-ttu-id="02d0f-545">Korrektur der Fehlerüberprüfung für epoll [GH 2798, 2801, 2857]</span><span class="sxs-lookup"><span data-stu-id="02d0f-545">Fixed bugcheck related to epoll [GH 2798, 2801, 2857]</span></span>
* <span data-ttu-id="02d0f-546">Korrektur von Hängern beim Deaktivieren von ASLR [GH 1185, 2870]</span><span class="sxs-lookup"><span data-stu-id="02d0f-546">Fixed hangs when turning off ASLR [GH 1185, 2870]</span></span>
* <span data-ttu-id="02d0f-547">Sicherstellen, dass mmap-Vorgänge atomarisch erscheinen [GH 2732]</span><span class="sxs-lookup"><span data-stu-id="02d0f-547">Ensure mmap operations appear atomic [GH 2732]</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-548">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-548">Console</span></span>
* <span data-ttu-id="02d0f-549">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-549">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-550">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-550">LTP Results:</span></span>
<span data-ttu-id="02d0f-551">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-551">Testing in progress.</span></span>

## <a name="build-17074"></a><span data-ttu-id="02d0f-552">Build 17074</span><span class="sxs-lookup"><span data-stu-id="02d0f-552">Build 17074</span></span>
<span data-ttu-id="02d0f-553">Allgemeine Windows-Informationen zu Build 17074 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-553">For general Windows information on build 17074 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-554">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-554">WSL</span></span>
* <span data-ttu-id="02d0f-555">Festes Speicherformat von DrvFs-Metadaten [GH 2777]</span><span class="sxs-lookup"><span data-stu-id="02d0f-555">Fixed storage format of DrvFs metadata [GH 2777]</span></span> </br>
<span data-ttu-id="02d0f-556">**Wichtig:** Die vor diesem Build erstellten DrvFs-Metadaten werden falsch oder überhaupt nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-556">**Important:** DrvFs metadata created before this build will show up incorrectly or not at all.</span></span> <span data-ttu-id="02d0f-557">Um betroffene Dateien zu korrigieren, verwenden Sie chmod und chown zum erneuten Anwenden der Metadaten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-557">To fix affected files, use chmod and chown to re-apply the metadata.</span></span>
* <span data-ttu-id="02d0f-558">Korrektur eines Problems mit mehreren Signalen und neu startbaren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-558">Fixed issue with multiple signals and restartable syscalls.</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-559">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-559">Console</span></span>
* <span data-ttu-id="02d0f-560">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-560">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-561">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-561">LTP Results:</span></span>
<span data-ttu-id="02d0f-562">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-562">Testing in progress.</span></span>

## <a name="build-17063"></a><span data-ttu-id="02d0f-563">Build 17063</span><span class="sxs-lookup"><span data-stu-id="02d0f-563">Build 17063</span></span>
<span data-ttu-id="02d0f-564">Allgemeine Windows-Informationen zu Build 17063 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-564">For general Windows information on build 17063 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="02d0f-565">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-565">WSL</span></span>
* <span data-ttu-id="02d0f-566">DrvFs unterstützt zusätzliche Linux-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-566">DrvFs supports additional Linux metadata.</span></span> <span data-ttu-id="02d0f-567">Dies ermöglicht das Festlegen des Besitzers und des Dateimodus mit chmod/chown sowie das Erstellen spezieller Dateien, etwa Fifos, Unix-Sockets und Gerätedateien.</span><span class="sxs-lookup"><span data-stu-id="02d0f-567">This allows setting the owner and mode of files using chmod/chown, and also the creation of special files such as fifos, unix sockets and device files.</span></span> <span data-ttu-id="02d0f-568">Diese Option ist zurzeit standardmäßig deaktiviert, da Sie noch experimentell ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-568">This is disabled by default for now since it's still experimental.</span></span>
<span data-ttu-id="02d0f-569">**Hinweis:**  Wir haben einen Fehler im Metadatenformat behoben, das von DrvFs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-569">**Note:**  We fixed a bug in the metadata format used by DrvFs.</span></span> <span data-ttu-id="02d0f-570">Obwohl Metadaten in diesem Build für Experimente funktionieren, lesen zukünftige Builds die von diesem Build erstellten Metadaten nicht ordnungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="02d0f-570">While metadata works on this build for experimentation, future builds will not correctly read metadata created by this build.</span></span>  <span data-ttu-id="02d0f-571">Möglicherweise müssen Sie den Besitzer für geänderte Dateien manuell aktualisieren, und Geräte mit einer benutzerdefinierten Geräte-ID müssen neu erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-571">You might need to manually update owner for modified files and devices with a custom device ID will have to be recreated.</span></span>

  <span data-ttu-id="02d0f-572">Um diese Funktion zu aktivieren, binden Sie DrvFs mit der Metadatenoption ein (um sie für eine vorhandene Einbindung zu aktivieren, müssen Sie die Einbindung zunächst aufheben):</span><span class="sxs-lookup"><span data-stu-id="02d0f-572">To enable, mount DrvFs with the metadata option (to enable it on an existing mount, you must first unmount it):</span></span>

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  <span data-ttu-id="02d0f-573">Linux-Berechtigungen werden der Datei als zusätzliche Metadaten hinzugefügt. Sie wirken sich nicht auf die Windows-Berechtigungen aus.</span><span class="sxs-lookup"><span data-stu-id="02d0f-573">Linux permissions are added as additional metadata to the file; they do not affect the Windows permissions.</span></span>  <span data-ttu-id="02d0f-574">Beachten Sie, dass beim Bearbeiten einer Datei mithilfe eines Windows-Editors die Metadaten möglicherweise entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-574">Remember, editing a file using a Windows editor may remove the metadata.</span></span> <span data-ttu-id="02d0f-575">In diesem Fall wird die Datei auf die Standardberechtigungen zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-575">In this case, the file will revert to its default permissions.</span></span>

* <span data-ttu-id="02d0f-576">Hinzufügen von Einbindungsoptionen zu DrvFs, um Dateien ohne Metadaten zu steuern.</span><span class="sxs-lookup"><span data-stu-id="02d0f-576">Added mount options to DrvFs to control files without metadata.</span></span>
  * <span data-ttu-id="02d0f-577">uid: die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-577">uid: the user ID used for the owner of all files.</span></span>
  * <span data-ttu-id="02d0f-578">gid: die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-578">gid: the group ID used for the owner of all files.</span></span>
  * <span data-ttu-id="02d0f-579">umask: Eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-579">umask: an octal mask of permissions to exclude for all files and directories.</span></span>
  * <span data-ttu-id="02d0f-580">fmask: Eine oktale Maske mit Berechtigungen, die für alle regulären Dateien ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-580">fmask: an octal mask of permissions to exclude for all regular files.</span></span>
  * <span data-ttu-id="02d0f-581">dmask: Eine oktale Maske mit Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-581">dmask: an octal mask of permissions to exclude for all directories.</span></span>

  <span data-ttu-id="02d0f-582">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="02d0f-582">For example:</span></span>
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  <span data-ttu-id="02d0f-583">Kombinieren Sie dies mit der Metadatenoption, um Standardberechtigungen für Dateien ohne Metadaten anzugeben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-583">Combine with the metadata option to specify default permissions for files without metadata.</span></span>

* <span data-ttu-id="02d0f-584">Wird in einer neuen Umgebungsvariablen (`WSLENV`) eingeführt, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32 ausgetauscht werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-584">Introduced a new environment variable, `WSLENV`, to configure how environment variables flow between WSL and Win32.</span></span>

  <span data-ttu-id="02d0f-585">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="02d0f-585">For example:</span></span>

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  <span data-ttu-id="02d0f-586">`WSLENV` eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozessen aus Win32 oder Win32-Prozessen aus WSL eingeschlossen werden können.</span><span class="sxs-lookup"><span data-stu-id="02d0f-586">`WSLENV` is a colon-delimited list of environment variables that can be included when launching WSL processes from Win32 or Win32 processes from WSL.</span></span>  <span data-ttu-id="02d0f-587">Jeder Variablen kann ein Schrägstrich als Suffix vorangestellt werden, gefolgt von Flags, um anzugeben, wie sie übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="02d0f-587">Each variable can be suffixed with a slash followed by flags to specify how it is translated.</span></span>
  * <span data-ttu-id="02d0f-588">p: Der Wert ist ein Pfad, der zwischen WSL-Pfaden und Win32-Pfaden übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="02d0f-588">p: The value is a path that should be translated between WSL paths and Win32 paths.</span></span>
  * <span data-ttu-id="02d0f-589">l: Der Wert ist eine Liste von Pfaden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-589">l: The value is a list of paths.</span></span> <span data-ttu-id="02d0f-590">In WSL ist es eine durch Doppelpunkte getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="02d0f-590">In WSL, it is a colon-delimited list.</span></span> <span data-ttu-id="02d0f-591">In Win32 ist es eine durch Semikolons getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="02d0f-591">In Win32, it is a semicolon-delimited list.</span></span>
  * <span data-ttu-id="02d0f-592">u: Der Wert sollte nur beim Aufrufen von WSL aus Win32 eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-592">u: The value should only be included when invoking WSL from Win32</span></span>
  * <span data-ttu-id="02d0f-593">w: Der Wert sollte nur beim Aufrufen von Win32 aus WSL eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-593">w: The value should only be included when invoking Win32 from WSL</span></span>

  <span data-ttu-id="02d0f-594">Sie können `WSLENV` in der BASHRC-Datei oder in der benutzerdefinierten Windows-Umgebung für Ihren Benutzer festlegen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-594">You can set `WSLENV` in .bashrc or in the custom Windows environment for your user.</span></span>

* <span data-ttu-id="02d0f-595">drvfs wird ordnungsgemäß eingebunden und behält Zeitstempel aus from tar, cp -p bei (GH 1939)</span><span class="sxs-lookup"><span data-stu-id="02d0f-595">drvfs mounts correctly preserves timestamps from tar, cp -p (GH 1939)</span></span>
* <span data-ttu-id="02d0f-596">Symbolische drvfs-Verknüpfungen geben die richtige Größe an (GH 2641)</span><span class="sxs-lookup"><span data-stu-id="02d0f-596">drvfs symlinks report the correct size (GH 2641)</span></span>
* <span data-ttu-id="02d0f-597">Lese-/Schreibvorgänge funktionieren für sehr große E/A-Größen (GH 2653)</span><span class="sxs-lookup"><span data-stu-id="02d0f-597">read/write works for very large IO sizes (GH 2653)</span></span>
* <span data-ttu-id="02d0f-598">waitpid funktioniert mit Prozessgruppen-IDs (GH 2534)</span><span class="sxs-lookup"><span data-stu-id="02d0f-598">waitpid works with process group IDs (GH 2534)</span></span>
* <span data-ttu-id="02d0f-599">Erheblich verbesserte mmap-Leistung für große reserve-Regionen, Verbesserung der ghc-Leistung (GH 1671)</span><span class="sxs-lookup"><span data-stu-id="02d0f-599">significantly improved mmap performance for large reserve regions; improves ghc performance (GH 1671)</span></span>
* <span data-ttu-id="02d0f-600">personality unterstützt READ_IMPLIES_EXEC, Korrekturen maxima und clisp (GH 1185)</span><span class="sxs-lookup"><span data-stu-id="02d0f-600">personality supports for READ_IMPLIES_EXEC; fixes maxima and clisp (GH 1185)</span></span>
* <span data-ttu-id="02d0f-601">mprotect unterstützt PROT_GROWSDOWN,;Korrekturen clisp (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="02d0f-601">mprotect supports PROT_GROWSDOWN; fixes clisp (GH 1128)</span></span>
* <span data-ttu-id="02d0f-602">Seitenfehlerkorrekturen im Overcommitmodus, Korrekturen sbcl (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="02d0f-602">page fault fixes in overcommit mode; fixes sbcl (GH 1128)</span></span>
* <span data-ttu-id="02d0f-603">clone unterstützt weitere Flagkombinationen</span><span class="sxs-lookup"><span data-stu-id="02d0f-603">clone supports more flags combinations</span></span>
* <span data-ttu-id="02d0f-604">Unterstützung von select/epoll von epoll-Dateien (zuvor eine Nulloperation).</span><span class="sxs-lookup"><span data-stu-id="02d0f-604">Support select/epoll of epoll files (previously a no-op).</span></span>
* <span data-ttu-id="02d0f-605">Benachrichtigen von ptrace über nicht implementierte Systemaufrufe.</span><span class="sxs-lookup"><span data-stu-id="02d0f-605">Notify ptrace of unimplemented syscalls.</span></span>
* <span data-ttu-id="02d0f-606">Ignorieren von Schnittstellen, die nicht aktiv sind, beim Generieren von resolv.conf-Namenservern [GH 2694]</span><span class="sxs-lookup"><span data-stu-id="02d0f-606">Ignore interfaces that are not up when generating resolv.conf nameservers [GH 2694]</span></span>
* <span data-ttu-id="02d0f-607">Aufzählen von Netzwerkschnittstellen ohne physische Adresse.</span><span class="sxs-lookup"><span data-stu-id="02d0f-607">Enumerate network interfaces with no physical address.</span></span> <span data-ttu-id="02d0f-608">[GH 2685]</span><span class="sxs-lookup"><span data-stu-id="02d0f-608">[GH 2685]</span></span>
* <span data-ttu-id="02d0f-609">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-609">Additional bug fixes and improvements.</span></span>

### <a name="linux-tools-available-to-developers-on-windows"></a><span data-ttu-id="02d0f-610">Linux-Tools für Entwickler unter Windows verfügbar</span><span class="sxs-lookup"><span data-stu-id="02d0f-610">Linux tools available to developers on Windows</span></span>

* <span data-ttu-id="02d0f-611">Windows-Befehlszeilen-Toolkette enthält bsdtar (tar) und curl.</span><span class="sxs-lookup"><span data-stu-id="02d0f-611">Windows Command line Toolchain includes bsdtar (tar) and curl.</span></span>
  <span data-ttu-id="02d0f-612">Lesen Sie [diesen Blog](https://aka.ms/tarcurlwindows), um mehr über das Hinzufügen dieser beiden neuen Tools zu erfahren, und sehen Sie, wie Sie das Entwicklererlebnis unter Windows formen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-612">Read [this blog](https://aka.ms/tarcurlwindows) to learn more about the addition of these two new tools and see how they’re shaping the developer experience on Windows.</span></span>

*   <span data-ttu-id="02d0f-613">`AF_UNIX` ist im Windows Insider SDK (17061 und höher) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="02d0f-613">`AF_UNIX` is available in the Windows Insider SDK (17061+).</span></span>
  <span data-ttu-id="02d0f-614">Lesen Sie [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/), um weitere Informationen zu `AF_UNIX` zu erhalten und mehr über die Verwendung in Windows durch Entwickler zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-614">Read [this blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) to learn more about `AF_UNIX` and how developers on Windows can use it.</span></span>

### <a name="console"></a><span data-ttu-id="02d0f-615">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-615">Console</span></span>
* <span data-ttu-id="02d0f-616">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-616">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-617">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-617">LTP Results:</span></span>
<span data-ttu-id="02d0f-618">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-618">Testing in progress.</span></span>


## <a name="build-17046"></a><span data-ttu-id="02d0f-619">Build 17046</span><span class="sxs-lookup"><span data-stu-id="02d0f-619">Build 17046</span></span>

<span data-ttu-id="02d0f-620">Allgemeine Windows-Informationen zu Build 17046 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span><span class="sxs-lookup"><span data-stu-id="02d0f-620">For general Windows information on build 17046 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-621">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-621">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-622">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-622">WSL</span></span>
- <span data-ttu-id="02d0f-623">Ermöglicht das Ausführen von Prozessen ohne ein aktives Terminal.</span><span class="sxs-lookup"><span data-stu-id="02d0f-623">Allow processes to run without an active terminal.</span></span> <span data-ttu-id="02d0f-624">[GH 709, 1007, 1511, 2252, 2391 usw.]</span><span class="sxs-lookup"><span data-stu-id="02d0f-624">[GH 709, 1007, 1511, 2252, 2391, et al.]</span></span>
- <span data-ttu-id="02d0f-625">Bessere Unterstützung von CLONE_VFORK und CLONE_VM.</span><span class="sxs-lookup"><span data-stu-id="02d0f-625">Better support of CLONE_VFORK and CLONE_VM.</span></span> <span data-ttu-id="02d0f-626">[GH 1878, 2615]</span><span class="sxs-lookup"><span data-stu-id="02d0f-626">[GH 1878, 2615]</span></span>
- <span data-ttu-id="02d0f-627">Überspringen der TDI-Filtertreiber für WSL-Netzwerkvorgänge.</span><span class="sxs-lookup"><span data-stu-id="02d0f-627">Skip TDI filter drivers for WSL networking operations.</span></span> <span data-ttu-id="02d0f-628">[GH 1554]</span><span class="sxs-lookup"><span data-stu-id="02d0f-628">[GH 1554]</span></span>
- <span data-ttu-id="02d0f-629">DrvFs erstellt symbolische NT-Verknüpfungen, wenn bestimmte Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="02d0f-629">DrvFs creates NT symlinks when certain conditions are met.</span></span> <span data-ttu-id="02d0f-630">[GH 353, 1475, 2602]</span><span class="sxs-lookup"><span data-stu-id="02d0f-630">[GH 353, 1475, 2602]</span></span>
    - <span data-ttu-id="02d0f-631">Das Verknüpfungsziel muss relativ sein, darf keine Einbindungspunkte oder symbolische Verknüpfungen kreuzen und muss vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="02d0f-631">The link target must be relative, must not cross any mount points or symlinks, and must exist.</span></span>
    - <span data-ttu-id="02d0f-632">Der Benutzer muss über SE_CREATE_SYMBOLIC_LINK_PRIVILEGE verfügen (dies erfordert normalerweise, dass Sie „wsl.exe“ mit erhöhten Rechten starten), sofern der Entwicklermodus nicht aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-632">The user must have SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (this normally requires you to launch wsl.exe elevated), unless Developer Mode is turned on.</span></span>
    - <span data-ttu-id="02d0f-633">Unter allen anderen Umständen erstellt DrvFs weiterhin symbolische WSL-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-633">In all other situations, DrvFs still creates WSL symlinks.</span></span>
- <span data-ttu-id="02d0f-634">Ermöglichen der gleichzeitigen Ausführung von WSL-Instanzen mit und ohne erhöhten Rechten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-634">Allow running elevated and non-elevated WSL instances simultaneously.</span></span>
- <span data-ttu-id="02d0f-635">Unterstützung von /proc/sys/kernel/Yama/ptrace_scope</span><span class="sxs-lookup"><span data-stu-id="02d0f-635">Support /proc/sys/kernel/yama/ptrace_scope</span></span>
- <span data-ttu-id="02d0f-636">Hinzufügen von wslpath zum Durchführen von Konvertierungen von WSL-<- >Windows-Pfaden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-636">Add wslpath to do WSL<->Windows path conversions.</span></span> <span data-ttu-id="02d0f-637">[GH 522, 1243, 1834, 2327 usw.]</span><span class="sxs-lookup"><span data-stu-id="02d0f-637">[GH 522, 1243, 1834, 2327, et al.]</span></span>
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a><span data-ttu-id="02d0f-638">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-638">Console</span></span>
- <span data-ttu-id="02d0f-639">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-639">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-640">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-640">LTP Results:</span></span>
<span data-ttu-id="02d0f-641">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-641">Testing in progress.</span></span>


## <a name="build-17040"></a><span data-ttu-id="02d0f-642">Build 17040</span><span class="sxs-lookup"><span data-stu-id="02d0f-642">Build 17040</span></span>

<span data-ttu-id="02d0f-643">Allgemeine Windows-Informationen zu Build 17040 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span><span class="sxs-lookup"><span data-stu-id="02d0f-643">For general Windows information on build 17040 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-644">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-644">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-645">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-645">WSL</span></span>
- <span data-ttu-id="02d0f-646">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="02d0f-646">No fixes since 17035.</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-647">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-647">Console</span></span>
- <span data-ttu-id="02d0f-648">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="02d0f-648">No fixes since 17035.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-649">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-649">LTP Results:</span></span>
<span data-ttu-id="02d0f-650">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-650">Testing in progress.</span></span>

## <a name="build-17035"></a><span data-ttu-id="02d0f-651">Build 17035</span><span class="sxs-lookup"><span data-stu-id="02d0f-651">Build 17035</span></span>

<span data-ttu-id="02d0f-652">Allgemeine Windows-Informationen zu Build 17035 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span><span class="sxs-lookup"><span data-stu-id="02d0f-652">For general Windows information on build 17035 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-653">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-653">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-654">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-654">WSL</span></span>
- <span data-ttu-id="02d0f-655">Der Zugriff auf Dateien auf DrvFs kann gelegentlich mit EINVAL fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-655">Accessing files on DrvFs could occasionally fail with EINVAL.</span></span> <span data-ttu-id="02d0f-656">[GH 2448]</span><span class="sxs-lookup"><span data-stu-id="02d0f-656">[GH 2448]</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-657">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-657">Console</span></span>
- <span data-ttu-id="02d0f-658">Farbverlust beim Einfügen/Löschen von Zeilen im VT-Modus.</span><span class="sxs-lookup"><span data-stu-id="02d0f-658">Some color loss when inserting/deleting lines in VT mode.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-659">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-659">LTP Results:</span></span>
<span data-ttu-id="02d0f-660">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-660">Testing in progress.</span></span>

## <a name="build-17025"></a><span data-ttu-id="02d0f-661">Build 17025</span><span class="sxs-lookup"><span data-stu-id="02d0f-661">Build 17025</span></span>

<span data-ttu-id="02d0f-662">Allgemeine Windows-Informationen zu Build 17025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span><span class="sxs-lookup"><span data-stu-id="02d0f-662">For general Windows information on build 17025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-663">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-663">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-664">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-664">WSL</span></span>
- <span data-ttu-id="02d0f-665">Starten anfänglicher Prozesse in einer neuen Vordergrundprozessgruppe [GH 1653, 2510].</span><span class="sxs-lookup"><span data-stu-id="02d0f-665">Start initial processes in a new foreground process group [GH 1653, 2510].</span></span>
- <span data-ttu-id="02d0f-666">Korrekturen der SIGHUP-Übermittlung [GH 2496].</span><span class="sxs-lookup"><span data-stu-id="02d0f-666">SIGHUP delivery fixes [GH 2496].</span></span>
- <span data-ttu-id="02d0f-667">Generieren eines Standardnamens für virtuelle Bridge generieren, wenn keine Angabe erfolgt [GH 2497].</span><span class="sxs-lookup"><span data-stu-id="02d0f-667">Generate default virtual bridge name if none provided [GH 2497].</span></span>
- <span data-ttu-id="02d0f-668">Implementieren von /proc/sys/kernel/Random/boot_id [GH 2518].</span><span class="sxs-lookup"><span data-stu-id="02d0f-668">Implement /proc/sys/kernel/random/boot_id [GH 2518].</span></span>
- <span data-ttu-id="02d0f-669">Weitere Interop-Pipekorrekturen für stdout/stderr.</span><span class="sxs-lookup"><span data-stu-id="02d0f-669">More interop stdout/stderr pipe fixes.</span></span>
- <span data-ttu-id="02d0f-670">Stub für syncfs-Systemaufruf.</span><span class="sxs-lookup"><span data-stu-id="02d0f-670">Stub syncfs system call.</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-671">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-671">Console</span></span>
- <span data-ttu-id="02d0f-672">Korrektur der VT-Eingabeübersetzung für Drittanbieterkonsolen [GH 111]</span><span class="sxs-lookup"><span data-stu-id="02d0f-672">Fix input VT translation for third party consoles [GH 111]</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-673">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-673">LTP Results:</span></span>
<span data-ttu-id="02d0f-674">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-674">Testing in progress.</span></span>

## <a name="build-17017"></a><span data-ttu-id="02d0f-675">Build 17017</span><span class="sxs-lookup"><span data-stu-id="02d0f-675">Build 17017</span></span>

<span data-ttu-id="02d0f-676">Allgemeine Windows-Informationen zu Build 17017 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span><span class="sxs-lookup"><span data-stu-id="02d0f-676">For general Windows information on build 17017 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-677">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-677">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-678">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-678">WSL</span></span>
- <span data-ttu-id="02d0f-679">Ignorieren leerer ELF-Programmheader [GH 330].</span><span class="sxs-lookup"><span data-stu-id="02d0f-679">Ignore empty ELF program headers [GH 330].</span></span>
- <span data-ttu-id="02d0f-680">Ermöglichen, dass LxssManager WSL-Instanzen für nicht interaktive Benutzer erstellt (Unterstützung für SSH und geplante Aufgaben) [GH 777, 1602].</span><span class="sxs-lookup"><span data-stu-id="02d0f-680">Allow LxssManager to create WSL instances for non-interactive users (ssh and scheduled task support) [GH 777, 1602].</span></span>
- <span data-ttu-id="02d0f-681">Unterstützung von WSL->Win32->WSL-Szenarien („Inception“) [GH 1228].</span><span class="sxs-lookup"><span data-stu-id="02d0f-681">Support WSL->Win32->WSL ("inception") scenarios [GH 1228].</span></span>
- <span data-ttu-id="02d0f-682">Eingeschränkte Unterstützung für das Beenden von Konsolen-Apps, die über Interop aufgerufen wurden [GH 1614].</span><span class="sxs-lookup"><span data-stu-id="02d0f-682">Limited support for termination of console apps invoked via interop [GH 1614].</span></span>
- <span data-ttu-id="02d0f-683">Unterstützung von Einbindungsoptionen für devpts [GH 1948].</span><span class="sxs-lookup"><span data-stu-id="02d0f-683">Support mount options for devpts [GH 1948].</span></span>
- <span data-ttu-id="02d0f-684">Ptrace blockiert den Start untergeordneter Prozesse [GH 2333].</span><span class="sxs-lookup"><span data-stu-id="02d0f-684">Ptrace blocking child startup [GH 2333].</span></span>
- <span data-ttu-id="02d0f-685">EPOLLET fehlen einige Ereignisse [GH 2462].</span><span class="sxs-lookup"><span data-stu-id="02d0f-685">EPOLLET missing some events [GH 2462].</span></span>
- <span data-ttu-id="02d0f-686">Rückgabe einer größeren Anzahl von Daten für PTRACE_GETSIGINFO.</span><span class="sxs-lookup"><span data-stu-id="02d0f-686">Return more data for PTRACE_GETSIGINFO.</span></span>
- <span data-ttu-id="02d0f-687">Getdents mit lseek liefert falsche Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="02d0f-687">Getdents with lseek gives incorrect results.</span></span>
- <span data-ttu-id="02d0f-688">Korrektur einiger Hänger von Win32-Interop-Apps, die auf Eingaben in einer Pipe warten, die keine weiteren Daten enthält.</span><span class="sxs-lookup"><span data-stu-id="02d0f-688">Fix some Win32 interop app hangs, waiting for input on a pipe that has no more data.</span></span>
- <span data-ttu-id="02d0f-689">O_ASYNC-Unterstützung für tty/pty-Dateien.</span><span class="sxs-lookup"><span data-stu-id="02d0f-689">O_ASYNC support for tty/pty files.</span></span>
- <span data-ttu-id="02d0f-690">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-690">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-691">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-691">Console</span></span>
- <span data-ttu-id="02d0f-692">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-692">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-693">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-693">LTP Results:</span></span>
<span data-ttu-id="02d0f-694">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-694">Testing in progress.</span></span>

## <a name="fall-creators-update"></a><span data-ttu-id="02d0f-695">Fall Creators Update</span><span class="sxs-lookup"><span data-stu-id="02d0f-695">Fall Creators Update</span></span>

## <a name="build-16288"></a><span data-ttu-id="02d0f-696">Build 16288</span><span class="sxs-lookup"><span data-stu-id="02d0f-696">Build 16288</span></span>

<span data-ttu-id="02d0f-697">Allgemeine Windows-Informationen zu Build 16288 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-697">For general Windows information on build 16288 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-698">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-698">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-699">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-699">WSL</span></span>
- <span data-ttu-id="02d0f-700">Ordnungsgemäße Initialisierung und Meldung von uid, gid und Modus für Socketdateideskriptoren [GH 2490]</span><span class="sxs-lookup"><span data-stu-id="02d0f-700">Correctly initialize and report uid, gid, and mode for socket file descriptors [GH 2490]</span></span>
- <span data-ttu-id="02d0f-701">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-701">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-702">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-702">Console</span></span>
- <span data-ttu-id="02d0f-703">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-703">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-704">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-704">LTP Results:</span></span>
<span data-ttu-id="02d0f-705">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="02d0f-705">No change since 16273</span></span>

## <a name="build-16278"></a><span data-ttu-id="02d0f-706">Build 16278</span><span class="sxs-lookup"><span data-stu-id="02d0f-706">Build 16278</span></span>

<span data-ttu-id="02d0f-707">Allgemeine Windows-Informationen zu Build 162738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-707">For general Windows information on build 162738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-708">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-708">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-709">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-709">WSL</span></span>
- <span data-ttu-id="02d0f-710">Explizite Aufhebung der Zuordnung zugeordneter Ansichten von dateigestützten Abschnitten beim Beenden des LX MM-Status [GH 2415]</span><span class="sxs-lookup"><span data-stu-id="02d0f-710">Explicitly unmap mapped views of file backed sections when tearing down LX MM state [GH 2415]</span></span>
- <span data-ttu-id="02d0f-711">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-711">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-712">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-712">Console</span></span>
- <span data-ttu-id="02d0f-713">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-713">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-714">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-714">LTP Results:</span></span>
<span data-ttu-id="02d0f-715">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="02d0f-715">No change since 16273</span></span>

## <a name="build-16275"></a><span data-ttu-id="02d0f-716">Build 16275</span><span class="sxs-lookup"><span data-stu-id="02d0f-716">Build 16275</span></span>

<span data-ttu-id="02d0f-717">Allgemeine Windows-Informationen zu Build 162735 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-717">For general Windows information on build 162735 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-718">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-718">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-719">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-719">WSL</span></span>
- <span data-ttu-id="02d0f-720">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-720">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-721">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-721">Console</span></span>
- <span data-ttu-id="02d0f-722">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-722">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-723">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-723">LTP Results:</span></span>
<span data-ttu-id="02d0f-724">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="02d0f-724">No change since 16273</span></span>

## <a name="build-16273"></a><span data-ttu-id="02d0f-725">Build 16273</span><span class="sxs-lookup"><span data-stu-id="02d0f-725">Build 16273</span></span>

<span data-ttu-id="02d0f-726">Allgemeine Windows-Informationen zu Build 16273 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-726">For general Windows information on build 16273 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-727">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-727">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-728">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-728">WSL</span></span>
- <span data-ttu-id="02d0f-729">Korrektur eines Problems, bei dem DrvFs manchmal den falschen Dateityp für Verzeichnisse gemeldet hat [GH 2392]</span><span class="sxs-lookup"><span data-stu-id="02d0f-729">Fixed an issue where DrvFs sometimes reported the wrong file type for directories [GH 2392]</span></span>
- <span data-ttu-id="02d0f-730">Ermöglichen der Erstellung von NETLINK_KOBJECT_UEVENT-Sockets zum Entsperren von Programmen, die uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span><span class="sxs-lookup"><span data-stu-id="02d0f-730">Allow creation of NETLINK_KOBJECT_UEVENT sockets to unblock programs that use uevent [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span></span>
- <span data-ttu-id="02d0f-731">Hinzufügen von Unterstützung für nicht blockierende Verbindungen [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span><span class="sxs-lookup"><span data-stu-id="02d0f-731">Add support for non-blocking connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span></span>
- <span data-ttu-id="02d0f-732">Implementieren des CLONE_FS-Klonsystem-Aufrufflags [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="02d0f-732">Implement CLONE_FS clone system call flag [GH 2242]</span></span>
- <span data-ttu-id="02d0f-733">Korrektur von Problemen im Zusammenhang mit der nicht ordnungsgemäßen Behandlung von Registerkarten oder Anführungszeichen in NT-Interop [GH 1625, 2164]</span><span class="sxs-lookup"><span data-stu-id="02d0f-733">Fix issues around not handling tabs or quotes correctly in NT interop [GH 1625, 2164]</span></span>
- <span data-ttu-id="02d0f-734">Beheben des Fehlers „Zugriff verweigert“ beim Versuch, WSL-Instanzen erneut zu starten [GH 651, 2095]</span><span class="sxs-lookup"><span data-stu-id="02d0f-734">Resolve access denied error when trying to re-launch WSL instances [GH 651, 2095]</span></span>
- <span data-ttu-id="02d0f-735">Implementieren von Futex-Vorgängen FUTEX_REQUEUE und FUTEX_CMP_REQUEUE [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="02d0f-735">Implement futex FUTEX_REQUEUE and FUTEX_CMP_REQUEUE operations [GH 2242]</span></span>
- <span data-ttu-id="02d0f-736">Korrigieren von Berechtigungen für verschiedene SysFs-Dateien [GH 2214]</span><span class="sxs-lookup"><span data-stu-id="02d0f-736">Fix permissions for various SysFs files [GH 2214]</span></span>
- <span data-ttu-id="02d0f-737">Korrigieren des Hängens des Haskell-Stapels während des Setups [GH 2290]</span><span class="sxs-lookup"><span data-stu-id="02d0f-737">Fix Haskell stack hang during setup [GH 2290]</span></span>
- <span data-ttu-id="02d0f-738">Implementieren der Flags „C“, „O“ und „P“ von binfmt_misc [GH 2103]</span><span class="sxs-lookup"><span data-stu-id="02d0f-738">Implement binfmt_misc 'C' 'O' and 'P' flags [GH 2103]</span></span>
- <span data-ttu-id="02d0f-739">Hinzufügen von /proc/sys/kernel/shmmax/shmmni und /threads-max [GH 1753]</span><span class="sxs-lookup"><span data-stu-id="02d0f-739">Add /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span></span>
- <span data-ttu-id="02d0f-740">Hinzufügen partieller Unterstützung für den ioprio_set-Systemaufruf [GH 498]</span><span class="sxs-lookup"><span data-stu-id="02d0f-740">Add partial support for ioprio_set system call [GH 498]</span></span>
- <span data-ttu-id="02d0f-741">Stub für SO_REUSEPORT und Hinzufügen von Unterstützung für SO_PASSCRED für netlink-Sockets [GH 69]</span><span class="sxs-lookup"><span data-stu-id="02d0f-741">Stub SO_REUSEPORT & adding support for SO_PASSCRED for netlink sockets [GH 69]</span></span>
- <span data-ttu-id="02d0f-742">Rückgabe anderer Fehlercodes aus RegisterDistribuiton, wenn zurzeit eine Distribution installiert oder deinstalliert wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-742">Return different error codes from RegisterDistribuiton if a distribution is currently being installed or uninstalled.</span></span>
- <span data-ttu-id="02d0f-743">Ermöglichen des Aufhebens der Registrierung von teilweise installierten WSL-Distributionen über „wslconfig.exe“</span><span class="sxs-lookup"><span data-stu-id="02d0f-743">Allow unregistration of partially installed WSL distributions via wslconfig.exe</span></span>
- <span data-ttu-id="02d0f-744">Korrektur des Hängens des Python-Sockettests von udp::msg_peek</span><span class="sxs-lookup"><span data-stu-id="02d0f-744">Fix python socket test hang from udp::msg_peek</span></span>
- <span data-ttu-id="02d0f-745">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-745">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-746">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-746">Console</span></span>
- <span data-ttu-id="02d0f-747">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-747">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-748">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-748">LTP Results:</span></span>
<span data-ttu-id="02d0f-749">Tests gesamt: 1904</span><span class="sxs-lookup"><span data-stu-id="02d0f-749">Total Tests: 1904</span></span><br/>
<span data-ttu-id="02d0f-750">Übersprungene Tests gesamt: 209</span><span class="sxs-lookup"><span data-stu-id="02d0f-750">Total Skipped Tests: 209</span></span><br/>
<span data-ttu-id="02d0f-751">Fehler gesamt: 229</span><span class="sxs-lookup"><span data-stu-id="02d0f-751">Total Failures: 229</span></span><br/>
[<span data-ttu-id="02d0f-752">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-752">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a><span data-ttu-id="02d0f-753">Build 16257</span><span class="sxs-lookup"><span data-stu-id="02d0f-753">Build 16257</span></span>

<span data-ttu-id="02d0f-754">Allgemeine Windows-Informationen zu Build 16257 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-754">For general Windows information on build 16257 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-755">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-755">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-756">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-756">WSL</span></span>
- <span data-ttu-id="02d0f-757">Implementieren des prlimit64-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="02d0f-757">Implement prlimit64 system call</span></span>
- <span data-ttu-id="02d0f-758">Hinzufügen von Unterstützung für ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span><span class="sxs-lookup"><span data-stu-id="02d0f-758">Add support for ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span></span>
- <span data-ttu-id="02d0f-759">Stub für MSG_MORE für TCP-Sockets [GH 2351]</span><span class="sxs-lookup"><span data-stu-id="02d0f-759">Stub MSG_MORE for TCP sockets [GH 2351]</span></span>
- <span data-ttu-id="02d0f-760">Korrektur des ungültigen Verhaltens des AT_EXECFN-Hilfsvektors [GH 2133]</span><span class="sxs-lookup"><span data-stu-id="02d0f-760">Fix invalid AT_EXECFN auxiliary vector behavior [GH 2133]</span></span>
- <span data-ttu-id="02d0f-761">Korrektur des Kopier-/Einfügeverhalten für Konsole/TTY und Hinzufügen einer besseren Verarbeitung voller Puffer [GH 2204, 2131]</span><span class="sxs-lookup"><span data-stu-id="02d0f-761">Fix copy/paste behavior for console/tty, and add better full buffer handling [GH 2204, 2131]</span></span>
- <span data-ttu-id="02d0f-762">Festlegen von T_SECURE im Hilfsvektor für set-user-ID- und set-group-ID-Programme [GH 2031]</span><span class="sxs-lookup"><span data-stu-id="02d0f-762">Set AT_SECURE in auxiliary vector for set-user-ID and set-group-ID programs [GH 2031]</span></span>
- <span data-ttu-id="02d0f-763">Psuedoterminal-Masterendpunkt verarbeitet TIOCPGRP nicht [GH 1063]</span><span class="sxs-lookup"><span data-stu-id="02d0f-763">Psuedo-terminal master endpoint not handling TIOCPGRP [GH 1063]</span></span>
- <span data-ttu-id="02d0f-764">Korrektur des Nichtzurückspulens von Verzeichnissen in LxFs durch lseek [GH 2310]</span><span class="sxs-lookup"><span data-stu-id="02d0f-764">Fix lseek does to rewind directories in LxFs [GH 2310]</span></span>
- <span data-ttu-id="02d0f-765">/dev/ptmx wird nach hoher Auslastung gesperrt [GH 1882]</span><span class="sxs-lookup"><span data-stu-id="02d0f-765">/dev/ptmx locks up after heavy usage [GH 1882]</span></span>
- <span data-ttu-id="02d0f-766">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-766">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-767">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-767">Console</span></span>
- <span data-ttu-id="02d0f-768">Korrektur für horizontale Linien/Unterstriche überall [GH 2168]</span><span class="sxs-lookup"><span data-stu-id="02d0f-768">Fix for horizontal Lines/Underscores Everywhere [GH 2168]</span></span>
- <span data-ttu-id="02d0f-769">Korrektur der Änderung der Prozessreihenfolge, wodurch das Schließen von NPM erschwert wird [GH 2170]</span><span class="sxs-lookup"><span data-stu-id="02d0f-769">Fix for process order changed making NPM harder to close [GH 2170]</span></span>
- <span data-ttu-id="02d0f-770">Hinzufügen des neuen Farbschemas: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span><span class="sxs-lookup"><span data-stu-id="02d0f-770">Added our new color scheme: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-771">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-771">LTP Results:</span></span>
<span data-ttu-id="02d0f-772">Keine Änderung seit 16251</span><span class="sxs-lookup"><span data-stu-id="02d0f-772">No change since 16251</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-773">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-773">Syscall Support</span></span>
<span data-ttu-id="02d0f-774">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-774">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-775">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-775">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`prlimit64`<br/>

### <a name="known-issues"></a><span data-ttu-id="02d0f-776">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="02d0f-776">Known Issues</span></span>
#### <a name="github-issue-2392-windows-folders-not-recognized-by-wsl-httpsgithubcommicrosoftbashonwindowsissues2392"></a><span data-ttu-id="02d0f-777">[GitHub-Issue 2392: Windows-Ordner werden von WSL nicht erkannt (](https://github.com/Microsoft/BashOnWindows/issues/2392))</span><span class="sxs-lookup"><span data-stu-id="02d0f-777">[GitHub Issue 2392: Windows Folders not recognized by WSL ...](https://github.com/Microsoft/BashOnWindows/issues/2392)</span></span>
<span data-ttu-id="02d0f-778">In Build 16257 hat WSL beim Aufzählen von Windows-Dateien/-Ordnern über `/mnt/c/...` Probleme.</span><span class="sxs-lookup"><span data-stu-id="02d0f-778">In build 16257, WSL has issues when enumerating Windows files/folders via `/mnt/c/...`.</span></span>
<span data-ttu-id="02d0f-779">Dieses Problem wurde behoben und sollte im Insider-Builds in der Woche ab dem 14.08.2017 veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-779">This issue has been fixed and should be released in Insiders build during week commencing 8/14/2017.</span></span>

<br/>

## <a name="build-16251"></a><span data-ttu-id="02d0f-780">Build 16251</span><span class="sxs-lookup"><span data-stu-id="02d0f-780">Build 16251</span></span>

<span data-ttu-id="02d0f-781">Allgemeine Windows-Informationen zu Build 16251 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-781">For general Windows information on build 16251 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-782">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-782">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-783">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-783">WSL</span></span>
- <span data-ttu-id="02d0f-784">Entfernen des Beta-Tags aus der optionalen WSL-Komponente. Weitere Informationen finden Sie im [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-784">Remove beta tag from WSL optional component, see [blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) for details.</span></span>
- <span data-ttu-id="02d0f-785">Ordnungsgemäße Initialisierung der saved-set uid und gid für set-user-ID- and set-group-ID-Binärdateien bei der Ausführung [GH 962, 1415, 2072]</span><span class="sxs-lookup"><span data-stu-id="02d0f-785">Correctly initialize saved-set uid and gid for set-user-ID and set-group-ID binaries on exec [GH 962, 1415, 2072]</span></span>
- <span data-ttu-id="02d0f-786">Hinzufügen von Unterstützung für PTRACE_O_TRACEEXIT [GH 555]</span><span class="sxs-lookup"><span data-stu-id="02d0f-786">Added support for ptrace PTRACE_O_TRACEEXIT [GH 555]</span></span>
- <span data-ttu-id="02d0f-787">Hinzufügen von Unterstützung für PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555]</span><span class="sxs-lookup"><span data-stu-id="02d0f-787">Added support for ptrace PTRACE_GETFPREGS and PTRACE_GETREGSET with NT_FPREGSET [GH 555]</span></span>
- <span data-ttu-id="02d0f-788">Korrektur von ptrace, um bei ignorierten Signalen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="02d0f-788">Fixed ptrace to stop on ignored signals</span></span>
- <span data-ttu-id="02d0f-789">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-789">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-790">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-790">Console</span></span>
- <span data-ttu-id="02d0f-791">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-791">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-792">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-792">LTP Results:</span></span>
<span data-ttu-id="02d0f-793">Anzahl bestandener Tests: 768</span><span class="sxs-lookup"><span data-stu-id="02d0f-793">Number of Passing Tests: 768</span></span></br>
<span data-ttu-id="02d0f-794">Anzahl fehlgeschlagener Tests: 244</span><span class="sxs-lookup"><span data-stu-id="02d0f-794">Number of Failing Tests: 244</span></span></br>
<span data-ttu-id="02d0f-795">Anzahl übersprungener Tests: 96</span><span class="sxs-lookup"><span data-stu-id="02d0f-795">Number of Skipped Tests: 96</span></span></br>
[<span data-ttu-id="02d0f-796">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-796">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a><span data-ttu-id="02d0f-797">Build 16241</span><span class="sxs-lookup"><span data-stu-id="02d0f-797">Build 16241</span></span>

<span data-ttu-id="02d0f-798">Allgemeine Windows-Informationen zu Build 16241 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-798">For general Windows information on build 16241 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-799">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-799">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="02d0f-800">WSL</span><span class="sxs-lookup"><span data-stu-id="02d0f-800">WSL</span></span>
- <span data-ttu-id="02d0f-801">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-801">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="02d0f-802">Console</span><span class="sxs-lookup"><span data-stu-id="02d0f-802">Console</span></span>
- <span data-ttu-id="02d0f-803">Korrektur für die Ausgabe des falschen Zeichens für Schnittlinien-DEC, ursprünglich [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/) gemeldet</span><span class="sxs-lookup"><span data-stu-id="02d0f-803">Fix for outputting the wrong character for the crossing-lines DEC, originally reported [here](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span></span>
- <span data-ttu-id="02d0f-804">Korrektur, dass kein Ausgabetext in Codepage 65001 (UTF8) angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="02d0f-804">Fix for no output text being displayed in codepage 65001 (utf8)</span></span>
- <span data-ttu-id="02d0f-805">Übertragen Sie an den RGB-Werten einer Farbe vorgenommene Änderungen nicht an andere Teile der Palette bei Änderungen der Auswahl.</span><span class="sxs-lookup"><span data-stu-id="02d0f-805">Do not transfer changes made to one color's RGB values to other parts of the palette on selection change.</span></span> <span data-ttu-id="02d0f-806">Dadurch wird die Verwendung des Konsoleneigenschaftenblatts erheblich vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-806">This will make the console properties sheet a lot easier to use.</span></span>
- <span data-ttu-id="02d0f-807">STRG+S funktioniert anscheinend nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="02d0f-807">Ctrl+S doesn't appear to work correctly</span></span>
- <span data-ttu-id="02d0f-808">Un-Bold/-Dim fehlt in ANSI-Escapecodes vollständig [GH 2174]</span><span class="sxs-lookup"><span data-stu-id="02d0f-808">Un-Bold/-Dim completely absent from ANSI escape codes [GH 2174]</span></span>
- <span data-ttu-id="02d0f-809">Die Konsole unterstützt VIM-Farbdesigns nicht ordnungsgemäß [GH 1706]</span><span class="sxs-lookup"><span data-stu-id="02d0f-809">Console doesn't correctly support Vim color themes [GH 1706]</span></span>
- <span data-ttu-id="02d0f-810">Bestimmte Zeichen können nicht eingefügt werden [GH 2149]</span><span class="sxs-lookup"><span data-stu-id="02d0f-810">Cannot paste particular characters [GH 2149]</span></span>
- <span data-ttu-id="02d0f-811">Die Größenänderung von dynamischem Umbruch interagiert seltsam mit der Größenänderung eines Bash-Fensters, wenn sich die Inhalte in der Bearbeitungs-/Befehlszeile befinden [GH-Verbindung 1123]</span><span class="sxs-lookup"><span data-stu-id="02d0f-811">Reflow resize interacts strangely with resizing a bash window when stuff is on the edit/command line [GH ConEmu 1123]</span></span>
- <span data-ttu-id="02d0f-812">STRG+L hinterlässt Fragmente auf dem Bildschirm [GH 1978]</span><span class="sxs-lookup"><span data-stu-id="02d0f-812">Ctrl-L leaves the screen dirty [GH 1978]</span></span>
- <span data-ttu-id="02d0f-813">Konsolenrenderingfehler bei der Anzeige von VT für HDPI [GH 1907]</span><span class="sxs-lookup"><span data-stu-id="02d0f-813">Console rendering bug when displaying VT on HDPI [GH 1907]</span></span>
- <span data-ttu-id="02d0f-814">Japanische Zeichen sehen mit dem Unicode-Zeichen U+30FB seltsam aus [GH 2146]</span><span class="sxs-lookup"><span data-stu-id="02d0f-814">Japansese characters look strange with Unicode Character U+30FB [GH 2146]</span></span>
- <span data-ttu-id="02d0f-815">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-815">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16237"></a><span data-ttu-id="02d0f-816">Build 16237</span><span class="sxs-lookup"><span data-stu-id="02d0f-816">Build 16237</span></span>

<span data-ttu-id="02d0f-817">Allgemeine Windows-Informationen zu Build 16237 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-817">For general Windows information on build 16237 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-818">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-818">Fixed</span></span>
- <span data-ttu-id="02d0f-819">Verwenden von Standardattributen für Dateien ohne E/As in lxfs (root, root, 0000)</span><span class="sxs-lookup"><span data-stu-id="02d0f-819">Use default attributes for files without EAs in lxfs (root, root, 0000)</span></span>
- <span data-ttu-id="02d0f-820">Hinzufügen von Unterstützung für Distributionen, die erweiterte Attribute verwenden</span><span class="sxs-lookup"><span data-stu-id="02d0f-820">Added support for distributions that use extended attributes</span></span>
- <span data-ttu-id="02d0f-821">Korrektur des Auffüllens für von getdents und getdents64 zurückgegebene Einträge</span><span class="sxs-lookup"><span data-stu-id="02d0f-821">Fix padding for entries returned by getdents and getdents64</span></span>
- <span data-ttu-id="02d0f-822">Korrektur der Berechtigungsüberprüfung für den SHM_STAT-Systemaufruf [GH 2068]</span><span class="sxs-lookup"><span data-stu-id="02d0f-822">Fix permissions check for the shmctl SHM_STAT system call [GH 2068]</span></span>
- <span data-ttu-id="02d0f-823">Korrektur des falschen anfänglichen epoll-Zustands für ttys [GH 2231]</span><span class="sxs-lookup"><span data-stu-id="02d0f-823">Fixed incorrect initial epoll state for ttys [GH 2231]</span></span>
- <span data-ttu-id="02d0f-824">Korrektur, dass DrvFs readdir nicht alle Einträge zurückgibt [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="02d0f-824">Fix DrvFs readdir not returning all entries [GH 2077]</span></span>
- <span data-ttu-id="02d0f-825">Korrektur von LxFs readdir, wenn Dateien nicht verknüpft sind [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="02d0f-825">Fix LxFs readdir when files are unlinked [GH 2077]</span></span>
- <span data-ttu-id="02d0f-826">Ermöglichen des erneuten Öffnens von nicht verknüpfter drvfs-Dateien über procfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-826">Allow unlinked drvfs files to be reopened through procfs</span></span>
- <span data-ttu-id="02d0f-827">Hinzufügen einer Außerkraftsetzung des globalen Registrierungsschlüssels zum Deaktivieren von WSL-Features (Interop/Laufwerkeinbindung)</span><span class="sxs-lookup"><span data-stu-id="02d0f-827">Added global registry key override for disabling WSL features (interop / drive mounting)</span></span>
- <span data-ttu-id="02d0f-828">Korrektur falscher Blockanzahl in „stat“ für DrvFs (und LxFs) [GH 1894]</span><span class="sxs-lookup"><span data-stu-id="02d0f-828">Fix incorrect block count in "stat" for DrvFs (and LxFs) [GH 1894]</span></span>
- <span data-ttu-id="02d0f-829">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-829">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16232"></a><span data-ttu-id="02d0f-830">Build 16232</span><span class="sxs-lookup"><span data-stu-id="02d0f-830">Build 16232</span></span>

<span data-ttu-id="02d0f-831">Allgemeine Windows-Informationen zu Build 16232 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-831">For general Windows information on build 16232 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-832">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-832">Fixed</span></span>
- <span data-ttu-id="02d0f-833">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-833">No WSL related changes in this release.</span></span>

</br>

## <a name="build-16226"></a><span data-ttu-id="02d0f-834">Build 16226</span><span class="sxs-lookup"><span data-stu-id="02d0f-834">Build 16226</span></span>

<span data-ttu-id="02d0f-835">Allgemeine Windows-Informationen zu Build 16226 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-835">For general Windows information on build 16226 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-836">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-836">Fixed</span></span>
- <span data-ttu-id="02d0f-837">Unterstützung von auf xattr bezogenen Systemaufrufen (getxattr, setxattr, listxattr, removexattr).</span><span class="sxs-lookup"><span data-stu-id="02d0f-837">xattr related syscalls support (getxattr, setxattr, listxattr, removexattr).</span></span>
- <span data-ttu-id="02d0f-838">xattr-Unterstützung für security.capablity.</span><span class="sxs-lookup"><span data-stu-id="02d0f-838">security.capablity xattr support.</span></span>
- <span data-ttu-id="02d0f-839">Verbesserte Kompatibilität mit bestimmten Dateisystemen und Filtern, einschließlich Nicht-MS-SMB-Servern.</span><span class="sxs-lookup"><span data-stu-id="02d0f-839">Improved compatibility with certain file systems and filters, including non-MS SMB servers.</span></span> <span data-ttu-id="02d0f-840">[GH #1952]</span><span class="sxs-lookup"><span data-stu-id="02d0f-840">[GH #1952]</span></span>
- <span data-ttu-id="02d0f-841">Verbesserte Unterstützung für OneDrive-Platzhalter, GVFS-Platzhalter und komprimierte Compact OS-Dateien.</span><span class="sxs-lookup"><span data-stu-id="02d0f-841">Improved support for OneDrive placeholders, GVFS placeholders, and Compact OS compressed files.</span></span>
- <span data-ttu-id="02d0f-842">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-842">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16215"></a><span data-ttu-id="02d0f-843">Build 16215</span><span class="sxs-lookup"><span data-stu-id="02d0f-843">Build 16215</span></span>

<span data-ttu-id="02d0f-844">Allgemeine Windows-Informationen zu Build 16215 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-844">For general Windows information on build 16215 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-845">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-845">Fixed</span></span>
- <span data-ttu-id="02d0f-846">Für WSL ist der Entwicklermodus nicht mehr erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02d0f-846">WSL no longer requires developer mode.</span></span>
- <span data-ttu-id="02d0f-847">Unterstützung von Verzeichnisverbindungen in drvfs.</span><span class="sxs-lookup"><span data-stu-id="02d0f-847">Support directory junctions in drvfs.</span></span>
- <span data-ttu-id="02d0f-848">Verarbeiten der Deinstallation von appx-Paketen der WSL-Distribution.</span><span class="sxs-lookup"><span data-stu-id="02d0f-848">Handle uninstalling of WSL distribution appx packages.</span></span>
- <span data-ttu-id="02d0f-849">Aktualisieren von procfs, um private und freigegebene Zuordnungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-849">Update procfs to show private and shared mappings.</span></span>
- <span data-ttu-id="02d0f-850">Hinzufügen einer Möglichkeit für „wslconfig.exe“ zum Bereinigen von Distributionen, die teilweise installiert oder deinstalliert wurden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-850">Add ability for wslconfig.exe to clean up distributions that are partially installed or uninstalled.</span></span>
- <span data-ttu-id="02d0f-851">Hinzufügen von Unterstützung für IP_MTU_DISCOVER für TCP-Sockets.</span><span class="sxs-lookup"><span data-stu-id="02d0f-851">Added support for IP_MTU_DISCOVER for TCP sockets.</span></span> <span data-ttu-id="02d0f-852">[GH 1639, 2115, 2205]</span><span class="sxs-lookup"><span data-stu-id="02d0f-852">[GH 1639, 2115, 2205]</span></span>
- <span data-ttu-id="02d0f-853">Ableiten der Protokollfamilie für Routen zu AF_INADDR.</span><span class="sxs-lookup"><span data-stu-id="02d0f-853">Infer protocol family for routes to AF_INADDR.</span></span>
- <span data-ttu-id="02d0f-854">Verbesserungen an seriellen Geräten [GH 1929].</span><span class="sxs-lookup"><span data-stu-id="02d0f-854">Serial device improvements [GH 1929].</span></span>

</br>

## <a name="build-16199"></a><span data-ttu-id="02d0f-855">Build 16199</span><span class="sxs-lookup"><span data-stu-id="02d0f-855">Build 16199</span></span>

<span data-ttu-id="02d0f-856">Allgemeine Windows-Informationen zu Build 16199 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-856">For general Windows information on build 16199 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-857">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-857">Fixed</span></span>
- <span data-ttu-id="02d0f-858">In diesen Releases gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-858">No WSL related changes in these releases.</span></span>

</br>

## <a name="build-16193"></a><span data-ttu-id="02d0f-859">Build 16193</span><span class="sxs-lookup"><span data-stu-id="02d0f-859">Build 16193</span></span>

<span data-ttu-id="02d0f-860">Allgemeine Windows-Informationen zu Build 16193 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-860">For general Windows information on build 16193 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-861">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-861">Fixed</span></span>
- <span data-ttu-id="02d0f-862">Racebedingung zwischen dem Senden von SIGCONT und einer Threadgruppe, die beendet wird [GH 1973]</span><span class="sxs-lookup"><span data-stu-id="02d0f-862">Race condition between sending SIGCONT and a threadgroup terminating [GH 1973]</span></span>
- <span data-ttu-id="02d0f-863">Ändern von TTY-und PTY-Geräten zum Melden von FILE_DEVICE_NAMED_PIPE anstelle von FILE_DEVICE_CONSOLE [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="02d0f-863">change tty and pty devices to report FILE_DEVICE_NAMED_PIPE instead of FILE_DEVICE_CONSOLE [GH 1840]</span></span>
- <span data-ttu-id="02d0f-864">SSH-Korrektur für IP_OPTIONS</span><span class="sxs-lookup"><span data-stu-id="02d0f-864">SSH fix for IP_OPTIONS</span></span>
- <span data-ttu-id="02d0f-865">Verschieben der DrvFs-Einbindung in den init-Daemon [GH 1862, 1968, 1767, 1933]</span><span class="sxs-lookup"><span data-stu-id="02d0f-865">Moved DrvFs mounting to init daemon [GH 1862, 1968, 1767, 1933]</span></span>
- <span data-ttu-id="02d0f-866">Hinzufügen von Unterstützung in DrvFs für die folgenden symbolischen NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-866">Added support in DrvFs for following NT symlinks.</span></span>

</br>

## <a name="build-16184"></a><span data-ttu-id="02d0f-867">Build 16184</span><span class="sxs-lookup"><span data-stu-id="02d0f-867">Build 16184</span></span>

<span data-ttu-id="02d0f-868">Allgemeine Windows-Informationen zu Build 16184 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-868">For general Windows information on build 16184 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-869">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-869">Fixed</span></span>
- <span data-ttu-id="02d0f-870">Entfernen des apt-Paketverwaltungstasks (lxrun.exe /update) wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-870">Removed apt package maintenance task (lxrun.exe /update)</span></span>
- <span data-ttu-id="02d0f-871">Korrektur der Nichtanzeige der Ausgabe aus Windows-Prozessen in node.js [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="02d0f-871">Fixed output not showing up in from Windows processes in node.js [GH 1840]</span></span>
- <span data-ttu-id="02d0f-872">Lockern der Ausrichtungsanforderungen in lxcore [GH 1794]</span><span class="sxs-lookup"><span data-stu-id="02d0f-872">Relax alignment requirements in lxcore [GH 1794]</span></span>
- <span data-ttu-id="02d0f-873">Korrektur der Verarbeitung des AT_EMPTY_PATH-Flags in mehreren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-873">Fixed handling of the AT_EMPTY_PATH flag in a numer of system calls.</span></span>
- <span data-ttu-id="02d0f-874">Korrektur eines Problems, bei dem das Löschen von DrvFs-Dateien mit geöffneten Handles bewirkt, dass die Datei nicht definiertes Verhalten aufweist [GH 544, 966, 1357, 1535, 1615]</span><span class="sxs-lookup"><span data-stu-id="02d0f-874">Fixed issue where deleting DrvFs files with open handles will cause the file to exhibit undefined behavior [GH 544,966,1357,1535,1615]</span></span>
- <span data-ttu-id="02d0f-875">„/etc/hosts“ erbt nun Einträge von der Windows-Hostdatei (%windir%\system32\drivers\etc\hosts) [GH 1495]</span><span class="sxs-lookup"><span data-stu-id="02d0f-875">/etc/hosts will now inherit entries from the Windows hosts file (%windir%\system32\drivers\etc\hosts) [GH 1495]</span></span>

</br>

## <a name="build-16179"></a><span data-ttu-id="02d0f-876">Build 16179</span><span class="sxs-lookup"><span data-stu-id="02d0f-876">Build 16179</span></span>

<span data-ttu-id="02d0f-877">Allgemeine Windows-Informationen zu Build 16179 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-877">For general Windows information on build 16179 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-878">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-878">Fixed</span></span>
- <span data-ttu-id="02d0f-879">Keine WSL-Änderungen in dieser Woche.</span><span class="sxs-lookup"><span data-stu-id="02d0f-879">No WSL changes this week.</span></span>

</br>

## <a name="build-16176"></a><span data-ttu-id="02d0f-880">Build 16176</span><span class="sxs-lookup"><span data-stu-id="02d0f-880">Build 16176</span></span>

<span data-ttu-id="02d0f-881">Allgemeine Windows-Informationen zu Build 16176 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-881">For general Windows information on build 16176 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-882">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-882">Fixed</span></span>

- [<span data-ttu-id="02d0f-883">Aktivierte serielle Unterstützung</span><span class="sxs-lookup"><span data-stu-id="02d0f-883">Enabled serial support</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- <span data-ttu-id="02d0f-884">Hinzufügen der IP-Socketoption IP_OPTIONS [GH 1116]</span><span class="sxs-lookup"><span data-stu-id="02d0f-884">Added IP socket option IP_OPTIONS [GH 1116]</span></span>
- <span data-ttu-id="02d0f-885">Implementierung der pwritev-Funktion (beim Hochladen der Datei nach nginx/PHP-FPM) [GH 1506]</span><span class="sxs-lookup"><span data-stu-id="02d0f-885">Implemented pwritev function (while uploading file to nginx/PHP-FPM) [GH 1506]</span></span>
- <span data-ttu-id="02d0f-886">Hinzufügen der IP-Socket-Optionen IP_MULTICAST_IF und IPV6_MULTICAST_IF [GH 990]</span><span class="sxs-lookup"><span data-stu-id="02d0f-886">Added IP socket options IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span></span>
- <span data-ttu-id="02d0f-887">Unterstützung für Socketoption IP_MULTICAST_LOOP und IPV6_MULTICAST_LOOP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="02d0f-887">Support for socket option IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span></span>
- <span data-ttu-id="02d0f-888">Hinzufügen von IP(V6)_MTU-Socketoption für den Knoten apps, traceroute, dig, nslookup, host</span><span class="sxs-lookup"><span data-stu-id="02d0f-888">Added IP(V6)_MTU socket option for apps node, traceroute, dig, nslookup, host</span></span>
- <span data-ttu-id="02d0f-889">Hinzufügen der IP-Socketoption IPV6_UNICAST_HOPS</span><span class="sxs-lookup"><span data-stu-id="02d0f-889">Added IP socket option IPV6_UNICAST_HOPS</span></span>
- [<span data-ttu-id="02d0f-890">Verbesserungen des Dateisystems</span><span class="sxs-lookup"><span data-stu-id="02d0f-890">Filesystem Improvements</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * <span data-ttu-id="02d0f-891">Ermöglichen der Einbindung von UNC-Pfaden</span><span class="sxs-lookup"><span data-stu-id="02d0f-891">Allow mounting of UNC paths</span></span>
    * <span data-ttu-id="02d0f-892">Ermöglichen von CDFS-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-892">Enable CDFS support in drvfs</span></span>
    * <span data-ttu-id="02d0f-893">Ordnungsgemäße Verarbeitung von Berechtigungen für Netzwerkdateisysteme in drvfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-893">Correctly handle permissions for network file systems in drvfs</span></span>
    * <span data-ttu-id="02d0f-894">Hinzufügen von Unterstützung für Remotelaufwerke zu drvfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-894">Add support for remote drives to drvfs</span></span>
    * <span data-ttu-id="02d0f-895">Ermöglichen von FAT-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-895">Enable FAT support in drvfs</span></span>
- <span data-ttu-id="02d0f-896">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-896">Additional fixes and Improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-897">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="02d0f-897">LTP Results</span></span>
<span data-ttu-id="02d0f-898">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="02d0f-898">No changes since 15042</span></span>

</br>

## <a name="build-16170"></a><span data-ttu-id="02d0f-899">Build 16170</span><span class="sxs-lookup"><span data-stu-id="02d0f-899">Build 16170</span></span>

<span data-ttu-id="02d0f-900">Allgemeine Windows-Informationen zu Build 16170 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-900">For general Windows information on build 16170 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span></span><br/>

<span data-ttu-id="02d0f-901">Wir haben einen neuen [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) veröffentlicht, in dem unsere Anstrengungen beim Testen von WSL erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-901">We released a new [blog post](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) discussing our efforts to test WSL.</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-902">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-902">Fixed</span></span>

- <span data-ttu-id="02d0f-903">Unterstützung für Socketoption IP_ADD_MEMBERSHIP und IPV6_ADD_MEMBERSHIP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="02d0f-903">Support socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span></span>
- <span data-ttu-id="02d0f-904">Hinzufügen von Unterstützung für PTRACE_OLDSETOPTIONS.</span><span class="sxs-lookup"><span data-stu-id="02d0f-904">Add support for PTRACE_OLDSETOPTIONS.</span></span> <span data-ttu-id="02d0f-905">[GH 1692]</span><span class="sxs-lookup"><span data-stu-id="02d0f-905">[GH 1692]</span></span>
- <span data-ttu-id="02d0f-906">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-906">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-907">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="02d0f-907">LTP Results</span></span>
<span data-ttu-id="02d0f-908">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="02d0f-908">No changes since 15042</span></span>

</br>

## <a name="build-15046-to-windows-10-creators-update"></a><span data-ttu-id="02d0f-909">Build 15046 für Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="02d0f-909">Build 15046 to Windows 10 Creators Update</span></span>
<span data-ttu-id="02d0f-910">Es gibt keine weiteren WSL-Korrekturen oder-Funktionen, die für die Einbindung in das Creators Update in Windows 10 geplant sind.</span><span class="sxs-lookup"><span data-stu-id="02d0f-910">There are no more WSL fixes or features planned for inclusion in the Creators Update to Windows 10.</span></span> <span data-ttu-id="02d0f-911">Die Anmerkungen zu dieser Version von WSL werden in den kommenden Wochen fortgesetzt, um Ergänzungen für das nächste Hauptupdate von Windows aufzuführen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-911">Release notes for WSL will resume in the coming weeks for additions targeting the next major Windows Update.</span></span> <span data-ttu-id="02d0f-912">Allgemeine Windows-Informationen zu Build 15046 und zukünftigen Insider Releases finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-912">For general Windows information on build 15046 and future Insider releases visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span></span> <br/><br/>
 <br/>

## <a name="build-15042"></a><span data-ttu-id="02d0f-913">Build 15042</span><span class="sxs-lookup"><span data-stu-id="02d0f-913">Build 15042</span></span>

<span data-ttu-id="02d0f-914">Allgemeine Windows-Informationen zu Build 15042 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-914">For general Windows information on build 15042 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-915">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-915">Fixed</span></span>

- <span data-ttu-id="02d0f-916">Korrektur eines Deadlocks beim Entfernen eines Pfades, der auf „..“ endet</span><span class="sxs-lookup"><span data-stu-id="02d0f-916">Fix for a deadlock when removing a path ending in ".."</span></span>
- <span data-ttu-id="02d0f-917">Korrektur eines Problems, bei dem FIONBIO bei Erfolg 0 zurückgibt [GH 1683]</span><span class="sxs-lookup"><span data-stu-id="02d0f-917">Fixed an issue where FIONBIO not returning 0 on success [GH 1683]</span></span>
- <span data-ttu-id="02d0f-918">Korrektur eines Problems bei Lesevorgängen mit einer Länge von Null von Internetdatagrammsockets</span><span class="sxs-lookup"><span data-stu-id="02d0f-918">Fixed issue with zero-length reads of inet datagram sockets</span></span>
- <span data-ttu-id="02d0f-919">Korrektur eines möglichen Deadlocks aufgrund einer Racebedingung bei der drvfs inode-Suche [GH 1675]</span><span class="sxs-lookup"><span data-stu-id="02d0f-919">Fix possible deadlock due to race condition in drvfs inode lookup [GH 1675]</span></span>
- <span data-ttu-id="02d0f-920">Erweiterte Unterstützung für Hilfsdaten von Unix-Sockets, SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613, 1326]</span><span class="sxs-lookup"><span data-stu-id="02d0f-920">Extended support for unix socket ancillary data; SCM_CREDENTIALS and SCM_RIGHTS [GH 514, 613, 1326]</span></span>
- <span data-ttu-id="02d0f-921">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-921">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-922">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-922">LTP Results:</span></span>
<span data-ttu-id="02d0f-923">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="02d0f-923">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="02d0f-924">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="02d0f-924">Number of non-Passing (failing, skipped, etc…): 255</span></span>

</br>

## <a name="build-15031"></a><span data-ttu-id="02d0f-925">Build 15031</span><span class="sxs-lookup"><span data-stu-id="02d0f-925">Build 15031</span></span>

<span data-ttu-id="02d0f-926">Allgemeine Windows-Informationen zu Build 15031 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-926">For general Windows information on build 15031 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-927">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-927">Fixed</span></span>

- <span data-ttu-id="02d0f-928">Korrektur eines Fehlers, bei dem sich time(2) sporadisch falsch verhielt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-928">Fixed a bug where time(2) would sporadically misbehave.</span></span>
- <span data-ttu-id="02d0f-929">Korrektur eines Problems, bei dem \*SIGPROCMASK-Systemaufrufe die Signalmaske beschädigen konnten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-929">Fixed and issue where \*SIGPROCMASK syscalls could corrupt signal mask.</span></span>
- <span data-ttu-id="02d0f-930">Jetzt Rückgabe der vollständigen Länge der Befehlszeile in WSL-Benachrichtigung zur Prozesserstellung.</span><span class="sxs-lookup"><span data-stu-id="02d0f-930">Now return full command line length in WSL process creation notification.</span></span> <span data-ttu-id="02d0f-931">[GH 1632]</span><span class="sxs-lookup"><span data-stu-id="02d0f-931">[GH 1632]</span></span>
- <span data-ttu-id="02d0f-932">WSL meldet jetzt die Threadbeendigung über ptrace für GDB-Hänger.</span><span class="sxs-lookup"><span data-stu-id="02d0f-932">WSL now reports thread exit through ptrace for GDB hangs.</span></span> <span data-ttu-id="02d0f-933">[GH 1196]</span><span class="sxs-lookup"><span data-stu-id="02d0f-933">[GH 1196]</span></span>
- <span data-ttu-id="02d0f-934">Korrektur eines Fehlers, bei dem ptys nach hoher tmux-E/A nicht mehr reagiert</span><span class="sxs-lookup"><span data-stu-id="02d0f-934">Fixed bug where ptys would hang after heavy tmux IO.</span></span> <span data-ttu-id="02d0f-935">[GH 1358]</span><span class="sxs-lookup"><span data-stu-id="02d0f-935">[GH 1358]</span></span>
- <span data-ttu-id="02d0f-936">Korrektur der Timeoutüberprüfung in zahlreichen Systemaufrufen (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span><span class="sxs-lookup"><span data-stu-id="02d0f-936">Fixed timeout validation in many system calls (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span></span>
- <span data-ttu-id="02d0f-937">Hinzufügen von eventfd EFD_SEMAPHORE-Unterstützung [GH 452]</span><span class="sxs-lookup"><span data-stu-id="02d0f-937">Added eventfd EFD_SEMAPHORE support [GH 452]</span></span>
- <span data-ttu-id="02d0f-938">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-938">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-939">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-939">LTP Results:</span></span>
<span data-ttu-id="02d0f-940">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="02d0f-940">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="02d0f-941">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="02d0f-941">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="02d0f-942">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-942">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a><span data-ttu-id="02d0f-943">Build 15025</span><span class="sxs-lookup"><span data-stu-id="02d0f-943">Build 15025</span></span>

<span data-ttu-id="02d0f-944">Allgemeine Windows-Informationen zu Build 15025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-944">For general Windows information on build 15025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-945">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-945">Fixed</span></span>

- <span data-ttu-id="02d0f-946">Korrektur eines Fehlers, bei dem grep 2.27 nicht mehr funktioniert [GH 1578]</span><span class="sxs-lookup"><span data-stu-id="02d0f-946">Fix for bug that broke grep 2.27 [GH 1578]</span></span>
- <span data-ttu-id="02d0f-947">Implementierung des EFD_SEMAPHORE-Flags für den eventfd2-Systemaufruf [GH 452]</span><span class="sxs-lookup"><span data-stu-id="02d0f-947">Implemented EFD_SEMAPHORE flag for eventfd2 syscall [GH 452]</span></span>
- <span data-ttu-id="02d0f-948">Implementierung von /proc/[pid]/net/ipv6_route [GH 1608]</span><span class="sxs-lookup"><span data-stu-id="02d0f-948">Implemented /proc/[pid]/net/ipv6_route [GH 1608]</span></span>
- <span data-ttu-id="02d0f-949">Signalgestützte E/A-Unterstützung für Unix-Streamsockets [GH 393, 68]</span><span class="sxs-lookup"><span data-stu-id="02d0f-949">Signal driven IO support for unix stream sockets [GH 393, 68]</span></span>
- <span data-ttu-id="02d0f-950">Unterstützung für F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]</span><span class="sxs-lookup"><span data-stu-id="02d0f-950">Support F_GETPIPE_SZ and F_SETPIPE_SZ [GH 1012]</span></span>
- <span data-ttu-id="02d0f-951">Implementierung des recvmmsg()-Systemaufrufs [GH 1531]</span><span class="sxs-lookup"><span data-stu-id="02d0f-951">Implement recvmmsg() syscall [GH 1531]</span></span>
- <span data-ttu-id="02d0f-952">Korrektur eines Fehlers, bei dem epoll_wait() nicht gewartet hat [GH 1609]</span><span class="sxs-lookup"><span data-stu-id="02d0f-952">Fixed bug where epoll_wait() wasn't waiting [GH 1609]</span></span>
- <span data-ttu-id="02d0f-953">Implementierung von /proc/version_signature</span><span class="sxs-lookup"><span data-stu-id="02d0f-953">Implement /proc/version_signature</span></span>
- <span data-ttu-id="02d0f-954">Tee-Systemaufruf gibt jetzt einen Fehler zurück, wenn beide Dateideskriptoren auf dieselbe Pipe verweisen</span><span class="sxs-lookup"><span data-stu-id="02d0f-954">Tee syscall now returns failure if both file descriptors refer to the same pipe</span></span>
- <span data-ttu-id="02d0f-955">Implementierung des richtigen Verhaltens für SO_PEERCRED für Unix-Sockets</span><span class="sxs-lookup"><span data-stu-id="02d0f-955">Implemented correct behavior for SO_PEERCRED for Unix sockets</span></span>
- <span data-ttu-id="02d0f-956">Korrektur der Verarbeitung ungültiger Parameter des tkill-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="02d0f-956">Fixed tkill syscall invalid parameter handling</span></span>
- <span data-ttu-id="02d0f-957">Änderungen zum Verbessern der Leistung von drvfs</span><span class="sxs-lookup"><span data-stu-id="02d0f-957">Changes to increase the preformace of drvfs</span></span>
- <span data-ttu-id="02d0f-958">Kleinere Korrektur für Ruby-E/A-Blockierung</span><span class="sxs-lookup"><span data-stu-id="02d0f-958">Minor fix for Ruby IO blocking</span></span>
- <span data-ttu-id="02d0f-959">Korrektur von recvmsg() beim Zurückgeben von EINVAL für das MSG_DONTWAIT-Flag für Inet-Sockets [GH 1296]</span><span class="sxs-lookup"><span data-stu-id="02d0f-959">Fixed recvmsg() returning EINVAL for the MSG_DONTWAIT flag for inet sockets [GH 1296]</span></span>
- <span data-ttu-id="02d0f-960">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-960">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-961">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-961">LTP Results:</span></span>
<span data-ttu-id="02d0f-962">Anzahl bestandener Tests: 732</span><span class="sxs-lookup"><span data-stu-id="02d0f-962">Number of Passing Test: 732</span></span></br>
<span data-ttu-id="02d0f-963">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="02d0f-963">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="02d0f-964">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-964">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a><span data-ttu-id="02d0f-965">Build 15019</span><span class="sxs-lookup"><span data-stu-id="02d0f-965">Build 15019</span></span>

<span data-ttu-id="02d0f-966">Allgemeine Windows-Informationen zu Build 15019 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-966">For general Windows information on build 15019 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-967">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-967">Fixed</span></span>

- <span data-ttu-id="02d0f-968">Korrektur eines Fehlers, der fälschlicherweise die CPU-Auslastung in procfs für Tools wie htop gemeldet hat [GH 823, 945, 971]</span><span class="sxs-lookup"><span data-stu-id="02d0f-968">Fixed bug that incorrectly reported CPU usage in procfs for tools like htop (GH 823, 945, 971)</span></span>
- <span data-ttu-id="02d0f-969">Beim Aufrufen von open() mit O_TRUNC für eine vorhandene Datei „inotify“ wird nun IN_MODIFY vor IN_OPEN generiert</span><span class="sxs-lookup"><span data-stu-id="02d0f-969">When calling open() with O_TRUNC on an existing file inotify now generates IN_MODIFY before IN_OPEN</span></span>
- <span data-ttu-id="02d0f-970">Korrekturen für den Unix-Socket getsockopt SO_ERROR zum Aktivieren von Postgress [GH 61, 1354]</span><span class="sxs-lookup"><span data-stu-id="02d0f-970">Fixes to unix socket getsockopt SO_ERROR to enable postgress [GH 61, 1354]</span></span>
- <span data-ttu-id="02d0f-971">Implementierung von /proc/sys/net/core/somaxconn für die Sprache GO</span><span class="sxs-lookup"><span data-stu-id="02d0f-971">Implement /proc/sys/net/core/somaxconn for the GO language</span></span>
- <span data-ttu-id="02d0f-972">Der Apt-get-Packageupdate-Hintergrundtask wird jetzt aus der Ansicht ausgeblendet</span><span class="sxs-lookup"><span data-stu-id="02d0f-972">Apt-get package update background task now runs hidden from view</span></span>
- <span data-ttu-id="02d0f-973">Löschen des Bereichs für ipv6 localhost (Fehler Spring-Framework (Java)).</span><span class="sxs-lookup"><span data-stu-id="02d0f-973">Clear scope for ipv6 localhost (Spring-Framework(Java) failure).</span></span>
- <span data-ttu-id="02d0f-974">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-974">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-975">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-975">LTP Results:</span></span>
<span data-ttu-id="02d0f-976">Anzahl bestandener Tests: 714</span><span class="sxs-lookup"><span data-stu-id="02d0f-976">Number of Passing Test: 714</span></span> </br>
<span data-ttu-id="02d0f-977">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 249</span><span class="sxs-lookup"><span data-stu-id="02d0f-977">Number of non-Passing (failing, skipped, etc…): 249</span></span> </br>
[<span data-ttu-id="02d0f-978">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-978">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a><span data-ttu-id="02d0f-979">Build 15014</span><span class="sxs-lookup"><span data-stu-id="02d0f-979">Build 15014</span></span>

<span data-ttu-id="02d0f-980">Allgemeine Windows-Informationen zu Build 15014 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="02d0f-980">For general Windows information on build 15014 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-981">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-981">Fixed</span></span>

- <span data-ttu-id="02d0f-982">STRG+C funktioniert nun wie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="02d0f-982">Ctrl+C now works as intended</span></span>
- <span data-ttu-id="02d0f-983">htop und ps auxw zeigen jetzt die richtige Ressourcenverwendung an (GH #516)</span><span class="sxs-lookup"><span data-stu-id="02d0f-983">htop and ps auxw now show correct resource utilization (GH #516)</span></span>
- <span data-ttu-id="02d0f-984">Grundlegende Übersetzung von NT-Ausnahmen in Signale.</span><span class="sxs-lookup"><span data-stu-id="02d0f-984">Basic translation of NT exceptions to signals.</span></span> <span data-ttu-id="02d0f-985">(GH #513)</span><span class="sxs-lookup"><span data-stu-id="02d0f-985">(GH #513)</span></span>
- <span data-ttu-id="02d0f-986">fallocate schlägt nun mit ENOSPC anstatt mit EINVAL fehl, wenn nicht genügend Speicherplatz verfügbar ist (GH #1571)</span><span class="sxs-lookup"><span data-stu-id="02d0f-986">fallocate now fails with ENOSPC  when running out of space instead of EINVAL (GH #1571)</span></span>
- <span data-ttu-id="02d0f-987">Hinzufügen von /proc/sys/kernel/sem.</span><span class="sxs-lookup"><span data-stu-id="02d0f-987">Added /proc/sys/kernel/sem.</span></span>
- <span data-ttu-id="02d0f-988">Implementierung der semop- und semtimedop-Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="02d0f-988">Implemented semop and semtimedop system calls</span></span>
- <span data-ttu-id="02d0f-989">Korrektur von nslookup-Fehlern mit der IP_RECVTOS- und IPV6_RECVTCLASS-Socketoption (GH 69)</span><span class="sxs-lookup"><span data-stu-id="02d0f-989">Fixed nslookup errors with IP_RECVTOS & IPV6_RECVTCLASS socket option (GH 69)</span></span>
- <span data-ttu-id="02d0f-990">Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT</span><span class="sxs-lookup"><span data-stu-id="02d0f-990">Support for socket options IP_RECVTTL and IPV6_RECVHOPLIMIT</span></span>
- <span data-ttu-id="02d0f-991">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-991">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-992">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-992">LTP Results:</span></span>
<span data-ttu-id="02d0f-993">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="02d0f-993">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="02d0f-994">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="02d0f-994">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="02d0f-995">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-995">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a><span data-ttu-id="02d0f-996">Zusammenfassung der Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="02d0f-996">Syscall Summary</span></span>
<span data-ttu-id="02d0f-997">Systemaufrufe gesamt: 384</span><span class="sxs-lookup"><span data-stu-id="02d0f-997">Total Syscalls: 384</span></span> </br>
<span data-ttu-id="02d0f-998">Implementiert gesamt: 235</span><span class="sxs-lookup"><span data-stu-id="02d0f-998">Total Implemented: 235</span></span> </br>
<span data-ttu-id="02d0f-999">Mit Stub versehen gesamt: 22</span><span class="sxs-lookup"><span data-stu-id="02d0f-999">Total Stubbed: 22</span></span> </br>
<span data-ttu-id="02d0f-1000">Nicht implementiert gesamt: 127</span><span class="sxs-lookup"><span data-stu-id="02d0f-1000">Total Unimplemented: 127</span></span> </br>
[<span data-ttu-id="02d0f-1001">Ausführliche Aufschlüsselung</span><span class="sxs-lookup"><span data-stu-id="02d0f-1001">Detailed Breakdown</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a><span data-ttu-id="02d0f-1002">Build 15007</span><span class="sxs-lookup"><span data-stu-id="02d0f-1002">Build 15007</span></span>

<span data-ttu-id="02d0f-1003">Allgemeine Windows-Informationen zu Build 15007 finden Sie im [Windows-Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1003">For general Windows information on build 15007 visit the [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="02d0f-1004">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="02d0f-1004">Known Issue</span></span>

- <span data-ttu-id="02d0f-1005">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1005">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="02d0f-1006">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1006">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="02d0f-1007">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1007">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="02d0f-1008">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1008">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="02d0f-1009">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1009">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="02d0f-1010">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1010">Users can explore the option to include this in their `.bashrc`</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-1011">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1011">Fixed</span></span>

- <span data-ttu-id="02d0f-1012">Korrektur eines Problems, bei dem die Ausführung von WSL 100 % eines CPU-Kerns verbraucht</span><span class="sxs-lookup"><span data-stu-id="02d0f-1012">Corrected the issue where running WSL would consume 100% of a CPU core</span></span>
- <span data-ttu-id="02d0f-1013">Socketoption IP_PKTINFO, IPV6_RECVPKTINFO wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1013">Socket option IP_PKTINFO, IPV6_RECVPKTINFO now supported.</span></span> <span data-ttu-id="02d0f-1014">(GH #851, 987)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1014">(GH #851, 987)</span></span>
- <span data-ttu-id="02d0f-1015">Abschneiden der physischen Adresse der Netzwerkschnittstelle auf 16 Bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1015">Truncate network interface physical address to 16 bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span></span>
- <span data-ttu-id="02d0f-1016">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1016">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1017">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1017">LTP Results:</span></span>
<span data-ttu-id="02d0f-1018">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="02d0f-1018">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="02d0f-1019">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="02d0f-1019">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="02d0f-1020">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1020">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a><span data-ttu-id="02d0f-1021">Build 15002</span><span class="sxs-lookup"><span data-stu-id="02d0f-1021">Build 15002</span></span>

<span data-ttu-id="02d0f-1022">Allgemeine Windows-Informationen zu Build 15002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1022">For general Windows information on build 15002 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="02d0f-1023">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="02d0f-1023">Known Issue</span></span>

<span data-ttu-id="02d0f-1024">Zwei bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1024">Two known issues:</span></span>
- <span data-ttu-id="02d0f-1025">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1025">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="02d0f-1026">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1026">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="02d0f-1027">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1027">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="02d0f-1028">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1028">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="02d0f-1029">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1029">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="02d0f-1030">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1030">Users can explore the option to include this in their `.bashrc`</span></span>

- <span data-ttu-id="02d0f-1031">Während der Ausführung von WSL werden von einem Systemthread 100 % eines CPU-Kerns beansprucht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1031">While WSL is running a system thread will consume 100% of a CPU core.</span></span>  <span data-ttu-id="02d0f-1032">Die Ursache wurde untersucht und intern behoben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1032">The root cause has been addressed and fixed internally.</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-1033">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1033">Fixed</span></span>

- <span data-ttu-id="02d0f-1034">Alle Bash-Sitzungen müssen jetzt auf derselben Berechtigungsebene erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1034">All bash sessions must now be created at the same permission level.</span></span>  <span data-ttu-id="02d0f-1035">Der Versuch, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1035">Attempting to start a session at a different level will be blocked.</span></span>  <span data-ttu-id="02d0f-1036">Dies bedeutet, dass Administrator-und Nicht-Administratorkonsolen nicht gleichzeitig ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1036">This means admin and non-admin consoles cannot run at the same time.</span></span> <span data-ttu-id="02d0f-1037">(GH #626)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1037">(GH #626)</span></span>
<br/>
- <span data-ttu-id="02d0f-1038">Implementierung der folgenden NETLINK_ROUTE-Meldungen (erfordert Windows-Administrator)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1038">Implemented the following NETLINK_ROUTE messages (requires Windows admin)</span></span>
     - <span data-ttu-id="02d0f-1039">RTM_NEWADDR (unterstützt `ip addr add`)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1039">RTM_NEWADDR (supports `ip addr add`)</span></span>
     - <span data-ttu-id="02d0f-1040">RTM_NEWROUTE (unterstützt `ip route add`)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1040">RTM_NEWROUTE (supports `ip route add`)</span></span>
     - <span data-ttu-id="02d0f-1041">RTM_DELADDR (unterstützt `ip addr del`)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1041">RTM_DELADDR (supports `ip addr del`)</span></span>
     - <span data-ttu-id="02d0f-1042">RTM_DELROUTE (unterstützt `ip route del`)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1042">RTM_DELROUTE (supports `ip route del`)</span></span>
- <span data-ttu-id="02d0f-1043">Die geplante Tasküberprüfung für zu aktualisierende Pakete wird nicht mehr über eine getaktete Verbindung ausgeführt (GH #1371)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1043">Scheduled task checking for packages to update will no longer run on a metered connection (GH #1371)</span></span>
- <span data-ttu-id="02d0f-1044">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1044">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="02d0f-1045">Implementierung der TCP_KEEPCNT-Socketoption (GH #843)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1045">Implemented TCP_KEEPCNT socket option (GH #843)</span></span>
- <span data-ttu-id="02d0f-1046">Implementierung der IP_MTU_DISCOVER INET-Socketoption (GH #720, 717, 170, 69)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1046">Implemented IP_MTU_DISCOVER INET socket option (GH #720, 717, 170, 69)</span></span>
- <span data-ttu-id="02d0f-1047">Entfernen der Legacyfnktionalität zum Ausführen von NT-Binärdateien aus init mit NT-Pfadsuche.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1047">Removed legacy functionality to run NT binaries from init with NT path lookup.</span></span> <span data-ttu-id="02d0f-1048">(GH #1325)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1048">(GH #1325)</span></span>
- <span data-ttu-id="02d0f-1049">Korrektur des Modus von /dev/kmsg zum Zulassen von Gruppen-/sonstigem Lesezugriff (0644) (GH #1321)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1049">Fix mode of /dev/kmsg to allow group / other read access (0644) (GH #1321)</span></span>
- <span data-ttu-id="02d0f-1050">Implementierung von /proc/sys/kernel/random/uuid (GH #1092)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1050">Implemented /proc/sys/kernel/random/uuid  (GH #1092)</span></span>
- <span data-ttu-id="02d0f-1051">Korrektur eines Fehlers, bei dem die Startzeit des Prozesses als Jahr 2432 angezeigt wurde (GH #974)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1051">Corrected error where process start time was showing as year 2432 (GH #974)</span></span>
- <span data-ttu-id="02d0f-1052">Wechseln der TERM-Standardumgebungsvariablen in xterm-256color (GH #1446)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1052">Switched default TERM environment variable to xterm-256color (GH #1446)</span></span>
- <span data-ttu-id="02d0f-1053">Änderung der Art und Weise, in der der Prozesscommit während des Prozessforks berechnet wird.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1053">Modified the way that process commit is calculated during process fork.</span></span> <span data-ttu-id="02d0f-1054">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1054">(GH #1286)</span></span>
- <span data-ttu-id="02d0f-1055">Implementierung von /proc/sys/vm/overcommit_memory.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1055">Implemented /proc/sys/vm/overcommit_memory.</span></span> <span data-ttu-id="02d0f-1056">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1056">(GH #1286)</span></span>
- <span data-ttu-id="02d0f-1057">Implementierung der /proc/net/route-Datei (GH #69)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1057">Implemented /proc/net/route file (GH #69)</span></span>
- <span data-ttu-id="02d0f-1058">Korrektur eines Fehlers, bei dem der Verknüpfungsname falsch lokalisiert wurde (GH #696)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1058">Fixed error where shortcut name was incorrectly localized (GH #696)</span></span>
- <span data-ttu-id="02d0f-1059">Korrektur der fehlerhaften ELF-Verarbeitungslogik, die die Programmheader nicht ordnungsgemäß so überprüft, dass sie kleiner als (oder gleich) PATH_MAX sein müssen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1059">Fixed elf parsing logic that is incorrectly validating the program headers must be less than (or equal to) PATH_MAX.</span></span> <span data-ttu-id="02d0f-1060">(GH #1048)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1060">(GH #1048)</span></span>
- <span data-ttu-id="02d0f-1061">Implementierung des statfs-Rückrufs für procfs, sysfs, cgroupfs und binfmts (GH #1378)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1061">Implemented statfs callback for procfs, sysfs, cgroupfs, and binfmtfs (GH #1378)</span></span>
- <span data-ttu-id="02d0f-1062">Korrektur der AptPackageIndexUpdate-Fenster, die nicht geschlossen werden (GH #1184, auch in GH #1193 beschrieben)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1062">Fixed AptPackageIndexUpdate windows that won’t close (GH #1184, also discussed in GH #1193)</span></span>
- <span data-ttu-id="02d0f-1063">Hinzufügen von ASLR-Personality, ADDR_NO_RANDOMIZE-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1063">Added ASLR personality  ADDR_NO_RANDOMIZE support.</span></span> <span data-ttu-id="02d0f-1064">[GH #1148, 1128]</span><span class="sxs-lookup"><span data-stu-id="02d0f-1064">(GH #1148, 1128)</span></span>
- <span data-ttu-id="02d0f-1065">Verbesserung von PTRACE_GETSIGINFO, SIGSEGV für ordnungsgemäße gdb-Stapelüberwachungen während AV (GH #875)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1065">Improved PTRACE_GETSIGINFO, SIGSEGV, for proper gdb stack traces during AV (GH #875)</span></span>
- <span data-ttu-id="02d0f-1066">Elf-Verarbeitung schlägt für patchelf-Binärdateien nicht mehr fehl.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1066">Elf parsing no longer fails for patchelf binaries.</span></span> <span data-ttu-id="02d0f-1067">[GH #471]</span><span class="sxs-lookup"><span data-stu-id="02d0f-1067">(GH #471)</span></span>
- <span data-ttu-id="02d0f-1068">VPN DNS-Weitergabe an /etc/resolv.conf (GH #416, 1350)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1068">VPN DNS propagated to /etc/resolv.conf (GH #416, 1350)</span></span>
- <span data-ttu-id="02d0f-1069">Verbesserungen an TCP Close für eine zuverlässigere Datenübertragung.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1069">Improvements to TCP close for more reliable data transfer.</span></span> <span data-ttu-id="02d0f-1070">(GH #610, 616, 1025, 1335)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1070">(GH #610, 616, 1025, 1335)</span></span>
- <span data-ttu-id="02d0f-1071">Jetzt Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden (EMFILE).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1071">Now return correct error code when too many files are opened (EMFILE).</span></span> <span data-ttu-id="02d0f-1072">(GH #1126, 2090)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1072">(GH #1126, 2090)</span></span>
- <span data-ttu-id="02d0f-1073">Windows-Überwachungsprotokoll erfasst jetzt den Imagenamen in Process Create Audit.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1073">Windows Audit log now reports the image name in process create audit.</span></span>
- <span data-ttu-id="02d0f-1074">Jetzt normaler Fehler beim Starten von „bash.exe“ in einem Bash-Fenster.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1074">Now gracefully fail when launching bash.exe from within a bash window</span></span>
- <span data-ttu-id="02d0f-1075">Hinzufügen einer Fehlermeldung, wenn Interop nicht auf ein Arbeitsverzeichnis unter LxFs zugreifen kann (z.B. BASHRC-Datei von „notepad.exe“).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1075">Added error message when interop is unable to access a working directory under LxFs (i.e. notepad.exe .bashrc)</span></span>
- <span data-ttu-id="02d0f-1076">Korrektur eines Problems, bei dem der Windows-Pfad in WSL abgeschnitten wurde</span><span class="sxs-lookup"><span data-stu-id="02d0f-1076">Fixed issue where Windows path was truncated in WSL</span></span>
- <span data-ttu-id="02d0f-1077">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1077">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1078">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1078">LTP Results:</span></span>
<span data-ttu-id="02d0f-1079">Anzahl bestandener Tests: 690</span><span class="sxs-lookup"><span data-stu-id="02d0f-1079">Number of Passing Test: 690</span></span> </br>
<span data-ttu-id="02d0f-1080">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 274</span><span class="sxs-lookup"><span data-stu-id="02d0f-1080">Number of non-Passing (failing, skipped, etc…): 274</span></span> </br>
[<span data-ttu-id="02d0f-1081">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1081">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1082">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1082">Syscall Support</span></span>
<span data-ttu-id="02d0f-1083">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1083">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1084">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1084">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a><span data-ttu-id="02d0f-1085">Build 14986</span><span class="sxs-lookup"><span data-stu-id="02d0f-1085">Build 14986</span></span>

<span data-ttu-id="02d0f-1086">Allgemeine Windows-Informationen zu Build 14986 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1086">For general Windows information on build 14986 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1087">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1087">Fixed</span></span>

- <span data-ttu-id="02d0f-1088">Korrektur von Fehlerüberprüfungen mit Netlink und Pty IOCTLs</span><span class="sxs-lookup"><span data-stu-id="02d0f-1088">Fixed bugchecks with Netlink and Pty IOCTLs</span></span>
- <span data-ttu-id="02d0f-1089">Kernel Version meldet nun 4.4.0-43 aus Gründen der Konsistenz mit Xenial</span><span class="sxs-lookup"><span data-stu-id="02d0f-1089">Kernel version now reports 4.4.0-43 for consistency with Xenial</span></span>
- <span data-ttu-id="02d0f-1090">„Bash.exe“ wird jetzt gestartet, wenn die Eingabe an „nul:“ gerichtet ist (GH #1259)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1090">Bash.exe now launches when input directed to 'nul:' (GH #1259)</span></span>
- <span data-ttu-id="02d0f-1091">Thread-IDs werden nun ordnungsgemäß in procfs erfasst (GH #967)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1091">Thread IDs now reported correctly in procfs (GH #967)</span></span>
- <span data-ttu-id="02d0f-1092">Flags IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR werden jetzt in inotify_add_watch() unterstützt (GH #1280)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1092">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR flags now supported in inotify_add_watch() (GH #1280)</span></span>
- <span data-ttu-id="02d0f-1093">Implementierung von timer_create und verwandten Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1093">Implement timer_create and related system calls.</span></span>  <span data-ttu-id="02d0f-1094">Dies ermöglicht die GHC-Unterstützung (GH #307).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1094">This enables GHC support (GH #307)</span></span>
- <span data-ttu-id="02d0f-1095">Korrektur eines Problems, bei dem Ping eine Zeitangabe von 0,000 ms zurückgab (GH #1296)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1095">Fixed issue where ping returned a time of 0.000ms (GH #1296)</span></span>
- <span data-ttu-id="02d0f-1096">Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1096">Return correct error code when too many files are opened.</span></span>
- <span data-ttu-id="02d0f-1097">Korrektur eines Problems in WSL, bei dem die Netlink-Anforderung für Netzwerkschnittstellendaten mit EINVAL fehlschlägt, wenn die Hardwareadresse der Schnittstelle 32 Bytes groß ist (z.B. die Teredo-Schnittstelle)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1097">Fixed issue in WSL where Netlink request for network interface data would fail with EINVAL if the interface's hardware address is 32-bytes (such as the Teredo interface)</span></span>
   - <span data-ttu-id="02d0f-1098">Beachten Sie, dass das Linux-Hilfsprogramm „ip“ einen Fehler enthält, bei dem ein Absturz erfolgt, wenn WSL eine 32-Byte-Hardwareadresse meldet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1098">Note that the Linux "ip" utility contains a bug where it will crash if WSL reports a 32-byte hardware address.</span></span> <span data-ttu-id="02d0f-1099">Dies ist ein Fehler in „ip“, nicht in WSL.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1099">This is a bug in "ip", not WSL.</span></span> <span data-ttu-id="02d0f-1100">Mit dem Hilfsprogramm „ip“ wird die Länge des Zeichenfolgenpuffers fest codiert, der zum Ausgeben der Hardwareadresse verwendet wird, und dieser Puffer ist zu klein, um eine 32-Byte-Hardwareadresse auszugeben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1100">The “ip” utility hard-codes the length of the string buffer used to print the hardware address, and that buffer is too small to print a 32-byte hardware address.</span></span>
- <span data-ttu-id="02d0f-1101">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1101">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1102">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1102">LTP Results:</span></span>
<span data-ttu-id="02d0f-1103">Anzahl bestandener Tests: 669</span><span class="sxs-lookup"><span data-stu-id="02d0f-1103">Number of Passing Test: 669</span></span> </br>
<span data-ttu-id="02d0f-1104">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="02d0f-1104">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="02d0f-1105">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1105">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1106">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1106">Syscall Support</span></span>
<span data-ttu-id="02d0f-1107">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1107">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1108">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1108">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a><span data-ttu-id="02d0f-1109">Build 14971</span><span class="sxs-lookup"><span data-stu-id="02d0f-1109">Build 14971</span></span>

<span data-ttu-id="02d0f-1110">Allgemeine Windows-Informationen zu Build 14971 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1110">For general Windows information on build 14971 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1111">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1111">Fixed</span></span>

 - <span data-ttu-id="02d0f-1112">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1112">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="02d0f-1113">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1113">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1114">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1114">LTP Results:</span></span>
<span data-ttu-id="02d0f-1115">Keine Änderungen seit 14965</span><span class="sxs-lookup"><span data-stu-id="02d0f-1115">Unchanged from 14965</span></span> </br>
<span data-ttu-id="02d0f-1116">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="02d0f-1116">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="02d0f-1117">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1117">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1118">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1118">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a><span data-ttu-id="02d0f-1119">Build 14965</span><span class="sxs-lookup"><span data-stu-id="02d0f-1119">Build 14965</span></span>

<span data-ttu-id="02d0f-1120">Allgemeine Windows-Informationen zu Build 14965 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1120">For general Windows information on build 14965 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1121">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1121">Fixed</span></span>

- <span data-ttu-id="02d0f-1122">Unterstützung für Netlink-Sockets RTM_GETLINK und RTM_GETADDR des NETLINK_ROUTE-Protokolls (GH #468)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1122">Support for Netlink sockets NETLINK_ROUTE protocol's RTM_GETLINK and RTM_GETADDR (GH #468)</span></span>
  - <span data-ttu-id="02d0f-1123">Aktiviert ifconfig- und ip-Befehle für die Netzwerkenumeration.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1123">Enables ifconfig and ip commands for network enumeration</span></span>
  - <span data-ttu-id="02d0f-1124">Weitere Informationen finden Sie in unserem [Blogbeitrag zu WSL-Netzwerken](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1124">More information can be found in our [WSL Networking blog post](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span></span>

- <span data-ttu-id="02d0f-1125">„/sbin“ befindet sich jetzt standardmäßig im Pfad des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1125">/sbin is now in the user's path by default</span></span>
- <span data-ttu-id="02d0f-1126">Der NT-Benutzerpfad wird jetzt standardmäßig an den WSL-Pfad angefügt (Sie können nun also „notepad.exe“ eingeben, ohne dem Linux-Pfad System32 hinzuzufügen).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1126">NT user path now appended to the WSL path by default (i.e. you can now type notepad.exe without adding System32 to the Linux path)</span></span>
- <span data-ttu-id="02d0f-1127">Hinzufügen von Unterstützung für /proc/sys/kernel/cap_last_cap</span><span class="sxs-lookup"><span data-stu-id="02d0f-1127">Added support for /proc/sys/kernel/cap_last_cap</span></span>
- <span data-ttu-id="02d0f-1128">NT-Binärdateien können nun aus WSL gestartet werden, wenn das aktuelle Arbeitsverzeichnis Nicht-ANSI-Zeichen enthält (GH #1254)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1128">NT Binaries can now be launched from WSL when the current working directory contains non-ansi characters (GH #1254)</span></span>
- <span data-ttu-id="02d0f-1129">Ermöglichen des Herunterfahrens für getrennten UNIX-Streamsocket</span><span class="sxs-lookup"><span data-stu-id="02d0f-1129">Allow shutdown on disconnected unix stream socket.</span></span>
- <span data-ttu-id="02d0f-1130">Hinzufügen von Unterstützung für PR_GET_PDEATHSIG.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1130">Added support for PR_GET_PDEATHSIG.</span></span>
- <span data-ttu-id="02d0f-1131">Hinzufügen von Unterstützung für CLONE_PARENT</span><span class="sxs-lookup"><span data-stu-id="02d0f-1131">Added support for CLONE_PARENT</span></span>
- <span data-ttu-id="02d0f-1132">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1132">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="02d0f-1133">Verarbeiten von Anforderungen zum Herstellen einer Verbindung mit dem aktuellen Terminal.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1133">Handle requests to connect to the current terminal.</span></span>
- <span data-ttu-id="02d0f-1134">Markieren von /proc/<pid>/oom_score_adj als beschreibbar.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1134">Mark /proc/<pid>/oom_score_adj as writable.</span></span>
- <span data-ttu-id="02d0f-1135">Hinzufügen des Ordners „/sys/fs/cgroup“.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1135">Add /sys/fs/cgroup folder.</span></span>
- <span data-ttu-id="02d0f-1136">sched_setaffinity sollte den Wert der Affinitätsbitsmaske zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1136">sched_setaffinity should return number of affinity bits mask</span></span>
- <span data-ttu-id="02d0f-1137">Korrektur der ELF-Validierungslogik, die fälschlicherweise annimmt, dass Interpreterpfade weniger als 64 Zeichen lang sein müssen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1137">Fix ELF validation logic which incorrectly assumes interpreter paths must be less than 64 characters long.</span></span> <span data-ttu-id="02d0f-1138">(GH #743)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1138">(GH #743)</span></span>
- <span data-ttu-id="02d0f-1139">Geöffnete Dateideskriptoren können das Konsolenfenster geöffnet lassen (GH #1187)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1139">Open file descriptors can keep console window open (GH #1187)</span></span>
- <span data-ttu-id="02d0f-1140">Korrektur eines Fehlers, bei dem rename() mit einem nachgestellten Schrägstrich für den Zielnamen fehlschlägt (GH #1008)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1140">Fixeed error where rename() failed with trailing slash on target name (GH #1008)</span></span>
- <span data-ttu-id="02d0f-1141">Implementierung der/proc/net/dev-Datei</span><span class="sxs-lookup"><span data-stu-id="02d0f-1141">Implement /proc/net/dev file</span></span>
- <span data-ttu-id="02d0f-1142">Korrektur von Pings mit 0,000 ms aufgrund der Timerauflösung.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1142">Fixed 0.000ms pings due to timer resolution.</span></span>
- <span data-ttu-id="02d0f-1143">Implementierung von /proc/self/environ (GH #730)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1143">Implemented /proc/self/environ (GH #730)</span></span>
- <span data-ttu-id="02d0f-1144">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1144">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1145">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1145">LTP Results:</span></span>
<span data-ttu-id="02d0f-1146">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="02d0f-1146">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="02d0f-1147">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1147">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1148">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1148">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a><span data-ttu-id="02d0f-1149">Build 14959</span><span class="sxs-lookup"><span data-stu-id="02d0f-1149">Build 14959</span></span>

<span data-ttu-id="02d0f-1150">Allgemeine Windows-Informationen zu Build 14959 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1150">For general Windows information on build 14959 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1151">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1151">Fixed</span></span>

- <span data-ttu-id="02d0f-1152">Verbesserte Pico-Prozessbenachrichtigung für Windows.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1152">Improved Pico Process notification for Windows.</span></span>  <span data-ttu-id="02d0f-1153">Weitere Informationen finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1153">Additional information found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span></span>
- <span data-ttu-id="02d0f-1154">Verbesserte Stabilität mit Windows-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="02d0f-1154">Improved stability with Windows interoperability</span></span>
- <span data-ttu-id="02d0f-1155">Korrektur von Fehler 0x80070057 beim Starten von „bash.exe“, wenn der Enterprise Data Protection (EDP) aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="02d0f-1155">Fixed error 0x80070057 when launching bash.exe when Enterprise Data Protection (EDP) is enabled</span></span>
- <span data-ttu-id="02d0f-1156">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1156">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1157">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1157">LTP Results:</span></span>
<span data-ttu-id="02d0f-1158">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="02d0f-1158">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="02d0f-1159">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1159">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1160">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1160">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a><span data-ttu-id="02d0f-1161">Build 14955</span><span class="sxs-lookup"><span data-stu-id="02d0f-1161">Build 14955</span></span>

<span data-ttu-id="02d0f-1162">Allgemeine Windows-Informationen zu Build 14955 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1162">For general Windows information on build 14955 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1163">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1163">Fixed</span></span>

 - <span data-ttu-id="02d0f-1164">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1164">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="02d0f-1165">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1165">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1166">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1166">LTP Results:</span></span>
<span data-ttu-id="02d0f-1167">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="02d0f-1167">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="02d0f-1168">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1168">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1169">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1169">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a><span data-ttu-id="02d0f-1170">Build 14951</span><span class="sxs-lookup"><span data-stu-id="02d0f-1170">Build 14951</span></span>

<span data-ttu-id="02d0f-1171">Allgemeine Windows-Informationen zu Build 14951 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1171">For general Windows information on build 14951 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span></span><br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a><span data-ttu-id="02d0f-1172">Neues Feature: Windows-/Ubuntu-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="02d0f-1172">New Feature: Windows / Ubuntu Interoperability</span></span>
<span data-ttu-id="02d0f-1173">Windows-Binärdateien können jetzt direkt über die WSL-Befehlszeile aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1173">Windows binaries can now be invoked directly from the WSL command line.</span></span>  <span data-ttu-id="02d0f-1174">Dadurch haben Benutzer die Möglichkeit, mit Ihrer Windows-Umgebung und dem -System auf eine Weise zu interagieren, die bisher nicht möglich war.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1174">This gives users the ability to interact with their Windows environment and system in a way that has not been possible.</span></span>  <span data-ttu-id="02d0f-1175">Als kurzes Beispiel können Benutzer nun die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1175">As a quick example, it is now possible for users to run the following commands:</span></span>

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

<span data-ttu-id="02d0f-1176">Weitere Informationen finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1176">More information can be found at:</span></span>

- [<span data-ttu-id="02d0f-1177">WSL-Teamblog für Interop</span><span class="sxs-lookup"><span data-stu-id="02d0f-1177">WSL Team Blog for Interop</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [<span data-ttu-id="02d0f-1178">MSDN-Interop-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="02d0f-1178">MSDN Interop Documentation</span></span>](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1179">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1179">Fixed</span></span>

- <span data-ttu-id="02d0f-1180">Ubuntu 16.04 (Xenial) wird jetzt für alle neuen WSL-Instanzen installiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1180">Ubuntu 16.04 (Xenial) is now installed for all new WSL instances.</span></span>  <span data-ttu-id="02d0f-1181">Benutzer mit vorhandenen 14.04-Instanzen (Trusty) erhalten kein automatisches Upgrade.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1181">Users with existing 14.04 (Trusty) instances will not be automatically upgraded.</span></span>
- <span data-ttu-id="02d0f-1182">Das während der Installation festgelegte Gebietsschema wird jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1182">Locale set during install is now displayed</span></span>
- <span data-ttu-id="02d0f-1183">Terminalverbesserungen, einschließlich des Fehlers bei der Umleitung eines WSL-Prozesses an eine Datei, funktionieren nicht immer</span><span class="sxs-lookup"><span data-stu-id="02d0f-1183">Terminal improvements including bug where redirecting a WSL process to a file does not always work</span></span>
- <span data-ttu-id="02d0f-1184">Die Konsolenlebensdauer muss an die Lebensdauer von „bash.exe“ gebunden sein</span><span class="sxs-lookup"><span data-stu-id="02d0f-1184">Console lifetime should be tied to bash.exe lifetime</span></span>
- <span data-ttu-id="02d0f-1185">Die Größe des Konsolenfensters sollte die sichtbare Größe und nicht die Puffergröße verwenden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1185">Console window size should use visible size, not buffer size</span></span>
- <span data-ttu-id="02d0f-1186">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1186">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1187">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1187">LTP Results:</span></span>
<span data-ttu-id="02d0f-1188">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="02d0f-1188">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="02d0f-1189">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1189">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1190">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1190">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a><span data-ttu-id="02d0f-1191">Build 14946</span><span class="sxs-lookup"><span data-stu-id="02d0f-1191">Build 14946</span></span>

<span data-ttu-id="02d0f-1192">Allgemeine Windows-Informationen zu Build 14946 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1192">For general Windows information on build 14946 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1193">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1193">Fixed</span></span>

- <span data-ttu-id="02d0f-1194">Korrektur eines Problems, das das Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen verhindert hat, die Leerzeichen oder Anführungszeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1194">Fixed an issue that prevented creating WSL user accounts for users with NT usernames that contain spaces or quotes.</span></span> 
- <span data-ttu-id="02d0f-1195">Änderung von VolFs und DrvFs, damit 0 für die Verknüpfungsanzahl des Verzeichnisses im Status zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="02d0f-1195">Change VolFs and DrvFs to return 0 for directory's link count in stat</span></span>
- <span data-ttu-id="02d0f-1196">Unterstützung der IPV6_MULTICAST_HOPS-Socketoption.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1196">Support IPV6_MULTICAST_HOPS socket option.</span></span>
- <span data-ttu-id="02d0f-1197">Einschränkung auf eine einzige Konsolen-E/A-Schleife pro TTY.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1197">Limit to a single console I/O loop per tty.</span></span> <span data-ttu-id="02d0f-1198">Der folgende Befehl ist beispielsweise möglich:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1198">Example: the following command is possible:</span></span>
  - <span data-ttu-id="02d0f-1199">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span><span class="sxs-lookup"><span data-stu-id="02d0f-1199">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span></span>

- <span data-ttu-id="02d0f-1200">Ersetzen von Leerzeichen durch Tabstoppzeichen in /proc/cpuinfo (GH #1115)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1200">replace spaces with tabs in /proc/cpuinfo (GH #1115)</span></span>
- <span data-ttu-id="02d0f-1201">DrvFs wird jetzt in den Einbindungsinformationen mit einem Namen angezeigt, der dem eingebundenen Windows-Volume entspricht</span><span class="sxs-lookup"><span data-stu-id="02d0f-1201">DrvFs now appears in mountinfo with a name that matches mounted Windows volume</span></span>
- <span data-ttu-id="02d0f-1202">/home und/root werden nun in den Einbindungsinformationen mit den richtigen Namen angezeigt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1202">/home and /root now appear in mountinfo with correct names</span></span>
- <span data-ttu-id="02d0f-1203">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1203">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1204">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1204">LTP Results:</span></span>
<span data-ttu-id="02d0f-1205">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="02d0f-1205">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="02d0f-1206">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1206">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1207">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1207">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a><span data-ttu-id="02d0f-1208">Build 14942</span><span class="sxs-lookup"><span data-stu-id="02d0f-1208">Build 14942</span></span>

<span data-ttu-id="02d0f-1209">Allgemeine Windows-Informationen zu Build 14942 finden Sie im [Windows-Blog](https://aka.ms/onefourninefourtwoooooo).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1209">For general Windows information on build 14942 visit the [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1210">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1210">Fixed</span></span>

- <span data-ttu-id="02d0f-1211">Eine Reihe von Fehlerüberprüfungen, einschließlich des Netzwerkabsturzes durch „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“, der SSH blockiert hat</span><span class="sxs-lookup"><span data-stu-id="02d0f-1211">A number of bugchecks addressed, including the “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY” networking crash which was blocking SSH</span></span>
- <span data-ttu-id="02d0f-1212">inotify-Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1212">inotifiy support for notifications generated from Windows applications on DrvFs is now in</span></span>
- <span data-ttu-id="02d0f-1213">Implementierung von TCP_KEEPIDLE und TCP_KEEPINTVL für mongod.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1213">Implement TCP_KEEPIDLE and TCP_KEEPINTVL for mongod.</span></span> <span data-ttu-id="02d0f-1214">(GH #695)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1214">(GH #695)</span></span>
- <span data-ttu-id="02d0f-1215">Implementierung des pivot_root-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="02d0f-1215">Implement the pivot_root system call</span></span>
- <span data-ttu-id="02d0f-1216">Implementierung der Socketoption für SO_DONTROUTE</span><span class="sxs-lookup"><span data-stu-id="02d0f-1216">Implement socket option for SO_DONTROUTE</span></span>
- <span data-ttu-id="02d0f-1217">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1217">Additional bugfixes and improvements</span></span>


### <a name="ltp-results"></a><span data-ttu-id="02d0f-1218">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1218">LTP Results:</span></span>
<span data-ttu-id="02d0f-1219">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="02d0f-1219">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="02d0f-1220">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="02d0f-1220">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="02d0f-1221">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1221">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1222">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1222">Syscall Support</span></span>
<span data-ttu-id="02d0f-1223">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1223">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1224">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1224">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a><span data-ttu-id="02d0f-1225">Build 14936</span><span class="sxs-lookup"><span data-stu-id="02d0f-1225">Build 14936</span></span>

<span data-ttu-id="02d0f-1226">Allgemeine Windows-Informationen zu Build 14936 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1226">For general Windows information on build 14936 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span></span><br/>


<span data-ttu-id="02d0f-1227">Hinweis: WSL wird in einem zukünftigen Release Ubuntu Version 16.04 (Xenial) anstelle von Ubuntu 14.04 (Trusty) installieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1227">Note: WSL will install Ubuntu version 16.04 (Xenial) instead of Ubuntu 14.04 (Trusty) in an upcoming release.</span></span>  <span data-ttu-id="02d0f-1228">Diese Änderung gilt für Insider, die neue Instanzen installieren (lxrun.exe /install oder erste Ausführung von „bash.exe“).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1228">This change will apply to Insiders installing new instances (lxrun.exe /install or first run of bash.exe).</span></span>  <span data-ttu-id="02d0f-1229">Vorhandene Instanzen mit Trusty werden nicht automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1229">Existing instances with Trusty will not be upgraded automatically.</span></span> <span data-ttu-id="02d0f-1230">Benutzer können mit dem Befehl „do-release-upgrade“ Ihr Trusty-Image auf Xenial aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1230">Users can upgrade their Trusty image to Xenial using the do-release-upgrade command.</span></span>

### <a name="known-issue"></a><span data-ttu-id="02d0f-1231">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="02d0f-1231">Known Issue</span></span>
<span data-ttu-id="02d0f-1232">Bei WSL treten Probleme mit einigen Socketimplementierungen auf.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1232">WSL is experiencing an issue with some socket implementations.</span></span>  <span data-ttu-id="02d0f-1233">Die Fehlerüberprüfung manifestiert sich als Absturz mit dem Fehler „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1233">The bugcheck manifests itself as a crash with the error “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY”.</span></span>  <span data-ttu-id="02d0f-1234">Die häufigste Variante dieses Problems ist ein Absturz bei der Verwendung von SSH.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1234">The most common manifestation of this issue is a crash when using ssh.</span></span>  <span data-ttu-id="02d0f-1235">Die Ursache ist bei internen Builds korrigiert und wird so bald wie möglich in Insider gepusht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1235">The root cause is fixed on internal builds and will be pushed to Insiders at the earliest opportunity.</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-1236">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1236">Fixed</span></span>

- <span data-ttu-id="02d0f-1237">Der chroot-Systemaufruf wurde implementiert.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1237">Implemented the chroot system call</span></span>
- <span data-ttu-id="02d0f-1238">Verbesserungen in inotify ~~einschließlich Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden~~</span><span class="sxs-lookup"><span data-stu-id="02d0f-1238">Improvements in inotify ~~including support for notifications generated from Windows applications on DrvFs~~</span></span>
  - <span data-ttu-id="02d0f-1239">Korrektur: Inotify-Unterstützung von Änderungen, die von Windows-Anwendungen stammen, ist zurzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1239">Correction: Inotify support for changes originating from Windows applications not available at this time.</span></span>
- <span data-ttu-id="02d0f-1240">Die Socketbindung an IPv6::<port n> unterstützt jetzt IPV6_V6ONLY (GH #68, #157, #393, #460, #674, #740, #982, #996)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1240">Socket binding to IPV6::<port n> now supports IPV6_V6ONLY  (GH #68, #157, #393, #460, #674, #740, #982, #996)</span></span>
- <span data-ttu-id="02d0f-1241">Implementierung des WNOWAIT-Verhaltens für den waitid-Systemaufruf (GH #638)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1241">WNOWAIT behavior for waitid systemcall implemented (GH #638)</span></span>
- <span data-ttu-id="02d0f-1242">Unterstützung für IP-Socketoptionen IP_HDRINCL und IP_TTL</span><span class="sxs-lookup"><span data-stu-id="02d0f-1242">Support for IP socket options IP_HDRINCL and IP_TTL</span></span>
- <span data-ttu-id="02d0f-1243">read() der Länge Null sollte sofort zurückgegeben werden (GH #975)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1243">Zero-length read() should return immediately (GH #975)</span></span>
- <span data-ttu-id="02d0f-1244">Ordnungsgemäße Verarbeitung von Dateinamen und Dateinamenpräfixen, die keinen NULL-Terminator in einer TAR-Datei enthalten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1244">Correctly handle filenames and filename prefixes that don't include a NULL terminator in a .tar file.</span></span>
- <span data-ttu-id="02d0f-1245">epoll-Unterstützung für/dev/null</span><span class="sxs-lookup"><span data-stu-id="02d0f-1245">epoll support for /dev/null</span></span>
- <span data-ttu-id="02d0f-1246">Korrektur der /dev/alarm-Zeitquelle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1246">Fix /dev/alarm time source</span></span>
- <span data-ttu-id="02d0f-1247">Bash -c kann nun in eine Datei umgeleitet werden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1247">Bash -c now able to redirect to a file</span></span>
- <span data-ttu-id="02d0f-1248">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1248">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1249">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1249">LTP Results:</span></span>
<span data-ttu-id="02d0f-1250">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="02d0f-1250">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="02d0f-1251">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 264</span><span class="sxs-lookup"><span data-stu-id="02d0f-1251">Number of non-Passing (failing, skipped, etc…): 264</span></span> </br>
[<span data-ttu-id="02d0f-1252">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1252">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1253">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1253">Syscall Support</span></span>
<span data-ttu-id="02d0f-1254">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1254">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1255">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1255">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`chroot`<br/>
<br/>

## <a name="build-14931"></a><span data-ttu-id="02d0f-1256">Build 14931</span><span class="sxs-lookup"><span data-stu-id="02d0f-1256">Build 14931</span></span>

<span data-ttu-id="02d0f-1257">Allgemeine Windows-Informationen zu Build 14931 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1257">For general Windows information on build 14931 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1258">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1258">Fixed</span></span>

 - <span data-ttu-id="02d0f-1259">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1259">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="02d0f-1260">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1260">Regularly scheduled updates will resume in the next release.</span></span>

<br/>

## <a name="build-14926"></a><span data-ttu-id="02d0f-1261">Build 14926</span><span class="sxs-lookup"><span data-stu-id="02d0f-1261">Build 14926</span></span>

<span data-ttu-id="02d0f-1262">Allgemeine Windows-Informationen zu Build 14926 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1262">For general Windows information on build 14926 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1263">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1263">Fixed</span></span>

- <span data-ttu-id="02d0f-1264">Ping funktioniert nun in Konsolen, die nicht über Administratorberechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1264">Ping now works in consoles which do not have administrator privileges</span></span>
- <span data-ttu-id="02d0f-1265">Ping6 wird jetzt auch ohne Administratorberechtigungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1265">Ping6 now supported, also without administrator privileges</span></span>
- <span data-ttu-id="02d0f-1266">Inotify-Unterstützung für Dateien, die über WSL geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1266">Inotify support for files modified through WSL.</span></span> <span data-ttu-id="02d0f-1267">(GH #216)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1267">(GH #216)</span></span>
  - <span data-ttu-id="02d0f-1268">Unterstützte Flags:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1268">Flags supported:</span></span>
    - <span data-ttu-id="02d0f-1269">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span><span class="sxs-lookup"><span data-stu-id="02d0f-1269">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span></span>
    - <span data-ttu-id="02d0f-1270">inotify_add_watchEreignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span><span class="sxs-lookup"><span data-stu-id="02d0f-1270">inotify_add_watch events: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span></span>
    - <span data-ttu-id="02d0f-1271">inotify_add_watch-Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span><span class="sxs-lookup"><span data-stu-id="02d0f-1271">inotify_add_watch attributes: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span></span>
    - <span data-ttu-id="02d0f-1272">Lesen der Ausgabe: LX_IN_ISDIR, LX_IN_IGNORED</span><span class="sxs-lookup"><span data-stu-id="02d0f-1272">read output: LX_IN_ISDIR, LX_IN_IGNORED</span></span>
  - <span data-ttu-id="02d0f-1273">Bekanntes Problem: Durch das Ändern von Dateien aus Windows-Anwendungen werden keine Ereignisse generiert</span><span class="sxs-lookup"><span data-stu-id="02d0f-1273">Known issue: Modifying files from Windows applications does not generate any events</span></span>
- <span data-ttu-id="02d0f-1274">Unix-Socket unterstützt jetzt SCM_CREDENTIALS</span><span class="sxs-lookup"><span data-stu-id="02d0f-1274">Unix socket now supports SCM_CREDENTIALS</span></span>

### <a name="ltp-results"></a><span data-ttu-id="02d0f-1275">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="02d0f-1275">LTP Results:</span></span>
<span data-ttu-id="02d0f-1276">Anzahl bestandener Tests: 651</span><span class="sxs-lookup"><span data-stu-id="02d0f-1276">Number of Passing Test: 651</span></span> </br>
<span data-ttu-id="02d0f-1277">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="02d0f-1277">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="02d0f-1278">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="02d0f-1278">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a><span data-ttu-id="02d0f-1279">Build 14915</span><span class="sxs-lookup"><span data-stu-id="02d0f-1279">Build 14915</span></span>

<span data-ttu-id="02d0f-1280">Allgemeine Windows-Informationen zu Build 14915 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1280">For general Windows information on build 14915 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1281">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1281">Fixed</span></span>
-  <span data-ttu-id="02d0f-1282">Socketpair für Unix-Datagrammsockets (GH #262)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1282">Socketpair for unix datagram sockets (GH #262)</span></span>
- <span data-ttu-id="02d0f-1283">Unix-Socketunterstützung für SO_REUSEADDR</span><span class="sxs-lookup"><span data-stu-id="02d0f-1283">Unix socket support for SO_REUSEADDR</span></span>
- <span data-ttu-id="02d0f-1284">Unix-Socketunterstützung für SO_BROADCAST (GH #568)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1284">UNIX socket support for SO_BROADCAST (GH #568)</span></span>
- <span data-ttu-id="02d0f-1285">Unix-Socketunterstützung für SOCK_SEQPACKET (GH #758, #546)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1285">Unix socket support for SOCK_SEQPACKET (GH #758, #546)</span></span>
- <span data-ttu-id="02d0f-1286">Hinzufügen von Unterstützung für unix datagram socket send, recv und shutdown</span><span class="sxs-lookup"><span data-stu-id="02d0f-1286">Adding support for unix datagram socket send, recv and shutdown</span></span>
- <span data-ttu-id="02d0f-1287">Korrektur einer Fehlerüberprüfung aufgrund einer ungültigen Überprüfung des mmap-Parameters für nicht feste Adressen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1287">Fix bugcheck due to invalid mmap parameter validation for non-fixed addresses.</span></span> <span data-ttu-id="02d0f-1288">(GH #847)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1288">(GH #847)</span></span>
- <span data-ttu-id="02d0f-1289">Unterstützung für das Anhalten/Fortsetzen von Terminalzuständen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1289">Support for suspend / resume of terminal states</span></span>
- <span data-ttu-id="02d0f-1290">Unterstützung für TIOCPKT ioctl zum Entsperren des Bildschirmhilfsprogramms (GH #774)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1290">Support for TIOCPKT ioctl to unblock the Screen utility (GH #774)</span></span>
    - <span data-ttu-id="02d0f-1291">Bekanntes Problem: Funktionstasten sind nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="02d0f-1291">Known issue: Function keys not operational</span></span>
- <span data-ttu-id="02d0f-1292">Korrektur einer Racebedingung in TimerFd, die dazu führen konnte, dass auf einen freigegebenen Member „ReaderReady“ durch LxpTimerFdWorkerRoutine zugegriffen wurde (GH #814)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1292">Corrected a race in TimerFd that could cause a freed member 'ReaderReady' to be accessed by LxpTimerFdWorkerRoutine (GH #814)</span></span>
- <span data-ttu-id="02d0f-1293">Aktivieren der Unterstützung für erneut startbaren Systemaufruf für futex, poll und clock_nanosleep</span><span class="sxs-lookup"><span data-stu-id="02d0f-1293">Enable restartable system call support for futex, poll, and clock_nanosleep</span></span>
- <span data-ttu-id="02d0f-1294">Hinzufügen von Unterstützung für Bindungseinbindung</span><span class="sxs-lookup"><span data-stu-id="02d0f-1294">Added bind mount support</span></span>
- <span data-ttu-id="02d0f-1295">Unterstützung für Aufheben der Freigabe für Einbindungsnamespace</span><span class="sxs-lookup"><span data-stu-id="02d0f-1295">unshare for mount namespace support</span></span>
    - <span data-ttu-id="02d0f-1296">Bekanntes Problem: Beim Erstellen eines neuen Einbindngsnamespace mit `unshare(CLONE_NEWNS)` zeigt das aktuelle Arbeitsverzeichnis weiterhin auf den alten Namespace</span><span class="sxs-lookup"><span data-stu-id="02d0f-1296">Known issue: When creating a new mount namespace with `unshare(CLONE_NEWNS)` the current working directory will continue to point to the old namespace</span></span>
- <span data-ttu-id="02d0f-1297">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1297">Additional improvements and bug fixes</span></span>

<br/>

## <a name="build-14905"></a><span data-ttu-id="02d0f-1298">Build 14905</span><span class="sxs-lookup"><span data-stu-id="02d0f-1298">Build 14905</span></span>

<span data-ttu-id="02d0f-1299">Allgemeine Windows-Informationen zu Build 14905 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1299">For general Windows information on build 14905 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1300">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1300">Fixed</span></span>
- <span data-ttu-id="02d0f-1301">Erneut startbare Systemaufrufe werden jetzt unterstützt (GH #349, GH #520)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1301">Restartable system calls are now supported (GH #349, GH #520)</span></span>
- <span data-ttu-id="02d0f-1302">Symbolische Verknüpfungen mit Verzeichnissen, die auf / wenden, sind jetzt funktionstüchtig (GH #650)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1302">Symlinks to directories ending in / now operational (GH #650)</span></span>
- <span data-ttu-id="02d0f-1303">Implementierung von RNDGETENTCNT ioctl für „/dev/random“</span><span class="sxs-lookup"><span data-stu-id="02d0f-1303">Implemented RNDGETENTCNT ioctl for /dev/random</span></span>
- <span data-ttu-id="02d0f-1304">Implementierung der /proc/[pid]/mounts, /proc/[pid]/mountinfo- und /proc/[pid]/mountstats-Dateien</span><span class="sxs-lookup"><span data-stu-id="02d0f-1304">Implemented the /proc/[pid]/mounts, /proc/[pid]/mountinfo and /proc/[pid]/mountstats files</span></span>
- <span data-ttu-id="02d0f-1305">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1305">Additional bugfixes and improvements</span></span>

</br>

## <a name="build-14901"></a><span data-ttu-id="02d0f-1306">Build 14901</span><span class="sxs-lookup"><span data-stu-id="02d0f-1306">Build 14901</span></span>
<span data-ttu-id="02d0f-1307">Der erste Insider-Build für das Windows 10 Anniversary Update-Release.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1307">First Insider build for the post Windows 10 Anniversary Update release.</span></span>

<span data-ttu-id="02d0f-1308">Allgemeine Windows-Informationen zu Build 14901 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1308">For general Windows information on build 14901 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1309">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1309">Fixed</span></span>
- <span data-ttu-id="02d0f-1310">Korrektur eines Problems mit nachfolgenden Schrägstrichen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1310">Fixed trailing slash issue</span></span>
    - <span data-ttu-id="02d0f-1311">Befehle wie `$ mv a/c/ a/b/` funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1311">Commands such as `$ mv a/c/ a/b/` now work</span></span>
- <span data-ttu-id="02d0f-1312">Installation von Eingabeaufforderungen, wenn das Ubuntu-Gebietsschema auf das Windows-Gebietsschema festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="02d0f-1312">Installing now prompts if Ubuntu locale should be set to Windows locale</span></span>
- <span data-ttu-id="02d0f-1313">Procfs-Unterstützung für den Ordner „ns“</span><span class="sxs-lookup"><span data-stu-id="02d0f-1313">Procfs support for ns folder</span></span>
- <span data-ttu-id="02d0f-1314">Hinzufügen von „mount“ und „unmount“ für tmpfs-, procfs-und sysfs-Dateisysteme</span><span class="sxs-lookup"><span data-stu-id="02d0f-1314">Added mount and unmount for tmpfs, procfs and sysfs file systems</span></span>
- <span data-ttu-id="02d0f-1315">Korrektur der 32-Bit-ABI-Signatur von mklod [at]</span><span class="sxs-lookup"><span data-stu-id="02d0f-1315">Fix mknod[at] 32-bit ABI signature</span></span>
- <span data-ttu-id="02d0f-1316">Verschieben von Unix-Sockets in Dispatchmodell</span><span class="sxs-lookup"><span data-stu-id="02d0f-1316">Unix sockets moved to dispatch model</span></span>
- <span data-ttu-id="02d0f-1317">Mit setsockopt festgelegte recv-Puffergröße von INET-Socket muss berücksichtigt werden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1317">INET socket recv buffer size set using the setsockopt should be honored</span></span>
- <span data-ttu-id="02d0f-1318">Implementierung des MSG_CMSG_CLOEXEC-Unis-Socket-Empfangsnachrichtenflags</span><span class="sxs-lookup"><span data-stu-id="02d0f-1318">Implement MSG_CMSG_CLOEXEC unix socket receive message flag</span></span>
- <span data-ttu-id="02d0f-1319">stdin/stdout-Pipeumleitung des Linux-Prozesses (GH #2)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1319">Linux process stdin/stdout pipe redirection (GH #2)</span></span>
    - <span data-ttu-id="02d0f-1320">Ermöglicht das Weiterleiten von bash -c-Befehlen in CMD.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1320">Allows for piping of bash -c commands in CMD.</span></span>  <span data-ttu-id="02d0f-1321">Beispiel: >dir | bash -c "grep foo"</span><span class="sxs-lookup"><span data-stu-id="02d0f-1321">Example:  >dir | bash -c "grep foo"</span></span>
- <span data-ttu-id="02d0f-1322">Bash kann nun auf Systemen mit mehreren Auslagerungsdateien installiert werden (GH #538, #358)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1322">Bash can now be installed on systems with multiple pagefiles (GH #538, #358)</span></span>
- <span data-ttu-id="02d0f-1323">Standardpuffergröße des INET-Sockets sollte mit der Größe des Ubuntu- Standardsetups übereinstimmen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1323">Default INET Socket buffer size should match that of default Ubuntu setup</span></span>
- <span data-ttu-id="02d0f-1324">Ausrichten von xattr-Systemaufrufen an listxattr</span><span class="sxs-lookup"><span data-stu-id="02d0f-1324">Align xattr syscalls to listxattr</span></span>
- <span data-ttu-id="02d0f-1325">Nur Rückgabe von Schnittstellen mit einer gültigen IPv4-Adresse von SIOCGIFCONF</span><span class="sxs-lookup"><span data-stu-id="02d0f-1325">Only return interfaces with a valid IPv4 address from SIOCGIFCONF</span></span>
- <span data-ttu-id="02d0f-1326">Korrektur der Signalatandardaktion, wenn von ptrace eingefügt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1326">Fix signal default action when injected by ptrace</span></span>
- <span data-ttu-id="02d0f-1327">Implementierung von /proc/sys/vm/min_free_kbytes</span><span class="sxs-lookup"><span data-stu-id="02d0f-1327">implement /proc/sys/vm/min_free_kbytes</span></span>
- <span data-ttu-id="02d0f-1328">Verwenden der Computerkontext-Registerwerte beim Wiederherstellen von Kontext in sigreturn</span><span class="sxs-lookup"><span data-stu-id="02d0f-1328">Use machine context register values when restoring context in sigreturn</span></span>
    - <span data-ttu-id="02d0f-1329">Dadurch wird das Problem behoben, dass Java und javac bei einigen Benutzern nicht mehr reagiert haben</span><span class="sxs-lookup"><span data-stu-id="02d0f-1329">This resolves the issue where java and javac were hanging for some users</span></span>
- <span data-ttu-id="02d0f-1330">Implementierung von /proc/sys/kernel/hostname</span><span class="sxs-lookup"><span data-stu-id="02d0f-1330">Implement /proc/sys/kernel/hostname</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1331">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1331">Syscall Support</span></span>
<span data-ttu-id="02d0f-1332">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1332">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1333">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1333">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a><span data-ttu-id="02d0f-1334">Update von Build 14388 auf Windows 10 Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="02d0f-1334">Build 14388 to Windows 10 Anniversary Update</span></span>
<span data-ttu-id="02d0f-1335">Allgemeine Windows-Informationen zu Build 14388 finden Sie im [Windows-Blog](https://aka.ms/14388wip).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1335">For general Windows information on build 14388 visit the [Windows Blog](https://aka.ms/14388wip).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1336">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1336">Fixed</span></span>
- <span data-ttu-id="02d0f-1337">Korrekturen als Vorbereitung auf das Windows 10 Anniversary Update am 02.08.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1337">Fixes to prepare for the Windows 10 Anniversary Update on 8/2</span></span>
  - <span data-ttu-id="02d0f-1338">Weitere Informationen zu WSL im Anniversary Update finden Sie in unserem [Blog](https://blogs.msdn.microsoft.com/wsl/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1338">More information about WSL in the Anniversary Update can be found on our [blog](https://blogs.msdn.microsoft.com/wsl/)</span></span>

<br/>

## <a name="build-14376"></a><span data-ttu-id="02d0f-1339">Build 14376</span><span class="sxs-lookup"><span data-stu-id="02d0f-1339">Build 14376</span></span>
<span data-ttu-id="02d0f-1340">Allgemeine Windows-Informationen zu Build 14376 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1340">For general Windows information on build 14376 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1341">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1341">Fixed</span></span>
- <span data-ttu-id="02d0f-1342">Entfernen einiger Instanzen, in denen apt-get nicht mehr reagiert (GH #493)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1342">Removed some instances where apt-get hangs (GH #493)</span></span>
- <span data-ttu-id="02d0f-1343">Korrektur eines Problems, bei dem leere Einbindungen nicht ordnungsgemäß verarbeitet wurden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1343">Fixed an issue where empty mounts were not handled correctly</span></span>
- <span data-ttu-id="02d0f-1344">Korrektur eines Problems, bei dem Ramdisks nicht ordnungsgemäß eingebunden wurden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1344">Fixed an issue where ramdisks were not mounted correctly</span></span>
- <span data-ttu-id="02d0f-1345">Änderung von „unix socket accept“ für die Unterstützung von Flags (Teil von GH #451)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1345">Change unix socket accept to support flags (partial GH #451)</span></span>
- <span data-ttu-id="02d0f-1346">Korrektur eines allgemeinen netzwerkbezogenen Bluescreens</span><span class="sxs-lookup"><span data-stu-id="02d0f-1346">Fixed common network related bluescreen</span></span>
- <span data-ttu-id="02d0f-1347">Korrektur des Bluescreens beim Zugriff auf /proc/[pid]/task (GH #523)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1347">Fixed bluescreen when accessing /proc/[pid]/task (GH #523)</span></span>
- <span data-ttu-id="02d0f-1348">Korrektur hoher CPU-Auslastung für einige Pty-Szenarien (GH #488, #504)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1348">Fixed high CPU utilization for some pty scenarios (GH #488, #504)</span></span>
- <span data-ttu-id="02d0f-1349">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1349">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14371"></a><span data-ttu-id="02d0f-1350">Build 14371</span><span class="sxs-lookup"><span data-stu-id="02d0f-1350">Build 14371</span></span>
<span data-ttu-id="02d0f-1351">Allgemeine Windows-Informationen zu Build 14371 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1351">For general Windows information on build 14371 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1352">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1352">Fixed</span></span>
- <span data-ttu-id="02d0f-1353">Korrektur der Timingracebedingung mit SIGCHLD und wait() bei Verwendung von ptrace</span><span class="sxs-lookup"><span data-stu-id="02d0f-1353">Corrected timing race with SIGCHLD and wait() when using ptrace</span></span>
- <span data-ttu-id="02d0f-1354">Korrektur von Verhalten, wenn Pfade ein nachfolgendes Zeichen / aufweisen (GH #432)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1354">Corrected some behavior when paths have a trailing /  (GH #432)</span></span>
- <span data-ttu-id="02d0f-1355">Korrektur eines Problems, bei dem Umbenennen/Aufheben der Verknüpfung aufgrund von geöffneten Handles für untergeordnete Elemente fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1355">Fixed issue with rename/unlink failing due to open handles to children</span></span>
- <span data-ttu-id="02d0f-1356">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1356">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14366"></a><span data-ttu-id="02d0f-1357">Build 14366</span><span class="sxs-lookup"><span data-stu-id="02d0f-1357">Build 14366</span></span>
<span data-ttu-id="02d0f-1358">Allgemeine Windows-Informationen zu Build 14366 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1358">For general Windows information on build 14366 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1359">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1359">Fixed</span></span>
- <span data-ttu-id="02d0f-1360">Korrektur der Dateierstellung durch symbolische Verknüpfungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1360">Fix in file creation through symlinks</span></span>
-   <span data-ttu-id="02d0f-1361">Hinzugefügter von listxattr für Python (GH 385)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1361">Added listxattr for Python (GH 385)</span></span>
-   <span data-ttu-id="02d0f-1362">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1362">Additional bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1363">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1363">Syscall Support</span></span>
-   <span data-ttu-id="02d0f-1364">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1364">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1365">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1365">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`listxattr`<br/>
<br/>

## <a name="build-14361"></a><span data-ttu-id="02d0f-1366">Build 14361</span><span class="sxs-lookup"><span data-stu-id="02d0f-1366">Build 14361</span></span>
<span data-ttu-id="02d0f-1367">Allgemeine Windows-Informationen zu Build 14361 finden Sie im [Windows-Blog](https://aka.ms/wip14361).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1367">For general Windows information on build 14361 visit the [Windows Blog](https://aka.ms/wip14361).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1368">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1368">Fixed</span></span>
- <span data-ttu-id="02d0f-1369">Für DrvFs wird nun bei der Ausführung in Bash unter Ubuntu unter Windows die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1369">DrvFs is now case sensitive when running in Bash on Ubuntu on Windows.</span></span>
  - <span data-ttu-id="02d0f-1370">Benutzer können case.txt und CASE.TXT auf Ihren /mnt/c-Laufwerken verwenden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1370">Users may case.txt and CASE.TXT on their /mnt/c drives</span></span>
  - <span data-ttu-id="02d0f-1371">Die Beachtung von Groß-/Kleinschreibung wird nur in Bash unter Ubuntu unter Windows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1371">Case sensitivity is only supported within Bash on Ubuntu on Windows.</span></span> <span data-ttu-id="02d0f-1372">Außerhalb von Bash zeigt NTFS die Dateien richtig an, aber es kann zu unerwartetem Verhalten bei der Interaktion mit den Dateien von Windows kommen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1372">When outside of Bash NTFS will report the files correctly, but unexpected behavior may occur interacting with the files from Windows.</span></span>
  - <span data-ttu-id="02d0f-1373">Für den Stamm der einzelnen Volumes (d.h. /mnt/c) wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1373">The root of each volume (i.e. /mnt/c) is not case sensitive</span></span>
  - <span data-ttu-id="02d0f-1374">Weitere Informationen zum Verarbeiten dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1374">More information on handling these files in Windows can be found [here](https://support.microsoft.com/en-us/kb/100625).</span></span>
- <span data-ttu-id="02d0f-1375">Stark verbesserte PTY-/TTY-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1375">Greatly enhanced pty / tty support.</span></span>  <span data-ttu-id="02d0f-1376">Anwendungen wie TMUX werden jetzt unterstützt (GH #40)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1376">Applications like TMUX now supported (GH #40)</span></span>
- <span data-ttu-id="02d0f-1377">Korrektur eines Installationsproblems, bei dem Benutzerkonten nicht immer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1377">Fixed install issue where user accounts not always created</span></span>
- <span data-ttu-id="02d0f-1378">Optimierte Befehlszeilen-Argumentstruktur, die eine extrem lange Argumentliste zulässt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1378">Optimized command line arg structure allowing for extremely long argument list.</span></span> <span data-ttu-id="02d0f-1379">(GH #153)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1379">(GH #153)</span></span>
- <span data-ttu-id="02d0f-1380">Jetzt können chmod read_only-Dateien aus DrvFs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1380">Now able to delete and chmod read_only files from DrvFs</span></span>
- <span data-ttu-id="02d0f-1381">Korrektur einiger Instanzen, bei denen das Terminal beim Trennen nicht mehr reagiert (GH #43)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1381">Fixed some instances where the terminal hangs on disconnect (GH #43)</span></span>
- <span data-ttu-id="02d0f-1382">chmod und chown funktionieren jetzt auf TTY-Geräten</span><span class="sxs-lookup"><span data-stu-id="02d0f-1382">chmod and chown now work on tty devices</span></span>
- <span data-ttu-id="02d0f-1383">Verbindung mit 0.0.0.0 und :: as localhost zulassen (GH #388)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1383">Allow connection to 0.0.0.0 and :: as localhost (GH #388)</span></span>
- <span data-ttu-id="02d0f-1384">Sendmsg/recvmsg verarbeitet nun eine E/A-Vektorlänge > 1 (Teil von GH #376)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1384">Sendmsg/recvmsg now handle an IO vector length of >1 (partial GH #376)</span></span>
- <span data-ttu-id="02d0f-1385">Benutzer können jetzt die automatisch generierte Hostdatei ablehnen (GH #398)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1385">Users can now opt-out of auto-generated hosts file (GH #398)</span></span>
- <span data-ttu-id="02d0f-1386">Automatisches Zuordnen des Linux-Gebietsschemas zum NT-Gebietsschema während der Installation (GH #11)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1386">Automatically match Linux locale to the NT locale during install (GH #11)</span></span>
- <span data-ttu-id="02d0f-1387">Hinzufügen der /proc/sys/vm/swappiness-Datei (GH #306)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1387">Added the /proc/sys/vm/swappiness file (GH #306)</span></span>
- <span data-ttu-id="02d0f-1388">strace wird jetzt ordnungsgemäß beendet</span><span class="sxs-lookup"><span data-stu-id="02d0f-1388">strace now exits correctly</span></span>
- <span data-ttu-id="02d0f-1389">Ermöglichen des erneuten Öffnens von Pipes über /proc/self/fd (GH #222)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1389">Allow pipes to be reopened through /proc/self/fd (GH #222)</span></span>
- <span data-ttu-id="02d0f-1390">Ausblenden von Verzeichnissen unter „%LOCALAPPDATA%\lxss“ aus DrvFs (GH #270)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1390">Hide directories under %LOCALAPPDATA%\lxss from DrvFs (GH #270)</span></span>
- <span data-ttu-id="02d0f-1391">Bessere Verarbeitung von bash.exe ~.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1391">Better handling of bash.exe ~.</span></span>  <span data-ttu-id="02d0f-1392">Befehle wie „bash ~ -c ls“ werden jetzt unterstützt (GH #467)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1392">Commands like “bash ~ -c ls” now supported (GH #467)</span></span>
- <span data-ttu-id="02d0f-1393">Sockets benachrichtigen nun darüber, dass epoll read beim Herunterfahren verfügbar ist (GH #271)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1393">Sockets now notify epoll read available during shutdown (GH #271)</span></span>
- <span data-ttu-id="02d0f-1394">lxrun/uninstall arbeitet besser beim Löschen der Dateien und Ordner.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1394">lxrun /uninstall does a better job of deleting the files and folders</span></span>
- <span data-ttu-id="02d0f-1395">Korrektur für ps-f (GH #246)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1395">Corrected ps -f (GH #246)</span></span>
- <span data-ttu-id="02d0f-1396">Verbesserte Unterstützung für X11-Apps, z.B. xEmacs (GH #481)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1396">Improved support for x11 apps such as xEmacs (GH #481)</span></span>
- <span data-ttu-id="02d0f-1397">Aktualisierte anfängliche Threadstapelgröße, um der standardmäßigen Ubuntu-Einstellung zu entsprechen und die Größe ordnungsgemäß an den get_rlimit-Systemaufruf zu melden (GH #172, #258)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1397">Updated initial thread stack size to match default Ubuntu setting and reporting the size correctly to the get_rlimit syscall (GH #172, #258)</span></span>
- <span data-ttu-id="02d0f-1398">Verbesserte Berichterstellung von Pico-Prozessimagenamen (z.B. für die Überwachung)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1398">Improved reporting of pico process image names (e.g., for auditing)</span></span>
- <span data-ttu-id="02d0f-1399">Implementierung von /proc/mountinfo für df-Befehl</span><span class="sxs-lookup"><span data-stu-id="02d0f-1399">Implemented /proc/mountinfo for df command</span></span>
- <span data-ttu-id="02d0f-1400">Korrektur des Fehlercodes der symbolischen Verknüpfung für den untergeordneten Namen .</span><span class="sxs-lookup"><span data-stu-id="02d0f-1400">Fixed symlink error code for child name .</span></span> <span data-ttu-id="02d0f-1401">und ..</span><span class="sxs-lookup"><span data-stu-id="02d0f-1401">and ..</span></span>
- <span data-ttu-id="02d0f-1402">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1402">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1403">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1403">Syscall Support</span></span>
<span data-ttu-id="02d0f-1404">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1404">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1405">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1405">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a><span data-ttu-id="02d0f-1406">Build 14352</span><span class="sxs-lookup"><span data-stu-id="02d0f-1406">Build 14352</span></span>
<span data-ttu-id="02d0f-1407">Allgemeine Windows-Informationen zu Build 14352 finden Sie im [Windows-Blog](https://aka.ms/wip14352).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1407">For general Windows information on build 14352 visit the [Windows Blog](https://aka.ms/wip14352).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1408">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1408">Fixed</span></span>
- <span data-ttu-id="02d0f-1409">Korrektur eines Problems, bei dem große Dateien nicht ordnungsgemäß heruntergeladen bzw. ordnungsgemäß erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1409">Fixed issue where large files were not downloaded / created correctly.</span></span>  <span data-ttu-id="02d0f-1410">Dadurch sollte die Blockierung von npm und anderen Szenarien aufgehoben werden (GH #3, GH #313)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1410">This should unblock npm and other scenarios (GH #3, GH #313)</span></span>
- <span data-ttu-id="02d0f-1411">Entfernen einiger Instanzen, in denen Sockets nicht mehr reagieren</span><span class="sxs-lookup"><span data-stu-id="02d0f-1411">Removed some instances where sockets hang</span></span>
- <span data-ttu-id="02d0f-1412">Korrektur einiger ptrace-Fehler</span><span class="sxs-lookup"><span data-stu-id="02d0f-1412">Corrected some ptrace errors</span></span>
- <span data-ttu-id="02d0f-1413">Korrektur eines Problems, bei dem WSL Dateinamen mit mehr als 255 Zeichen zuließ</span><span class="sxs-lookup"><span data-stu-id="02d0f-1413">Fixed issue with WSL allowing filenames longer than 255 characters</span></span>
- <span data-ttu-id="02d0f-1414">Verbesserte Unterstützung nicht-englischer Zeichen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1414">Improved support for non-English characters</span></span>
- <span data-ttu-id="02d0f-1415">Hinzufügen aktueller Windows-Zeitzonendaten und Festlegen als Standard</span><span class="sxs-lookup"><span data-stu-id="02d0f-1415">Add current Windows timezone data and set as default</span></span>
- <span data-ttu-id="02d0f-1416">Eindeutige Geräte-IDs für jeden Einbindungspunkt (jre-Korrektur – GH #49)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1416">Unique device id’s for each mount point (jre fix – GH #49)</span></span>
- <span data-ttu-id="02d0f-1417">Korrektur eines Problems mit Pfaden, die „.“</span><span class="sxs-lookup"><span data-stu-id="02d0f-1417">Correct issue with paths containing “.”</span></span> <span data-ttu-id="02d0f-1418">und „..“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1418">and “..”</span></span>
- <span data-ttu-id="02d0f-1419">Hinzufügen von FIFO-Unterstützung (GH #71)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1419">Added Fifo support (GH #71)</span></span>
- <span data-ttu-id="02d0f-1420">Aktualisiertes Format von „resolv.conf“ entsprechend dem nativen Ubuntu-Format</span><span class="sxs-lookup"><span data-stu-id="02d0f-1420">Updated format of resolv.conf to match native Ubuntu format</span></span>
- <span data-ttu-id="02d0f-1421">procfs-Bereinigung</span><span class="sxs-lookup"><span data-stu-id="02d0f-1421">Some procfs cleanup</span></span>
- <span data-ttu-id="02d0f-1422">Aktivierten von Ping für Administratorkonsolen (GH #18)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1422">Enabled ping for Administrator consoles (GH #18)</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1423">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1423">Syscall Support</span></span>
<span data-ttu-id="02d0f-1424">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1424">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1425">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1425">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a><span data-ttu-id="02d0f-1426">Build 14342</span><span class="sxs-lookup"><span data-stu-id="02d0f-1426">Build 14342</span></span>
<span data-ttu-id="02d0f-1427">Allgemeine Windows-Informationen zu Build 14342 finden Sie im [Windows-Blog](https://aka.ms/wip14342).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1427">For general Windows information on build 14342 the [Windows Blog](https://aka.ms/wip14342).</span></span> <br/>

<span data-ttu-id="02d0f-1428">Informationen zu VolFs und DriveFs finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1428">Information on VolFs and DriveFs can be found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="02d0f-1429">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1429">Fixed</span></span>
- <span data-ttu-id="02d0f-1430">Korrektur eines Installationsproblems, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen enthielt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1430">Fixed install issue when the Windows user had Unicode characters in the username</span></span>
- <span data-ttu-id="02d0f-1431">Die Problemumgehung „apt-get update udev“ in den FAQ wird jetzt standardmäßig bei der ersten Ausführung bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1431">The apt-get update udev workaround in the FAQ is now provided by default on first run</span></span>
- <span data-ttu-id="02d0f-1432">Aktivierte symbolische Verknüpfungen in DriveFs-Verzeichnissen (/mnt/<drive>)</span><span class="sxs-lookup"><span data-stu-id="02d0f-1432">Enabled symlinks in DriveFs (/mnt/<drive>) directories</span></span>
- <span data-ttu-id="02d0f-1433">Symbolische Verknüpfungen funktionieren nun zwischen DriveFs und VolFs</span><span class="sxs-lookup"><span data-stu-id="02d0f-1433">Symlinks now work between DriveFs and VolFs</span></span>
- <span data-ttu-id="02d0f-1434">Korrektur des Pfadanalyseproblems auf oberster Ebene: ls .// funktioniert jetzt wie erwartet</span><span class="sxs-lookup"><span data-stu-id="02d0f-1434">Addressed top level path parsing issue: ls .// will now work as expected</span></span>
- <span data-ttu-id="02d0f-1435">npm install auf DriveFs und die -g-Optionen funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1435">npm install on DriveFs and the -g options are now working</span></span>
- <span data-ttu-id="02d0f-1436">Korrektur eines Problems, das den Start des PHP-Servers verhinderte</span><span class="sxs-lookup"><span data-stu-id="02d0f-1436">Fixed issue preventing PHP server from launching</span></span>
- <span data-ttu-id="02d0f-1437">Aktualisierte Standardumgebungswerte, z.B. $PATH, um nativem Ubuntu besser zu entsprechen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1437">Updated default environment values, such as $PATH to closer match native Ubuntu</span></span>
- <span data-ttu-id="02d0f-1438">Hinzufügen eines wöchentlichen Wartungstasks in Windows zum Aktualisieren des apt-Paketcaches</span><span class="sxs-lookup"><span data-stu-id="02d0f-1438">Added a weekly maintenance task in Windows to update the apt package cache</span></span>
- <span data-ttu-id="02d0f-1439">Korrektur eines Problems bei der Überprüfung von ELF-Headern, WSL unterstützt jetzt alle Melkor-Optionen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1439">Fixed issue with ELF header validation, WSL now supports all Melkor options</span></span>
- <span data-ttu-id="02d0f-1440">Zsh-Shell ist funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="02d0f-1440">Zsh shell is functional</span></span>
- <span data-ttu-id="02d0f-1441">Vorkompilierte Go-Binärdateien werden jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1441">Precompiled Go binaries are now supported</span></span>
- <span data-ttu-id="02d0f-1442">Eingabeaufforderung bei der ersten Ausführung von „bash.exe“ ist nun richtig lokalisiert</span><span class="sxs-lookup"><span data-stu-id="02d0f-1442">Prompting on Bash.exe first run is now localized correctly</span></span>
- <span data-ttu-id="02d0f-1443">/proc/meminfo gibt jetzt richtige Informationen zurück</span><span class="sxs-lookup"><span data-stu-id="02d0f-1443">/proc/meminfo now returns correct information</span></span>
- <span data-ttu-id="02d0f-1444">Sockets werden jetzt in VFS unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1444">Sockets now supported in VFS</span></span>
- <span data-ttu-id="02d0f-1445">/dev jetzt als tempfs eingebunden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1445">/dev now mounted as tempfs</span></span>
- <span data-ttu-id="02d0f-1446">Fifo wird jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1446">Fifo now supported</span></span>
- <span data-ttu-id="02d0f-1447">Mehrkernsysteme werden nun ordnungsgemäß in /proc/cpuinfo angezeigt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1447">Multi-core systems now showing correctly in /proc/cpuinfo</span></span>
- <span data-ttu-id="02d0f-1448">Weitere Verbesserungen und Fehlermeldungen, die während der ersten Ausführung heruntergeladen werden</span><span class="sxs-lookup"><span data-stu-id="02d0f-1448">Additional improvements and error messages downloading during first run</span></span>
- <span data-ttu-id="02d0f-1449">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1449">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="02d0f-1450">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1450">Supported syscall list below.</span></span>
- <span data-ttu-id="02d0f-1451">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1451">Additional bugfixes and improvements</span></span>

### <a name="known-issues"></a><span data-ttu-id="02d0f-1452">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="02d0f-1452">Known Issues</span></span>
- <span data-ttu-id="02d0f-1453">„.“ wird in einigen Fällen nicht</span><span class="sxs-lookup"><span data-stu-id="02d0f-1453">Not resolving ‘..’</span></span> <span data-ttu-id="02d0f-1454">ordnungsgemäß auf DriveFs aufgelöst</span><span class="sxs-lookup"><span data-stu-id="02d0f-1454">correctly on DriveFs in some cases</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1455">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1455">Syscall Support</span></span>
<span data-ttu-id="02d0f-1456">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1456">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1457">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1457">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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

## <a name="build-14332"></a><span data-ttu-id="02d0f-1458">Build 14332</span><span class="sxs-lookup"><span data-stu-id="02d0f-1458">Build 14332</span></span>

<span data-ttu-id="02d0f-1459">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14332).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1459">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14332).</span></span> <br/>


### <a name="fixed"></a><span data-ttu-id="02d0f-1460">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1460">Fixed</span></span>
- <span data-ttu-id="02d0f-1461">Bessere resolv.conf-Generierung einschließlich Priorisieren von DNS-Einträgen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1461">Better resolv.conf generation including prioritizing DNS entries</span></span>
- <span data-ttu-id="02d0f-1462">Problem beim Verschieben von Dateien und Verzeichnissen zwischen/mnt- und Nicht-/mnt-Laufwerken</span><span class="sxs-lookup"><span data-stu-id="02d0f-1462">Issue with moving files and directories between /mnt and non-/mnt drives</span></span>
- <span data-ttu-id="02d0f-1463">TAR-Dateien können jetzt mit symbolischen Verknüpfungen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1463">Tar files can now be created with symlinks</span></span>
- <span data-ttu-id="02d0f-1464">Hinzufügen des /run/lock-Standardverzeichnisses bei der Instanzerstellung</span><span class="sxs-lookup"><span data-stu-id="02d0f-1464">Added default /run/lock directory on instance creation</span></span>
- <span data-ttu-id="02d0f-1465">Aktualisieren von /dev/null, um die richtigen Statusinformationen zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="02d0f-1465">Update /dev/null to return proper stat info</span></span>
- <span data-ttu-id="02d0f-1466">Weitere Fehler beim Herunterladen während der ersten Ausführung</span><span class="sxs-lookup"><span data-stu-id="02d0f-1466">Additional errors when downloading during first run</span></span>
- <span data-ttu-id="02d0f-1467">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1467">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="02d0f-1468">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1468">Supported syscall list below.</span></span>
- <span data-ttu-id="02d0f-1469">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1469">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1470">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1470">Syscall Support</span></span>
<span data-ttu-id="02d0f-1471">Im folgenden finden Sie den neuen Systemaufruf, der in WSL implementiert ist.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1471">Below is the new syscall that has some implementation in WSL.</span></span> <span data-ttu-id="02d0f-1472">Der Systemaufruf in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1472">The syscall on this list is supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a><span data-ttu-id="02d0f-1473">Build 14328</span><span class="sxs-lookup"><span data-stu-id="02d0f-1473">Build 14328</span></span>

<span data-ttu-id="02d0f-1474">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14328).</span><span class="sxs-lookup"><span data-stu-id="02d0f-1474">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14328).</span></span> <br/>


### <a name="new-features"></a><span data-ttu-id="02d0f-1475">Neue Funktionen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1475">New Features</span></span>
* <span data-ttu-id="02d0f-1476">Jetzt werden Linux-Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1476">Now support Linux users.</span></span>  <span data-ttu-id="02d0f-1477">Bei der Installation von Bash unter Ubuntu unter Windows werden Sie aufgefordert, einen Linux-Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1477">Installing Bash on Ubuntu on Windows will prompt for creation of a Linux user.</span></span>  <span data-ttu-id="02d0f-1478">Weitere Informationen finden Sie unter https://aka.ms/wslusers.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1478">For more information, visit https://aka.ms/wslusers</span></span>
* <span data-ttu-id="02d0f-1479">Der Hostname ist jetzt auf den Windows-Computernamen festgelegt, nicht mehr auf @localhost</span><span class="sxs-lookup"><span data-stu-id="02d0f-1479">Hostname is now set to the Windows computer name, no more @localhost</span></span>
* <span data-ttu-id="02d0f-1480">Weitere Informationen zu Build 14328 finden Sie unter: https://aka.ms/wip14328</span><span class="sxs-lookup"><span data-stu-id="02d0f-1480">For more information on build 14328, visit: https://aka.ms/wip14328</span></span>

### <a name="fixed"></a><span data-ttu-id="02d0f-1481">Fest</span><span class="sxs-lookup"><span data-stu-id="02d0f-1481">Fixed</span></span>
* <span data-ttu-id="02d0f-1482">Verbesserungen von symbolischen Verknüpfungen für Nicht-/mnt/<drive>-Dateien</span><span class="sxs-lookup"><span data-stu-id="02d0f-1482">Symlink improvements for non /mnt/<drive> files</span></span>
    * <span data-ttu-id="02d0f-1483">Die npm-Installation funktioniert jetzt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1483">npm install now works</span></span>
    * <span data-ttu-id="02d0f-1484">jdk/jre kann nun mithilfe der Anweisungen installiert werden, die Sie [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html) finden.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1484">jdk / jre now installable using instructions found [here](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span></span>
    * <span data-ttu-id="02d0f-1485">Bekanntes Problem: Symbolische Verknüpfungen funktionieren für Windows-Einbindungen nicht.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1485">known issue: symlinks do not work for Windows mounts.</span></span>  <span data-ttu-id="02d0f-1486">Diese Funktionen werden in einem späteren Build verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1486">Functionality will be available in a later build</span></span>
* <span data-ttu-id="02d0f-1487">top und htop werden jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="02d0f-1487">top and htop now display</span></span>
* <span data-ttu-id="02d0f-1488">Zusätzliche Fehlermeldungen bei einigen Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="02d0f-1488">Additional error messages for some install failures</span></span>
* <span data-ttu-id="02d0f-1489">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1489">Syscall improvements and bugfixes.</span></span>  <span data-ttu-id="02d0f-1490">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1490">Supported syscall list below.</span></span>
* <span data-ttu-id="02d0f-1491">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1491">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="02d0f-1492">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="02d0f-1492">Syscall Support</span></span>
<span data-ttu-id="02d0f-1493">Im folgenden finden Sie eine Liste der Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1493">Below is a list of syscalls that have some implementation in WSL.</span></span>  <span data-ttu-id="02d0f-1494">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02d0f-1494">Syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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
