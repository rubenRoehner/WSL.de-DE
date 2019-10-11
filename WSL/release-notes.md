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
ms.openlocfilehash: b92c20bad50d0c58da05bb0c8f26a69d4c0b2970
ms.sourcegitcommit: 050f6095e92469b903db8ddf9356df5b22b21804
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/03/2019
ms.locfileid: "71910300"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a><span data-ttu-id="9daaa-105">Anmerkungen zu dieser Version des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="9daaa-105">Release Notes for Windows Subsystem for Linux</span></span>

## <a name="build-18995"></a><span data-ttu-id="9daaa-106">Build 18995</span><span class="sxs-lookup"><span data-stu-id="9daaa-106">Build 18995</span></span>
<span data-ttu-id="9daaa-107">Allgemeine Windows-Informationen zu Build 18995 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/10/03/announcing-windows-10-insider-preview-build-18995/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-107">For general Windows information on build 18995 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/10/03/announcing-windows-10-insider-preview-build-18995/).</span></span>

* <span data-ttu-id="9daaa-108">[WSL2] Korrektur eines Problems, bei dem DrvFs-Einbindungen nach dem Abbruch eines Vorgangs (z.B. STRG-C) zu funktionieren aufhörten [GH 4377]</span><span class="sxs-lookup"><span data-stu-id="9daaa-108">[WSL2] Fix an issue where DrvFs mounts stopped working after an operation was interrupted (e.g. ctrl-c) [GH 4377]</span></span>
* <span data-ttu-id="9daaa-109">[WSL2] Korrektur der Verarbeitung sehr großer hvsocket-Nachrichten [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="9daaa-109">[WSL2] Fix handling of very large hvsocket messages [GH 4105]</span></span>
* <span data-ttu-id="9daaa-110">[WSL2] Korrektur eines Interop-Problems, wenn stdin eine Datei ist [GH 4475]</span><span class="sxs-lookup"><span data-stu-id="9daaa-110">[WSL2] Fix issue with interop when stdin is a file [GH 4475]</span></span>
* <span data-ttu-id="9daaa-111">[WSL2] Korrektur eines Absturzes, wenn ein unerwarteter Netzwerkstatus festgestellt wird [GH 4474]</span><span class="sxs-lookup"><span data-stu-id="9daaa-111">[WSL2] Fix service crash when unexpected network state is encountered [GH 4474]</span></span>
* <span data-ttu-id="9daaa-112">[WSL2] Abfragen des Namens der Distribution beim Interopserver, wenn der aktuelle Prozess nicht über die Umgebungsvariable verfügt</span><span class="sxs-lookup"><span data-stu-id="9daaa-112">[WSL2] Query the distro name from the interop server if the current process does not have the environment variable</span></span>
* <span data-ttu-id="9daaa-113">[WSL2] Korrektur eines Interop-Problems, wenn stdin eine Datei ist</span><span class="sxs-lookup"><span data-stu-id="9daaa-113">[WSL2] Fix issue with interop whe stdin is a file</span></span>
* <span data-ttu-id="9daaa-114">[WSL2] Aktualisieren der Linux-Kernelversion auf 4.19.72</span><span class="sxs-lookup"><span data-stu-id="9daaa-114">[WSL2] Update Linux kernel version to 4.19.72</span></span>
* <span data-ttu-id="9daaa-115">[WSL2] Neu hinzugefügte Möglichkeit zum Angeben weiterer Kernelbefehle in der Befehlszeile mithilfe von WSLCONFIG</span><span class="sxs-lookup"><span data-stu-id="9daaa-115">[WSL2] Add ability to specify additional kernel command line parameters via .wslconfig</span></span>
```
[wsl2]
kernelCommandLine = <string> # Additional kernel command line arguments

```

## <a name="build-18990"></a><span data-ttu-id="9daaa-116">Build 18990</span><span class="sxs-lookup"><span data-stu-id="9daaa-116">Build 18990</span></span>
<span data-ttu-id="9daaa-117">Allgemeine Windows-Informationen zu Build 18990 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-117">For general Windows information on build 18990 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span></span>

* <span data-ttu-id="9daaa-118">Verbesserte Leistung für Verzeichnisauflistungen in \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="9daaa-118">Improve the performance for directory listings in \\\\wsl$</span></span>
* <span data-ttu-id="9daaa-119">[WSL2] Einführen zusätzlicher Entropie beim Systemstart [GH 4416]</span><span class="sxs-lookup"><span data-stu-id="9daaa-119">[WSL2] Inject additional boot entropy [GH 4416]</span></span>
* <span data-ttu-id="9daaa-120">[WSL2] Problembehebung für Windows-Interop bei der Verwendung von „su“ / „sudo“ [GH 4465]</span><span class="sxs-lookup"><span data-stu-id="9daaa-120">[WSL2] Fix for Windows interop when using su / sudo [GH 4465]</span></span>


## <a name="build-18980"></a><span data-ttu-id="9daaa-121">Build 18980</span><span class="sxs-lookup"><span data-stu-id="9daaa-121">Build 18980</span></span>
<span data-ttu-id="9daaa-122">Allgemeine Windows-Informationen zu Build 18980 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-122">For general Windows information on build 18980 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span></span>

* <span data-ttu-id="9daaa-123">Korrektur des Lesen von symbolischen Verknüpfungen, die FILE_READ_DATA verweigern.</span><span class="sxs-lookup"><span data-stu-id="9daaa-123">Fix reading symlinks that deny FILE_READ_DATA.</span></span> <span data-ttu-id="9daaa-124">Dies umfasst alle symbolischen Verknüpfungen, die von Windows aus Gründen der Abwärtskompatibilität erstellt werden, z.B. „C:\Dokumente und Einstellungen“ und eine Reihe von symbolischen Verknüpfungen im Benutzerprofilverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="9daaa-124">This includes all the symlinks Windows creates for backwards compatibility such as "C:\Document and Settings" and a bunch of symlinks in the user profile directory</span></span>
* <span data-ttu-id="9daaa-125">Festlegen eines unerwarteten Dateisystemzustands als nicht schwerwiegend [GH 4334, 4305]</span><span class="sxs-lookup"><span data-stu-id="9daaa-125">Make unexpected filesystem state non-fatal [GH 4334, 4305]</span></span>
* <span data-ttu-id="9daaa-126">[WSL2] Hinzufügen von Unterstützung für arm64, wenn Ihre CPU/Firmware Virtualisierung unterstützt</span><span class="sxs-lookup"><span data-stu-id="9daaa-126">[WSL2] Add support for arm64 if your CPU / firmware supports virtualization</span></span>
* <span data-ttu-id="9daaa-127">[WSL2] Zulassen der Anzeige von Kernelprotokollen durch nicht berechtigte Benutzer</span><span class="sxs-lookup"><span data-stu-id="9daaa-127">[WSL2] Allow unprivileged users to view kernel log</span></span>
* <span data-ttu-id="9daaa-128">[WSL2] Korrigieren des Ausgaberelays, wenn stdout/stderr-Sockets geschlossen wurden [GH 4375]</span><span class="sxs-lookup"><span data-stu-id="9daaa-128">[WSL2] Fix output relay when stdout / stderr sockets have been closed [GH 4375]</span></span>
* <span data-ttu-id="9daaa-129">[WSL2] Unterstützung von Akku- und AC-Adapter-Passthrough</span><span class="sxs-lookup"><span data-stu-id="9daaa-129">[WSL2] Support battery and AC adapter passthrough</span></span>
* <span data-ttu-id="9daaa-130">[WSL2] Aktualisieren des Linux-Kernels auf 4.19.67</span><span class="sxs-lookup"><span data-stu-id="9daaa-130">[WSL2] Update Linux kernel to 4.19.67</span></span>
* <span data-ttu-id="9daaa-131">Hinzufügen der Möglichkeit, den Standardbenutzernamen in „/etc/wsl.conf“ festzulegen:</span><span class="sxs-lookup"><span data-stu-id="9daaa-131">Add the ability to set default username in /etc/wsl.conf:</span></span>
```
[user]
default=<string>
```

## <a name="build-18975"></a><span data-ttu-id="9daaa-132">Build 18975</span><span class="sxs-lookup"><span data-stu-id="9daaa-132">Build 18975</span></span>
<span data-ttu-id="9daaa-133">Allgemeine Windows-Informationen zu Build 18975 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-133">For general Windows information on build 18975 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span></span>

* <span data-ttu-id="9daaa-134">[WSL2] Korrektur einer Reihe von Problemen mit der localhost-Zuverlässigkeit [GH 4340]</span><span class="sxs-lookup"><span data-stu-id="9daaa-134">[WSL2] Fixed a number of localhost reliability issues [GH 4340]</span></span>

## <a name="build-18970"></a><span data-ttu-id="9daaa-135">Build 18970</span><span class="sxs-lookup"><span data-stu-id="9daaa-135">Build 18970</span></span>
<span data-ttu-id="9daaa-136">Allgemeine Windows-Informationen zu Build 18970 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-136">For general Windows information on build 18970 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span></span>

* <span data-ttu-id="9daaa-137">[WSL2] Synchronisierung der Uhrzeit mit der Hostzeit, wenn das System nach dem Ruhezustand fortgesetzt wird [GH 4245]</span><span class="sxs-lookup"><span data-stu-id="9daaa-137">[WSL2] Sync time with host time when system resumes from sleep state [GH 4245]</span></span>
* <span data-ttu-id="9daaa-138">[WSL2] Nach Möglichkeit Erstellen symbolischer NT-Verknüpfungen auf den Windows-Volumes</span><span class="sxs-lookup"><span data-stu-id="9daaa-138">[WSL2] Create NT symlinks on the Windows volumes when possible.</span></span>
* <span data-ttu-id="9daaa-139">[WSL2] Erstellen von Distributionen in den UTS-, IPC-, PID- und Mount-Namespaces.</span><span class="sxs-lookup"><span data-stu-id="9daaa-139">[WSL2] Create distros in UTS, IPC, PID, and Mount namespaces.</span></span>
* <span data-ttu-id="9daaa-140">[WSL2] Korrigieren des localhost-Portrelays, wenn der Server direkt an localhost gebunden wird [GH 4353]</span><span class="sxs-lookup"><span data-stu-id="9daaa-140">[WSL2] Fix localhost port relay when server binds to localhost directly [GH 4353]</span></span>
* <span data-ttu-id="9daaa-141">[WSL2] Korrigieren von Interop, wenn die Ausgabe umgeleitet wird [GH 4337]</span><span class="sxs-lookup"><span data-stu-id="9daaa-141">[WSL2] Fix interop when output is redirected [GH 4337]</span></span>
* <span data-ttu-id="9daaa-142">[WSL2] Unterstützung der Übersetzung absoluter symbolischer NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-142">[WSL2] Support translating absolute NT symlinks.</span></span>
* <span data-ttu-id="9daaa-143">[WSL2] Aktualisieren des Kernels auf 4.19.59</span><span class="sxs-lookup"><span data-stu-id="9daaa-143">[WSL2] Update kernel to 4.19.59</span></span>
* <span data-ttu-id="9daaa-144">[WSL2] Ordnungsgemäße Festlegung der Subnetzmaske für eth0.</span><span class="sxs-lookup"><span data-stu-id="9daaa-144">[WSL2] Properly set subnet mask for eth0.</span></span>
* <span data-ttu-id="9daaa-145">[WSL2] Ändern der Logik, um die Konsolenworkerschleife zu verlassen, wenn das Beendigungsereignis signalisiert wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-145">[WSL2] Change logic to break out of console worker loop when exit event is signaled.</span></span>
* <span data-ttu-id="9daaa-146">[WSL2] Auswerfen der Distributions-VHD, wenn die Distribution nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-146">[WSL2] Eject distribution vhd when the distro is not running.</span></span>
* <span data-ttu-id="9daaa-147">[WSL2] Korrigieren der Analysebibliothek, um leere Werte ordnungsgemäß zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-147">[WSL2] Fix config parsing library to correctly handle empty values.</span></span>
* <span data-ttu-id="9daaa-148">[WSL2] Unterstützung von Docker Desktop durch Erstellen von distributionsübergreifenden Einbindungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-148">[WSL2] Support Docker Desktop by creating cross distro mounts.</span></span> <span data-ttu-id="9daaa-149">Dieses Verhalten kann durch eine Distribution übernommen werden, indem die folgende Zeile der Datei „/etc/wsl.conf“ hinzugefügt wird:</span><span class="sxs-lookup"><span data-stu-id="9daaa-149">A distro can opt-in to this behavior by adding the following line to the /etc/wsl.conf file:</span></span>
```
[automount]
crossDistro = true
```

## <a name="build-18945"></a><span data-ttu-id="9daaa-150">Build 18945</span><span class="sxs-lookup"><span data-stu-id="9daaa-150">Build 18945</span></span>
<span data-ttu-id="9daaa-151">Allgemeine Windows-Informationen zu Build 18945 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-151">For general Windows information on build 18945 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-152">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-152">WSL</span></span>
* <span data-ttu-id="9daaa-153">[WSL2] Zulassen, dass der Zugriff auf lauschende TCP-Sockets in WSL2 über „localhost:port“ vom Host erfolgen kann.</span><span class="sxs-lookup"><span data-stu-id="9daaa-153">[WSL2] Allow listening tcp sockets in WSL2 to be accessible from the host by using localhost:port</span></span>
* <span data-ttu-id="9daaa-154">[WSL2] Korrekturen für Installations- und Konvertierungsfehler und zusätzliche Diagnose zur Nachverfolgung zukünftiger Probleme [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="9daaa-154">[WSL2] Fixes for install / conversion failures and additional diagnostics to track down future issues [GH 4105]</span></span> 
* <span data-ttu-id="9daaa-155">[WSL2] Verbessern der Diagnose von WSL2-Netzwerkproblemen</span><span class="sxs-lookup"><span data-stu-id="9daaa-155">[WSL2] Improve diagnosability of WSL2 network issues</span></span>
* <span data-ttu-id="9daaa-156">[WSL2] Aktualisieren der Kernelversion auf 4.19.55</span><span class="sxs-lookup"><span data-stu-id="9daaa-156">[WSL2] Update kernel version to 4.19.55</span></span>
* <span data-ttu-id="9daaa-157">[WSL2] Aktualisieren des Kernels mit Konfigurationsoptionen, die für Docker erforderlich sind [GH 4165]</span><span class="sxs-lookup"><span data-stu-id="9daaa-157">[WSL2] Update kernel with config options required for docker [GH 4165]</span></span>
* <span data-ttu-id="9daaa-158">[WSL2] Erhöhen der Anzahl der CPUs, die der Lightweight Utility-VM zugeordnet sind, um eine mit dem Host identische Anzahl zu erreichen (wurde zuvor durch CONFIG_NR_CPUS in der Kernelkonfiguration auf 8 begrenzt) [GH 4137]</span><span class="sxs-lookup"><span data-stu-id="9daaa-158">[WSL2] Increase the number of CPUs assigned to the lightweight utility VM to be the same as the host (was previously capped at 8 by CONFIG_NR_CPUS in the kernel config) [GH 4137]</span></span>
* <span data-ttu-id="9daaa-159">[WSL2] Erstellen einer Auslagerungsdatei für die WSL2-Lightweight-VM</span><span class="sxs-lookup"><span data-stu-id="9daaa-159">[WSL2] Create a swap file for the WSL2 lightweight VM</span></span>
* <span data-ttu-id="9daaa-160">[WSL2] Zulassen, dass Benutzereinbindungen über die \\\\wsl$\\-Distribution (z.B. sshfs) sichtbar sind [GH 4172]</span><span class="sxs-lookup"><span data-stu-id="9daaa-160">[WSL2] Allow user mounts to be visible via \\\\wsl$\\distro (for example sshfs) [GH 4172]</span></span>
* <span data-ttu-id="9daaa-161">[WSL2] Verbessern der Leistung des 9P-Dateisystems</span><span class="sxs-lookup"><span data-stu-id="9daaa-161">[WSL2] Improve 9p filesystem performance</span></span>
* <span data-ttu-id="9daaa-162">[WSL2] Sicherstellen, dass die VHD-ACL nicht unbegrenzt anwächst [GH 4126]</span><span class="sxs-lookup"><span data-stu-id="9daaa-162">[WSL2] Ensure vhd ACL does not grow unbounded [GH 4126]</span></span>
* <span data-ttu-id="9daaa-163">[WSL2] Aktualisieren der Kernelkonfiguration für die Unterstützung von squashfs und xt_conntrack [GH 4107, 4123]</span><span class="sxs-lookup"><span data-stu-id="9daaa-163">[WSL2] Update kernel config to support squashfs and xt_conntrack [GH 4107, 4123]</span></span>
* <span data-ttu-id="9daaa-164">[WSL2] Korrektur für interopaktivierte „/etc/wsl.conf“-Option [GH 4140]</span><span class="sxs-lookup"><span data-stu-id="9daaa-164">[WSL2] Fix for interop.enabled /etc/wsl.conf option [GH 4140]</span></span>
* <span data-ttu-id="9daaa-165">[WSL2] Rückgabe von ENOTSUP, wenn das Dateisystem EAS nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9daaa-165">[WSL2] Return ENOTSUP if the file system does not support EAs</span></span>
* <span data-ttu-id="9daaa-166">[WSL2] Korrigieren von CopyFile-Hänger mit \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="9daaa-166">[WSL2] Fix CopyFile hang with \\\\wsl$</span></span>
* <span data-ttu-id="9daaa-167">Umschalten von Standard-umask in 0022 und Hinzufügen der filesystem.umask-Einstellung zu „/etc/wsl.conf“</span><span class="sxs-lookup"><span data-stu-id="9daaa-167">Switch default umask to 0022 and add filesystem.umask setting to /etc/wsl.conf</span></span>
* <span data-ttu-id="9daaa-168">Korrigieren von wslpath, um symbolische Verknüpfungen ordnungsgemäß aufzulösen, dies wurde in 19h1 zurückgesetzt [GH 4078]</span><span class="sxs-lookup"><span data-stu-id="9daaa-168">Fix wslpath to properly resolve symlinks, this was regressed in 19h1 [GH 4078]</span></span>
* <span data-ttu-id="9daaa-169">Einführung der Datei „%UserProfile%\\.wslconfig“ für die Optimierung der WSL2-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-169">Introduce %UserProfile%\\.wslconfig file for tweaking WSL2 settings</span></span>
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

## <a name="build-18917"></a><span data-ttu-id="9daaa-170">Build 18917</span><span class="sxs-lookup"><span data-stu-id="9daaa-170">Build 18917</span></span>
<span data-ttu-id="9daaa-171">Allgemeine Windows-Informationen zu Build 18917 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-171">For general Windows information on build 18917 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-172">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-172">WSL</span></span>
* <span data-ttu-id="9daaa-173">WSL 2 ist Jetzt verfügbar!</span><span class="sxs-lookup"><span data-stu-id="9daaa-173">WSL 2 is now available!</span></span> <span data-ttu-id="9daaa-174">Weitere Informationen finden Sie im [Blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-174">Please see [blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) for more details.</span></span>
* <span data-ttu-id="9daaa-175">Korrektur einer Regression, bei der das Starten von Windows-Prozessen über symbolische Verknüpfungen nicht ordnungsgemäß funktioniert hat [GH 3999]</span><span class="sxs-lookup"><span data-stu-id="9daaa-175">Fix a regression where launching Windows processes via symlinks did not work correctly [GH 3999]</span></span>
* <span data-ttu-id="9daaa-176">Hinzufügen der Optionen wsl.exe --list --verbose, wsl.exe --list --quiet und wsl.exe --import --version zu „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="9daaa-176">Add wsl.exe --list --verbose, wsl.exe --list --quiet, and wsl.exe --import --version options to wsl.exe</span></span>
* <span data-ttu-id="9daaa-177">Hinzufügen der Option wsl.exe --shutdown</span><span class="sxs-lookup"><span data-stu-id="9daaa-177">Add wsl.exe --shutdown option</span></span>
* <span data-ttu-id="9daaa-178">Plan 9: Zulassen des Öffnend eines Verzeichnisses für einen erfolgreichen Schreibvorgang</span><span class="sxs-lookup"><span data-stu-id="9daaa-178">Plan 9: Allow opening a directory for write to succeed</span></span>

## <a name="build-18890"></a><span data-ttu-id="9daaa-179">Build 18890</span><span class="sxs-lookup"><span data-stu-id="9daaa-179">Build 18890</span></span>
<span data-ttu-id="9daaa-180">Allgemeine Windows-Informationen zu Build 18890 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-180">For general Windows information on build 18890 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-181">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-181">WSL</span></span>
* <span data-ttu-id="9daaa-182">Nicht blockierender Socketverlust [GH 2913]</span><span class="sxs-lookup"><span data-stu-id="9daaa-182">Non-blocking socket leak [GH 2913]</span></span>
* <span data-ttu-id="9daaa-183">EOF-Eingabe für Terminal kann nachfolgende Lesevorgänge blockieren [GH 3421]</span><span class="sxs-lookup"><span data-stu-id="9daaa-183">EOF input to terminal can block subsequent reads [GH 3421]</span></span>
* <span data-ttu-id="9daaa-184">Aktualisieren des resolv.conf-Headers, damit er auf „wsl.conf“ verweist [in GH 3928 beschrieben].</span><span class="sxs-lookup"><span data-stu-id="9daaa-184">Update resolv.conf header to refer to wsl.conf [discussed in GH 3928]</span></span>
* <span data-ttu-id="9daaa-185">Deadlock im epoll-Löschcode [GH 3922]</span><span class="sxs-lookup"><span data-stu-id="9daaa-185">Deadlock in epoll delete code [GH 3922]</span></span>
* <span data-ttu-id="9daaa-186">Verarbeiten von Leerzeichen in Argumenten für --import und --export [GH 3932]</span><span class="sxs-lookup"><span data-stu-id="9daaa-186">Handle spaces in arguments to --import and –export [GH 3932]</span></span>
* <span data-ttu-id="9daaa-187">Erweitern von mit mmap behandelten Dateien funktioniert nicht ordnungsgemäß [GH 3939]</span><span class="sxs-lookup"><span data-stu-id="9daaa-187">Extending mmap’d files does not work properly [GH 3939]</span></span>
* <span data-ttu-id="9daaa-188">Korrektur eines Problems mit ARM64 \\\\wsl$-Zugriff funktioniert nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="9daaa-188">Fix issue with ARM64 \\\\wsl$ access not working properly</span></span>
* <span data-ttu-id="9daaa-189">Hinzufügen eines besseren Standardsymbols für „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="9daaa-189">Add better default icon for wsl.exe</span></span>

## <a name="build-18342"></a><span data-ttu-id="9daaa-190">Build 18342</span><span class="sxs-lookup"><span data-stu-id="9daaa-190">Build 18342</span></span>
<span data-ttu-id="9daaa-191">Allgemeine Windows-Informationen zu Build 18342 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-191">For general Windows information on build 18342 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-192">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-192">WSL</span></span>
* <span data-ttu-id="9daaa-193">Wir haben für Benutzer die Möglichkeit hinzugefügt, auf Linux-Dateien in einer WSL-Distribution aus Windows zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-193">We've added the ability for users to access Linux files in a WSL distro from Windows.</span></span> <span data-ttu-id="9daaa-194">Auf diese Dateien kann über die Befehlszeile zugegriffen werden. Außerdem können Windows-Apps wie der Datei-Explorer, VSCode usw. mit diesen Dateien interagieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-194">These files can be accessed through the command line, and also Windows apps, like file explorer, VSCode, etc. can interact with these files.</span></span> <span data-ttu-id="9daaa-195">Greifen Sie auf Ihre Dateien zu, indem Sie zu \\\\wsl$\\<distributions_name> navigieren, oder zeigen Sie eine Liste der ausgeführten Distributionen an, indem Sie zu \\\\wsl$ navigieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-195">Access your files by navigating to \\\\wsl$\\<distro_name>, or see a list of running distributions by navigating to \\\\wsl$</span></span>
* <span data-ttu-id="9daaa-196">Hinzufügen zusätzlicher CPU-Infotags und Korrigieren der Cpus_allowed[_list]-Werte [GH 2234]</span><span class="sxs-lookup"><span data-stu-id="9daaa-196">Add additional CPU info tags and fix Cpus_allowed[_list] values [GH 2234]</span></span>
* <span data-ttu-id="9daaa-197">Unterstützung der Ausführung aus Nicht-Leaderthread [GH 3800]</span><span class="sxs-lookup"><span data-stu-id="9daaa-197">Support exec from non-leader thread [GH 3800]</span></span>
* <span data-ttu-id="9daaa-198">Behandeln von Konfigurationsupdatefehlern als nicht schwerwiegend [GH 3785]</span><span class="sxs-lookup"><span data-stu-id="9daaa-198">Treat configuration update failures as non-fatal [GH 3785]</span></span>
* <span data-ttu-id="9daaa-199">Aktualisieren von binfmt für die ordnungsgemäße Verarbeitung von Offsets [GH 3768]</span><span class="sxs-lookup"><span data-stu-id="9daaa-199">Update binfmt to properly handle offsets [GH 3768]</span></span>
* <span data-ttu-id="9daaa-200">Aktivieren der Zuordnung von Netzlaufwerken für Plan 9 [GH 3854]</span><span class="sxs-lookup"><span data-stu-id="9daaa-200">Enable mapping network drives for Plan 9 [GH 3854]</span></span>
* <span data-ttu-id="9daaa-201">Unterstützung von Windows -> Linux und Linux -> Windows-Pfadübersetzung für Bindungseinbindungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-201">Support Windows -> Linux and Linux -> Windows path translation for bind mounts</span></span>
* <span data-ttu-id="9daaa-202">Erstellen schreibgeschützter Abschnitte für Zuordnungen für Dateien, die schreibgeschützt geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="9daaa-202">Create read-only sections for mappings on files opened read-only</span></span>

## <a name="build-18334"></a><span data-ttu-id="9daaa-203">Build 18334</span><span class="sxs-lookup"><span data-stu-id="9daaa-203">Build 18334</span></span>
<span data-ttu-id="9daaa-204">Allgemeine Windows-Informationen zu Build 18334 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-204">For general Windows information on build 18334 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-205">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-205">WSL</span></span>
* <span data-ttu-id="9daaa-206">Umgestalten der Art und Weise, in der die Windows-Zeitzone einer Linux-Zeitzone zugeordnet wird [GH 3747]</span><span class="sxs-lookup"><span data-stu-id="9daaa-206">Redesign the way that Windows time zone is mapped to a  Linux time zone [GH 3747]</span></span>
* <span data-ttu-id="9daaa-207">Beheben von Speicherverlusten und Hinzufügen neuer Zeichenfolgenübersetzungsfunktionen [GH 3746]</span><span class="sxs-lookup"><span data-stu-id="9daaa-207">Fix memory leaks and add new string translation functions [GH 3746]</span></span>
* <span data-ttu-id="9daaa-208">SIGCONT für eine Threadgruppe ohne Threads ist eine Nulloperation [GH 3741]</span><span class="sxs-lookup"><span data-stu-id="9daaa-208">SIGCONT on a threadgroup with no threads is a no-op [GH 3741]</span></span> 
* <span data-ttu-id="9daaa-209">Richtige Anzeige von Socket- und Epoll-Dateideskriptoren in „/proc/self/fd“</span><span class="sxs-lookup"><span data-stu-id="9daaa-209">Correctly display socket and epoll file descriptors in /proc/self/fd</span></span>

## <a name="build-18305"></a><span data-ttu-id="9daaa-210">Build 18305</span><span class="sxs-lookup"><span data-stu-id="9daaa-210">Build 18305</span></span>
<span data-ttu-id="9daaa-211">Allgemeine Windows-Informationen zu Build 18305 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-211">For general Windows information on build 18305 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-212">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-212">WSL</span></span>
* <span data-ttu-id="9daaa-213">pthreads verlieren den Zugriff auf Dateien, wenn der primäre Thread beendet wird [GH 3589]</span><span class="sxs-lookup"><span data-stu-id="9daaa-213">pthreads lose access to files when the primary thread exits [GH 3589]</span></span>
* <span data-ttu-id="9daaa-214">TIOCSCTTY sollte den Parameter „force“ ignorieren, wenn er nicht erforderlich ist [GH 3652]</span><span class="sxs-lookup"><span data-stu-id="9daaa-214">TIOCSCTTY should ignore the “force” parameter unless it is required [GH 3652]</span></span>
* <span data-ttu-id="9daaa-215">Verbesserungen an der Befehlszeile von „wsl.exe“ und Hinzufügung von Import-/Exportfunktionen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-215">wsl.exe command line improvements and addition of import / export functionality.</span></span>
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

## <a name="build-18277"></a><span data-ttu-id="9daaa-216">Build 18277</span><span class="sxs-lookup"><span data-stu-id="9daaa-216">Build 18277</span></span>
<span data-ttu-id="9daaa-217">Allgemeine Windows-Informationen zu Build 18277 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-217">For general Windows information on build 18277 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-218">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-218">WSL</span></span>
* <span data-ttu-id="9daaa-219">Korrektur des Fehlers „no such interface supported“ in Build 18272 [GH 3645]</span><span class="sxs-lookup"><span data-stu-id="9daaa-219">Fix "no such interface supported" error introduced in build 18272 [GH 3645]</span></span>
* <span data-ttu-id="9daaa-220">Ignorieren des MNT_FORCE-Flags für Systemaufruf zum Aufheben der Einbindung [GH 3605]</span><span class="sxs-lookup"><span data-stu-id="9daaa-220">Ignore the MNT_FORCE flag for umount syscall [GH 3605]</span></span>
* <span data-ttu-id="9daaa-221">Umschalten von WSL-Interop für die Verwendung der offiziellen CreatePseudoConsole-API</span><span class="sxs-lookup"><span data-stu-id="9daaa-221">Switch WSL interop to use the official CreatePseudoConsole API</span></span>
* <span data-ttu-id="9daaa-222">Keinen Timeoutwert beibehalten, wenn FUTEX_WAIT neu gestartet wird</span><span class="sxs-lookup"><span data-stu-id="9daaa-222">Maintain no timeout value when FUTEX_WAIT restarts</span></span>

## <a name="build-18272"></a><span data-ttu-id="9daaa-223">Build 18272</span><span class="sxs-lookup"><span data-stu-id="9daaa-223">Build 18272</span></span>
<span data-ttu-id="9daaa-224">Allgemeine Windows-Informationen zu Build 18272 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-224">For general Windows information on build 18272 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-225">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-225">WSL</span></span>
* <span data-ttu-id="9daaa-226">**WARNUNG:** In diesem Build liegt ein Problem vor, durch das WSL nicht funktionsfähig wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-226">**WARNING:** There is an issue in this build that makes WSL inoperable.</span></span> <span data-ttu-id="9daaa-227">Wenn Sie versuchen, die Distribution zu starten, wird der Fehler „No such interface supported“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-227">When trying to launch your distribution you will see a “No such interface supported” error.</span></span> <span data-ttu-id="9daaa-228">Das Problem wurde behoben und ist im Insider Fast-Build der nächsten Woche nicht mehr enthalten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-228">The issue has been fixed and will be in next week's Insider Fast build.</span></span> <span data-ttu-id="9daaa-229">Wenn Sie diesen Build installiert haben, können Sie ein Rollback auf den vorherigen Windows-Build durchführen, indem Sie unter „Einstellungen > Update und Sicherheit > Wiederherstellung“ die Option „Zur vorherigen Version von Windows 10 zurückkehren“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-229">If you've installed this build you can roll back to the previous Windows build using “Go back to the previous version of Windows 10” in Settings->Update & Security->Recovery.</span></span>

## <a name="build-18267"></a><span data-ttu-id="9daaa-230">Build 18267</span><span class="sxs-lookup"><span data-stu-id="9daaa-230">Build 18267</span></span>
<span data-ttu-id="9daaa-231">Allgemeine Windows-Informationen zu Build 18267 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-231">For general Windows information on build 18267 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-232">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-232">WSL</span></span>
* <span data-ttu-id="9daaa-233">Korrektur eines Problems, bei dem der Zombieprozess möglicherweise nicht beendet und unbegrenzt ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-233">Fix issue where zombie process may not be reaped and remain indefinitely.</span></span>
* <span data-ttu-id="9daaa-234">WslRegisterDistribution hängt, wenn die Fehlermeldung die maximale Länge überschreitet [GH 3592]</span><span class="sxs-lookup"><span data-stu-id="9daaa-234">WslRegisterDistribution hangs if error message exceeds max length [GH 3592]</span></span>
* <span data-ttu-id="9daaa-235">Zulassen der erfolgreichen Ausführung von fsync für schreibgeschützte Dateien auf DrvFs [GH 3556]</span><span class="sxs-lookup"><span data-stu-id="9daaa-235">Allow fsync to succeed for read-only files on DrvFs [GH 3556]</span></span>
* <span data-ttu-id="9daaa-236">Sicherstellen, dass die Verzeichnisse „/bin“ und „/sbin“ vorhanden sind, bevor symbolische Verknüpfungen darin erstellt werden [GH 3584]</span><span class="sxs-lookup"><span data-stu-id="9daaa-236">Ensure that /bin and /sbin directories exist before creating symlinks inside [GH 3584]</span></span>
* <span data-ttu-id="9daaa-237">Hinzufügen eines Instanztimeoutmechanismus für WSL-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-237">Added an instance termination timeout mechanism for WSL instances.</span></span> <span data-ttu-id="9daaa-238">Der Timeoutwert ist derzeit auf 15 Sekunden festgelegt. Das bedeutet, dass die Instanz 15 Sekunden nach Beendigung des letzten WSL-Prozesses beendet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-238">The timeout is currently set to 15 seconds, meaning the instance will terminate 15 seconds after the last WSL process exits.</span></span> <span data-ttu-id="9daaa-239">Um eine Distribution sofort zu beenden, verwenden Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="9daaa-239">To terminate a distribution immediately, use:</span></span>
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a><span data-ttu-id="9daaa-240">Build 17763 (1809)</span><span class="sxs-lookup"><span data-stu-id="9daaa-240">Build 17763 (1809)</span></span>
<span data-ttu-id="9daaa-241">Allgemeine Windows-Informationen zu Build 17763 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-241">For general Windows information on build 17763 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-242">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-242">WSL</span></span>
* <span data-ttu-id="9daaa-243">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="9daaa-243">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="9daaa-244">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="9daaa-244">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="9daaa-245">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="9daaa-245">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="9daaa-246">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="9daaa-246">Better handling of threadgroup leader file descriptor cleanup.</span></span>
* <span data-ttu-id="9daaa-247">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="9daaa-247">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="9daaa-248">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="9daaa-248">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="9daaa-249">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="9daaa-249">Fix several AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="9daaa-250">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="9daaa-250">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>
* <span data-ttu-id="9daaa-251">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="9daaa-251">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="9daaa-252">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="9daaa-252">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="9daaa-253">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-253">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="9daaa-254">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="9daaa-254">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="9daaa-255">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9daaa-255">Pipe filesystem inadvertently clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9daaa-256">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9daaa-256">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>
* <span data-ttu-id="9daaa-257">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="9daaa-257">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="9daaa-258">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="9daaa-258">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="9daaa-259">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="9daaa-259">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="9daaa-260">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="9daaa-260">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="9daaa-261">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="9daaa-261">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="9daaa-262">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="9daaa-262">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="9daaa-263">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="9daaa-263">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="9daaa-264">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="9daaa-264">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="9daaa-265">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-265">Windows UI apps should execute even when launched in the background.</span></span>
* <span data-ttu-id="9daaa-266">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="9daaa-266">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="9daaa-267">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="9daaa-267">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="9daaa-268">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="9daaa-268">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="9daaa-269">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="9daaa-269">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="9daaa-270">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="9daaa-270">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="9daaa-271">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-271">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="9daaa-272">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="9daaa-272">Add wslconfig /terminate to stop running distributions.</span></span>
* <span data-ttu-id="9daaa-273">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="9daaa-273">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="9daaa-274">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="9daaa-274">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="9daaa-275">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-275">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="9daaa-276">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="9daaa-276">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="9daaa-277">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-277">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>
* <span data-ttu-id="9daaa-278">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="9daaa-278">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="9daaa-279">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="9daaa-279">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="9daaa-280">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-280">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="9daaa-281">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9daaa-281">Atomically create case sensitive directories in DrvFs.</span></span>
* <span data-ttu-id="9daaa-282">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-282">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9daaa-283">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9daaa-283">[GH 2712]</span></span>
* <span data-ttu-id="9daaa-284">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="9daaa-284">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="9daaa-285">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="9daaa-285">[GH 3020]</span></span>
* <span data-ttu-id="9daaa-286">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="9daaa-286">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="9daaa-287">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-287">To use, hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="9daaa-288">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="9daaa-288">Fix Unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="9daaa-289">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-289">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="9daaa-290">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="9daaa-290">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="9daaa-291">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="9daaa-291">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="9daaa-292">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="9daaa-292">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="9daaa-293">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-293">Add --distribution option for wsl.exe to select a specific distro.</span></span>
* <span data-ttu-id="9daaa-294">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="9daaa-294">Limited support for dmesg.</span></span> <span data-ttu-id="9daaa-295">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-295">Applications can now log to dmesg.</span></span> <span data-ttu-id="9daaa-296">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="9daaa-296">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="9daaa-297">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-297">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="9daaa-298">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-298">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="9daaa-299">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-299">`syslog` syscall interface is not yet supported.</span></span> <span data-ttu-id="9daaa-300">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-300">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="9daaa-301">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="9daaa-301">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="9daaa-302">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="9daaa-302">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="9daaa-303">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="9daaa-303">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="9daaa-304">Einige Zeichen (etwa „/“, „:“ und „\*“) sind unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-304">Some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-18252-skip-ahead"></a><span data-ttu-id="9daaa-305">Build 18252 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-305">Build 18252 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-306">Allgemeine Windows-Informationen zu Build 18252 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-306">For general Windows information on build 18252 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-307">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-307">WSL</span></span>
* <span data-ttu-id="9daaa-308">Verschieben von init- und bsdtar-Binärdateien aus der lxssmanager-DLL in einen separaten Toolsordner</span><span class="sxs-lookup"><span data-stu-id="9daaa-308">Move init and bsdtar binaries out of lxssmanager dll and into a separate tools folder</span></span>
* <span data-ttu-id="9daaa-309">Korrektur von Racebedingung um schließenden Dateideskriptor bei Verwendung von CLONE_FILES</span><span class="sxs-lookup"><span data-stu-id="9daaa-309">Fix race around closing file descriptor when using CLONE_FILES</span></span>
* <span data-ttu-id="9daaa-310">Verarbeiten optionaler Felder in „/proc/pid/mountinfo“ bei der Übersetzung von DrvFs-Pfaden</span><span class="sxs-lookup"><span data-stu-id="9daaa-310">Handle optional fields in /proc/pid/mountinfo when translating DrvFs paths</span></span>
* <span data-ttu-id="9daaa-311">Zulassen, dass DrvFs mklod ohne Metadatenunterstützung für S_IFREG erfolgreich ist</span><span class="sxs-lookup"><span data-stu-id="9daaa-311">Allow DrvFs mknod to succeed without metadata support for S_IFREG</span></span>
* <span data-ttu-id="9daaa-312">Für schreibgeschützte Dateien, die auf DrvFs erstellt wurden, muss das schreibgeschützte Attribut festgelegt werden [GH 3411]</span><span class="sxs-lookup"><span data-stu-id="9daaa-312">Readonly files created on DrvFs should have the readonly attribute set [GH 3411]</span></span>
* <span data-ttu-id="9daaa-313">Hinzufügen von /sbin/mount.drvfs-Hilfsprogramm zur Verarbeitung der DrvFs-Einbindung</span><span class="sxs-lookup"><span data-stu-id="9daaa-313">Add /sbin/mount.drvfs helper to handle DrvFs mounting</span></span>
* <span data-ttu-id="9daaa-314">Verwenden der POSIX-Umbenennung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9daaa-314">Use POSIX rename in DrvFs.</span></span>
* <span data-ttu-id="9daaa-315">Ermöglichen der Pfadübersetzung für Volumes ohne Volume-GUID.</span><span class="sxs-lookup"><span data-stu-id="9daaa-315">Allow path translation on volumes without a volume GUID.</span></span>

## <a name="build-17738-fast"></a><span data-ttu-id="9daaa-316">Build 17738 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9daaa-316">Build 17738 (Fast)</span></span>
<span data-ttu-id="9daaa-317">Allgemeine Windows-Informationen zu Build 17738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-317">For general Windows information on build 17738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-318">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-318">WSL</span></span>
* <span data-ttu-id="9daaa-319">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="9daaa-319">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="9daaa-320">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="9daaa-320">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="9daaa-321">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="9daaa-321">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="9daaa-322">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="9daaa-322">Better handling of threadgroup leader file descriptor cleanup.</span></span>

## <a name="build-17728-fast"></a><span data-ttu-id="9daaa-323">Build 17728 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9daaa-323">Build 17728 (Fast)</span></span>
<span data-ttu-id="9daaa-324">Allgemeine Windows-Informationen zu Build 17728 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-324">For general Windows information on build 17728 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-325">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-325">WSL</span></span>
* <span data-ttu-id="9daaa-326">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="9daaa-326">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="9daaa-327">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="9daaa-327">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="9daaa-328">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="9daaa-328">Fix a number of AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="9daaa-329">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="9daaa-329">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>

## <a name="build-18204-skip-ahead"></a><span data-ttu-id="9daaa-330">Build 18204 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-330">Build 18204 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-331">Allgemeine Windows-Informationen zu Build 18204 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-331">For general Windows information on build 18204 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-332">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-332">WSL</span></span>
* <span data-ttu-id="9daaa-333">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9daaa-333">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9daaa-334">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9daaa-334">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17723-fast"></a><span data-ttu-id="9daaa-335">Build 17723 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9daaa-335">Build 17723 (Fast)</span></span>
<span data-ttu-id="9daaa-336">Allgemeine Windows-Informationen zu Build 17723 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-336">For general Windows information on build 17723 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-337">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-337">WSL</span></span>
* <span data-ttu-id="9daaa-338">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="9daaa-338">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="9daaa-339">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="9daaa-339">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="9daaa-340">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-340">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="9daaa-341">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="9daaa-341">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="9daaa-342">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9daaa-342">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9daaa-343">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9daaa-343">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17713"></a><span data-ttu-id="9daaa-344">Build 17713</span><span class="sxs-lookup"><span data-stu-id="9daaa-344">Build 17713</span></span>
<span data-ttu-id="9daaa-345">Allgemeine Windows-Informationen zu Build 17713 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-345">For general Windows information on build 17713 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-346">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-346">WSL</span></span>
* <span data-ttu-id="9daaa-347">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="9daaa-347">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="9daaa-348">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="9daaa-348">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="9daaa-349">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="9daaa-349">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="9daaa-350">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="9daaa-350">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="9daaa-351">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="9daaa-351">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="9daaa-352">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="9daaa-352">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="9daaa-353">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="9daaa-353">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="9daaa-354">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="9daaa-354">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="9daaa-355">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-355">Windows UI apps should execute even when launched in the background.</span></span>

## <a name="build-17704"></a><span data-ttu-id="9daaa-356">Build 17704</span><span class="sxs-lookup"><span data-stu-id="9daaa-356">Build 17704</span></span>
<span data-ttu-id="9daaa-357">Allgemeine Windows-Informationen zu Build 17704 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-357">For general Windows information on build 17704 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-358">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-358">WSL</span></span>
* <span data-ttu-id="9daaa-359">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="9daaa-359">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="9daaa-360">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="9daaa-360">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="9daaa-361">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="9daaa-361">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="9daaa-362">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="9daaa-362">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="9daaa-363">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="9daaa-363">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="9daaa-364">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-364">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="9daaa-365">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="9daaa-365">Add wslconfig /terminate to stop running distributions.</span></span>

## <a name="build-17692"></a><span data-ttu-id="9daaa-366">Build 17692</span><span class="sxs-lookup"><span data-stu-id="9daaa-366">Build 17692</span></span>
<span data-ttu-id="9daaa-367">Allgemeine Windows-Informationen zu Build 17692 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span><span class="sxs-lookup"><span data-stu-id="9daaa-367">For general Windows information on build 17692 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-368">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-368">WSL</span></span>
* <span data-ttu-id="9daaa-369">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="9daaa-369">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="9daaa-370">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="9daaa-370">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="9daaa-371">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-371">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="9daaa-372">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="9daaa-372">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="9daaa-373">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-373">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>

## <a name="build-17686"></a><span data-ttu-id="9daaa-374">Build 17686</span><span class="sxs-lookup"><span data-stu-id="9daaa-374">Build 17686</span></span>
<span data-ttu-id="9daaa-375">Allgemeine Windows-Informationen zu Build 17686 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span><span class="sxs-lookup"><span data-stu-id="9daaa-375">For general Windows information on build 17686 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-376">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-376">WSL</span></span>
* <span data-ttu-id="9daaa-377">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="9daaa-377">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="9daaa-378">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="9daaa-378">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="9daaa-379">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-379">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="9daaa-380">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9daaa-380">Atomically create case sensitive directories in DrvFs.</span></span>

## <a name="build-17677"></a><span data-ttu-id="9daaa-381">Build 17677</span><span class="sxs-lookup"><span data-stu-id="9daaa-381">Build 17677</span></span>
<span data-ttu-id="9daaa-382">Allgemeine Windows-Informationen zu Build 17677 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-382">For general Windows information on build 17677 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-383">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-383">WSL</span></span>
* <span data-ttu-id="9daaa-384">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-384">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9daaa-385">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9daaa-385">[GH 2712]</span></span>
* <span data-ttu-id="9daaa-386">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="9daaa-386">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="9daaa-387">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="9daaa-387">[GH 3020]</span></span>

## <a name="build-17666"></a><span data-ttu-id="9daaa-388">Build 17666</span><span class="sxs-lookup"><span data-stu-id="9daaa-388">Build 17666</span></span>
<span data-ttu-id="9daaa-389">Allgemeine Windows-Informationen zu Build 17666 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-389">For general Windows information on build 17666 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-390">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-390">WSL</span></span>
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a><span data-ttu-id="9daaa-391">WARNUNG: Es gibt ein Problem, das das Ausführen von WSL in einigen AMD-Chipsätzen verhindert [GH 3134].</span><span class="sxs-lookup"><span data-stu-id="9daaa-391">WARNING: There is an issue preventing WSL from running on some AMD chipsets [GH 3134].</span></span> <span data-ttu-id="9daaa-392">Eine Korrektur ist verfügbar und wird in den Insider Build-Branch integriert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-392">A fix is ready and making its way to the Insider Build branch.</span></span>
* <span data-ttu-id="9daaa-393">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="9daaa-393">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="9daaa-394">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-394">To use hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="9daaa-395">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="9daaa-395">Fix unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="9daaa-396">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-396">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="9daaa-397">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="9daaa-397">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="9daaa-398">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="9daaa-398">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="9daaa-399">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="9daaa-399">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="9daaa-400">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-400">Add --distribution option for wsl.exe to select a specific distro.</span></span>

## <a name="build-17655-skip-ahead"></a><span data-ttu-id="9daaa-401">Build 17655 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-401">Build 17655 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-402">Allgemeine Windows-Informationen zu Build 17655 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-402">For general Windows information on build 17655 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-403">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-403">WSL</span></span>
* <span data-ttu-id="9daaa-404">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="9daaa-404">Limited support for dmesg.</span></span> <span data-ttu-id="9daaa-405">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-405">Applications can now log to dmesg.</span></span> <span data-ttu-id="9daaa-406">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="9daaa-406">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="9daaa-407">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-407">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="9daaa-408">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-408">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="9daaa-409">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-409">`syslog` sycall interface is not yet supported.</span></span> <span data-ttu-id="9daaa-410">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-410">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="9daaa-411">Korrektur eines Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-411">Fixed an issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9daaa-412">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9daaa-412">[GH 2712]</span></span>

## <a name="build-17639-skip-ahead"></a><span data-ttu-id="9daaa-413">Build 17639 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-413">Build 17639 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-414">Allgemeine Windows-Informationen zu Build 17639 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-414">For general Windows information on build 17639 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-415">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-415">WSL</span></span>
* <span data-ttu-id="9daaa-416">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="9daaa-416">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="9daaa-417">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="9daaa-417">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="9daaa-418">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="9daaa-418">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="9daaa-419">Insbesondere sind einige Zeichen (etwa „/“, „:“ und „\*“) unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-419">In particular, some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-17133-fast"></a><span data-ttu-id="9daaa-420">Build 17133 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9daaa-420">Build 17133 (Fast)</span></span>
<span data-ttu-id="9daaa-421">Allgemeine Windows-Informationen zu Build 17133 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-421">For general Windows information on build 17133 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-422">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-422">WSL</span></span>
* <span data-ttu-id="9daaa-423">Fehlerbehebung für Hängen in WSL.</span><span class="sxs-lookup"><span data-stu-id="9daaa-423">Fix for hang in WSL.</span></span> <span data-ttu-id="9daaa-424">[GH 3039, 3034]</span><span class="sxs-lookup"><span data-stu-id="9daaa-424">[GH 3039, 3034]</span></span>

## <a name="build-17128-fast"></a><span data-ttu-id="9daaa-425">Build 17128 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9daaa-425">Build 17128 (Fast)</span></span>
<span data-ttu-id="9daaa-426">Allgemeine Windows-Informationen zu Build 17128 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-426">For general Windows information on build 17128 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-427">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-427">WSL</span></span>
* <span data-ttu-id="9daaa-428">Keine</span><span class="sxs-lookup"><span data-stu-id="9daaa-428">None</span></span>

## <a name="build-17627-skip-ahead"></a><span data-ttu-id="9daaa-429">Build 17627 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-429">Build 17627 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-430">Allgemeine Windows-Informationen zu Build 17627 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-430">For general Windows information on build 17627 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-431">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-431">WSL</span></span>
* <span data-ttu-id="9daaa-432">Hinzufügen von Unterstützung für futex-pi-fähige Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="9daaa-432">Add support for the futex pi-aware operations.</span></span> <span data-ttu-id="9daaa-433">[GH 1006]</span><span class="sxs-lookup"><span data-stu-id="9daaa-433">[GH 1006]</span></span>
    * <span data-ttu-id="9daaa-434">Beachten Sie, dass Prioritäten derzeit keine unterstützte WSL-Funktion sind, sodass Einschränkungen bestehen. Die Standardverwenund sollte jedoch aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-434">Note that priorities are not currently a supported WSL feature so there are limitations, but standard usage should be unblocked.</span></span>
* <span data-ttu-id="9daaa-435">Windows-Firewallunterstützung für WSL-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="9daaa-435">Windows firewall support for WSL processes.</span></span> <span data-ttu-id="9daaa-436">[GH 1852]</span><span class="sxs-lookup"><span data-stu-id="9daaa-436">[GH 1852]</span></span>
    * <span data-ttu-id="9daaa-437">Um beispielsweise zuzulassen, dass der WSL python-Prozess an einem beliebigen Port lauschen kann, verwenden Sie Windows-CMD mit erhöhten Rechten: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span><span class="sxs-lookup"><span data-stu-id="9daaa-437">For example, to allow the WSL python process to listen on any port, use the elevated Windows cmd: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span></span>
    * <span data-ttu-id="9daaa-438">Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link.](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span><span class="sxs-lookup"><span data-stu-id="9daaa-438">For additional details on how to add firewall rules, see [link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span></span>
* <span data-ttu-id="9daaa-439">Beachten der Standardshell des Benutzers bei der Verwendung von „wsl.exe“.</span><span class="sxs-lookup"><span data-stu-id="9daaa-439">Respect user's default shell when using wsl.exe.</span></span> <span data-ttu-id="9daaa-440">[GH 2372]</span><span class="sxs-lookup"><span data-stu-id="9daaa-440">[GH 2372]</span></span>
* <span data-ttu-id="9daaa-441">Melden aller Netzwerkschnittstellen als Ethernet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-441">Report all network interfaces as ethernet.</span></span> <span data-ttu-id="9daaa-442">[GH 2996]</span><span class="sxs-lookup"><span data-stu-id="9daaa-442">[GH 2996]</span></span>
* <span data-ttu-id="9daaa-443">Bessere Verarbeitung von beschädigten /etc/passwd-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9daaa-443">Better handling of corrupt /etc/passwd file.</span></span> <span data-ttu-id="9daaa-444">[GH 3001]</span><span class="sxs-lookup"><span data-stu-id="9daaa-444">[GH 3001]</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-445">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-445">Console</span></span>
* <span data-ttu-id="9daaa-446">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-446">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-447">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-447">LTP Results:</span></span>
<span data-ttu-id="9daaa-448">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-448">Testing in progress.</span></span>

## <a name="build-17618-skip-ahead"></a><span data-ttu-id="9daaa-449">Build 17618 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9daaa-449">Build 17618 (Skip Ahead)</span></span>
<span data-ttu-id="9daaa-450">Allgemeine Windows-Informationen zu Build 17618 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-450">For general Windows information on build 17618 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-451">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-451">WSL</span></span>
* <span data-ttu-id="9daaa-452">Einführung in Pseudoconsolenfunktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span><span class="sxs-lookup"><span data-stu-id="9daaa-452">Introduce pseudoconsole functionality for NT interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span></span>
* <span data-ttu-id="9daaa-453">Der Legacyinstallationsmechanismus („lxrun.exe“) ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-453">The legacy install mechanism (lxrun.exe) has been deprecated.</span></span> <span data-ttu-id="9daaa-454">Der unterstützte Mechanismus zum Installieren von Distributionen ist der Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="9daaa-454">The supported mechanism for installing distributions is through the Microsoft Store.</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-455">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-455">Console</span></span>
* <span data-ttu-id="9daaa-456">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-456">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-457">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-457">LTP Results:</span></span>
<span data-ttu-id="9daaa-458">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-458">Testing in progress.</span></span>

## <a name="build-17110"></a><span data-ttu-id="9daaa-459">Build 17110</span><span class="sxs-lookup"><span data-stu-id="9daaa-459">Build 17110</span></span>
<span data-ttu-id="9daaa-460">Allgemeine Windows-Informationen zu Build 17110 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-460">For general Windows information on build 17110 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-461">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-461">WSL</span></span>
* <span data-ttu-id="9daaa-462">Zulassen, dass /init aus Windows beendet wird [GH 2928].</span><span class="sxs-lookup"><span data-stu-id="9daaa-462">Allow /init to be terminated from Windows [GH 2928].</span></span>
* <span data-ttu-id="9daaa-463">DrvFs verwendet nun standardmäßig Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis (entspricht der Einbindungsoption „case=dir“).</span><span class="sxs-lookup"><span data-stu-id="9daaa-463">DrvFs now uses per-directory case sensitivity by default (equivalent to the “case=dir” mount option).</span></span>
    * <span data-ttu-id="9daaa-464">Wenn Sie „case=force“ verwenden (das alte Verhalten), muss ein Registrierungsschlüssel festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-464">Using “case=force” (the old behavior) requires setting a registry key.</span></span> <span data-ttu-id="9daaa-465">Führen Sie den folgenden Befehl aus, um „case=force“ zu aktivieren, wenn Sie diese Option verwenden müssen: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span><span class="sxs-lookup"><span data-stu-id="9daaa-465">Run the following command to enable “case=force” if you need to use it: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span></span>
    * <span data-ttu-id="9daaa-466">Wenn Sie über vorhandene Verzeichnisse verfügen, die mit WSL in einer älteren Version von Windows erstellt wurden, bei denen die Groß-/Kleinschreibung beachtet werden muss, verwenden Sie „fsutil.exe“, um sie für Unterscheidung von Groß-/Kleinschreibung zu markieren: fsutil.exe file setcasesensitiveinfo <path> enable</span><span class="sxs-lookup"><span data-stu-id="9daaa-466">If you have existing directories created with WSL in older version of Windows which need to be case sensitive, use fsutil.exe to mark them as case sensitive: fsutil.exe file setcasesensitiveinfo <path> enable</span></span>
* <span data-ttu-id="9daaa-467">NULL-Beendigungszeichenfolgen werden vom uname-Systemaufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-467">NULL terminate strings returned from the uname syscall.</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-468">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-468">Console</span></span>
* <span data-ttu-id="9daaa-469">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-469">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-470">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-470">LTP Results:</span></span>
<span data-ttu-id="9daaa-471">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-471">Testing in progress.</span></span>

## <a name="build-17107"></a><span data-ttu-id="9daaa-472">Build 17107</span><span class="sxs-lookup"><span data-stu-id="9daaa-472">Build 17107</span></span>
<span data-ttu-id="9daaa-473">Allgemeine Windows-Informationen zu Build 17107 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-473">For general Windows information on build 17107 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-474">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-474">WSL</span></span>
* <span data-ttu-id="9daaa-475">Unterstützung von TCSETSF und TCSETSW für pty-Masterendpunkte [GH 2552].</span><span class="sxs-lookup"><span data-stu-id="9daaa-475">Support TCSETSF and TCSETSW on master pty endpoints [GH 2552].</span></span>
* <span data-ttu-id="9daaa-476">Starten von gleichzeitigen Interop-Prozessen kann zu EINVAL führen [GH 2813].</span><span class="sxs-lookup"><span data-stu-id="9daaa-476">Starting simultaneous interop processes can result in EINVAL [GH 2813].</span></span>
* <span data-ttu-id="9daaa-477">Korrektur von PTRACE_ATTACH, um den richtigen Ablaufverfolgungsstatus in „/proc/pid/status“ anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-477">Fix PTRACE_ATTACH to show proper tracing status in /proc/pid/status.</span></span>
* <span data-ttu-id="9daaa-478">Korrektur der Racebedingung, bei der kurzlebige Prozesse, die mit den CLEARTID- und SETTID-Flags geklont wurden, ohne Löschen der TID-Adresse beendet werden konnten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-478">Fix race where short-lived processes cloned with both the CLEARTID and SETTID flags could exit without clearing the TID address.</span></span>
* <span data-ttu-id="9daaa-479">Anzeigen einer Meldung beim Aktualisieren der Linux-Dateisystemverzeichnisse beim Umstieg von einem Build vor 17093.</span><span class="sxs-lookup"><span data-stu-id="9daaa-479">Display a message when upgrading the Linux file system directories when moving from a pre-17093 build.</span></span> <span data-ttu-id="9daaa-480">Weitere Informationen zu den Änderungen für das 17093-Dateisystem finden Sie in den Anmerkungen zur Version für [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span><span class="sxs-lookup"><span data-stu-id="9daaa-480">For more details on the 17093 file system changes, see the release notes for [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-481">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-481">Console</span></span>
* <span data-ttu-id="9daaa-482">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-482">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-483">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-483">LTP Results:</span></span>
<span data-ttu-id="9daaa-484">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-484">Testing in progress.</span></span>

## <a name="build-17101"></a><span data-ttu-id="9daaa-485">Build 17101</span><span class="sxs-lookup"><span data-stu-id="9daaa-485">Build 17101</span></span>
<span data-ttu-id="9daaa-486">Allgemeine Windows-Informationen zu Build 17101 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-486">For general Windows information on build 17101 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-487">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-487">WSL</span></span>
* <span data-ttu-id="9daaa-488">Unterstützung für signalfd.</span><span class="sxs-lookup"><span data-stu-id="9daaa-488">Support for signalfd.</span></span> <span data-ttu-id="9daaa-489">[GH 129]</span><span class="sxs-lookup"><span data-stu-id="9daaa-489">[GH 129]</span></span>
* <span data-ttu-id="9daaa-490">Unterstützung von Dateinamen, die ungültige NTFS-Zeichen enthalten, durch Codieren als private Unicode-Zeichen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-490">Support file-names containing illegal NTFS characters by encoding them as private Unicode characters.</span></span> <span data-ttu-id="9daaa-491">[GH 1514]</span><span class="sxs-lookup"><span data-stu-id="9daaa-491">[GH 1514]</span></span>
* <span data-ttu-id="9daaa-492">Automatisches Einbinden greift auf den schreibgeschützten Modus zurück, wenn Schreibvorgänge nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-492">Auto mount will fallback to read-only when write is not supported.</span></span> <span data-ttu-id="9daaa-493">[GH 2603]</span><span class="sxs-lookup"><span data-stu-id="9daaa-493">[GH 2603]</span></span>
* <span data-ttu-id="9daaa-494">Ermöglichen des Einfügens von Unicode-Ersatzzeichenpaaren (z.B. Emojis).</span><span class="sxs-lookup"><span data-stu-id="9daaa-494">Allow pasting of Unicode surrogate pairs (like emoji characters).</span></span> <span data-ttu-id="9daaa-495">[GH 2765]</span><span class="sxs-lookup"><span data-stu-id="9daaa-495">[GH 2765]</span></span>
* <span data-ttu-id="9daaa-496">Pseudodateien in „/proc“ und „/sys“ sollten „read“ und „write ready“ aus select, poll, epoll, usw. zurückgeben [GH 2838].</span><span class="sxs-lookup"><span data-stu-id="9daaa-496">Pseudo-files in /proc and /sys should return read and write ready from select, poll, epoll, et al. [GH 2838]</span></span>
* <span data-ttu-id="9daaa-497">Korrektur eines Problems, das dazu führen kann, dass der Dienst in eine Endlosschleife übergeht, wenn die Registrierung manipuliert wurde oder beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-497">Fix issue that could cause service to go into infinite loop when the registry has been tampered with or is corrupt.</span></span>
* <span data-ttu-id="9daaa-498">Korrektur von Netlink-Nachrichten, sodass sie mit neueren Versionen von iproute2 (upstream 4.14) funktionieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-498">Fix netlink messages to work with newer (upstream 4.14) version of iproute2.</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-499">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-499">Console</span></span>
* <span data-ttu-id="9daaa-500">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-500">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-501">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-501">LTP Results:</span></span>
<span data-ttu-id="9daaa-502">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-502">Testing in progress.</span></span>

## <a name="build-17093"></a><span data-ttu-id="9daaa-503">Build 17093</span><span class="sxs-lookup"><span data-stu-id="9daaa-503">Build 17093</span></span>
<span data-ttu-id="9daaa-504">Allgemeine Windows-Informationen zu Build 17093 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-504">For general Windows information on build 17093 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span></span>

#### <a name="important"></a><span data-ttu-id="9daaa-505">Wichtig:</span><span class="sxs-lookup"><span data-stu-id="9daaa-505">Important:</span></span>
<span data-ttu-id="9daaa-506">Wenn Sie WSL zum ersten Mal nach dem Upgrade auf diesen Build starten, müssen Sie einige Aufgaben durchführen, um die Linux-Dateisystemverzeichnisse zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-506">When starting WSL for the first time after upgrading to this build, it needs to perform some work upgrading the Linux file system directories.</span></span> <span data-ttu-id="9daaa-507">Dieser Vorgang kann einige Minuten in Anspruch nehmen, sodass WSL möglicherweise langsam zu starten scheint.</span><span class="sxs-lookup"><span data-stu-id="9daaa-507">This may take up to several minutes, so WSL may appear to start slowly.</span></span> <span data-ttu-id="9daaa-508">Dies sollte nur ein Mal für jede Distribution erfolgen, die Sie aus dem Store installiert haben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-508">This should only happen once for each distribution you have installed from the store.</span></span>
* <span data-ttu-id="9daaa-509">Verbesserte Unterscheidung von Groß-/Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9daaa-509">Improved case sensitivity support in DrvFs.</span></span>
    * <span data-ttu-id="9daaa-510">DrvFs unterstützt jetzt Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="9daaa-510">DrvFs now supports per-directory case sensitivity.</span></span> <span data-ttu-id="9daaa-511">Dies ist ein neues Flag, das für Verzeichnisse festgelegt werden kann, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen mit Unterscheidung zwischen Groß-/Kleinschreibung behandelt werden sollen, sodass sogar Windows-Anwendungen Dateien ordnungsgemäß öffnen können, bei denen sich nur die Groß-/Kleinschreibung unterscheidet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-511">This is a new flag that can be set on directories to indicate all operations in those directories should be treated as case sensitive, which allows even Windows applications to correctly open files that differ only by case.</span></span>
    * <span data-ttu-id="9daaa-512">DrvFs verfügt über neue Einbindungsoptionen, die die Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis steuern.</span><span class="sxs-lookup"><span data-stu-id="9daaa-512">DrvFs has new mount options controlling case sensitivity on a per-directory basis</span></span>
        * <span data-ttu-id="9daaa-513">case=force: Für alle Verzeichnisse wird zwischen Groß-/Kleinschreibung unterschieden (mit Ausnahme des Laufwerkstamms).</span><span class="sxs-lookup"><span data-stu-id="9daaa-513">case=force: all directories are treated as case sensitive (except for the drive root).</span></span> <span data-ttu-id="9daaa-514">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-514">New directories created with WSL are marked as case sensitive.</span></span> <span data-ttu-id="9daaa-515">Dies ist das Legacyverhalten (ausgenommen, wenn neue Verzeichnisse für Unterscheidung zwischen Groß-/Kleinschreibung markiert werden).</span><span class="sxs-lookup"><span data-stu-id="9daaa-515">This is the legacy behavior except for marking new directories case sensitive.</span></span>
        * <span data-ttu-id="9daaa-516">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-516">case=dir: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="9daaa-517">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-517">New directories created with WSL are marked as case sensitive.</span></span>
        * <span data-ttu-id="9daaa-518">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-518">case=off: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="9daaa-519">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-519">New directories created with WSL are marked as case insensitive.</span></span>
    * <span data-ttu-id="9daaa-520">Hinweis: Für Verzeichnisse, die in früheren Versionen von WSL erstellt wurden, ist dieses Flag nicht festgelegt, sodass bei Verwendung der Option „case=dir“ keine Groß-/Kleinschreibung beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-520">Note: directories created by WSL in previous releases do not have this flag set, so will not be treated as case sensitive if you use the “case=dir” option.</span></span> <span data-ttu-id="9daaa-521">Eine Möglichkeit, dieses Flag für vorhandene Verzeichnisse festzulegen, ist in Kürze verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9daaa-521">A way to set this flag on existing directories is coming soon.</span></span>
    * <span data-ttu-id="9daaa-522">Beispiel für die Einbindung mit diesen Optionen (für vorhandene Laufwerke müssen Sie zuerst die Einbindung aufheben, bevor Sie die Einbindung mit anderen Optionen ausführen können): sudo mount -t drvfs C: /mnt/c -o case=dir</span><span class="sxs-lookup"><span data-stu-id="9daaa-522">Example of mounting with these options (for existing drives, you must first unmount before you can mount with different options): sudo mount -t drvfs C: /mnt/c -o case=dir</span></span>
    * <span data-ttu-id="9daaa-523">Momentan ist case=force immer noch die Standardoption.</span><span class="sxs-lookup"><span data-stu-id="9daaa-523">For now, case=force is still the default option.</span></span> <span data-ttu-id="9daaa-524">Dies wird in Zukunft in case=dir geändert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-524">This will be changed to case=dir in the future.</span></span>
* <span data-ttu-id="9daaa-525">Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, wenn Sie DrvFs einbinden, z.B. sudo mount -t drvfs //server/share /mnt/share</span><span class="sxs-lookup"><span data-stu-id="9daaa-525">You can now use forward slashes in Windows paths when mounting DrvFs, e.g.: sudo mount -t drvfs //server/share /mnt/share</span></span>
* <span data-ttu-id="9daaa-526">WSL verarbeitet nun die /etc/fstab-Datei während des Instanzstarts [GH 2636].</span><span class="sxs-lookup"><span data-stu-id="9daaa-526">WSL now processes the /etc/fstab file during instance start [GH 2636].</span></span>
    * <span data-ttu-id="9daaa-527">Dies erfolgt vor der automatischen Einbindung von DrvFs-Laufwerken. Alle Laufwerke, die bereits von fstab eingebunden wurden, werden nicht automatisch erneut eingebunden, sodass Sie den Einbindungspunkt für bestimmte Laufwerke ändern können.</span><span class="sxs-lookup"><span data-stu-id="9daaa-527">This is done prior to automatically mounting DrvFs drives; any drives that were already mounted by fstab will not be remounted automatically, allowing you to change the mount point for specific drives.</span></span>
    * <span data-ttu-id="9daaa-528">Dieses Verhalten kann mithilfe von „wsl.conf“ deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-528">This behavior can be turned off using wsl.conf.</span></span>
* <span data-ttu-id="9daaa-529">Die mount, mountinfo- und mountstats-Dateien in „/proc“ versehen Sonderzeichen wie umgekehrte Schrägstriche und Leerzeichen ordnungsgemäß mit Escapezeichen [GH 2799]</span><span class="sxs-lookup"><span data-stu-id="9daaa-529">The mount, mountinfo and mountstats files in /proc properly escape special characters like backslashes and spaces [GH 2799]</span></span>
* <span data-ttu-id="9daaa-530">Spezielle Dateien, die mit DrvFs erstellt werden (z.B. symbolische WSL-Verknüpfungen oder Fifos und Sockets, wenn Metadaten aktiviert sind), können nun aus Windows kopiert und verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-530">Special files created with DrvFs such as WSL symbolic links, or fifos and sockets when metadata is enabled, can now be copied and moved from Windows.</span></span>

#### <a name="wsl-is-more-configurable-with-wslconf"></a><span data-ttu-id="9daaa-531">WSL ist mit „wsl.conf“ besser konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="9daaa-531">WSL is more configurable with wsl.conf</span></span>
<span data-ttu-id="9daaa-532">Es wurde eine Methode zum automatischen Konfigurieren bestimmter Funktionen in WSL hinzugefügt, die jedes Mal angewendet wird, wenn Sie das Subsystem starten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-532">We added a method for you to automatically configure certain functionality in WSL that will be applied every time you launch the subsystem.</span></span> <span data-ttu-id="9daaa-533">Dies umfasst Optionen für die automatische Einbindung und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9daaa-533">This includes automount options and network configuration.</span></span> <span data-ttu-id="9daaa-534">Weitere Informationen hierzu finden Sie in unserem Blogbeitrag unter: https://aka.ms/wslconf</span><span class="sxs-lookup"><span data-stu-id="9daaa-534">Learn more about it in our blog post at: https://aka.ms/wslconf</span></span>

#### <a name="af_unix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a><span data-ttu-id="9daaa-535">AF_UNIX ermöglicht Socketverbindungen zwischen Linux-Prozessen für WSL- und native Windows-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="9daaa-535">AF_UNIX allows socket connections between Linux processes on WSL and Windows native processes</span></span>
<span data-ttu-id="9daaa-536">WSL- und Windows-Anwendungen können nun über Unix-Sockets miteinander kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-536">WSL and Windows applications can now communicate with each other over Unix sockets.</span></span> <span data-ttu-id="9daaa-537">Stellen Sie sich vor, Sie möchten einen Dienst in Windows ausführen und sowohl für Windows- als auch für WSL-Apps verfügbar machen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-537">Imagine you want to run a service in Windows and make it available to both Windows and WSL apps.</span></span> <span data-ttu-id="9daaa-538">Das ist nun mit UNIX-Sockets möglich.</span><span class="sxs-lookup"><span data-stu-id="9daaa-538">Now, that’s possible with Unix sockets.</span></span> <span data-ttu-id="9daaa-539">Weitere Informationen finden Sie in unserem Blogbeitrag unter https://aka.ms/afunixinterop.</span><span class="sxs-lookup"><span data-stu-id="9daaa-539">Read more in our blog post at https://aka.ms/afunixinterop</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-540">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-540">WSL</span></span>
* <span data-ttu-id="9daaa-541">Unterstützung von mmap() mit MAP_NORESERVE [GH 121, 2784]</span><span class="sxs-lookup"><span data-stu-id="9daaa-541">Support mmap() with MAP_NORESERVE [GH 121, 2784]</span></span>
* <span data-ttu-id="9daaa-542">Unterstützung von CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="9daaa-542">Support CLONE_PTRACE and CLONE_UNTRACED [GH 121, 2781]</span></span>
* <span data-ttu-id="9daaa-543">Verarbeiten eines Nicht-SIGCHLD-Beendigungssignals im Klon [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="9daaa-543">Handle non-SIGCHLD termination signal in clone [GH 121, 2781]</span></span>
* <span data-ttu-id="9daaa-544">Stub für /proc/sys/fs/inotify/max_user_instances und /proc/sys/fs/inotify/max_user_watches [GH 1705]</span><span class="sxs-lookup"><span data-stu-id="9daaa-544">Stub /proc/sys/fs/inotify/max_user_instances and /proc/sys/fs/inotify/max_user_watches [GH 1705]</span></span>
* <span data-ttu-id="9daaa-545">Fehler beim Laden von ELF-Binärdateien, die Ladeheader mit Offsets ungleich NULL enthalten [GH 1884]</span><span class="sxs-lookup"><span data-stu-id="9daaa-545">Error loading ELF binaries that contain load headers with non-zero offsets [GH 1884]</span></span>
* <span data-ttu-id="9daaa-546">Eliminieren von nachfolgenden Seitenbytes beim Laden von Images.</span><span class="sxs-lookup"><span data-stu-id="9daaa-546">Zero out trailing page bytes when loading images.</span></span>
* <span data-ttu-id="9daaa-547">Verringern der Fälle, in denen execve den Prozess automatisch beendet</span><span class="sxs-lookup"><span data-stu-id="9daaa-547">Reduce cases where execve silently terminates process</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-548">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-548">Console</span></span>
* <span data-ttu-id="9daaa-549">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-549">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-550">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-550">LTP Results:</span></span>
<span data-ttu-id="9daaa-551">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-551">Testing in progress.</span></span>

## <a name="build-17083"></a><span data-ttu-id="9daaa-552">Build 17083</span><span class="sxs-lookup"><span data-stu-id="9daaa-552">Build 17083</span></span>
<span data-ttu-id="9daaa-553">Allgemeine Windows-Informationen zu Build 17083 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-553">For general Windows information on build 17083 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-554">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-554">WSL</span></span>
* <span data-ttu-id="9daaa-555">Korrektur der Fehlerüberprüfung für epoll [GH 2798, 2801, 2857]</span><span class="sxs-lookup"><span data-stu-id="9daaa-555">Fixed bugcheck related to epoll [GH 2798, 2801, 2857]</span></span>
* <span data-ttu-id="9daaa-556">Korrektur von Hängern beim Deaktivieren von ASLR [GH 1185, 2870]</span><span class="sxs-lookup"><span data-stu-id="9daaa-556">Fixed hangs when turning off ASLR [GH 1185, 2870]</span></span>
* <span data-ttu-id="9daaa-557">Sicherstellen, dass mmap-Vorgänge atomarisch erscheinen [GH 2732]</span><span class="sxs-lookup"><span data-stu-id="9daaa-557">Ensure mmap operations appear atomic [GH 2732]</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-558">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-558">Console</span></span>
* <span data-ttu-id="9daaa-559">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-559">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-560">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-560">LTP Results:</span></span>
<span data-ttu-id="9daaa-561">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-561">Testing in progress.</span></span>

## <a name="build-17074"></a><span data-ttu-id="9daaa-562">Build 17074</span><span class="sxs-lookup"><span data-stu-id="9daaa-562">Build 17074</span></span>
<span data-ttu-id="9daaa-563">Allgemeine Windows-Informationen zu Build 17074 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-563">For general Windows information on build 17074 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-564">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-564">WSL</span></span>
* <span data-ttu-id="9daaa-565">Festes Speicherformat von DrvFs-Metadaten [GH 2777]</span><span class="sxs-lookup"><span data-stu-id="9daaa-565">Fixed storage format of DrvFs metadata [GH 2777]</span></span> </br>
<span data-ttu-id="9daaa-566">**Wichtig:** Die vor diesem Build erstellten DrvFs-Metadaten werden falsch oder überhaupt nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-566">**Important:** DrvFs metadata created before this build will show up incorrectly or not at all.</span></span> <span data-ttu-id="9daaa-567">Um betroffene Dateien zu korrigieren, verwenden Sie chmod und chown zum erneuten Anwenden der Metadaten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-567">To fix affected files, use chmod and chown to re-apply the metadata.</span></span>
* <span data-ttu-id="9daaa-568">Korrektur eines Problems mit mehreren Signalen und neu startbaren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-568">Fixed issue with multiple signals and restartable syscalls.</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-569">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-569">Console</span></span>
* <span data-ttu-id="9daaa-570">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-570">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-571">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-571">LTP Results:</span></span>
<span data-ttu-id="9daaa-572">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-572">Testing in progress.</span></span>

## <a name="build-17063"></a><span data-ttu-id="9daaa-573">Build 17063</span><span class="sxs-lookup"><span data-stu-id="9daaa-573">Build 17063</span></span>
<span data-ttu-id="9daaa-574">Allgemeine Windows-Informationen zu Build 17063 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-574">For general Windows information on build 17063 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9daaa-575">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-575">WSL</span></span>
* <span data-ttu-id="9daaa-576">DrvFs unterstützt zusätzliche Linux-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-576">DrvFs supports additional Linux metadata.</span></span> <span data-ttu-id="9daaa-577">Dies ermöglicht das Festlegen des Besitzers und des Dateimodus mit chmod/chown sowie das Erstellen spezieller Dateien, etwa Fifos, Unix-Sockets und Gerätedateien.</span><span class="sxs-lookup"><span data-stu-id="9daaa-577">This allows setting the owner and mode of files using chmod/chown, and also the creation of special files such as fifos, unix sockets and device files.</span></span> <span data-ttu-id="9daaa-578">Diese Option ist zurzeit standardmäßig deaktiviert, da Sie noch experimentell ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-578">This is disabled by default for now since it's still experimental.</span></span>
<span data-ttu-id="9daaa-579">**Hinweis:**  Wir haben einen Fehler im Metadatenformat behoben, das von DrvFs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-579">**Note:**  We fixed a bug in the metadata format used by DrvFs.</span></span> <span data-ttu-id="9daaa-580">Obwohl Metadaten in diesem Build für Experimente funktionieren, lesen zukünftige Builds die von diesem Build erstellten Metadaten nicht ordnungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="9daaa-580">While metadata works on this build for experimentation, future builds will not correctly read metadata created by this build.</span></span>  <span data-ttu-id="9daaa-581">Möglicherweise müssen Sie den Besitzer für geänderte Dateien manuell aktualisieren, und Geräte mit einer benutzerdefinierten Geräte-ID müssen neu erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-581">You might need to manually update owner for modified files and devices with a custom device ID will have to be recreated.</span></span>

  <span data-ttu-id="9daaa-582">Um diese Funktion zu aktivieren, binden Sie DrvFs mit der Metadatenoption ein (um sie für eine vorhandene Einbindung zu aktivieren, müssen Sie die Einbindung zunächst aufheben):</span><span class="sxs-lookup"><span data-stu-id="9daaa-582">To enable, mount DrvFs with the metadata option (to enable it on an existing mount, you must first unmount it):</span></span>

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  <span data-ttu-id="9daaa-583">Linux-Berechtigungen werden der Datei als zusätzliche Metadaten hinzugefügt. Sie wirken sich nicht auf die Windows-Berechtigungen aus.</span><span class="sxs-lookup"><span data-stu-id="9daaa-583">Linux permissions are added as additional metadata to the file; they do not affect the Windows permissions.</span></span>  <span data-ttu-id="9daaa-584">Beachten Sie, dass beim Bearbeiten einer Datei mithilfe eines Windows-Editors die Metadaten möglicherweise entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-584">Remember, editing a file using a Windows editor may remove the metadata.</span></span> <span data-ttu-id="9daaa-585">In diesem Fall wird die Datei auf die Standardberechtigungen zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-585">In this case, the file will revert to its default permissions.</span></span>

* <span data-ttu-id="9daaa-586">Hinzufügen von Einbindungsoptionen zu DrvFs, um Dateien ohne Metadaten zu steuern.</span><span class="sxs-lookup"><span data-stu-id="9daaa-586">Added mount options to DrvFs to control files without metadata.</span></span>
  * <span data-ttu-id="9daaa-587">uid: die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-587">uid: the user ID used for the owner of all files.</span></span>
  * <span data-ttu-id="9daaa-588">gid: die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-588">gid: the group ID used for the owner of all files.</span></span>
  * <span data-ttu-id="9daaa-589">umask: Eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-589">umask: an octal mask of permissions to exclude for all files and directories.</span></span>
  * <span data-ttu-id="9daaa-590">fmask: Eine oktale Maske mit Berechtigungen, die für alle regulären Dateien ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-590">fmask: an octal mask of permissions to exclude for all regular files.</span></span>
  * <span data-ttu-id="9daaa-591">dmask: Eine oktale Maske mit Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-591">dmask: an octal mask of permissions to exclude for all directories.</span></span>

  <span data-ttu-id="9daaa-592">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9daaa-592">For example:</span></span>
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  <span data-ttu-id="9daaa-593">Kombinieren Sie dies mit der Metadatenoption, um Standardberechtigungen für Dateien ohne Metadaten anzugeben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-593">Combine with the metadata option to specify default permissions for files without metadata.</span></span>

* <span data-ttu-id="9daaa-594">Wird in einer neuen Umgebungsvariablen (`WSLENV`) eingeführt, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32 ausgetauscht werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-594">Introduced a new environment variable, `WSLENV`, to configure how environment variables flow between WSL and Win32.</span></span>

  <span data-ttu-id="9daaa-595">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9daaa-595">For example:</span></span>

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  <span data-ttu-id="9daaa-596">`WSLENV` eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozessen aus Win32 oder Win32-Prozessen aus WSL eingeschlossen werden können.</span><span class="sxs-lookup"><span data-stu-id="9daaa-596">`WSLENV` is a colon-delimited list of environment variables that can be included when launching WSL processes from Win32 or Win32 processes from WSL.</span></span>  <span data-ttu-id="9daaa-597">Jeder Variablen kann ein Schrägstrich als Suffix vorangestellt werden, gefolgt von Flags, um anzugeben, wie sie übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9daaa-597">Each variable can be suffixed with a slash followed by flags to specify how it is translated.</span></span>
  * <span data-ttu-id="9daaa-598">p: Der Wert ist ein Pfad, der zwischen WSL-Pfaden und Win32-Pfaden übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9daaa-598">p: The value is a path that should be translated between WSL paths and Win32 paths.</span></span>
  * <span data-ttu-id="9daaa-599">l: Der Wert ist eine Liste von Pfaden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-599">l: The value is a list of paths.</span></span> <span data-ttu-id="9daaa-600">In WSL ist es eine durch Doppelpunkte getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="9daaa-600">In WSL, it is a colon-delimited list.</span></span> <span data-ttu-id="9daaa-601">In Win32 ist es eine durch Semikolons getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="9daaa-601">In Win32, it is a semicolon-delimited list.</span></span>
  * <span data-ttu-id="9daaa-602">u: Der Wert sollte nur beim Aufrufen von WSL aus Win32 eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-602">u: The value should only be included when invoking WSL from Win32</span></span>
  * <span data-ttu-id="9daaa-603">w: Der Wert sollte nur beim Aufrufen von Win32 aus WSL eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-603">w: The value should only be included when invoking Win32 from WSL</span></span>

  <span data-ttu-id="9daaa-604">Sie können `WSLENV` in der BASHRC-Datei oder in der benutzerdefinierten Windows-Umgebung für Ihren Benutzer festlegen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-604">You can set `WSLENV` in .bashrc or in the custom Windows environment for your user.</span></span>

* <span data-ttu-id="9daaa-605">drvfs wird ordnungsgemäß eingebunden und behält Zeitstempel aus from tar, cp -p bei (GH 1939)</span><span class="sxs-lookup"><span data-stu-id="9daaa-605">drvfs mounts correctly preserves timestamps from tar, cp -p (GH 1939)</span></span>
* <span data-ttu-id="9daaa-606">Symbolische drvfs-Verknüpfungen geben die richtige Größe an (GH 2641)</span><span class="sxs-lookup"><span data-stu-id="9daaa-606">drvfs symlinks report the correct size (GH 2641)</span></span>
* <span data-ttu-id="9daaa-607">Lese-/Schreibvorgänge funktionieren für sehr große E/A-Größen (GH 2653)</span><span class="sxs-lookup"><span data-stu-id="9daaa-607">read/write works for very large IO sizes (GH 2653)</span></span>
* <span data-ttu-id="9daaa-608">waitpid funktioniert mit Prozessgruppen-IDs (GH 2534)</span><span class="sxs-lookup"><span data-stu-id="9daaa-608">waitpid works with process group IDs (GH 2534)</span></span>
* <span data-ttu-id="9daaa-609">Erheblich verbesserte mmap-Leistung für große reserve-Regionen, Verbesserung der ghc-Leistung (GH 1671)</span><span class="sxs-lookup"><span data-stu-id="9daaa-609">significantly improved mmap performance for large reserve regions; improves ghc performance (GH 1671)</span></span>
* <span data-ttu-id="9daaa-610">personality unterstützt READ_IMPLIES_EXEC, Korrekturen maxima und clisp (GH 1185)</span><span class="sxs-lookup"><span data-stu-id="9daaa-610">personality supports for READ_IMPLIES_EXEC; fixes maxima and clisp (GH 1185)</span></span>
* <span data-ttu-id="9daaa-611">mprotect unterstützt PROT_GROWSDOWN,;Korrekturen clisp (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="9daaa-611">mprotect supports PROT_GROWSDOWN; fixes clisp (GH 1128)</span></span>
* <span data-ttu-id="9daaa-612">Seitenfehlerkorrekturen im Overcommitmodus, Korrekturen sbcl (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="9daaa-612">page fault fixes in overcommit mode; fixes sbcl (GH 1128)</span></span>
* <span data-ttu-id="9daaa-613">clone unterstützt weitere Flagkombinationen</span><span class="sxs-lookup"><span data-stu-id="9daaa-613">clone supports more flags combinations</span></span>
* <span data-ttu-id="9daaa-614">Unterstützung von select/epoll von epoll-Dateien (zuvor eine Nulloperation).</span><span class="sxs-lookup"><span data-stu-id="9daaa-614">Support select/epoll of epoll files (previously a no-op).</span></span>
* <span data-ttu-id="9daaa-615">Benachrichtigen von ptrace über nicht implementierte Systemaufrufe.</span><span class="sxs-lookup"><span data-stu-id="9daaa-615">Notify ptrace of unimplemented syscalls.</span></span>
* <span data-ttu-id="9daaa-616">Ignorieren von Schnittstellen, die nicht aktiv sind, beim Generieren von resolv.conf-Namenservern [GH 2694]</span><span class="sxs-lookup"><span data-stu-id="9daaa-616">Ignore interfaces that are not up when generating resolv.conf nameservers [GH 2694]</span></span>
* <span data-ttu-id="9daaa-617">Aufzählen von Netzwerkschnittstellen ohne physische Adresse.</span><span class="sxs-lookup"><span data-stu-id="9daaa-617">Enumerate network interfaces with no physical address.</span></span> <span data-ttu-id="9daaa-618">[GH 2685]</span><span class="sxs-lookup"><span data-stu-id="9daaa-618">[GH 2685]</span></span>
* <span data-ttu-id="9daaa-619">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-619">Additional bug fixes and improvements.</span></span>

### <a name="linux-tools-available-to-developers-on-windows"></a><span data-ttu-id="9daaa-620">Linux-Tools für Entwickler unter Windows verfügbar</span><span class="sxs-lookup"><span data-stu-id="9daaa-620">Linux tools available to developers on Windows</span></span>

* <span data-ttu-id="9daaa-621">Windows-Befehlszeilen-Toolkette enthält bsdtar (tar) und curl.</span><span class="sxs-lookup"><span data-stu-id="9daaa-621">Windows Command line Toolchain includes bsdtar (tar) and curl.</span></span>
  <span data-ttu-id="9daaa-622">Lesen Sie [diesen Blog](https://aka.ms/tarcurlwindows), um mehr über das Hinzufügen dieser beiden neuen Tools zu erfahren, und sehen Sie, wie Sie das Entwicklererlebnis unter Windows formen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-622">Read [this blog](https://aka.ms/tarcurlwindows) to learn more about the addition of these two new tools and see how they’re shaping the developer experience on Windows.</span></span>

*   <span data-ttu-id="9daaa-623">`AF_UNIX` ist im Windows Insider SDK (17061 und höher) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9daaa-623">`AF_UNIX` is available in the Windows Insider SDK (17061+).</span></span>
  <span data-ttu-id="9daaa-624">Lesen Sie [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/), um weitere Informationen zu `AF_UNIX` zu erhalten und mehr über die Verwendung in Windows durch Entwickler zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-624">Read [this blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) to learn more about `AF_UNIX` and how developers on Windows can use it.</span></span>

### <a name="console"></a><span data-ttu-id="9daaa-625">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-625">Console</span></span>
* <span data-ttu-id="9daaa-626">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-626">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-627">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-627">LTP Results:</span></span>
<span data-ttu-id="9daaa-628">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-628">Testing in progress.</span></span>


## <a name="build-17046"></a><span data-ttu-id="9daaa-629">Build 17046</span><span class="sxs-lookup"><span data-stu-id="9daaa-629">Build 17046</span></span>

<span data-ttu-id="9daaa-630">Allgemeine Windows-Informationen zu Build 17046 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span><span class="sxs-lookup"><span data-stu-id="9daaa-630">For general Windows information on build 17046 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-631">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-631">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-632">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-632">WSL</span></span>
- <span data-ttu-id="9daaa-633">Ermöglicht das Ausführen von Prozessen ohne ein aktives Terminal.</span><span class="sxs-lookup"><span data-stu-id="9daaa-633">Allow processes to run without an active terminal.</span></span> <span data-ttu-id="9daaa-634">[GH 709, 1007, 1511, 2252, 2391 usw.]</span><span class="sxs-lookup"><span data-stu-id="9daaa-634">[GH 709, 1007, 1511, 2252, 2391, et al.]</span></span>
- <span data-ttu-id="9daaa-635">Bessere Unterstützung von CLONE_VFORK und CLONE_VM.</span><span class="sxs-lookup"><span data-stu-id="9daaa-635">Better support of CLONE_VFORK and CLONE_VM.</span></span> <span data-ttu-id="9daaa-636">[GH 1878, 2615]</span><span class="sxs-lookup"><span data-stu-id="9daaa-636">[GH 1878, 2615]</span></span>
- <span data-ttu-id="9daaa-637">Überspringen der TDI-Filtertreiber für WSL-Netzwerkvorgänge.</span><span class="sxs-lookup"><span data-stu-id="9daaa-637">Skip TDI filter drivers for WSL networking operations.</span></span> <span data-ttu-id="9daaa-638">[GH 1554]</span><span class="sxs-lookup"><span data-stu-id="9daaa-638">[GH 1554]</span></span>
- <span data-ttu-id="9daaa-639">DrvFs erstellt symbolische NT-Verknüpfungen, wenn bestimmte Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="9daaa-639">DrvFs creates NT symlinks when certain conditions are met.</span></span> <span data-ttu-id="9daaa-640">[GH 353, 1475, 2602]</span><span class="sxs-lookup"><span data-stu-id="9daaa-640">[GH 353, 1475, 2602]</span></span>
    - <span data-ttu-id="9daaa-641">Das Verknüpfungsziel muss relativ sein, darf keine Einbindungspunkte oder symbolische Verknüpfungen kreuzen und muss vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="9daaa-641">The link target must be relative, must not cross any mount points or symlinks, and must exist.</span></span>
    - <span data-ttu-id="9daaa-642">Der Benutzer muss über SE_CREATE_SYMBOLIC_LINK_PRIVILEGE verfügen (dies erfordert normalerweise, dass Sie „wsl.exe“ mit erhöhten Rechten starten), sofern der Entwicklermodus nicht aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-642">The user must have SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (this normally requires you to launch wsl.exe elevated), unless Developer Mode is turned on.</span></span>
    - <span data-ttu-id="9daaa-643">Unter allen anderen Umständen erstellt DrvFs weiterhin symbolische WSL-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-643">In all other situations, DrvFs still creates WSL symlinks.</span></span>
- <span data-ttu-id="9daaa-644">Ermöglichen der gleichzeitigen Ausführung von WSL-Instanzen mit und ohne erhöhten Rechten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-644">Allow running elevated and non-elevated WSL instances simultaneously.</span></span>
- <span data-ttu-id="9daaa-645">Unterstützung von /proc/sys/kernel/Yama/ptrace_scope</span><span class="sxs-lookup"><span data-stu-id="9daaa-645">Support /proc/sys/kernel/yama/ptrace_scope</span></span>
- <span data-ttu-id="9daaa-646">Hinzufügen von wslpath zum Durchführen von Konvertierungen von WSL-<- >Windows-Pfaden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-646">Add wslpath to do WSL<->Windows path conversions.</span></span> <span data-ttu-id="9daaa-647">[GH 522, 1243, 1834, 2327 usw.]</span><span class="sxs-lookup"><span data-stu-id="9daaa-647">[GH 522, 1243, 1834, 2327, et al.]</span></span>
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a><span data-ttu-id="9daaa-648">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-648">Console</span></span>
- <span data-ttu-id="9daaa-649">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-649">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-650">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-650">LTP Results:</span></span>
<span data-ttu-id="9daaa-651">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-651">Testing in progress.</span></span>


## <a name="build-17040"></a><span data-ttu-id="9daaa-652">Build 17040</span><span class="sxs-lookup"><span data-stu-id="9daaa-652">Build 17040</span></span>

<span data-ttu-id="9daaa-653">Allgemeine Windows-Informationen zu Build 17040 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span><span class="sxs-lookup"><span data-stu-id="9daaa-653">For general Windows information on build 17040 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-654">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-654">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-655">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-655">WSL</span></span>
- <span data-ttu-id="9daaa-656">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="9daaa-656">No fixes since 17035.</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-657">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-657">Console</span></span>
- <span data-ttu-id="9daaa-658">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="9daaa-658">No fixes since 17035.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-659">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-659">LTP Results:</span></span>
<span data-ttu-id="9daaa-660">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-660">Testing in progress.</span></span>

## <a name="build-17035"></a><span data-ttu-id="9daaa-661">Build 17035</span><span class="sxs-lookup"><span data-stu-id="9daaa-661">Build 17035</span></span>

<span data-ttu-id="9daaa-662">Allgemeine Windows-Informationen zu Build 17035 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span><span class="sxs-lookup"><span data-stu-id="9daaa-662">For general Windows information on build 17035 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-663">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-663">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-664">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-664">WSL</span></span>
- <span data-ttu-id="9daaa-665">Der Zugriff auf Dateien auf DrvFs kann gelegentlich mit EINVAL fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-665">Accessing files on DrvFs could occasionally fail with EINVAL.</span></span> <span data-ttu-id="9daaa-666">[GH 2448]</span><span class="sxs-lookup"><span data-stu-id="9daaa-666">[GH 2448]</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-667">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-667">Console</span></span>
- <span data-ttu-id="9daaa-668">Farbverlust beim Einfügen/Löschen von Zeilen im VT-Modus.</span><span class="sxs-lookup"><span data-stu-id="9daaa-668">Some color loss when inserting/deleting lines in VT mode.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-669">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-669">LTP Results:</span></span>
<span data-ttu-id="9daaa-670">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-670">Testing in progress.</span></span>

## <a name="build-17025"></a><span data-ttu-id="9daaa-671">Build 17025</span><span class="sxs-lookup"><span data-stu-id="9daaa-671">Build 17025</span></span>

<span data-ttu-id="9daaa-672">Allgemeine Windows-Informationen zu Build 17025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span><span class="sxs-lookup"><span data-stu-id="9daaa-672">For general Windows information on build 17025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-673">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-673">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-674">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-674">WSL</span></span>
- <span data-ttu-id="9daaa-675">Starten anfänglicher Prozesse in einer neuen Vordergrundprozessgruppe [GH 1653, 2510].</span><span class="sxs-lookup"><span data-stu-id="9daaa-675">Start initial processes in a new foreground process group [GH 1653, 2510].</span></span>
- <span data-ttu-id="9daaa-676">Korrekturen der SIGHUP-Übermittlung [GH 2496].</span><span class="sxs-lookup"><span data-stu-id="9daaa-676">SIGHUP delivery fixes [GH 2496].</span></span>
- <span data-ttu-id="9daaa-677">Generieren eines Standardnamens für virtuelle Bridge generieren, wenn keine Angabe erfolgt [GH 2497].</span><span class="sxs-lookup"><span data-stu-id="9daaa-677">Generate default virtual bridge name if none provided [GH 2497].</span></span>
- <span data-ttu-id="9daaa-678">Implementieren von /proc/sys/kernel/Random/boot_id [GH 2518].</span><span class="sxs-lookup"><span data-stu-id="9daaa-678">Implement /proc/sys/kernel/random/boot_id [GH 2518].</span></span>
- <span data-ttu-id="9daaa-679">Weitere Interop-Pipekorrekturen für stdout/stderr.</span><span class="sxs-lookup"><span data-stu-id="9daaa-679">More interop stdout/stderr pipe fixes.</span></span>
- <span data-ttu-id="9daaa-680">Stub für syncfs-Systemaufruf.</span><span class="sxs-lookup"><span data-stu-id="9daaa-680">Stub syncfs system call.</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-681">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-681">Console</span></span>
- <span data-ttu-id="9daaa-682">Korrektur der VT-Eingabeübersetzung für Drittanbieterkonsolen [GH 111]</span><span class="sxs-lookup"><span data-stu-id="9daaa-682">Fix input VT translation for third party consoles [GH 111]</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-683">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-683">LTP Results:</span></span>
<span data-ttu-id="9daaa-684">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-684">Testing in progress.</span></span>

## <a name="build-17017"></a><span data-ttu-id="9daaa-685">Build 17017</span><span class="sxs-lookup"><span data-stu-id="9daaa-685">Build 17017</span></span>

<span data-ttu-id="9daaa-686">Allgemeine Windows-Informationen zu Build 17017 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span><span class="sxs-lookup"><span data-stu-id="9daaa-686">For general Windows information on build 17017 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-687">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-687">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-688">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-688">WSL</span></span>
- <span data-ttu-id="9daaa-689">Ignorieren leerer ELF-Programmheader [GH 330].</span><span class="sxs-lookup"><span data-stu-id="9daaa-689">Ignore empty ELF program headers [GH 330].</span></span>
- <span data-ttu-id="9daaa-690">Ermöglichen, dass LxssManager WSL-Instanzen für nicht interaktive Benutzer erstellt (Unterstützung für SSH und geplante Aufgaben) [GH 777, 1602].</span><span class="sxs-lookup"><span data-stu-id="9daaa-690">Allow LxssManager to create WSL instances for non-interactive users (ssh and scheduled task support) [GH 777, 1602].</span></span>
- <span data-ttu-id="9daaa-691">Unterstützung von WSL->Win32->WSL-Szenarien („Inception“) [GH 1228].</span><span class="sxs-lookup"><span data-stu-id="9daaa-691">Support WSL->Win32->WSL ("inception") scenarios [GH 1228].</span></span>
- <span data-ttu-id="9daaa-692">Eingeschränkte Unterstützung für das Beenden von Konsolen-Apps, die über Interop aufgerufen wurden [GH 1614].</span><span class="sxs-lookup"><span data-stu-id="9daaa-692">Limited support for termination of console apps invoked via interop [GH 1614].</span></span>
- <span data-ttu-id="9daaa-693">Unterstützung von Einbindungsoptionen für devpts [GH 1948].</span><span class="sxs-lookup"><span data-stu-id="9daaa-693">Support mount options for devpts [GH 1948].</span></span>
- <span data-ttu-id="9daaa-694">Ptrace blockiert den Start untergeordneter Prozesse [GH 2333].</span><span class="sxs-lookup"><span data-stu-id="9daaa-694">Ptrace blocking child startup [GH 2333].</span></span>
- <span data-ttu-id="9daaa-695">EPOLLET fehlen einige Ereignisse [GH 2462].</span><span class="sxs-lookup"><span data-stu-id="9daaa-695">EPOLLET missing some events [GH 2462].</span></span>
- <span data-ttu-id="9daaa-696">Rückgabe einer größeren Anzahl von Daten für PTRACE_GETSIGINFO.</span><span class="sxs-lookup"><span data-stu-id="9daaa-696">Return more data for PTRACE_GETSIGINFO.</span></span>
- <span data-ttu-id="9daaa-697">Getdents mit lseek liefert falsche Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="9daaa-697">Getdents with lseek gives incorrect results.</span></span>
- <span data-ttu-id="9daaa-698">Korrektur einiger Hänger von Win32-Interop-Apps, die auf Eingaben in einer Pipe warten, die keine weiteren Daten enthält.</span><span class="sxs-lookup"><span data-stu-id="9daaa-698">Fix some Win32 interop app hangs, waiting for input on a pipe that has no more data.</span></span>
- <span data-ttu-id="9daaa-699">O_ASYNC-Unterstützung für tty/pty-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9daaa-699">O_ASYNC support for tty/pty files.</span></span>
- <span data-ttu-id="9daaa-700">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-700">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-701">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-701">Console</span></span>
- <span data-ttu-id="9daaa-702">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-702">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-703">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-703">LTP Results:</span></span>
<span data-ttu-id="9daaa-704">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-704">Testing in progress.</span></span>

## <a name="fall-creators-update"></a><span data-ttu-id="9daaa-705">Fall Creators Update</span><span class="sxs-lookup"><span data-stu-id="9daaa-705">Fall Creators Update</span></span>

## <a name="build-16288"></a><span data-ttu-id="9daaa-706">Build 16288</span><span class="sxs-lookup"><span data-stu-id="9daaa-706">Build 16288</span></span>

<span data-ttu-id="9daaa-707">Allgemeine Windows-Informationen zu Build 16288 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-707">For general Windows information on build 16288 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-708">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-708">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-709">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-709">WSL</span></span>
- <span data-ttu-id="9daaa-710">Ordnungsgemäße Initialisierung und Meldung von uid, gid und Modus für Socketdateideskriptoren [GH 2490]</span><span class="sxs-lookup"><span data-stu-id="9daaa-710">Correctly initialize and report uid, gid, and mode for socket file descriptors [GH 2490]</span></span>
- <span data-ttu-id="9daaa-711">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-711">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-712">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-712">Console</span></span>
- <span data-ttu-id="9daaa-713">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-713">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-714">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-714">LTP Results:</span></span>
<span data-ttu-id="9daaa-715">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9daaa-715">No change since 16273</span></span>

## <a name="build-16278"></a><span data-ttu-id="9daaa-716">Build 16278</span><span class="sxs-lookup"><span data-stu-id="9daaa-716">Build 16278</span></span>

<span data-ttu-id="9daaa-717">Allgemeine Windows-Informationen zu Build 162738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-717">For general Windows information on build 162738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-718">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-718">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-719">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-719">WSL</span></span>
- <span data-ttu-id="9daaa-720">Explizite Aufhebung der Zuordnung zugeordneter Ansichten von dateigestützten Abschnitten beim Beenden des LX MM-Status [GH 2415]</span><span class="sxs-lookup"><span data-stu-id="9daaa-720">Explicitly unmap mapped views of file backed sections when tearing down LX MM state [GH 2415]</span></span>
- <span data-ttu-id="9daaa-721">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-721">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-722">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-722">Console</span></span>
- <span data-ttu-id="9daaa-723">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-723">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-724">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-724">LTP Results:</span></span>
<span data-ttu-id="9daaa-725">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9daaa-725">No change since 16273</span></span>

## <a name="build-16275"></a><span data-ttu-id="9daaa-726">Build 16275</span><span class="sxs-lookup"><span data-stu-id="9daaa-726">Build 16275</span></span>

<span data-ttu-id="9daaa-727">Allgemeine Windows-Informationen zu Build 162735 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-727">For general Windows information on build 162735 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-728">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-728">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-729">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-729">WSL</span></span>
- <span data-ttu-id="9daaa-730">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-730">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-731">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-731">Console</span></span>
- <span data-ttu-id="9daaa-732">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-732">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-733">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-733">LTP Results:</span></span>
<span data-ttu-id="9daaa-734">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9daaa-734">No change since 16273</span></span>

## <a name="build-16273"></a><span data-ttu-id="9daaa-735">Build 16273</span><span class="sxs-lookup"><span data-stu-id="9daaa-735">Build 16273</span></span>

<span data-ttu-id="9daaa-736">Allgemeine Windows-Informationen zu Build 16273 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-736">For general Windows information on build 16273 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-737">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-737">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-738">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-738">WSL</span></span>
- <span data-ttu-id="9daaa-739">Korrektur eines Problems, bei dem DrvFs manchmal den falschen Dateityp für Verzeichnisse gemeldet hat [GH 2392]</span><span class="sxs-lookup"><span data-stu-id="9daaa-739">Fixed an issue where DrvFs sometimes reported the wrong file type for directories [GH 2392]</span></span>
- <span data-ttu-id="9daaa-740">Ermöglichen der Erstellung von NETLINK_KOBJECT_UEVENT-Sockets zum Entsperren von Programmen, die uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span><span class="sxs-lookup"><span data-stu-id="9daaa-740">Allow creation of NETLINK_KOBJECT_UEVENT sockets to unblock programs that use uevent [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span></span>
- <span data-ttu-id="9daaa-741">Hinzufügen von Unterstützung für nicht blockierende Verbindungen [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span><span class="sxs-lookup"><span data-stu-id="9daaa-741">Add support for non-blocking connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span></span>
- <span data-ttu-id="9daaa-742">Implementieren des CLONE_FS-Klonsystem-Aufrufflags [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="9daaa-742">Implement CLONE_FS clone system call flag [GH 2242]</span></span>
- <span data-ttu-id="9daaa-743">Korrektur von Problemen im Zusammenhang mit der nicht ordnungsgemäßen Behandlung von Registerkarten oder Anführungszeichen in NT-Interop [GH 1625, 2164]</span><span class="sxs-lookup"><span data-stu-id="9daaa-743">Fix issues around not handling tabs or quotes correctly in NT interop [GH 1625, 2164]</span></span>
- <span data-ttu-id="9daaa-744">Beheben des Fehlers „Zugriff verweigert“ beim Versuch, WSL-Instanzen erneut zu starten [GH 651, 2095]</span><span class="sxs-lookup"><span data-stu-id="9daaa-744">Resolve access denied error when trying to re-launch WSL instances [GH 651, 2095]</span></span>
- <span data-ttu-id="9daaa-745">Implementieren von Futex-Vorgängen FUTEX_REQUEUE und FUTEX_CMP_REQUEUE [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="9daaa-745">Implement futex FUTEX_REQUEUE and FUTEX_CMP_REQUEUE operations [GH 2242]</span></span>
- <span data-ttu-id="9daaa-746">Korrigieren von Berechtigungen für verschiedene SysFs-Dateien [GH 2214]</span><span class="sxs-lookup"><span data-stu-id="9daaa-746">Fix permissions for various SysFs files [GH 2214]</span></span>
- <span data-ttu-id="9daaa-747">Korrigieren des Hängens des Haskell-Stapels während des Setups [GH 2290]</span><span class="sxs-lookup"><span data-stu-id="9daaa-747">Fix Haskell stack hang during setup [GH 2290]</span></span>
- <span data-ttu-id="9daaa-748">Implementieren der Flags „C“, „O“ und „P“ von binfmt_misc [GH 2103]</span><span class="sxs-lookup"><span data-stu-id="9daaa-748">Implement binfmt_misc 'C' 'O' and 'P' flags [GH 2103]</span></span>
- <span data-ttu-id="9daaa-749">Hinzufügen von /proc/sys/kernel/shmmax/shmmni und /threads-max [GH 1753]</span><span class="sxs-lookup"><span data-stu-id="9daaa-749">Add /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span></span>
- <span data-ttu-id="9daaa-750">Hinzufügen partieller Unterstützung für den ioprio_set-Systemaufruf [GH 498]</span><span class="sxs-lookup"><span data-stu-id="9daaa-750">Add partial support for ioprio_set system call [GH 498]</span></span>
- <span data-ttu-id="9daaa-751">Stub für SO_REUSEPORT und Hinzufügen von Unterstützung für SO_PASSCRED für netlink-Sockets [GH 69]</span><span class="sxs-lookup"><span data-stu-id="9daaa-751">Stub SO_REUSEPORT & adding support for SO_PASSCRED for netlink sockets [GH 69]</span></span>
- <span data-ttu-id="9daaa-752">Rückgabe anderer Fehlercodes aus RegisterDistribuiton, wenn zurzeit eine Distribution installiert oder deinstalliert wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-752">Return different error codes from RegisterDistribuiton if a distribution is currently being installed or uninstalled.</span></span>
- <span data-ttu-id="9daaa-753">Ermöglichen des Aufhebens der Registrierung von teilweise installierten WSL-Distributionen über „wslconfig.exe“</span><span class="sxs-lookup"><span data-stu-id="9daaa-753">Allow unregistration of partially installed WSL distributions via wslconfig.exe</span></span>
- <span data-ttu-id="9daaa-754">Korrektur des Hängens des Python-Sockettests von udp::msg_peek</span><span class="sxs-lookup"><span data-stu-id="9daaa-754">Fix python socket test hang from udp::msg_peek</span></span>
- <span data-ttu-id="9daaa-755">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-755">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-756">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-756">Console</span></span>
- <span data-ttu-id="9daaa-757">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-757">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-758">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-758">LTP Results:</span></span>
<span data-ttu-id="9daaa-759">Tests gesamt: 1904</span><span class="sxs-lookup"><span data-stu-id="9daaa-759">Total Tests: 1904</span></span><br/>
<span data-ttu-id="9daaa-760">Übersprungene Tests gesamt: 209</span><span class="sxs-lookup"><span data-stu-id="9daaa-760">Total Skipped Tests: 209</span></span><br/>
<span data-ttu-id="9daaa-761">Fehler gesamt: 229</span><span class="sxs-lookup"><span data-stu-id="9daaa-761">Total Failures: 229</span></span><br/>
[<span data-ttu-id="9daaa-762">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-762">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a><span data-ttu-id="9daaa-763">Build 16257</span><span class="sxs-lookup"><span data-stu-id="9daaa-763">Build 16257</span></span>

<span data-ttu-id="9daaa-764">Allgemeine Windows-Informationen zu Build 16257 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-764">For general Windows information on build 16257 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-765">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-765">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-766">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-766">WSL</span></span>
- <span data-ttu-id="9daaa-767">Implementieren des prlimit64-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9daaa-767">Implement prlimit64 system call</span></span>
- <span data-ttu-id="9daaa-768">Hinzufügen von Unterstützung für ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span><span class="sxs-lookup"><span data-stu-id="9daaa-768">Add support for ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span></span>
- <span data-ttu-id="9daaa-769">Stub für MSG_MORE für TCP-Sockets [GH 2351]</span><span class="sxs-lookup"><span data-stu-id="9daaa-769">Stub MSG_MORE for TCP sockets [GH 2351]</span></span>
- <span data-ttu-id="9daaa-770">Korrektur des ungültigen Verhaltens des AT_EXECFN-Hilfsvektors [GH 2133]</span><span class="sxs-lookup"><span data-stu-id="9daaa-770">Fix invalid AT_EXECFN auxiliary vector behavior [GH 2133]</span></span>
- <span data-ttu-id="9daaa-771">Korrektur des Kopier-/Einfügeverhalten für Konsole/TTY und Hinzufügen einer besseren Verarbeitung voller Puffer [GH 2204, 2131]</span><span class="sxs-lookup"><span data-stu-id="9daaa-771">Fix copy/paste behavior for console/tty, and add better full buffer handling [GH 2204, 2131]</span></span>
- <span data-ttu-id="9daaa-772">Festlegen von T_SECURE im Hilfsvektor für set-user-ID- und set-group-ID-Programme [GH 2031]</span><span class="sxs-lookup"><span data-stu-id="9daaa-772">Set AT_SECURE in auxiliary vector for set-user-ID and set-group-ID programs [GH 2031]</span></span>
- <span data-ttu-id="9daaa-773">Psuedoterminal-Masterendpunkt verarbeitet TIOCPGRP nicht [GH 1063]</span><span class="sxs-lookup"><span data-stu-id="9daaa-773">Psuedo-terminal master endpoint not handling TIOCPGRP [GH 1063]</span></span>
- <span data-ttu-id="9daaa-774">Korrektur des Nichtzurückspulens von Verzeichnissen in LxFs durch lseek [GH 2310]</span><span class="sxs-lookup"><span data-stu-id="9daaa-774">Fix lseek does to rewind directories in LxFs [GH 2310]</span></span>
- <span data-ttu-id="9daaa-775">/dev/ptmx wird nach hoher Auslastung gesperrt [GH 1882]</span><span class="sxs-lookup"><span data-stu-id="9daaa-775">/dev/ptmx locks up after heavy usage [GH 1882]</span></span>
- <span data-ttu-id="9daaa-776">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-776">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-777">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-777">Console</span></span>
- <span data-ttu-id="9daaa-778">Korrektur für horizontale Linien/Unterstriche überall [GH 2168]</span><span class="sxs-lookup"><span data-stu-id="9daaa-778">Fix for horizontal Lines/Underscores Everywhere [GH 2168]</span></span>
- <span data-ttu-id="9daaa-779">Korrektur der Änderung der Prozessreihenfolge, wodurch das Schließen von NPM erschwert wird [GH 2170]</span><span class="sxs-lookup"><span data-stu-id="9daaa-779">Fix for process order changed making NPM harder to close [GH 2170]</span></span>
- <span data-ttu-id="9daaa-780">Hinzufügen des neuen Farbschemas: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span><span class="sxs-lookup"><span data-stu-id="9daaa-780">Added our new color scheme: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-781">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-781">LTP Results:</span></span>
<span data-ttu-id="9daaa-782">Keine Änderung seit 16251</span><span class="sxs-lookup"><span data-stu-id="9daaa-782">No change since 16251</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-783">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-783">Syscall Support</span></span>
<span data-ttu-id="9daaa-784">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-784">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-785">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-785">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`prlimit64`<br/>

### <a name="known-issues"></a><span data-ttu-id="9daaa-786">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="9daaa-786">Known Issues</span></span>
#### <a name="github-issue-2392-windows-folders-not-recognized-by-wsl-httpsgithubcommicrosoftbashonwindowsissues2392"></a><span data-ttu-id="9daaa-787">[GitHub-Issue 2392: Windows-Ordner werden von WSL nicht erkannt (](https://github.com/Microsoft/BashOnWindows/issues/2392))</span><span class="sxs-lookup"><span data-stu-id="9daaa-787">[GitHub Issue 2392: Windows Folders not recognized by WSL ...](https://github.com/Microsoft/BashOnWindows/issues/2392)</span></span>
<span data-ttu-id="9daaa-788">In Build 16257 hat WSL beim Aufzählen von Windows-Dateien/-Ordnern über `/mnt/c/...` Probleme.</span><span class="sxs-lookup"><span data-stu-id="9daaa-788">In build 16257, WSL has issues when enumerating Windows files/folders via `/mnt/c/...`.</span></span>
<span data-ttu-id="9daaa-789">Dieses Problem wurde behoben und sollte im Insider-Builds in der Woche ab dem 14.08.2017 veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-789">This issue has been fixed and should be released in Insiders build during week commencing 8/14/2017.</span></span>

<br/>

## <a name="build-16251"></a><span data-ttu-id="9daaa-790">Build 16251</span><span class="sxs-lookup"><span data-stu-id="9daaa-790">Build 16251</span></span>

<span data-ttu-id="9daaa-791">Allgemeine Windows-Informationen zu Build 16251 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-791">For general Windows information on build 16251 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-792">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-792">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-793">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-793">WSL</span></span>
- <span data-ttu-id="9daaa-794">Entfernen des Beta-Tags aus der optionalen WSL-Komponente. Weitere Informationen finden Sie im [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-794">Remove beta tag from WSL optional component, see [blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) for details.</span></span>
- <span data-ttu-id="9daaa-795">Ordnungsgemäße Initialisierung der saved-set uid und gid für set-user-ID- and set-group-ID-Binärdateien bei der Ausführung [GH 962, 1415, 2072]</span><span class="sxs-lookup"><span data-stu-id="9daaa-795">Correctly initialize saved-set uid and gid for set-user-ID and set-group-ID binaries on exec [GH 962, 1415, 2072]</span></span>
- <span data-ttu-id="9daaa-796">Hinzufügen von Unterstützung für PTRACE_O_TRACEEXIT [GH 555]</span><span class="sxs-lookup"><span data-stu-id="9daaa-796">Added support for ptrace PTRACE_O_TRACEEXIT [GH 555]</span></span>
- <span data-ttu-id="9daaa-797">Hinzufügen von Unterstützung für PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555]</span><span class="sxs-lookup"><span data-stu-id="9daaa-797">Added support for ptrace PTRACE_GETFPREGS and PTRACE_GETREGSET with NT_FPREGSET [GH 555]</span></span>
- <span data-ttu-id="9daaa-798">Korrektur von ptrace, um bei ignorierten Signalen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="9daaa-798">Fixed ptrace to stop on ignored signals</span></span>
- <span data-ttu-id="9daaa-799">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-799">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-800">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-800">Console</span></span>
- <span data-ttu-id="9daaa-801">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-801">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-802">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-802">LTP Results:</span></span>
<span data-ttu-id="9daaa-803">Anzahl bestandener Tests: 768</span><span class="sxs-lookup"><span data-stu-id="9daaa-803">Number of Passing Tests: 768</span></span></br>
<span data-ttu-id="9daaa-804">Anzahl fehlgeschlagener Tests: 244</span><span class="sxs-lookup"><span data-stu-id="9daaa-804">Number of Failing Tests: 244</span></span></br>
<span data-ttu-id="9daaa-805">Anzahl übersprungener Tests: 96</span><span class="sxs-lookup"><span data-stu-id="9daaa-805">Number of Skipped Tests: 96</span></span></br>
[<span data-ttu-id="9daaa-806">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-806">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a><span data-ttu-id="9daaa-807">Build 16241</span><span class="sxs-lookup"><span data-stu-id="9daaa-807">Build 16241</span></span>

<span data-ttu-id="9daaa-808">Allgemeine Windows-Informationen zu Build 16241 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-808">For general Windows information on build 16241 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-809">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-809">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9daaa-810">WSL</span><span class="sxs-lookup"><span data-stu-id="9daaa-810">WSL</span></span>
- <span data-ttu-id="9daaa-811">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-811">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="9daaa-812">Console</span><span class="sxs-lookup"><span data-stu-id="9daaa-812">Console</span></span>
- <span data-ttu-id="9daaa-813">Korrektur für die Ausgabe des falschen Zeichens für Schnittlinien-DEC, ursprünglich [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/) gemeldet</span><span class="sxs-lookup"><span data-stu-id="9daaa-813">Fix for outputting the wrong character for the crossing-lines DEC, originally reported [here](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span></span>
- <span data-ttu-id="9daaa-814">Korrektur, dass kein Ausgabetext in Codepage 65001 (UTF8) angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="9daaa-814">Fix for no output text being displayed in codepage 65001 (utf8)</span></span>
- <span data-ttu-id="9daaa-815">Übertragen Sie an den RGB-Werten einer Farbe vorgenommene Änderungen nicht an andere Teile der Palette bei Änderungen der Auswahl.</span><span class="sxs-lookup"><span data-stu-id="9daaa-815">Do not transfer changes made to one color's RGB values to other parts of the palette on selection change.</span></span> <span data-ttu-id="9daaa-816">Dadurch wird die Verwendung des Konsoleneigenschaftenblatts erheblich vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-816">This will make the console properties sheet a lot easier to use.</span></span>
- <span data-ttu-id="9daaa-817">STRG+S funktioniert anscheinend nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="9daaa-817">Ctrl+S doesn't appear to work correctly</span></span>
- <span data-ttu-id="9daaa-818">Un-Bold/-Dim fehlt in ANSI-Escapecodes vollständig [GH 2174]</span><span class="sxs-lookup"><span data-stu-id="9daaa-818">Un-Bold/-Dim completely absent from ANSI escape codes [GH 2174]</span></span>
- <span data-ttu-id="9daaa-819">Die Konsole unterstützt VIM-Farbdesigns nicht ordnungsgemäß [GH 1706]</span><span class="sxs-lookup"><span data-stu-id="9daaa-819">Console doesn't correctly support Vim color themes [GH 1706]</span></span>
- <span data-ttu-id="9daaa-820">Bestimmte Zeichen können nicht eingefügt werden [GH 2149]</span><span class="sxs-lookup"><span data-stu-id="9daaa-820">Cannot paste particular characters [GH 2149]</span></span>
- <span data-ttu-id="9daaa-821">Die Größenänderung von dynamischem Umbruch interagiert seltsam mit der Größenänderung eines Bash-Fensters, wenn sich die Inhalte in der Bearbeitungs-/Befehlszeile befinden [GH-Verbindung 1123]</span><span class="sxs-lookup"><span data-stu-id="9daaa-821">Reflow resize interacts strangely with resizing a bash window when stuff is on the edit/command line [GH ConEmu 1123]</span></span>
- <span data-ttu-id="9daaa-822">STRG+L hinterlässt Fragmente auf dem Bildschirm [GH 1978]</span><span class="sxs-lookup"><span data-stu-id="9daaa-822">Ctrl-L leaves the screen dirty [GH 1978]</span></span>
- <span data-ttu-id="9daaa-823">Konsolenrenderingfehler bei der Anzeige von VT für HDPI [GH 1907]</span><span class="sxs-lookup"><span data-stu-id="9daaa-823">Console rendering bug when displaying VT on HDPI [GH 1907]</span></span>
- <span data-ttu-id="9daaa-824">Japanische Zeichen sehen mit dem Unicode-Zeichen U+30FB seltsam aus [GH 2146]</span><span class="sxs-lookup"><span data-stu-id="9daaa-824">Japansese characters look strange with Unicode Character U+30FB [GH 2146]</span></span>
- <span data-ttu-id="9daaa-825">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-825">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16237"></a><span data-ttu-id="9daaa-826">Build 16237</span><span class="sxs-lookup"><span data-stu-id="9daaa-826">Build 16237</span></span>

<span data-ttu-id="9daaa-827">Allgemeine Windows-Informationen zu Build 16237 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-827">For general Windows information on build 16237 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-828">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-828">Fixed</span></span>
- <span data-ttu-id="9daaa-829">Verwenden von Standardattributen für Dateien ohne E/As in lxfs (root, root, 0000)</span><span class="sxs-lookup"><span data-stu-id="9daaa-829">Use default attributes for files without EAs in lxfs (root, root, 0000)</span></span>
- <span data-ttu-id="9daaa-830">Hinzufügen von Unterstützung für Distributionen, die erweiterte Attribute verwenden</span><span class="sxs-lookup"><span data-stu-id="9daaa-830">Added support for distributions that use extended attributes</span></span>
- <span data-ttu-id="9daaa-831">Korrektur des Auffüllens für von getdents und getdents64 zurückgegebene Einträge</span><span class="sxs-lookup"><span data-stu-id="9daaa-831">Fix padding for entries returned by getdents and getdents64</span></span>
- <span data-ttu-id="9daaa-832">Korrektur der Berechtigungsüberprüfung für den SHM_STAT-Systemaufruf [GH 2068]</span><span class="sxs-lookup"><span data-stu-id="9daaa-832">Fix permissions check for the shmctl SHM_STAT system call [GH 2068]</span></span>
- <span data-ttu-id="9daaa-833">Korrektur des falschen anfänglichen epoll-Zustands für ttys [GH 2231]</span><span class="sxs-lookup"><span data-stu-id="9daaa-833">Fixed incorrect initial epoll state for ttys [GH 2231]</span></span>
- <span data-ttu-id="9daaa-834">Korrektur, dass DrvFs readdir nicht alle Einträge zurückgibt [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="9daaa-834">Fix DrvFs readdir not returning all entries [GH 2077]</span></span>
- <span data-ttu-id="9daaa-835">Korrektur von LxFs readdir, wenn Dateien nicht verknüpft sind [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="9daaa-835">Fix LxFs readdir when files are unlinked [GH 2077]</span></span>
- <span data-ttu-id="9daaa-836">Ermöglichen des erneuten Öffnens von nicht verknüpfter drvfs-Dateien über procfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-836">Allow unlinked drvfs files to be reopened through procfs</span></span>
- <span data-ttu-id="9daaa-837">Hinzufügen einer Außerkraftsetzung des globalen Registrierungsschlüssels zum Deaktivieren von WSL-Features (Interop/Laufwerkeinbindung)</span><span class="sxs-lookup"><span data-stu-id="9daaa-837">Added global registry key override for disabling WSL features (interop / drive mounting)</span></span>
- <span data-ttu-id="9daaa-838">Korrektur falscher Blockanzahl in „stat“ für DrvFs (und LxFs) [GH 1894]</span><span class="sxs-lookup"><span data-stu-id="9daaa-838">Fix incorrect block count in "stat" for DrvFs (and LxFs) [GH 1894]</span></span>
- <span data-ttu-id="9daaa-839">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-839">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16232"></a><span data-ttu-id="9daaa-840">Build 16232</span><span class="sxs-lookup"><span data-stu-id="9daaa-840">Build 16232</span></span>

<span data-ttu-id="9daaa-841">Allgemeine Windows-Informationen zu Build 16232 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-841">For general Windows information on build 16232 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-842">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-842">Fixed</span></span>
- <span data-ttu-id="9daaa-843">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-843">No WSL related changes in this release.</span></span>

</br>

## <a name="build-16226"></a><span data-ttu-id="9daaa-844">Build 16226</span><span class="sxs-lookup"><span data-stu-id="9daaa-844">Build 16226</span></span>

<span data-ttu-id="9daaa-845">Allgemeine Windows-Informationen zu Build 16226 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-845">For general Windows information on build 16226 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-846">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-846">Fixed</span></span>
- <span data-ttu-id="9daaa-847">Unterstützung von auf xattr bezogenen Systemaufrufen (getxattr, setxattr, listxattr, removexattr).</span><span class="sxs-lookup"><span data-stu-id="9daaa-847">xattr related syscalls support (getxattr, setxattr, listxattr, removexattr).</span></span>
- <span data-ttu-id="9daaa-848">xattr-Unterstützung für security.capablity.</span><span class="sxs-lookup"><span data-stu-id="9daaa-848">security.capablity xattr support.</span></span>
- <span data-ttu-id="9daaa-849">Verbesserte Kompatibilität mit bestimmten Dateisystemen und Filtern, einschließlich Nicht-MS-SMB-Servern.</span><span class="sxs-lookup"><span data-stu-id="9daaa-849">Improved compatibility with certain file systems and filters, including non-MS SMB servers.</span></span> <span data-ttu-id="9daaa-850">[GH #1952]</span><span class="sxs-lookup"><span data-stu-id="9daaa-850">[GH #1952]</span></span>
- <span data-ttu-id="9daaa-851">Verbesserte Unterstützung für OneDrive-Platzhalter, GVFS-Platzhalter und komprimierte Compact OS-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9daaa-851">Improved support for OneDrive placeholders, GVFS placeholders, and Compact OS compressed files.</span></span>
- <span data-ttu-id="9daaa-852">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-852">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16215"></a><span data-ttu-id="9daaa-853">Build 16215</span><span class="sxs-lookup"><span data-stu-id="9daaa-853">Build 16215</span></span>

<span data-ttu-id="9daaa-854">Allgemeine Windows-Informationen zu Build 16215 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-854">For general Windows information on build 16215 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-855">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-855">Fixed</span></span>
- <span data-ttu-id="9daaa-856">Für WSL ist der Entwicklermodus nicht mehr erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9daaa-856">WSL no longer requires developer mode.</span></span>
- <span data-ttu-id="9daaa-857">Unterstützung von Verzeichnisverbindungen in drvfs.</span><span class="sxs-lookup"><span data-stu-id="9daaa-857">Support directory junctions in drvfs.</span></span>
- <span data-ttu-id="9daaa-858">Verarbeiten der Deinstallation von appx-Paketen der WSL-Distribution.</span><span class="sxs-lookup"><span data-stu-id="9daaa-858">Handle uninstalling of WSL distribution appx packages.</span></span>
- <span data-ttu-id="9daaa-859">Aktualisieren von procfs, um private und freigegebene Zuordnungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-859">Update procfs to show private and shared mappings.</span></span>
- <span data-ttu-id="9daaa-860">Hinzufügen einer Möglichkeit für „wslconfig.exe“ zum Bereinigen von Distributionen, die teilweise installiert oder deinstalliert wurden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-860">Add ability for wslconfig.exe to clean up distributions that are partially installed or uninstalled.</span></span>
- <span data-ttu-id="9daaa-861">Hinzufügen von Unterstützung für IP_MTU_DISCOVER für TCP-Sockets.</span><span class="sxs-lookup"><span data-stu-id="9daaa-861">Added support for IP_MTU_DISCOVER for TCP sockets.</span></span> <span data-ttu-id="9daaa-862">[GH 1639, 2115, 2205]</span><span class="sxs-lookup"><span data-stu-id="9daaa-862">[GH 1639, 2115, 2205]</span></span>
- <span data-ttu-id="9daaa-863">Ableiten der Protokollfamilie für Routen zu AF_INADDR.</span><span class="sxs-lookup"><span data-stu-id="9daaa-863">Infer protocol family for routes to AF_INADDR.</span></span>
- <span data-ttu-id="9daaa-864">Verbesserungen an seriellen Geräten [GH 1929].</span><span class="sxs-lookup"><span data-stu-id="9daaa-864">Serial device improvements [GH 1929].</span></span>

</br>

## <a name="build-16199"></a><span data-ttu-id="9daaa-865">Build 16199</span><span class="sxs-lookup"><span data-stu-id="9daaa-865">Build 16199</span></span>

<span data-ttu-id="9daaa-866">Allgemeine Windows-Informationen zu Build 16199 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-866">For general Windows information on build 16199 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-867">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-867">Fixed</span></span>
- <span data-ttu-id="9daaa-868">In diesen Releases gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-868">No WSL related changes in these releases.</span></span>

</br>

## <a name="build-16193"></a><span data-ttu-id="9daaa-869">Build 16193</span><span class="sxs-lookup"><span data-stu-id="9daaa-869">Build 16193</span></span>

<span data-ttu-id="9daaa-870">Allgemeine Windows-Informationen zu Build 16193 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-870">For general Windows information on build 16193 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-871">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-871">Fixed</span></span>
- <span data-ttu-id="9daaa-872">Racebedingung zwischen dem Senden von SIGCONT und einer Threadgruppe, die beendet wird [GH 1973]</span><span class="sxs-lookup"><span data-stu-id="9daaa-872">Race condition between sending SIGCONT and a threadgroup terminating [GH 1973]</span></span>
- <span data-ttu-id="9daaa-873">Ändern von TTY-und PTY-Geräten zum Melden von FILE_DEVICE_NAMED_PIPE anstelle von FILE_DEVICE_CONSOLE [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="9daaa-873">change tty and pty devices to report FILE_DEVICE_NAMED_PIPE instead of FILE_DEVICE_CONSOLE [GH 1840]</span></span>
- <span data-ttu-id="9daaa-874">SSH-Korrektur für IP_OPTIONS</span><span class="sxs-lookup"><span data-stu-id="9daaa-874">SSH fix for IP_OPTIONS</span></span>
- <span data-ttu-id="9daaa-875">Verschieben der DrvFs-Einbindung in den init-Daemon [GH 1862, 1968, 1767, 1933]</span><span class="sxs-lookup"><span data-stu-id="9daaa-875">Moved DrvFs mounting to init daemon [GH 1862, 1968, 1767, 1933]</span></span>
- <span data-ttu-id="9daaa-876">Hinzufügen von Unterstützung in DrvFs für die folgenden symbolischen NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-876">Added support in DrvFs for following NT symlinks.</span></span>

</br>

## <a name="build-16184"></a><span data-ttu-id="9daaa-877">Build 16184</span><span class="sxs-lookup"><span data-stu-id="9daaa-877">Build 16184</span></span>

<span data-ttu-id="9daaa-878">Allgemeine Windows-Informationen zu Build 16184 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-878">For general Windows information on build 16184 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-879">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-879">Fixed</span></span>
- <span data-ttu-id="9daaa-880">Entfernen des apt-Paketverwaltungstasks (lxrun.exe /update) wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-880">Removed apt package maintenance task (lxrun.exe /update)</span></span>
- <span data-ttu-id="9daaa-881">Korrektur der Nichtanzeige der Ausgabe aus Windows-Prozessen in node.js [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="9daaa-881">Fixed output not showing up in from Windows processes in node.js [GH 1840]</span></span>
- <span data-ttu-id="9daaa-882">Lockern der Ausrichtungsanforderungen in lxcore [GH 1794]</span><span class="sxs-lookup"><span data-stu-id="9daaa-882">Relax alignment requirements in lxcore [GH 1794]</span></span>
- <span data-ttu-id="9daaa-883">Korrektur der Verarbeitung des AT_EMPTY_PATH-Flags in mehreren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-883">Fixed handling of the AT_EMPTY_PATH flag in a numer of system calls.</span></span>
- <span data-ttu-id="9daaa-884">Korrektur eines Problems, bei dem das Löschen von DrvFs-Dateien mit geöffneten Handles bewirkt, dass die Datei nicht definiertes Verhalten aufweist [GH 544, 966, 1357, 1535, 1615]</span><span class="sxs-lookup"><span data-stu-id="9daaa-884">Fixed issue where deleting DrvFs files with open handles will cause the file to exhibit undefined behavior [GH 544,966,1357,1535,1615]</span></span>
- <span data-ttu-id="9daaa-885">„/etc/hosts“ erbt nun Einträge von der Windows-Hostdatei (%windir%\system32\drivers\etc\hosts) [GH 1495]</span><span class="sxs-lookup"><span data-stu-id="9daaa-885">/etc/hosts will now inherit entries from the Windows hosts file (%windir%\system32\drivers\etc\hosts) [GH 1495]</span></span>

</br>

## <a name="build-16179"></a><span data-ttu-id="9daaa-886">Build 16179</span><span class="sxs-lookup"><span data-stu-id="9daaa-886">Build 16179</span></span>

<span data-ttu-id="9daaa-887">Allgemeine Windows-Informationen zu Build 16179 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-887">For general Windows information on build 16179 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-888">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-888">Fixed</span></span>
- <span data-ttu-id="9daaa-889">Keine WSL-Änderungen in dieser Woche.</span><span class="sxs-lookup"><span data-stu-id="9daaa-889">No WSL changes this week.</span></span>

</br>

## <a name="build-16176"></a><span data-ttu-id="9daaa-890">Build 16176</span><span class="sxs-lookup"><span data-stu-id="9daaa-890">Build 16176</span></span>

<span data-ttu-id="9daaa-891">Allgemeine Windows-Informationen zu Build 16176 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-891">For general Windows information on build 16176 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-892">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-892">Fixed</span></span>

- [<span data-ttu-id="9daaa-893">Aktivierte serielle Unterstützung</span><span class="sxs-lookup"><span data-stu-id="9daaa-893">Enabled serial support</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- <span data-ttu-id="9daaa-894">Hinzufügen der IP-Socketoption IP_OPTIONS [GH 1116]</span><span class="sxs-lookup"><span data-stu-id="9daaa-894">Added IP socket option IP_OPTIONS [GH 1116]</span></span>
- <span data-ttu-id="9daaa-895">Implementierung der pwritev-Funktion (beim Hochladen der Datei nach nginx/PHP-FPM) [GH 1506]</span><span class="sxs-lookup"><span data-stu-id="9daaa-895">Implemented pwritev function (while uploading file to nginx/PHP-FPM) [GH 1506]</span></span>
- <span data-ttu-id="9daaa-896">Hinzufügen der IP-Socket-Optionen IP_MULTICAST_IF und IPV6_MULTICAST_IF [GH 990]</span><span class="sxs-lookup"><span data-stu-id="9daaa-896">Added IP socket options IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span></span>
- <span data-ttu-id="9daaa-897">Unterstützung für Socketoption IP_MULTICAST_LOOP und IPV6_MULTICAST_LOOP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="9daaa-897">Support for socket option IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span></span>
- <span data-ttu-id="9daaa-898">Hinzufügen von IP(V6)_MTU-Socketoption für den Knoten apps, traceroute, dig, nslookup, host</span><span class="sxs-lookup"><span data-stu-id="9daaa-898">Added IP(V6)_MTU socket option for apps node, traceroute, dig, nslookup, host</span></span>
- <span data-ttu-id="9daaa-899">Hinzufügen der IP-Socketoption IPV6_UNICAST_HOPS</span><span class="sxs-lookup"><span data-stu-id="9daaa-899">Added IP socket option IPV6_UNICAST_HOPS</span></span>
- [<span data-ttu-id="9daaa-900">Verbesserungen des Dateisystems</span><span class="sxs-lookup"><span data-stu-id="9daaa-900">Filesystem Improvements</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * <span data-ttu-id="9daaa-901">Ermöglichen der Einbindung von UNC-Pfaden</span><span class="sxs-lookup"><span data-stu-id="9daaa-901">Allow mounting of UNC paths</span></span>
    * <span data-ttu-id="9daaa-902">Ermöglichen von CDFS-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-902">Enable CDFS support in drvfs</span></span>
    * <span data-ttu-id="9daaa-903">Ordnungsgemäße Verarbeitung von Berechtigungen für Netzwerkdateisysteme in drvfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-903">Correctly handle permissions for network file systems in drvfs</span></span>
    * <span data-ttu-id="9daaa-904">Hinzufügen von Unterstützung für Remotelaufwerke zu drvfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-904">Add support for remote drives to drvfs</span></span>
    * <span data-ttu-id="9daaa-905">Ermöglichen von FAT-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-905">Enable FAT support in drvfs</span></span>
- <span data-ttu-id="9daaa-906">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-906">Additional fixes and Improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-907">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="9daaa-907">LTP Results</span></span>
<span data-ttu-id="9daaa-908">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="9daaa-908">No changes since 15042</span></span>

</br>

## <a name="build-16170"></a><span data-ttu-id="9daaa-909">Build 16170</span><span class="sxs-lookup"><span data-stu-id="9daaa-909">Build 16170</span></span>

<span data-ttu-id="9daaa-910">Allgemeine Windows-Informationen zu Build 16170 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-910">For general Windows information on build 16170 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span></span><br/>

<span data-ttu-id="9daaa-911">Wir haben einen neuen [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) veröffentlicht, in dem unsere Anstrengungen beim Testen von WSL erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-911">We released a new [blog post](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) discussing our efforts to test WSL.</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-912">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-912">Fixed</span></span>

- <span data-ttu-id="9daaa-913">Unterstützung für Socketoption IP_ADD_MEMBERSHIP und IPV6_ADD_MEMBERSHIP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="9daaa-913">Support socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span></span>
- <span data-ttu-id="9daaa-914">Hinzufügen von Unterstützung für PTRACE_OLDSETOPTIONS.</span><span class="sxs-lookup"><span data-stu-id="9daaa-914">Add support for PTRACE_OLDSETOPTIONS.</span></span> <span data-ttu-id="9daaa-915">[GH 1692]</span><span class="sxs-lookup"><span data-stu-id="9daaa-915">[GH 1692]</span></span>
- <span data-ttu-id="9daaa-916">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-916">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-917">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="9daaa-917">LTP Results</span></span>
<span data-ttu-id="9daaa-918">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="9daaa-918">No changes since 15042</span></span>

</br>

## <a name="build-15046-to-windows-10-creators-update"></a><span data-ttu-id="9daaa-919">Build 15046 für Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="9daaa-919">Build 15046 to Windows 10 Creators Update</span></span>
<span data-ttu-id="9daaa-920">Es gibt keine weiteren WSL-Korrekturen oder-Funktionen, die für die Einbindung in das Creators Update in Windows 10 geplant sind.</span><span class="sxs-lookup"><span data-stu-id="9daaa-920">There are no more WSL fixes or features planned for inclusion in the Creators Update to Windows 10.</span></span> <span data-ttu-id="9daaa-921">Die Anmerkungen zu dieser Version von WSL werden in den kommenden Wochen fortgesetzt, um Ergänzungen für das nächste Hauptupdate von Windows aufzuführen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-921">Release notes for WSL will resume in the coming weeks for additions targeting the next major Windows Update.</span></span> <span data-ttu-id="9daaa-922">Allgemeine Windows-Informationen zu Build 15046 und zukünftigen Insider Releases finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-922">For general Windows information on build 15046 and future Insider releases visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span></span> <br/><br/>
 <br/>

## <a name="build-15042"></a><span data-ttu-id="9daaa-923">Build 15042</span><span class="sxs-lookup"><span data-stu-id="9daaa-923">Build 15042</span></span>

<span data-ttu-id="9daaa-924">Allgemeine Windows-Informationen zu Build 15042 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-924">For general Windows information on build 15042 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-925">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-925">Fixed</span></span>

- <span data-ttu-id="9daaa-926">Korrektur eines Deadlocks beim Entfernen eines Pfades, der auf „..“ endet</span><span class="sxs-lookup"><span data-stu-id="9daaa-926">Fix for a deadlock when removing a path ending in ".."</span></span>
- <span data-ttu-id="9daaa-927">Korrektur eines Problems, bei dem FIONBIO bei Erfolg 0 zurückgibt [GH 1683]</span><span class="sxs-lookup"><span data-stu-id="9daaa-927">Fixed an issue where FIONBIO not returning 0 on success [GH 1683]</span></span>
- <span data-ttu-id="9daaa-928">Korrektur eines Problems bei Lesevorgängen mit einer Länge von Null von Internetdatagrammsockets</span><span class="sxs-lookup"><span data-stu-id="9daaa-928">Fixed issue with zero-length reads of inet datagram sockets</span></span>
- <span data-ttu-id="9daaa-929">Korrektur eines möglichen Deadlocks aufgrund einer Racebedingung bei der drvfs inode-Suche [GH 1675]</span><span class="sxs-lookup"><span data-stu-id="9daaa-929">Fix possible deadlock due to race condition in drvfs inode lookup [GH 1675]</span></span>
- <span data-ttu-id="9daaa-930">Erweiterte Unterstützung für Hilfsdaten von Unix-Sockets, SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613, 1326]</span><span class="sxs-lookup"><span data-stu-id="9daaa-930">Extended support for unix socket ancillary data; SCM_CREDENTIALS and SCM_RIGHTS [GH 514, 613, 1326]</span></span>
- <span data-ttu-id="9daaa-931">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-931">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-932">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-932">LTP Results:</span></span>
<span data-ttu-id="9daaa-933">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="9daaa-933">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="9daaa-934">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9daaa-934">Number of non-Passing (failing, skipped, etc…): 255</span></span>

</br>

## <a name="build-15031"></a><span data-ttu-id="9daaa-935">Build 15031</span><span class="sxs-lookup"><span data-stu-id="9daaa-935">Build 15031</span></span>

<span data-ttu-id="9daaa-936">Allgemeine Windows-Informationen zu Build 15031 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-936">For general Windows information on build 15031 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-937">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-937">Fixed</span></span>

- <span data-ttu-id="9daaa-938">Korrektur eines Fehlers, bei dem sich time(2) sporadisch falsch verhielt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-938">Fixed a bug where time(2) would sporadically misbehave.</span></span>
- <span data-ttu-id="9daaa-939">Korrektur eines Problems, bei dem \*SIGPROCMASK-Systemaufrufe die Signalmaske beschädigen konnten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-939">Fixed and issue where \*SIGPROCMASK syscalls could corrupt signal mask.</span></span>
- <span data-ttu-id="9daaa-940">Jetzt Rückgabe der vollständigen Länge der Befehlszeile in WSL-Benachrichtigung zur Prozesserstellung.</span><span class="sxs-lookup"><span data-stu-id="9daaa-940">Now return full command line length in WSL process creation notification.</span></span> <span data-ttu-id="9daaa-941">[GH 1632]</span><span class="sxs-lookup"><span data-stu-id="9daaa-941">[GH 1632]</span></span>
- <span data-ttu-id="9daaa-942">WSL meldet jetzt die Threadbeendigung über ptrace für GDB-Hänger.</span><span class="sxs-lookup"><span data-stu-id="9daaa-942">WSL now reports thread exit through ptrace for GDB hangs.</span></span> <span data-ttu-id="9daaa-943">[GH 1196]</span><span class="sxs-lookup"><span data-stu-id="9daaa-943">[GH 1196]</span></span>
- <span data-ttu-id="9daaa-944">Korrektur eines Fehlers, bei dem ptys nach hoher tmux-E/A nicht mehr reagiert</span><span class="sxs-lookup"><span data-stu-id="9daaa-944">Fixed bug where ptys would hang after heavy tmux IO.</span></span> <span data-ttu-id="9daaa-945">[GH 1358]</span><span class="sxs-lookup"><span data-stu-id="9daaa-945">[GH 1358]</span></span>
- <span data-ttu-id="9daaa-946">Korrektur der Timeoutüberprüfung in zahlreichen Systemaufrufen (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span><span class="sxs-lookup"><span data-stu-id="9daaa-946">Fixed timeout validation in many system calls (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span></span>
- <span data-ttu-id="9daaa-947">Hinzufügen von eventfd EFD_SEMAPHORE-Unterstützung [GH 452]</span><span class="sxs-lookup"><span data-stu-id="9daaa-947">Added eventfd EFD_SEMAPHORE support [GH 452]</span></span>
- <span data-ttu-id="9daaa-948">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-948">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-949">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-949">LTP Results:</span></span>
<span data-ttu-id="9daaa-950">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="9daaa-950">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="9daaa-951">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9daaa-951">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9daaa-952">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-952">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a><span data-ttu-id="9daaa-953">Build 15025</span><span class="sxs-lookup"><span data-stu-id="9daaa-953">Build 15025</span></span>

<span data-ttu-id="9daaa-954">Allgemeine Windows-Informationen zu Build 15025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-954">For general Windows information on build 15025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-955">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-955">Fixed</span></span>

- <span data-ttu-id="9daaa-956">Korrektur eines Fehlers, bei dem grep 2.27 nicht mehr funktioniert [GH 1578]</span><span class="sxs-lookup"><span data-stu-id="9daaa-956">Fix for bug that broke grep 2.27 [GH 1578]</span></span>
- <span data-ttu-id="9daaa-957">Implementierung des EFD_SEMAPHORE-Flags für den eventfd2-Systemaufruf [GH 452]</span><span class="sxs-lookup"><span data-stu-id="9daaa-957">Implemented EFD_SEMAPHORE flag for eventfd2 syscall [GH 452]</span></span>
- <span data-ttu-id="9daaa-958">Implementierung von /proc/[pid]/net/ipv6_route [GH 1608]</span><span class="sxs-lookup"><span data-stu-id="9daaa-958">Implemented /proc/[pid]/net/ipv6_route [GH 1608]</span></span>
- <span data-ttu-id="9daaa-959">Signalgestützte E/A-Unterstützung für Unix-Streamsockets [GH 393, 68]</span><span class="sxs-lookup"><span data-stu-id="9daaa-959">Signal driven IO support for unix stream sockets [GH 393, 68]</span></span>
- <span data-ttu-id="9daaa-960">Unterstützung für F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]</span><span class="sxs-lookup"><span data-stu-id="9daaa-960">Support F_GETPIPE_SZ and F_SETPIPE_SZ [GH 1012]</span></span>
- <span data-ttu-id="9daaa-961">Implementierung des recvmmsg()-Systemaufrufs [GH 1531]</span><span class="sxs-lookup"><span data-stu-id="9daaa-961">Implement recvmmsg() syscall [GH 1531]</span></span>
- <span data-ttu-id="9daaa-962">Korrektur eines Fehlers, bei dem epoll_wait() nicht gewartet hat [GH 1609]</span><span class="sxs-lookup"><span data-stu-id="9daaa-962">Fixed bug where epoll_wait() wasn't waiting [GH 1609]</span></span>
- <span data-ttu-id="9daaa-963">Implementierung von /proc/version_signature</span><span class="sxs-lookup"><span data-stu-id="9daaa-963">Implement /proc/version_signature</span></span>
- <span data-ttu-id="9daaa-964">Tee-Systemaufruf gibt jetzt einen Fehler zurück, wenn beide Dateideskriptoren auf dieselbe Pipe verweisen</span><span class="sxs-lookup"><span data-stu-id="9daaa-964">Tee syscall now returns failure if both file descriptors refer to the same pipe</span></span>
- <span data-ttu-id="9daaa-965">Implementierung des richtigen Verhaltens für SO_PEERCRED für Unix-Sockets</span><span class="sxs-lookup"><span data-stu-id="9daaa-965">Implemented correct behavior for SO_PEERCRED for Unix sockets</span></span>
- <span data-ttu-id="9daaa-966">Korrektur der Verarbeitung ungültiger Parameter des tkill-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9daaa-966">Fixed tkill syscall invalid parameter handling</span></span>
- <span data-ttu-id="9daaa-967">Änderungen zum Verbessern der Leistung von drvfs</span><span class="sxs-lookup"><span data-stu-id="9daaa-967">Changes to increase the preformace of drvfs</span></span>
- <span data-ttu-id="9daaa-968">Kleinere Korrektur für Ruby-E/A-Blockierung</span><span class="sxs-lookup"><span data-stu-id="9daaa-968">Minor fix for Ruby IO blocking</span></span>
- <span data-ttu-id="9daaa-969">Korrektur von recvmsg() beim Zurückgeben von EINVAL für das MSG_DONTWAIT-Flag für Inet-Sockets [GH 1296]</span><span class="sxs-lookup"><span data-stu-id="9daaa-969">Fixed recvmsg() returning EINVAL for the MSG_DONTWAIT flag for inet sockets [GH 1296]</span></span>
- <span data-ttu-id="9daaa-970">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-970">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-971">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-971">LTP Results:</span></span>
<span data-ttu-id="9daaa-972">Anzahl bestandener Tests: 732</span><span class="sxs-lookup"><span data-stu-id="9daaa-972">Number of Passing Test: 732</span></span></br>
<span data-ttu-id="9daaa-973">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9daaa-973">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9daaa-974">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-974">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a><span data-ttu-id="9daaa-975">Build 15019</span><span class="sxs-lookup"><span data-stu-id="9daaa-975">Build 15019</span></span>

<span data-ttu-id="9daaa-976">Allgemeine Windows-Informationen zu Build 15019 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-976">For general Windows information on build 15019 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-977">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-977">Fixed</span></span>

- <span data-ttu-id="9daaa-978">Korrektur eines Fehlers, der fälschlicherweise die CPU-Auslastung in procfs für Tools wie htop gemeldet hat [GH 823, 945, 971]</span><span class="sxs-lookup"><span data-stu-id="9daaa-978">Fixed bug that incorrectly reported CPU usage in procfs for tools like htop (GH 823, 945, 971)</span></span>
- <span data-ttu-id="9daaa-979">Beim Aufrufen von open() mit O_TRUNC für eine vorhandene Datei „inotify“ wird nun IN_MODIFY vor IN_OPEN generiert</span><span class="sxs-lookup"><span data-stu-id="9daaa-979">When calling open() with O_TRUNC on an existing file inotify now generates IN_MODIFY before IN_OPEN</span></span>
- <span data-ttu-id="9daaa-980">Korrekturen für den Unix-Socket getsockopt SO_ERROR zum Aktivieren von Postgress [GH 61, 1354]</span><span class="sxs-lookup"><span data-stu-id="9daaa-980">Fixes to unix socket getsockopt SO_ERROR to enable postgress [GH 61, 1354]</span></span>
- <span data-ttu-id="9daaa-981">Implementierung von /proc/sys/net/core/somaxconn für die Sprache GO</span><span class="sxs-lookup"><span data-stu-id="9daaa-981">Implement /proc/sys/net/core/somaxconn for the GO language</span></span>
- <span data-ttu-id="9daaa-982">Der Apt-get-Packageupdate-Hintergrundtask wird jetzt aus der Ansicht ausgeblendet</span><span class="sxs-lookup"><span data-stu-id="9daaa-982">Apt-get package update background task now runs hidden from view</span></span>
- <span data-ttu-id="9daaa-983">Löschen des Bereichs für ipv6 localhost (Fehler Spring-Framework (Java)).</span><span class="sxs-lookup"><span data-stu-id="9daaa-983">Clear scope for ipv6 localhost (Spring-Framework(Java) failure).</span></span>
- <span data-ttu-id="9daaa-984">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-984">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-985">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-985">LTP Results:</span></span>
<span data-ttu-id="9daaa-986">Anzahl bestandener Tests: 714</span><span class="sxs-lookup"><span data-stu-id="9daaa-986">Number of Passing Test: 714</span></span> </br>
<span data-ttu-id="9daaa-987">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 249</span><span class="sxs-lookup"><span data-stu-id="9daaa-987">Number of non-Passing (failing, skipped, etc…): 249</span></span> </br>
[<span data-ttu-id="9daaa-988">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-988">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a><span data-ttu-id="9daaa-989">Build 15014</span><span class="sxs-lookup"><span data-stu-id="9daaa-989">Build 15014</span></span>

<span data-ttu-id="9daaa-990">Allgemeine Windows-Informationen zu Build 15014 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="9daaa-990">For general Windows information on build 15014 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-991">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-991">Fixed</span></span>

- <span data-ttu-id="9daaa-992">STRG+C funktioniert nun wie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="9daaa-992">Ctrl+C now works as intended</span></span>
- <span data-ttu-id="9daaa-993">htop und ps auxw zeigen jetzt die richtige Ressourcenverwendung an (GH #516)</span><span class="sxs-lookup"><span data-stu-id="9daaa-993">htop and ps auxw now show correct resource utilization (GH #516)</span></span>
- <span data-ttu-id="9daaa-994">Grundlegende Übersetzung von NT-Ausnahmen in Signale.</span><span class="sxs-lookup"><span data-stu-id="9daaa-994">Basic translation of NT exceptions to signals.</span></span> <span data-ttu-id="9daaa-995">(GH #513)</span><span class="sxs-lookup"><span data-stu-id="9daaa-995">(GH #513)</span></span>
- <span data-ttu-id="9daaa-996">fallocate schlägt nun mit ENOSPC anstatt mit EINVAL fehl, wenn nicht genügend Speicherplatz verfügbar ist (GH #1571)</span><span class="sxs-lookup"><span data-stu-id="9daaa-996">fallocate now fails with ENOSPC  when running out of space instead of EINVAL (GH #1571)</span></span>
- <span data-ttu-id="9daaa-997">Hinzufügen von /proc/sys/kernel/sem.</span><span class="sxs-lookup"><span data-stu-id="9daaa-997">Added /proc/sys/kernel/sem.</span></span>
- <span data-ttu-id="9daaa-998">Implementierung der semop- und semtimedop-Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="9daaa-998">Implemented semop and semtimedop system calls</span></span>
- <span data-ttu-id="9daaa-999">Korrektur von nslookup-Fehlern mit der IP_RECVTOS- und IPV6_RECVTCLASS-Socketoption (GH 69)</span><span class="sxs-lookup"><span data-stu-id="9daaa-999">Fixed nslookup errors with IP_RECVTOS & IPV6_RECVTCLASS socket option (GH 69)</span></span>
- <span data-ttu-id="9daaa-1000">Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT</span><span class="sxs-lookup"><span data-stu-id="9daaa-1000">Support for socket options IP_RECVTTL and IPV6_RECVHOPLIMIT</span></span>
- <span data-ttu-id="9daaa-1001">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1001">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1002">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1002">LTP Results:</span></span>
<span data-ttu-id="9daaa-1003">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="9daaa-1003">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="9daaa-1004">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9daaa-1004">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9daaa-1005">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1005">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a><span data-ttu-id="9daaa-1006">Zusammenfassung der Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="9daaa-1006">Syscall Summary</span></span>
<span data-ttu-id="9daaa-1007">Systemaufrufe gesamt: 384</span><span class="sxs-lookup"><span data-stu-id="9daaa-1007">Total Syscalls: 384</span></span> </br>
<span data-ttu-id="9daaa-1008">Implementiert gesamt: 235</span><span class="sxs-lookup"><span data-stu-id="9daaa-1008">Total Implemented: 235</span></span> </br>
<span data-ttu-id="9daaa-1009">Mit Stub versehen gesamt: 22</span><span class="sxs-lookup"><span data-stu-id="9daaa-1009">Total Stubbed: 22</span></span> </br>
<span data-ttu-id="9daaa-1010">Nicht implementiert gesamt: 127</span><span class="sxs-lookup"><span data-stu-id="9daaa-1010">Total Unimplemented: 127</span></span> </br>
[<span data-ttu-id="9daaa-1011">Ausführliche Aufschlüsselung</span><span class="sxs-lookup"><span data-stu-id="9daaa-1011">Detailed Breakdown</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a><span data-ttu-id="9daaa-1012">Build 15007</span><span class="sxs-lookup"><span data-stu-id="9daaa-1012">Build 15007</span></span>

<span data-ttu-id="9daaa-1013">Allgemeine Windows-Informationen zu Build 15007 finden Sie im [Windows-Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1013">For general Windows information on build 15007 visit the [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="9daaa-1014">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9daaa-1014">Known Issue</span></span>

- <span data-ttu-id="9daaa-1015">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1015">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="9daaa-1016">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1016">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="9daaa-1017">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1017">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="9daaa-1018">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1018">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="9daaa-1019">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1019">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="9daaa-1020">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1020">Users can explore the option to include this in their `.bashrc`</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-1021">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1021">Fixed</span></span>

- <span data-ttu-id="9daaa-1022">Korrektur eines Problems, bei dem die Ausführung von WSL 100 % eines CPU-Kerns verbraucht</span><span class="sxs-lookup"><span data-stu-id="9daaa-1022">Corrected the issue where running WSL would consume 100% of a CPU core</span></span>
- <span data-ttu-id="9daaa-1023">Socketoption IP_PKTINFO, IPV6_RECVPKTINFO wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1023">Socket option IP_PKTINFO, IPV6_RECVPKTINFO now supported.</span></span> <span data-ttu-id="9daaa-1024">(GH #851, 987)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1024">(GH #851, 987)</span></span>
- <span data-ttu-id="9daaa-1025">Abschneiden der physischen Adresse der Netzwerkschnittstelle auf 16 Bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1025">Truncate network interface physical address to 16 bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span></span>
- <span data-ttu-id="9daaa-1026">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1026">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1027">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1027">LTP Results:</span></span>
<span data-ttu-id="9daaa-1028">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="9daaa-1028">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="9daaa-1029">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9daaa-1029">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9daaa-1030">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1030">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a><span data-ttu-id="9daaa-1031">Build 15002</span><span class="sxs-lookup"><span data-stu-id="9daaa-1031">Build 15002</span></span>

<span data-ttu-id="9daaa-1032">Allgemeine Windows-Informationen zu Build 15002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1032">For general Windows information on build 15002 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="9daaa-1033">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9daaa-1033">Known Issue</span></span>

<span data-ttu-id="9daaa-1034">Zwei bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1034">Two known issues:</span></span>
- <span data-ttu-id="9daaa-1035">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1035">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="9daaa-1036">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1036">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="9daaa-1037">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1037">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="9daaa-1038">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1038">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="9daaa-1039">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1039">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="9daaa-1040">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1040">Users can explore the option to include this in their `.bashrc`</span></span>

- <span data-ttu-id="9daaa-1041">Während der Ausführung von WSL werden von einem Systemthread 100 % eines CPU-Kerns beansprucht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1041">While WSL is running a system thread will consume 100% of a CPU core.</span></span>  <span data-ttu-id="9daaa-1042">Die Ursache wurde untersucht und intern behoben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1042">The root cause has been addressed and fixed internally.</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-1043">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1043">Fixed</span></span>

- <span data-ttu-id="9daaa-1044">Alle Bash-Sitzungen müssen jetzt auf derselben Berechtigungsebene erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1044">All bash sessions must now be created at the same permission level.</span></span>  <span data-ttu-id="9daaa-1045">Der Versuch, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1045">Attempting to start a session at a different level will be blocked.</span></span>  <span data-ttu-id="9daaa-1046">Dies bedeutet, dass Administrator-und Nicht-Administratorkonsolen nicht gleichzeitig ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1046">This means admin and non-admin consoles cannot run at the same time.</span></span> <span data-ttu-id="9daaa-1047">(GH #626)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1047">(GH #626)</span></span>
<br/>
- <span data-ttu-id="9daaa-1048">Implementierung der folgenden NETLINK_ROUTE-Meldungen (erfordert Windows-Administrator)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1048">Implemented the following NETLINK_ROUTE messages (requires Windows admin)</span></span>
     - <span data-ttu-id="9daaa-1049">RTM_NEWADDR (unterstützt `ip addr add`)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1049">RTM_NEWADDR (supports `ip addr add`)</span></span>
     - <span data-ttu-id="9daaa-1050">RTM_NEWROUTE (unterstützt `ip route add`)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1050">RTM_NEWROUTE (supports `ip route add`)</span></span>
     - <span data-ttu-id="9daaa-1051">RTM_DELADDR (unterstützt `ip addr del`)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1051">RTM_DELADDR (supports `ip addr del`)</span></span>
     - <span data-ttu-id="9daaa-1052">RTM_DELROUTE (unterstützt `ip route del`)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1052">RTM_DELROUTE (supports `ip route del`)</span></span>
- <span data-ttu-id="9daaa-1053">Die geplante Tasküberprüfung für zu aktualisierende Pakete wird nicht mehr über eine getaktete Verbindung ausgeführt (GH #1371)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1053">Scheduled task checking for packages to update will no longer run on a metered connection (GH #1371)</span></span>
- <span data-ttu-id="9daaa-1054">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1054">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="9daaa-1055">Implementierung der TCP_KEEPCNT-Socketoption (GH #843)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1055">Implemented TCP_KEEPCNT socket option (GH #843)</span></span>
- <span data-ttu-id="9daaa-1056">Implementierung der IP_MTU_DISCOVER INET-Socketoption (GH #720, 717, 170, 69)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1056">Implemented IP_MTU_DISCOVER INET socket option (GH #720, 717, 170, 69)</span></span>
- <span data-ttu-id="9daaa-1057">Entfernen der Legacyfnktionalität zum Ausführen von NT-Binärdateien aus init mit NT-Pfadsuche.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1057">Removed legacy functionality to run NT binaries from init with NT path lookup.</span></span> <span data-ttu-id="9daaa-1058">(GH #1325)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1058">(GH #1325)</span></span>
- <span data-ttu-id="9daaa-1059">Korrektur des Modus von /dev/kmsg zum Zulassen von Gruppen-/sonstigem Lesezugriff (0644) (GH #1321)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1059">Fix mode of /dev/kmsg to allow group / other read access (0644) (GH #1321)</span></span>
- <span data-ttu-id="9daaa-1060">Implementierung von /proc/sys/kernel/random/uuid (GH #1092)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1060">Implemented /proc/sys/kernel/random/uuid  (GH #1092)</span></span>
- <span data-ttu-id="9daaa-1061">Korrektur eines Fehlers, bei dem die Startzeit des Prozesses als Jahr 2432 angezeigt wurde (GH #974)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1061">Corrected error where process start time was showing as year 2432 (GH #974)</span></span>
- <span data-ttu-id="9daaa-1062">Wechseln der TERM-Standardumgebungsvariablen in xterm-256color (GH #1446)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1062">Switched default TERM environment variable to xterm-256color (GH #1446)</span></span>
- <span data-ttu-id="9daaa-1063">Änderung der Art und Weise, in der der Prozesscommit während des Prozessforks berechnet wird.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1063">Modified the way that process commit is calculated during process fork.</span></span> <span data-ttu-id="9daaa-1064">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1064">(GH #1286)</span></span>
- <span data-ttu-id="9daaa-1065">Implementierung von /proc/sys/vm/overcommit_memory.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1065">Implemented /proc/sys/vm/overcommit_memory.</span></span> <span data-ttu-id="9daaa-1066">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1066">(GH #1286)</span></span>
- <span data-ttu-id="9daaa-1067">Implementierung der /proc/net/route-Datei (GH #69)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1067">Implemented /proc/net/route file (GH #69)</span></span>
- <span data-ttu-id="9daaa-1068">Korrektur eines Fehlers, bei dem der Verknüpfungsname falsch lokalisiert wurde (GH #696)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1068">Fixed error where shortcut name was incorrectly localized (GH #696)</span></span>
- <span data-ttu-id="9daaa-1069">Korrektur der fehlerhaften ELF-Verarbeitungslogik, die die Programmheader nicht ordnungsgemäß so überprüft, dass sie kleiner als (oder gleich) PATH_MAX sein müssen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1069">Fixed elf parsing logic that is incorrectly validating the program headers must be less than (or equal to) PATH_MAX.</span></span> <span data-ttu-id="9daaa-1070">(GH #1048)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1070">(GH #1048)</span></span>
- <span data-ttu-id="9daaa-1071">Implementierung des statfs-Rückrufs für procfs, sysfs, cgroupfs und binfmts (GH #1378)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1071">Implemented statfs callback for procfs, sysfs, cgroupfs, and binfmtfs (GH #1378)</span></span>
- <span data-ttu-id="9daaa-1072">Korrektur der AptPackageIndexUpdate-Fenster, die nicht geschlossen werden (GH #1184, auch in GH #1193 beschrieben)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1072">Fixed AptPackageIndexUpdate windows that won’t close (GH #1184, also discussed in GH #1193)</span></span>
- <span data-ttu-id="9daaa-1073">Hinzufügen von ASLR-Personality, ADDR_NO_RANDOMIZE-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1073">Added ASLR personality  ADDR_NO_RANDOMIZE support.</span></span> <span data-ttu-id="9daaa-1074">[GH #1148, 1128]</span><span class="sxs-lookup"><span data-stu-id="9daaa-1074">(GH #1148, 1128)</span></span>
- <span data-ttu-id="9daaa-1075">Verbesserung von PTRACE_GETSIGINFO, SIGSEGV für ordnungsgemäße gdb-Stapelüberwachungen während AV (GH #875)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1075">Improved PTRACE_GETSIGINFO, SIGSEGV, for proper gdb stack traces during AV (GH #875)</span></span>
- <span data-ttu-id="9daaa-1076">Elf-Verarbeitung schlägt für patchelf-Binärdateien nicht mehr fehl.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1076">Elf parsing no longer fails for patchelf binaries.</span></span> <span data-ttu-id="9daaa-1077">[GH #471]</span><span class="sxs-lookup"><span data-stu-id="9daaa-1077">(GH #471)</span></span>
- <span data-ttu-id="9daaa-1078">VPN DNS-Weitergabe an /etc/resolv.conf (GH #416, 1350)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1078">VPN DNS propagated to /etc/resolv.conf (GH #416, 1350)</span></span>
- <span data-ttu-id="9daaa-1079">Verbesserungen an TCP Close für eine zuverlässigere Datenübertragung.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1079">Improvements to TCP close for more reliable data transfer.</span></span> <span data-ttu-id="9daaa-1080">(GH #610, 616, 1025, 1335)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1080">(GH #610, 616, 1025, 1335)</span></span>
- <span data-ttu-id="9daaa-1081">Jetzt Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden (EMFILE).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1081">Now return correct error code when too many files are opened (EMFILE).</span></span> <span data-ttu-id="9daaa-1082">(GH #1126, 2090)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1082">(GH #1126, 2090)</span></span>
- <span data-ttu-id="9daaa-1083">Windows-Überwachungsprotokoll erfasst jetzt den Imagenamen in Process Create Audit.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1083">Windows Audit log now reports the image name in process create audit.</span></span>
- <span data-ttu-id="9daaa-1084">Jetzt normaler Fehler beim Starten von „bash.exe“ in einem Bash-Fenster.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1084">Now gracefully fail when launching bash.exe from within a bash window</span></span>
- <span data-ttu-id="9daaa-1085">Hinzufügen einer Fehlermeldung, wenn Interop nicht auf ein Arbeitsverzeichnis unter LxFs zugreifen kann (z.B. BASHRC-Datei von „notepad.exe“).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1085">Added error message when interop is unable to access a working directory under LxFs (i.e. notepad.exe .bashrc)</span></span>
- <span data-ttu-id="9daaa-1086">Korrektur eines Problems, bei dem der Windows-Pfad in WSL abgeschnitten wurde</span><span class="sxs-lookup"><span data-stu-id="9daaa-1086">Fixed issue where Windows path was truncated in WSL</span></span>
- <span data-ttu-id="9daaa-1087">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1087">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1088">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1088">LTP Results:</span></span>
<span data-ttu-id="9daaa-1089">Anzahl bestandener Tests: 690</span><span class="sxs-lookup"><span data-stu-id="9daaa-1089">Number of Passing Test: 690</span></span> </br>
<span data-ttu-id="9daaa-1090">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 274</span><span class="sxs-lookup"><span data-stu-id="9daaa-1090">Number of non-Passing (failing, skipped, etc…): 274</span></span> </br>
[<span data-ttu-id="9daaa-1091">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1091">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1092">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1092">Syscall Support</span></span>
<span data-ttu-id="9daaa-1093">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1093">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1094">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1094">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a><span data-ttu-id="9daaa-1095">Build 14986</span><span class="sxs-lookup"><span data-stu-id="9daaa-1095">Build 14986</span></span>

<span data-ttu-id="9daaa-1096">Allgemeine Windows-Informationen zu Build 14986 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1096">For general Windows information on build 14986 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1097">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1097">Fixed</span></span>

- <span data-ttu-id="9daaa-1098">Korrektur von Fehlerüberprüfungen mit Netlink und Pty IOCTLs</span><span class="sxs-lookup"><span data-stu-id="9daaa-1098">Fixed bugchecks with Netlink and Pty IOCTLs</span></span>
- <span data-ttu-id="9daaa-1099">Kernel Version meldet nun 4.4.0-43 aus Gründen der Konsistenz mit Xenial</span><span class="sxs-lookup"><span data-stu-id="9daaa-1099">Kernel version now reports 4.4.0-43 for consistency with Xenial</span></span>
- <span data-ttu-id="9daaa-1100">„Bash.exe“ wird jetzt gestartet, wenn die Eingabe an „nul:“ gerichtet ist (GH #1259)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1100">Bash.exe now launches when input directed to 'nul:' (GH #1259)</span></span>
- <span data-ttu-id="9daaa-1101">Thread-IDs werden nun ordnungsgemäß in procfs erfasst (GH #967)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1101">Thread IDs now reported correctly in procfs (GH #967)</span></span>
- <span data-ttu-id="9daaa-1102">Flags IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR werden jetzt in inotify_add_watch() unterstützt (GH #1280)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1102">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR flags now supported in inotify_add_watch() (GH #1280)</span></span>
- <span data-ttu-id="9daaa-1103">Implementierung von timer_create und verwandten Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1103">Implement timer_create and related system calls.</span></span>  <span data-ttu-id="9daaa-1104">Dies ermöglicht die GHC-Unterstützung (GH #307).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1104">This enables GHC support (GH #307)</span></span>
- <span data-ttu-id="9daaa-1105">Korrektur eines Problems, bei dem Ping eine Zeitangabe von 0,000 ms zurückgab (GH #1296)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1105">Fixed issue where ping returned a time of 0.000ms (GH #1296)</span></span>
- <span data-ttu-id="9daaa-1106">Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1106">Return correct error code when too many files are opened.</span></span>
- <span data-ttu-id="9daaa-1107">Korrektur eines Problems in WSL, bei dem die Netlink-Anforderung für Netzwerkschnittstellendaten mit EINVAL fehlschlägt, wenn die Hardwareadresse der Schnittstelle 32 Bytes groß ist (z.B. die Teredo-Schnittstelle)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1107">Fixed issue in WSL where Netlink request for network interface data would fail with EINVAL if the interface's hardware address is 32-bytes (such as the Teredo interface)</span></span>
   - <span data-ttu-id="9daaa-1108">Beachten Sie, dass das Linux-Hilfsprogramm „ip“ einen Fehler enthält, bei dem ein Absturz erfolgt, wenn WSL eine 32-Byte-Hardwareadresse meldet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1108">Note that the Linux "ip" utility contains a bug where it will crash if WSL reports a 32-byte hardware address.</span></span> <span data-ttu-id="9daaa-1109">Dies ist ein Fehler in „ip“, nicht in WSL.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1109">This is a bug in "ip", not WSL.</span></span> <span data-ttu-id="9daaa-1110">Mit dem Hilfsprogramm „ip“ wird die Länge des Zeichenfolgenpuffers fest codiert, der zum Ausgeben der Hardwareadresse verwendet wird, und dieser Puffer ist zu klein, um eine 32-Byte-Hardwareadresse auszugeben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1110">The “ip” utility hard-codes the length of the string buffer used to print the hardware address, and that buffer is too small to print a 32-byte hardware address.</span></span>
- <span data-ttu-id="9daaa-1111">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1111">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1112">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1112">LTP Results:</span></span>
<span data-ttu-id="9daaa-1113">Anzahl bestandener Tests: 669</span><span class="sxs-lookup"><span data-stu-id="9daaa-1113">Number of Passing Test: 669</span></span> </br>
<span data-ttu-id="9daaa-1114">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="9daaa-1114">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="9daaa-1115">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1115">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1116">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1116">Syscall Support</span></span>
<span data-ttu-id="9daaa-1117">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1117">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1118">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1118">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a><span data-ttu-id="9daaa-1119">Build 14971</span><span class="sxs-lookup"><span data-stu-id="9daaa-1119">Build 14971</span></span>

<span data-ttu-id="9daaa-1120">Allgemeine Windows-Informationen zu Build 14971 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1120">For general Windows information on build 14971 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1121">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1121">Fixed</span></span>

 - <span data-ttu-id="9daaa-1122">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1122">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9daaa-1123">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1123">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1124">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1124">LTP Results:</span></span>
<span data-ttu-id="9daaa-1125">Keine Änderungen seit 14965</span><span class="sxs-lookup"><span data-stu-id="9daaa-1125">Unchanged from 14965</span></span> </br>
<span data-ttu-id="9daaa-1126">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9daaa-1126">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9daaa-1127">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1127">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1128">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1128">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a><span data-ttu-id="9daaa-1129">Build 14965</span><span class="sxs-lookup"><span data-stu-id="9daaa-1129">Build 14965</span></span>

<span data-ttu-id="9daaa-1130">Allgemeine Windows-Informationen zu Build 14965 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1130">For general Windows information on build 14965 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1131">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1131">Fixed</span></span>

- <span data-ttu-id="9daaa-1132">Unterstützung für Netlink-Sockets RTM_GETLINK und RTM_GETADDR des NETLINK_ROUTE-Protokolls (GH #468)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1132">Support for Netlink sockets NETLINK_ROUTE protocol's RTM_GETLINK and RTM_GETADDR (GH #468)</span></span>
  - <span data-ttu-id="9daaa-1133">Aktiviert ifconfig- und ip-Befehle für die Netzwerkenumeration.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1133">Enables ifconfig and ip commands for network enumeration</span></span>
  - <span data-ttu-id="9daaa-1134">Weitere Informationen finden Sie in unserem [Blogbeitrag zu WSL-Netzwerken](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1134">More information can be found in our [WSL Networking blog post](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span></span>

- <span data-ttu-id="9daaa-1135">„/sbin“ befindet sich jetzt standardmäßig im Pfad des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1135">/sbin is now in the user's path by default</span></span>
- <span data-ttu-id="9daaa-1136">Der NT-Benutzerpfad wird jetzt standardmäßig an den WSL-Pfad angefügt (Sie können nun also „notepad.exe“ eingeben, ohne dem Linux-Pfad System32 hinzuzufügen).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1136">NT user path now appended to the WSL path by default (i.e. you can now type notepad.exe without adding System32 to the Linux path)</span></span>
- <span data-ttu-id="9daaa-1137">Hinzufügen von Unterstützung für /proc/sys/kernel/cap_last_cap</span><span class="sxs-lookup"><span data-stu-id="9daaa-1137">Added support for /proc/sys/kernel/cap_last_cap</span></span>
- <span data-ttu-id="9daaa-1138">NT-Binärdateien können nun aus WSL gestartet werden, wenn das aktuelle Arbeitsverzeichnis Nicht-ANSI-Zeichen enthält (GH #1254)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1138">NT Binaries can now be launched from WSL when the current working directory contains non-ansi characters (GH #1254)</span></span>
- <span data-ttu-id="9daaa-1139">Ermöglichen des Herunterfahrens für getrennten UNIX-Streamsocket</span><span class="sxs-lookup"><span data-stu-id="9daaa-1139">Allow shutdown on disconnected unix stream socket.</span></span>
- <span data-ttu-id="9daaa-1140">Hinzufügen von Unterstützung für PR_GET_PDEATHSIG.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1140">Added support for PR_GET_PDEATHSIG.</span></span>
- <span data-ttu-id="9daaa-1141">Hinzufügen von Unterstützung für CLONE_PARENT</span><span class="sxs-lookup"><span data-stu-id="9daaa-1141">Added support for CLONE_PARENT</span></span>
- <span data-ttu-id="9daaa-1142">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1142">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="9daaa-1143">Verarbeiten von Anforderungen zum Herstellen einer Verbindung mit dem aktuellen Terminal.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1143">Handle requests to connect to the current terminal.</span></span>
- <span data-ttu-id="9daaa-1144">Markieren von /proc/<pid>/oom_score_adj als beschreibbar.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1144">Mark /proc/<pid>/oom_score_adj as writable.</span></span>
- <span data-ttu-id="9daaa-1145">Hinzufügen des Ordners „/sys/fs/cgroup“.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1145">Add /sys/fs/cgroup folder.</span></span>
- <span data-ttu-id="9daaa-1146">sched_setaffinity sollte den Wert der Affinitätsbitsmaske zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1146">sched_setaffinity should return number of affinity bits mask</span></span>
- <span data-ttu-id="9daaa-1147">Korrektur der ELF-Validierungslogik, die fälschlicherweise annimmt, dass Interpreterpfade weniger als 64 Zeichen lang sein müssen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1147">Fix ELF validation logic which incorrectly assumes interpreter paths must be less than 64 characters long.</span></span> <span data-ttu-id="9daaa-1148">(GH #743)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1148">(GH #743)</span></span>
- <span data-ttu-id="9daaa-1149">Geöffnete Dateideskriptoren können das Konsolenfenster geöffnet lassen (GH #1187)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1149">Open file descriptors can keep console window open (GH #1187)</span></span>
- <span data-ttu-id="9daaa-1150">Korrektur eines Fehlers, bei dem rename() mit einem nachgestellten Schrägstrich für den Zielnamen fehlschlägt (GH #1008)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1150">Fixeed error where rename() failed with trailing slash on target name (GH #1008)</span></span>
- <span data-ttu-id="9daaa-1151">Implementierung der/proc/net/dev-Datei</span><span class="sxs-lookup"><span data-stu-id="9daaa-1151">Implement /proc/net/dev file</span></span>
- <span data-ttu-id="9daaa-1152">Korrektur von Pings mit 0,000 ms aufgrund der Timerauflösung.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1152">Fixed 0.000ms pings due to timer resolution.</span></span>
- <span data-ttu-id="9daaa-1153">Implementierung von /proc/self/environ (GH #730)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1153">Implemented /proc/self/environ (GH #730)</span></span>
- <span data-ttu-id="9daaa-1154">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1154">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1155">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1155">LTP Results:</span></span>
<span data-ttu-id="9daaa-1156">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9daaa-1156">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9daaa-1157">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1157">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1158">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1158">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a><span data-ttu-id="9daaa-1159">Build 14959</span><span class="sxs-lookup"><span data-stu-id="9daaa-1159">Build 14959</span></span>

<span data-ttu-id="9daaa-1160">Allgemeine Windows-Informationen zu Build 14959 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1160">For general Windows information on build 14959 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1161">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1161">Fixed</span></span>

- <span data-ttu-id="9daaa-1162">Verbesserte Pico-Prozessbenachrichtigung für Windows.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1162">Improved Pico Process notification for Windows.</span></span>  <span data-ttu-id="9daaa-1163">Weitere Informationen finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1163">Additional information found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span></span>
- <span data-ttu-id="9daaa-1164">Verbesserte Stabilität mit Windows-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="9daaa-1164">Improved stability with Windows interoperability</span></span>
- <span data-ttu-id="9daaa-1165">Korrektur von Fehler 0x80070057 beim Starten von „bash.exe“, wenn der Enterprise Data Protection (EDP) aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="9daaa-1165">Fixed error 0x80070057 when launching bash.exe when Enterprise Data Protection (EDP) is enabled</span></span>
- <span data-ttu-id="9daaa-1166">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1166">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1167">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1167">LTP Results:</span></span>
<span data-ttu-id="9daaa-1168">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9daaa-1168">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9daaa-1169">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1169">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1170">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1170">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a><span data-ttu-id="9daaa-1171">Build 14955</span><span class="sxs-lookup"><span data-stu-id="9daaa-1171">Build 14955</span></span>

<span data-ttu-id="9daaa-1172">Allgemeine Windows-Informationen zu Build 14955 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1172">For general Windows information on build 14955 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1173">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1173">Fixed</span></span>

 - <span data-ttu-id="9daaa-1174">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1174">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9daaa-1175">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1175">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1176">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1176">LTP Results:</span></span>
<span data-ttu-id="9daaa-1177">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9daaa-1177">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9daaa-1178">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1178">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1179">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1179">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a><span data-ttu-id="9daaa-1180">Build 14951</span><span class="sxs-lookup"><span data-stu-id="9daaa-1180">Build 14951</span></span>

<span data-ttu-id="9daaa-1181">Allgemeine Windows-Informationen zu Build 14951 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1181">For general Windows information on build 14951 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span></span><br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a><span data-ttu-id="9daaa-1182">Neues Feature: Windows-/Ubuntu-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="9daaa-1182">New Feature: Windows / Ubuntu Interoperability</span></span>
<span data-ttu-id="9daaa-1183">Windows-Binärdateien können jetzt direkt über die WSL-Befehlszeile aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1183">Windows binaries can now be invoked directly from the WSL command line.</span></span>  <span data-ttu-id="9daaa-1184">Dadurch haben Benutzer die Möglichkeit, mit Ihrer Windows-Umgebung und dem -System auf eine Weise zu interagieren, die bisher nicht möglich war.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1184">This gives users the ability to interact with their Windows environment and system in a way that has not been possible.</span></span>  <span data-ttu-id="9daaa-1185">Als kurzes Beispiel können Benutzer nun die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1185">As a quick example, it is now possible for users to run the following commands:</span></span>

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

<span data-ttu-id="9daaa-1186">Weitere Informationen finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1186">More information can be found at:</span></span>

- [<span data-ttu-id="9daaa-1187">WSL-Teamblog für Interop</span><span class="sxs-lookup"><span data-stu-id="9daaa-1187">WSL Team Blog for Interop</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [<span data-ttu-id="9daaa-1188">MSDN-Interop-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="9daaa-1188">MSDN Interop Documentation</span></span>](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1189">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1189">Fixed</span></span>

- <span data-ttu-id="9daaa-1190">Ubuntu 16.04 (Xenial) wird jetzt für alle neuen WSL-Instanzen installiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1190">Ubuntu 16.04 (Xenial) is now installed for all new WSL instances.</span></span>  <span data-ttu-id="9daaa-1191">Benutzer mit vorhandenen 14.04-Instanzen (Trusty) erhalten kein automatisches Upgrade.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1191">Users with existing 14.04 (Trusty) instances will not be automatically upgraded.</span></span>
- <span data-ttu-id="9daaa-1192">Das während der Installation festgelegte Gebietsschema wird jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1192">Locale set during install is now displayed</span></span>
- <span data-ttu-id="9daaa-1193">Terminalverbesserungen, einschließlich des Fehlers bei der Umleitung eines WSL-Prozesses an eine Datei, funktionieren nicht immer</span><span class="sxs-lookup"><span data-stu-id="9daaa-1193">Terminal improvements including bug where redirecting a WSL process to a file does not always work</span></span>
- <span data-ttu-id="9daaa-1194">Die Konsolenlebensdauer muss an die Lebensdauer von „bash.exe“ gebunden sein</span><span class="sxs-lookup"><span data-stu-id="9daaa-1194">Console lifetime should be tied to bash.exe lifetime</span></span>
- <span data-ttu-id="9daaa-1195">Die Größe des Konsolenfensters sollte die sichtbare Größe und nicht die Puffergröße verwenden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1195">Console window size should use visible size, not buffer size</span></span>
- <span data-ttu-id="9daaa-1196">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1196">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1197">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1197">LTP Results:</span></span>
<span data-ttu-id="9daaa-1198">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9daaa-1198">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9daaa-1199">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1199">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1200">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1200">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a><span data-ttu-id="9daaa-1201">Build 14946</span><span class="sxs-lookup"><span data-stu-id="9daaa-1201">Build 14946</span></span>

<span data-ttu-id="9daaa-1202">Allgemeine Windows-Informationen zu Build 14946 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1202">For general Windows information on build 14946 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1203">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1203">Fixed</span></span>

- <span data-ttu-id="9daaa-1204">Korrektur eines Problems, das das Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen verhindert hat, die Leerzeichen oder Anführungszeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1204">Fixed an issue that prevented creating WSL user accounts for users with NT usernames that contain spaces or quotes.</span></span> 
- <span data-ttu-id="9daaa-1205">Änderung von VolFs und DrvFs, damit 0 für die Verknüpfungsanzahl des Verzeichnisses im Status zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="9daaa-1205">Change VolFs and DrvFs to return 0 for directory's link count in stat</span></span>
- <span data-ttu-id="9daaa-1206">Unterstützung der IPV6_MULTICAST_HOPS-Socketoption.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1206">Support IPV6_MULTICAST_HOPS socket option.</span></span>
- <span data-ttu-id="9daaa-1207">Einschränkung auf eine einzige Konsolen-E/A-Schleife pro TTY.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1207">Limit to a single console I/O loop per tty.</span></span> <span data-ttu-id="9daaa-1208">Der folgende Befehl ist beispielsweise möglich:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1208">Example: the following command is possible:</span></span>
  - <span data-ttu-id="9daaa-1209">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span><span class="sxs-lookup"><span data-stu-id="9daaa-1209">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span></span>

- <span data-ttu-id="9daaa-1210">Ersetzen von Leerzeichen durch Tabstoppzeichen in /proc/cpuinfo (GH #1115)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1210">replace spaces with tabs in /proc/cpuinfo (GH #1115)</span></span>
- <span data-ttu-id="9daaa-1211">DrvFs wird jetzt in den Einbindungsinformationen mit einem Namen angezeigt, der dem eingebundenen Windows-Volume entspricht</span><span class="sxs-lookup"><span data-stu-id="9daaa-1211">DrvFs now appears in mountinfo with a name that matches mounted Windows volume</span></span>
- <span data-ttu-id="9daaa-1212">/home und/root werden nun in den Einbindungsinformationen mit den richtigen Namen angezeigt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1212">/home and /root now appear in mountinfo with correct names</span></span>
- <span data-ttu-id="9daaa-1213">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1213">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1214">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1214">LTP Results:</span></span>
<span data-ttu-id="9daaa-1215">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9daaa-1215">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9daaa-1216">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1216">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1217">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1217">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a><span data-ttu-id="9daaa-1218">Build 14942</span><span class="sxs-lookup"><span data-stu-id="9daaa-1218">Build 14942</span></span>

<span data-ttu-id="9daaa-1219">Allgemeine Windows-Informationen zu Build 14942 finden Sie im [Windows-Blog](https://aka.ms/onefourninefourtwoooooo).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1219">For general Windows information on build 14942 visit the [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1220">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1220">Fixed</span></span>

- <span data-ttu-id="9daaa-1221">Eine Reihe von Fehlerüberprüfungen, einschließlich des Netzwerkabsturzes durch „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“, der SSH blockiert hat</span><span class="sxs-lookup"><span data-stu-id="9daaa-1221">A number of bugchecks addressed, including the “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY” networking crash which was blocking SSH</span></span>
- <span data-ttu-id="9daaa-1222">inotify-Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1222">inotifiy support for notifications generated from Windows applications on DrvFs is now in</span></span>
- <span data-ttu-id="9daaa-1223">Implementierung von TCP_KEEPIDLE und TCP_KEEPINTVL für mongod.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1223">Implement TCP_KEEPIDLE and TCP_KEEPINTVL for mongod.</span></span> <span data-ttu-id="9daaa-1224">(GH #695)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1224">(GH #695)</span></span>
- <span data-ttu-id="9daaa-1225">Implementierung des pivot_root-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9daaa-1225">Implement the pivot_root system call</span></span>
- <span data-ttu-id="9daaa-1226">Implementierung der Socketoption für SO_DONTROUTE</span><span class="sxs-lookup"><span data-stu-id="9daaa-1226">Implement socket option for SO_DONTROUTE</span></span>
- <span data-ttu-id="9daaa-1227">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1227">Additional bugfixes and improvements</span></span>


### <a name="ltp-results"></a><span data-ttu-id="9daaa-1228">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1228">LTP Results:</span></span>
<span data-ttu-id="9daaa-1229">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9daaa-1229">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9daaa-1230">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9daaa-1230">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9daaa-1231">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1231">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1232">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1232">Syscall Support</span></span>
<span data-ttu-id="9daaa-1233">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1233">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1234">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1234">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a><span data-ttu-id="9daaa-1235">Build 14936</span><span class="sxs-lookup"><span data-stu-id="9daaa-1235">Build 14936</span></span>

<span data-ttu-id="9daaa-1236">Allgemeine Windows-Informationen zu Build 14936 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1236">For general Windows information on build 14936 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span></span><br/>


<span data-ttu-id="9daaa-1237">Hinweis: WSL wird in einem zukünftigen Release Ubuntu Version 16.04 (Xenial) anstelle von Ubuntu 14.04 (Trusty) installieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1237">Note: WSL will install Ubuntu version 16.04 (Xenial) instead of Ubuntu 14.04 (Trusty) in an upcoming release.</span></span>  <span data-ttu-id="9daaa-1238">Diese Änderung gilt für Insider, die neue Instanzen installieren (lxrun.exe /install oder erste Ausführung von „bash.exe“).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1238">This change will apply to Insiders installing new instances (lxrun.exe /install or first run of bash.exe).</span></span>  <span data-ttu-id="9daaa-1239">Vorhandene Instanzen mit Trusty werden nicht automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1239">Existing instances with Trusty will not be upgraded automatically.</span></span> <span data-ttu-id="9daaa-1240">Benutzer können mit dem Befehl „do-release-upgrade“ Ihr Trusty-Image auf Xenial aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1240">Users can upgrade their Trusty image to Xenial using the do-release-upgrade command.</span></span>

### <a name="known-issue"></a><span data-ttu-id="9daaa-1241">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9daaa-1241">Known Issue</span></span>
<span data-ttu-id="9daaa-1242">Bei WSL treten Probleme mit einigen Socketimplementierungen auf.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1242">WSL is experiencing an issue with some socket implementations.</span></span>  <span data-ttu-id="9daaa-1243">Die Fehlerüberprüfung manifestiert sich als Absturz mit dem Fehler „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1243">The bugcheck manifests itself as a crash with the error “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY”.</span></span>  <span data-ttu-id="9daaa-1244">Die häufigste Variante dieses Problems ist ein Absturz bei der Verwendung von SSH.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1244">The most common manifestation of this issue is a crash when using ssh.</span></span>  <span data-ttu-id="9daaa-1245">Die Ursache ist bei internen Builds korrigiert und wird so bald wie möglich in Insider gepusht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1245">The root cause is fixed on internal builds and will be pushed to Insiders at the earliest opportunity.</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-1246">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1246">Fixed</span></span>

- <span data-ttu-id="9daaa-1247">Der chroot-Systemaufruf wurde implementiert.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1247">Implemented the chroot system call</span></span>
- <span data-ttu-id="9daaa-1248">Verbesserungen in inotify ~~einschließlich Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden~~</span><span class="sxs-lookup"><span data-stu-id="9daaa-1248">Improvements in inotify ~~including support for notifications generated from Windows applications on DrvFs~~</span></span>
  - <span data-ttu-id="9daaa-1249">Korrektur: Inotify-Unterstützung von Änderungen, die von Windows-Anwendungen stammen, ist zurzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1249">Correction: Inotify support for changes originating from Windows applications not available at this time.</span></span>
- <span data-ttu-id="9daaa-1250">Die Socketbindung an IPv6::<port n> unterstützt jetzt IPV6_V6ONLY (GH #68, #157, #393, #460, #674, #740, #982, #996)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1250">Socket binding to IPV6::<port n> now supports IPV6_V6ONLY  (GH #68, #157, #393, #460, #674, #740, #982, #996)</span></span>
- <span data-ttu-id="9daaa-1251">Implementierung des WNOWAIT-Verhaltens für den waitid-Systemaufruf (GH #638)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1251">WNOWAIT behavior for waitid systemcall implemented (GH #638)</span></span>
- <span data-ttu-id="9daaa-1252">Unterstützung für IP-Socketoptionen IP_HDRINCL und IP_TTL</span><span class="sxs-lookup"><span data-stu-id="9daaa-1252">Support for IP socket options IP_HDRINCL and IP_TTL</span></span>
- <span data-ttu-id="9daaa-1253">read() der Länge Null sollte sofort zurückgegeben werden (GH #975)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1253">Zero-length read() should return immediately (GH #975)</span></span>
- <span data-ttu-id="9daaa-1254">Ordnungsgemäße Verarbeitung von Dateinamen und Dateinamenpräfixen, die keinen NULL-Terminator in einer TAR-Datei enthalten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1254">Correctly handle filenames and filename prefixes that don't include a NULL terminator in a .tar file.</span></span>
- <span data-ttu-id="9daaa-1255">epoll-Unterstützung für/dev/null</span><span class="sxs-lookup"><span data-stu-id="9daaa-1255">epoll support for /dev/null</span></span>
- <span data-ttu-id="9daaa-1256">Korrektur der /dev/alarm-Zeitquelle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1256">Fix /dev/alarm time source</span></span>
- <span data-ttu-id="9daaa-1257">Bash -c kann nun in eine Datei umgeleitet werden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1257">Bash -c now able to redirect to a file</span></span>
- <span data-ttu-id="9daaa-1258">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1258">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1259">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1259">LTP Results:</span></span>
<span data-ttu-id="9daaa-1260">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9daaa-1260">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9daaa-1261">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 264</span><span class="sxs-lookup"><span data-stu-id="9daaa-1261">Number of non-Passing (failing, skipped, etc…): 264</span></span> </br>
[<span data-ttu-id="9daaa-1262">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1262">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1263">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1263">Syscall Support</span></span>
<span data-ttu-id="9daaa-1264">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1264">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1265">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1265">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`chroot`<br/>
<br/>

## <a name="build-14931"></a><span data-ttu-id="9daaa-1266">Build 14931</span><span class="sxs-lookup"><span data-stu-id="9daaa-1266">Build 14931</span></span>

<span data-ttu-id="9daaa-1267">Allgemeine Windows-Informationen zu Build 14931 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1267">For general Windows information on build 14931 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1268">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1268">Fixed</span></span>

 - <span data-ttu-id="9daaa-1269">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1269">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9daaa-1270">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1270">Regularly scheduled updates will resume in the next release.</span></span>

<br/>

## <a name="build-14926"></a><span data-ttu-id="9daaa-1271">Build 14926</span><span class="sxs-lookup"><span data-stu-id="9daaa-1271">Build 14926</span></span>

<span data-ttu-id="9daaa-1272">Allgemeine Windows-Informationen zu Build 14926 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1272">For general Windows information on build 14926 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1273">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1273">Fixed</span></span>

- <span data-ttu-id="9daaa-1274">Ping funktioniert nun in Konsolen, die nicht über Administratorberechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1274">Ping now works in consoles which do not have administrator privileges</span></span>
- <span data-ttu-id="9daaa-1275">Ping6 wird jetzt auch ohne Administratorberechtigungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1275">Ping6 now supported, also without administrator privileges</span></span>
- <span data-ttu-id="9daaa-1276">Inotify-Unterstützung für Dateien, die über WSL geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1276">Inotify support for files modified through WSL.</span></span> <span data-ttu-id="9daaa-1277">(GH #216)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1277">(GH #216)</span></span>
  - <span data-ttu-id="9daaa-1278">Unterstützte Flags:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1278">Flags supported:</span></span>
    - <span data-ttu-id="9daaa-1279">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span><span class="sxs-lookup"><span data-stu-id="9daaa-1279">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span></span>
    - <span data-ttu-id="9daaa-1280">inotify_add_watchEreignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span><span class="sxs-lookup"><span data-stu-id="9daaa-1280">inotify_add_watch events: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span></span>
    - <span data-ttu-id="9daaa-1281">inotify_add_watch-Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span><span class="sxs-lookup"><span data-stu-id="9daaa-1281">inotify_add_watch attributes: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span></span>
    - <span data-ttu-id="9daaa-1282">Lesen der Ausgabe: LX_IN_ISDIR, LX_IN_IGNORED</span><span class="sxs-lookup"><span data-stu-id="9daaa-1282">read output: LX_IN_ISDIR, LX_IN_IGNORED</span></span>
  - <span data-ttu-id="9daaa-1283">Bekanntes Problem: Durch das Ändern von Dateien aus Windows-Anwendungen werden keine Ereignisse generiert</span><span class="sxs-lookup"><span data-stu-id="9daaa-1283">Known issue: Modifying files from Windows applications does not generate any events</span></span>
- <span data-ttu-id="9daaa-1284">Unix-Socket unterstützt jetzt SCM_CREDENTIALS</span><span class="sxs-lookup"><span data-stu-id="9daaa-1284">Unix socket now supports SCM_CREDENTIALS</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9daaa-1285">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9daaa-1285">LTP Results:</span></span>
<span data-ttu-id="9daaa-1286">Anzahl bestandener Tests: 651</span><span class="sxs-lookup"><span data-stu-id="9daaa-1286">Number of Passing Test: 651</span></span> </br>
<span data-ttu-id="9daaa-1287">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="9daaa-1287">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="9daaa-1288">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9daaa-1288">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a><span data-ttu-id="9daaa-1289">Build 14915</span><span class="sxs-lookup"><span data-stu-id="9daaa-1289">Build 14915</span></span>

<span data-ttu-id="9daaa-1290">Allgemeine Windows-Informationen zu Build 14915 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1290">For general Windows information on build 14915 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1291">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1291">Fixed</span></span>
-  <span data-ttu-id="9daaa-1292">Socketpair für Unix-Datagrammsockets (GH #262)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1292">Socketpair for unix datagram sockets (GH #262)</span></span>
- <span data-ttu-id="9daaa-1293">Unix-Socketunterstützung für SO_REUSEADDR</span><span class="sxs-lookup"><span data-stu-id="9daaa-1293">Unix socket support for SO_REUSEADDR</span></span>
- <span data-ttu-id="9daaa-1294">Unix-Socketunterstützung für SO_BROADCAST (GH #568)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1294">UNIX socket support for SO_BROADCAST (GH #568)</span></span>
- <span data-ttu-id="9daaa-1295">Unix-Socketunterstützung für SOCK_SEQPACKET (GH #758, #546)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1295">Unix socket support for SOCK_SEQPACKET (GH #758, #546)</span></span>
- <span data-ttu-id="9daaa-1296">Hinzufügen von Unterstützung für unix datagram socket send, recv und shutdown</span><span class="sxs-lookup"><span data-stu-id="9daaa-1296">Adding support for unix datagram socket send, recv and shutdown</span></span>
- <span data-ttu-id="9daaa-1297">Korrektur einer Fehlerüberprüfung aufgrund einer ungültigen Überprüfung des mmap-Parameters für nicht feste Adressen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1297">Fix bugcheck due to invalid mmap parameter validation for non-fixed addresses.</span></span> <span data-ttu-id="9daaa-1298">(GH #847)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1298">(GH #847)</span></span>
- <span data-ttu-id="9daaa-1299">Unterstützung für das Anhalten/Fortsetzen von Terminalzuständen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1299">Support for suspend / resume of terminal states</span></span>
- <span data-ttu-id="9daaa-1300">Unterstützung für TIOCPKT ioctl zum Entsperren des Bildschirmhilfsprogramms (GH #774)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1300">Support for TIOCPKT ioctl to unblock the Screen utility (GH #774)</span></span>
    - <span data-ttu-id="9daaa-1301">Bekanntes Problem: Funktionstasten sind nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="9daaa-1301">Known issue: Function keys not operational</span></span>
- <span data-ttu-id="9daaa-1302">Korrektur einer Racebedingung in TimerFd, die dazu führen konnte, dass auf einen freigegebenen Member „ReaderReady“ durch LxpTimerFdWorkerRoutine zugegriffen wurde (GH #814)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1302">Corrected a race in TimerFd that could cause a freed member 'ReaderReady' to be accessed by LxpTimerFdWorkerRoutine (GH #814)</span></span>
- <span data-ttu-id="9daaa-1303">Aktivieren der Unterstützung für erneut startbaren Systemaufruf für futex, poll und clock_nanosleep</span><span class="sxs-lookup"><span data-stu-id="9daaa-1303">Enable restartable system call support for futex, poll, and clock_nanosleep</span></span>
- <span data-ttu-id="9daaa-1304">Hinzufügen von Unterstützung für Bindungseinbindung</span><span class="sxs-lookup"><span data-stu-id="9daaa-1304">Added bind mount support</span></span>
- <span data-ttu-id="9daaa-1305">Unterstützung für Aufheben der Freigabe für Einbindungsnamespace</span><span class="sxs-lookup"><span data-stu-id="9daaa-1305">unshare for mount namespace support</span></span>
    - <span data-ttu-id="9daaa-1306">Bekanntes Problem: Beim Erstellen eines neuen Einbindngsnamespace mit `unshare(CLONE_NEWNS)` zeigt das aktuelle Arbeitsverzeichnis weiterhin auf den alten Namespace</span><span class="sxs-lookup"><span data-stu-id="9daaa-1306">Known issue: When creating a new mount namespace with `unshare(CLONE_NEWNS)` the current working directory will continue to point to the old namespace</span></span>
- <span data-ttu-id="9daaa-1307">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1307">Additional improvements and bug fixes</span></span>

<br/>

## <a name="build-14905"></a><span data-ttu-id="9daaa-1308">Build 14905</span><span class="sxs-lookup"><span data-stu-id="9daaa-1308">Build 14905</span></span>

<span data-ttu-id="9daaa-1309">Allgemeine Windows-Informationen zu Build 14905 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1309">For general Windows information on build 14905 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1310">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1310">Fixed</span></span>
- <span data-ttu-id="9daaa-1311">Erneut startbare Systemaufrufe werden jetzt unterstützt (GH #349, GH #520)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1311">Restartable system calls are now supported (GH #349, GH #520)</span></span>
- <span data-ttu-id="9daaa-1312">Symbolische Verknüpfungen mit Verzeichnissen, die auf / wenden, sind jetzt funktionstüchtig (GH #650)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1312">Symlinks to directories ending in / now operational (GH #650)</span></span>
- <span data-ttu-id="9daaa-1313">Implementierung von RNDGETENTCNT ioctl für „/dev/random“</span><span class="sxs-lookup"><span data-stu-id="9daaa-1313">Implemented RNDGETENTCNT ioctl for /dev/random</span></span>
- <span data-ttu-id="9daaa-1314">Implementierung der /proc/[pid]/mounts, /proc/[pid]/mountinfo- und /proc/[pid]/mountstats-Dateien</span><span class="sxs-lookup"><span data-stu-id="9daaa-1314">Implemented the /proc/[pid]/mounts, /proc/[pid]/mountinfo and /proc/[pid]/mountstats files</span></span>
- <span data-ttu-id="9daaa-1315">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1315">Additional bugfixes and improvements</span></span>

</br>

## <a name="build-14901"></a><span data-ttu-id="9daaa-1316">Build 14901</span><span class="sxs-lookup"><span data-stu-id="9daaa-1316">Build 14901</span></span>
<span data-ttu-id="9daaa-1317">Der erste Insider-Build für das Windows 10 Anniversary Update-Release.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1317">First Insider build for the post Windows 10 Anniversary Update release.</span></span>

<span data-ttu-id="9daaa-1318">Allgemeine Windows-Informationen zu Build 14901 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1318">For general Windows information on build 14901 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1319">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1319">Fixed</span></span>
- <span data-ttu-id="9daaa-1320">Korrektur eines Problems mit nachfolgenden Schrägstrichen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1320">Fixed trailing slash issue</span></span>
    - <span data-ttu-id="9daaa-1321">Befehle wie `$ mv a/c/ a/b/` funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1321">Commands such as `$ mv a/c/ a/b/` now work</span></span>
- <span data-ttu-id="9daaa-1322">Installation von Eingabeaufforderungen, wenn das Ubuntu-Gebietsschema auf das Windows-Gebietsschema festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="9daaa-1322">Installing now prompts if Ubuntu locale should be set to Windows locale</span></span>
- <span data-ttu-id="9daaa-1323">Procfs-Unterstützung für den Ordner „ns“</span><span class="sxs-lookup"><span data-stu-id="9daaa-1323">Procfs support for ns folder</span></span>
- <span data-ttu-id="9daaa-1324">Hinzufügen von „mount“ und „unmount“ für tmpfs-, procfs-und sysfs-Dateisysteme</span><span class="sxs-lookup"><span data-stu-id="9daaa-1324">Added mount and unmount for tmpfs, procfs and sysfs file systems</span></span>
- <span data-ttu-id="9daaa-1325">Korrektur der 32-Bit-ABI-Signatur von mklod [at]</span><span class="sxs-lookup"><span data-stu-id="9daaa-1325">Fix mknod[at] 32-bit ABI signature</span></span>
- <span data-ttu-id="9daaa-1326">Verschieben von Unix-Sockets in Dispatchmodell</span><span class="sxs-lookup"><span data-stu-id="9daaa-1326">Unix sockets moved to dispatch model</span></span>
- <span data-ttu-id="9daaa-1327">Mit setsockopt festgelegte recv-Puffergröße von INET-Socket muss berücksichtigt werden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1327">INET socket recv buffer size set using the setsockopt should be honored</span></span>
- <span data-ttu-id="9daaa-1328">Implementierung des MSG_CMSG_CLOEXEC-Unis-Socket-Empfangsnachrichtenflags</span><span class="sxs-lookup"><span data-stu-id="9daaa-1328">Implement MSG_CMSG_CLOEXEC unix socket receive message flag</span></span>
- <span data-ttu-id="9daaa-1329">stdin/stdout-Pipeumleitung des Linux-Prozesses (GH #2)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1329">Linux process stdin/stdout pipe redirection (GH #2)</span></span>
    - <span data-ttu-id="9daaa-1330">Ermöglicht das Weiterleiten von bash -c-Befehlen in CMD.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1330">Allows for piping of bash -c commands in CMD.</span></span>  <span data-ttu-id="9daaa-1331">Beispiel: >dir | bash -c "grep foo"</span><span class="sxs-lookup"><span data-stu-id="9daaa-1331">Example:  >dir | bash -c "grep foo"</span></span>
- <span data-ttu-id="9daaa-1332">Bash kann nun auf Systemen mit mehreren Auslagerungsdateien installiert werden (GH #538, #358)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1332">Bash can now be installed on systems with multiple pagefiles (GH #538, #358)</span></span>
- <span data-ttu-id="9daaa-1333">Standardpuffergröße des INET-Sockets sollte mit der Größe des Ubuntu- Standardsetups übereinstimmen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1333">Default INET Socket buffer size should match that of default Ubuntu setup</span></span>
- <span data-ttu-id="9daaa-1334">Ausrichten von xattr-Systemaufrufen an listxattr</span><span class="sxs-lookup"><span data-stu-id="9daaa-1334">Align xattr syscalls to listxattr</span></span>
- <span data-ttu-id="9daaa-1335">Nur Rückgabe von Schnittstellen mit einer gültigen IPv4-Adresse von SIOCGIFCONF</span><span class="sxs-lookup"><span data-stu-id="9daaa-1335">Only return interfaces with a valid IPv4 address from SIOCGIFCONF</span></span>
- <span data-ttu-id="9daaa-1336">Korrektur der Signalatandardaktion, wenn von ptrace eingefügt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1336">Fix signal default action when injected by ptrace</span></span>
- <span data-ttu-id="9daaa-1337">Implementierung von /proc/sys/vm/min_free_kbytes</span><span class="sxs-lookup"><span data-stu-id="9daaa-1337">implement /proc/sys/vm/min_free_kbytes</span></span>
- <span data-ttu-id="9daaa-1338">Verwenden der Computerkontext-Registerwerte beim Wiederherstellen von Kontext in sigreturn</span><span class="sxs-lookup"><span data-stu-id="9daaa-1338">Use machine context register values when restoring context in sigreturn</span></span>
    - <span data-ttu-id="9daaa-1339">Dadurch wird das Problem behoben, dass Java und javac bei einigen Benutzern nicht mehr reagiert haben</span><span class="sxs-lookup"><span data-stu-id="9daaa-1339">This resolves the issue where java and javac were hanging for some users</span></span>
- <span data-ttu-id="9daaa-1340">Implementierung von /proc/sys/kernel/hostname</span><span class="sxs-lookup"><span data-stu-id="9daaa-1340">Implement /proc/sys/kernel/hostname</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1341">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1341">Syscall Support</span></span>
<span data-ttu-id="9daaa-1342">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1342">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1343">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1343">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a><span data-ttu-id="9daaa-1344">Update von Build 14388 auf Windows 10 Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="9daaa-1344">Build 14388 to Windows 10 Anniversary Update</span></span>
<span data-ttu-id="9daaa-1345">Allgemeine Windows-Informationen zu Build 14388 finden Sie im [Windows-Blog](https://aka.ms/14388wip).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1345">For general Windows information on build 14388 visit the [Windows Blog](https://aka.ms/14388wip).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1346">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1346">Fixed</span></span>
- <span data-ttu-id="9daaa-1347">Korrekturen als Vorbereitung auf das Windows 10 Anniversary Update am 02.08.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1347">Fixes to prepare for the Windows 10 Anniversary Update on 8/2</span></span>
  - <span data-ttu-id="9daaa-1348">Weitere Informationen zu WSL im Anniversary Update finden Sie in unserem [Blog](https://blogs.msdn.microsoft.com/wsl/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1348">More information about WSL in the Anniversary Update can be found on our [blog](https://blogs.msdn.microsoft.com/wsl/)</span></span>

<br/>

## <a name="build-14376"></a><span data-ttu-id="9daaa-1349">Build 14376</span><span class="sxs-lookup"><span data-stu-id="9daaa-1349">Build 14376</span></span>
<span data-ttu-id="9daaa-1350">Allgemeine Windows-Informationen zu Build 14376 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1350">For general Windows information on build 14376 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1351">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1351">Fixed</span></span>
- <span data-ttu-id="9daaa-1352">Entfernen einiger Instanzen, in denen apt-get nicht mehr reagiert (GH #493)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1352">Removed some instances where apt-get hangs (GH #493)</span></span>
- <span data-ttu-id="9daaa-1353">Korrektur eines Problems, bei dem leere Einbindungen nicht ordnungsgemäß verarbeitet wurden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1353">Fixed an issue where empty mounts were not handled correctly</span></span>
- <span data-ttu-id="9daaa-1354">Korrektur eines Problems, bei dem Ramdisks nicht ordnungsgemäß eingebunden wurden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1354">Fixed an issue where ramdisks were not mounted correctly</span></span>
- <span data-ttu-id="9daaa-1355">Änderung von „unix socket accept“ für die Unterstützung von Flags (Teil von GH #451)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1355">Change unix socket accept to support flags (partial GH #451)</span></span>
- <span data-ttu-id="9daaa-1356">Korrektur eines allgemeinen netzwerkbezogenen Bluescreens</span><span class="sxs-lookup"><span data-stu-id="9daaa-1356">Fixed common network related bluescreen</span></span>
- <span data-ttu-id="9daaa-1357">Korrektur des Bluescreens beim Zugriff auf /proc/[pid]/task (GH #523)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1357">Fixed bluescreen when accessing /proc/[pid]/task (GH #523)</span></span>
- <span data-ttu-id="9daaa-1358">Korrektur hoher CPU-Auslastung für einige Pty-Szenarien (GH #488, #504)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1358">Fixed high CPU utilization for some pty scenarios (GH #488, #504)</span></span>
- <span data-ttu-id="9daaa-1359">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1359">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14371"></a><span data-ttu-id="9daaa-1360">Build 14371</span><span class="sxs-lookup"><span data-stu-id="9daaa-1360">Build 14371</span></span>
<span data-ttu-id="9daaa-1361">Allgemeine Windows-Informationen zu Build 14371 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1361">For general Windows information on build 14371 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1362">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1362">Fixed</span></span>
- <span data-ttu-id="9daaa-1363">Korrektur der Timingracebedingung mit SIGCHLD und wait() bei Verwendung von ptrace</span><span class="sxs-lookup"><span data-stu-id="9daaa-1363">Corrected timing race with SIGCHLD and wait() when using ptrace</span></span>
- <span data-ttu-id="9daaa-1364">Korrektur von Verhalten, wenn Pfade ein nachfolgendes Zeichen / aufweisen (GH #432)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1364">Corrected some behavior when paths have a trailing /  (GH #432)</span></span>
- <span data-ttu-id="9daaa-1365">Korrektur eines Problems, bei dem Umbenennen/Aufheben der Verknüpfung aufgrund von geöffneten Handles für untergeordnete Elemente fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1365">Fixed issue with rename/unlink failing due to open handles to children</span></span>
- <span data-ttu-id="9daaa-1366">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1366">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14366"></a><span data-ttu-id="9daaa-1367">Build 14366</span><span class="sxs-lookup"><span data-stu-id="9daaa-1367">Build 14366</span></span>
<span data-ttu-id="9daaa-1368">Allgemeine Windows-Informationen zu Build 14366 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1368">For general Windows information on build 14366 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1369">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1369">Fixed</span></span>
- <span data-ttu-id="9daaa-1370">Korrektur der Dateierstellung durch symbolische Verknüpfungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1370">Fix in file creation through symlinks</span></span>
-   <span data-ttu-id="9daaa-1371">Hinzugefügter von listxattr für Python (GH 385)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1371">Added listxattr for Python (GH 385)</span></span>
-   <span data-ttu-id="9daaa-1372">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1372">Additional bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1373">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1373">Syscall Support</span></span>
-   <span data-ttu-id="9daaa-1374">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1374">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1375">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1375">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`listxattr`<br/>
<br/>

## <a name="build-14361"></a><span data-ttu-id="9daaa-1376">Build 14361</span><span class="sxs-lookup"><span data-stu-id="9daaa-1376">Build 14361</span></span>
<span data-ttu-id="9daaa-1377">Allgemeine Windows-Informationen zu Build 14361 finden Sie im [Windows-Blog](https://aka.ms/wip14361).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1377">For general Windows information on build 14361 visit the [Windows Blog](https://aka.ms/wip14361).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1378">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1378">Fixed</span></span>
- <span data-ttu-id="9daaa-1379">Für DrvFs wird nun bei der Ausführung in Bash unter Ubuntu unter Windows die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1379">DrvFs is now case sensitive when running in Bash on Ubuntu on Windows.</span></span>
  - <span data-ttu-id="9daaa-1380">Benutzer können case.txt und CASE.TXT auf Ihren /mnt/c-Laufwerken verwenden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1380">Users may case.txt and CASE.TXT on their /mnt/c drives</span></span>
  - <span data-ttu-id="9daaa-1381">Die Beachtung von Groß-/Kleinschreibung wird nur in Bash unter Ubuntu unter Windows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1381">Case sensitivity is only supported within Bash on Ubuntu on Windows.</span></span> <span data-ttu-id="9daaa-1382">Außerhalb von Bash zeigt NTFS die Dateien richtig an, aber es kann zu unerwartetem Verhalten bei der Interaktion mit den Dateien von Windows kommen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1382">When outside of Bash NTFS will report the files correctly, but unexpected behavior may occur interacting with the files from Windows.</span></span>
  - <span data-ttu-id="9daaa-1383">Für den Stamm der einzelnen Volumes (d.h. /mnt/c) wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1383">The root of each volume (i.e. /mnt/c) is not case sensitive</span></span>
  - <span data-ttu-id="9daaa-1384">Weitere Informationen zum Verarbeiten dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1384">More information on handling these files in Windows can be found [here](https://support.microsoft.com/en-us/kb/100625).</span></span>
- <span data-ttu-id="9daaa-1385">Stark verbesserte PTY-/TTY-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1385">Greatly enhanced pty / tty support.</span></span>  <span data-ttu-id="9daaa-1386">Anwendungen wie TMUX werden jetzt unterstützt (GH #40)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1386">Applications like TMUX now supported (GH #40)</span></span>
- <span data-ttu-id="9daaa-1387">Korrektur eines Installationsproblems, bei dem Benutzerkonten nicht immer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1387">Fixed install issue where user accounts not always created</span></span>
- <span data-ttu-id="9daaa-1388">Optimierte Befehlszeilen-Argumentstruktur, die eine extrem lange Argumentliste zulässt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1388">Optimized command line arg structure allowing for extremely long argument list.</span></span> <span data-ttu-id="9daaa-1389">(GH #153)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1389">(GH #153)</span></span>
- <span data-ttu-id="9daaa-1390">Jetzt können chmod read_only-Dateien aus DrvFs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1390">Now able to delete and chmod read_only files from DrvFs</span></span>
- <span data-ttu-id="9daaa-1391">Korrektur einiger Instanzen, bei denen das Terminal beim Trennen nicht mehr reagiert (GH #43)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1391">Fixed some instances where the terminal hangs on disconnect (GH #43)</span></span>
- <span data-ttu-id="9daaa-1392">chmod und chown funktionieren jetzt auf TTY-Geräten</span><span class="sxs-lookup"><span data-stu-id="9daaa-1392">chmod and chown now work on tty devices</span></span>
- <span data-ttu-id="9daaa-1393">Verbindung mit 0.0.0.0 und :: as localhost zulassen (GH #388)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1393">Allow connection to 0.0.0.0 and :: as localhost (GH #388)</span></span>
- <span data-ttu-id="9daaa-1394">Sendmsg/recvmsg verarbeitet nun eine E/A-Vektorlänge > 1 (Teil von GH #376)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1394">Sendmsg/recvmsg now handle an IO vector length of >1 (partial GH #376)</span></span>
- <span data-ttu-id="9daaa-1395">Benutzer können jetzt die automatisch generierte Hostdatei ablehnen (GH #398)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1395">Users can now opt-out of auto-generated hosts file (GH #398)</span></span>
- <span data-ttu-id="9daaa-1396">Automatisches Zuordnen des Linux-Gebietsschemas zum NT-Gebietsschema während der Installation (GH #11)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1396">Automatically match Linux locale to the NT locale during install (GH #11)</span></span>
- <span data-ttu-id="9daaa-1397">Hinzufügen der /proc/sys/vm/swappiness-Datei (GH #306)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1397">Added the /proc/sys/vm/swappiness file (GH #306)</span></span>
- <span data-ttu-id="9daaa-1398">strace wird jetzt ordnungsgemäß beendet</span><span class="sxs-lookup"><span data-stu-id="9daaa-1398">strace now exits correctly</span></span>
- <span data-ttu-id="9daaa-1399">Ermöglichen des erneuten Öffnens von Pipes über /proc/self/fd (GH #222)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1399">Allow pipes to be reopened through /proc/self/fd (GH #222)</span></span>
- <span data-ttu-id="9daaa-1400">Ausblenden von Verzeichnissen unter „%LOCALAPPDATA%\lxss“ aus DrvFs (GH #270)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1400">Hide directories under %LOCALAPPDATA%\lxss from DrvFs (GH #270)</span></span>
- <span data-ttu-id="9daaa-1401">Bessere Verarbeitung von bash.exe ~.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1401">Better handling of bash.exe ~.</span></span>  <span data-ttu-id="9daaa-1402">Befehle wie „bash ~ -c ls“ werden jetzt unterstützt (GH #467)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1402">Commands like “bash ~ -c ls” now supported (GH #467)</span></span>
- <span data-ttu-id="9daaa-1403">Sockets benachrichtigen nun darüber, dass epoll read beim Herunterfahren verfügbar ist (GH #271)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1403">Sockets now notify epoll read available during shutdown (GH #271)</span></span>
- <span data-ttu-id="9daaa-1404">lxrun/uninstall arbeitet besser beim Löschen der Dateien und Ordner.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1404">lxrun /uninstall does a better job of deleting the files and folders</span></span>
- <span data-ttu-id="9daaa-1405">Korrektur für ps-f (GH #246)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1405">Corrected ps -f (GH #246)</span></span>
- <span data-ttu-id="9daaa-1406">Verbesserte Unterstützung für X11-Apps, z.B. xEmacs (GH #481)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1406">Improved support for x11 apps such as xEmacs (GH #481)</span></span>
- <span data-ttu-id="9daaa-1407">Aktualisierte anfängliche Threadstapelgröße, um der standardmäßigen Ubuntu-Einstellung zu entsprechen und die Größe ordnungsgemäß an den get_rlimit-Systemaufruf zu melden (GH #172, #258)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1407">Updated initial thread stack size to match default Ubuntu setting and reporting the size correctly to the get_rlimit syscall (GH #172, #258)</span></span>
- <span data-ttu-id="9daaa-1408">Verbesserte Berichterstellung von Pico-Prozessimagenamen (z.B. für die Überwachung)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1408">Improved reporting of pico process image names (e.g., for auditing)</span></span>
- <span data-ttu-id="9daaa-1409">Implementierung von /proc/mountinfo für df-Befehl</span><span class="sxs-lookup"><span data-stu-id="9daaa-1409">Implemented /proc/mountinfo for df command</span></span>
- <span data-ttu-id="9daaa-1410">Korrektur des Fehlercodes der symbolischen Verknüpfung für den untergeordneten Namen .</span><span class="sxs-lookup"><span data-stu-id="9daaa-1410">Fixed symlink error code for child name .</span></span> <span data-ttu-id="9daaa-1411">und ..</span><span class="sxs-lookup"><span data-stu-id="9daaa-1411">and ..</span></span>
- <span data-ttu-id="9daaa-1412">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1412">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1413">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1413">Syscall Support</span></span>
<span data-ttu-id="9daaa-1414">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1414">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1415">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1415">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a><span data-ttu-id="9daaa-1416">Build 14352</span><span class="sxs-lookup"><span data-stu-id="9daaa-1416">Build 14352</span></span>
<span data-ttu-id="9daaa-1417">Allgemeine Windows-Informationen zu Build 14352 finden Sie im [Windows-Blog](https://aka.ms/wip14352).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1417">For general Windows information on build 14352 visit the [Windows Blog](https://aka.ms/wip14352).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1418">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1418">Fixed</span></span>
- <span data-ttu-id="9daaa-1419">Korrektur eines Problems, bei dem große Dateien nicht ordnungsgemäß heruntergeladen bzw. ordnungsgemäß erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1419">Fixed issue where large files were not downloaded / created correctly.</span></span>  <span data-ttu-id="9daaa-1420">Dadurch sollte die Blockierung von npm und anderen Szenarien aufgehoben werden (GH #3, GH #313)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1420">This should unblock npm and other scenarios (GH #3, GH #313)</span></span>
- <span data-ttu-id="9daaa-1421">Entfernen einiger Instanzen, in denen Sockets nicht mehr reagieren</span><span class="sxs-lookup"><span data-stu-id="9daaa-1421">Removed some instances where sockets hang</span></span>
- <span data-ttu-id="9daaa-1422">Korrektur einiger ptrace-Fehler</span><span class="sxs-lookup"><span data-stu-id="9daaa-1422">Corrected some ptrace errors</span></span>
- <span data-ttu-id="9daaa-1423">Korrektur eines Problems, bei dem WSL Dateinamen mit mehr als 255 Zeichen zuließ</span><span class="sxs-lookup"><span data-stu-id="9daaa-1423">Fixed issue with WSL allowing filenames longer than 255 characters</span></span>
- <span data-ttu-id="9daaa-1424">Verbesserte Unterstützung nicht-englischer Zeichen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1424">Improved support for non-English characters</span></span>
- <span data-ttu-id="9daaa-1425">Hinzufügen aktueller Windows-Zeitzonendaten und Festlegen als Standard</span><span class="sxs-lookup"><span data-stu-id="9daaa-1425">Add current Windows timezone data and set as default</span></span>
- <span data-ttu-id="9daaa-1426">Eindeutige Geräte-IDs für jeden Einbindungspunkt (jre-Korrektur – GH #49)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1426">Unique device id’s for each mount point (jre fix – GH #49)</span></span>
- <span data-ttu-id="9daaa-1427">Korrektur eines Problems mit Pfaden, die „.“</span><span class="sxs-lookup"><span data-stu-id="9daaa-1427">Correct issue with paths containing “.”</span></span> <span data-ttu-id="9daaa-1428">und „..“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1428">and “..”</span></span>
- <span data-ttu-id="9daaa-1429">Hinzufügen von FIFO-Unterstützung (GH #71)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1429">Added Fifo support (GH #71)</span></span>
- <span data-ttu-id="9daaa-1430">Aktualisiertes Format von „resolv.conf“ entsprechend dem nativen Ubuntu-Format</span><span class="sxs-lookup"><span data-stu-id="9daaa-1430">Updated format of resolv.conf to match native Ubuntu format</span></span>
- <span data-ttu-id="9daaa-1431">procfs-Bereinigung</span><span class="sxs-lookup"><span data-stu-id="9daaa-1431">Some procfs cleanup</span></span>
- <span data-ttu-id="9daaa-1432">Aktivierten von Ping für Administratorkonsolen (GH #18)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1432">Enabled ping for Administrator consoles (GH #18)</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1433">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1433">Syscall Support</span></span>
<span data-ttu-id="9daaa-1434">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1434">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1435">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1435">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a><span data-ttu-id="9daaa-1436">Build 14342</span><span class="sxs-lookup"><span data-stu-id="9daaa-1436">Build 14342</span></span>
<span data-ttu-id="9daaa-1437">Allgemeine Windows-Informationen zu Build 14342 finden Sie im [Windows-Blog](https://aka.ms/wip14342).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1437">For general Windows information on build 14342 the [Windows Blog](https://aka.ms/wip14342).</span></span> <br/>

<span data-ttu-id="9daaa-1438">Informationen zu VolFs und DriveFs finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1438">Information on VolFs and DriveFs can be found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9daaa-1439">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1439">Fixed</span></span>
- <span data-ttu-id="9daaa-1440">Korrektur eines Installationsproblems, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen enthielt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1440">Fixed install issue when the Windows user had Unicode characters in the username</span></span>
- <span data-ttu-id="9daaa-1441">Die Problemumgehung „apt-get update udev“ in den FAQ wird jetzt standardmäßig bei der ersten Ausführung bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1441">The apt-get update udev workaround in the FAQ is now provided by default on first run</span></span>
- <span data-ttu-id="9daaa-1442">Aktivierte symbolische Verknüpfungen in DriveFs-Verzeichnissen (/mnt/<drive>)</span><span class="sxs-lookup"><span data-stu-id="9daaa-1442">Enabled symlinks in DriveFs (/mnt/<drive>) directories</span></span>
- <span data-ttu-id="9daaa-1443">Symbolische Verknüpfungen funktionieren nun zwischen DriveFs und VolFs</span><span class="sxs-lookup"><span data-stu-id="9daaa-1443">Symlinks now work between DriveFs and VolFs</span></span>
- <span data-ttu-id="9daaa-1444">Korrektur des Pfadanalyseproblems auf oberster Ebene: ls .// funktioniert jetzt wie erwartet</span><span class="sxs-lookup"><span data-stu-id="9daaa-1444">Addressed top level path parsing issue: ls .// will now work as expected</span></span>
- <span data-ttu-id="9daaa-1445">npm install auf DriveFs und die -g-Optionen funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1445">npm install on DriveFs and the -g options are now working</span></span>
- <span data-ttu-id="9daaa-1446">Korrektur eines Problems, das den Start des PHP-Servers verhinderte</span><span class="sxs-lookup"><span data-stu-id="9daaa-1446">Fixed issue preventing PHP server from launching</span></span>
- <span data-ttu-id="9daaa-1447">Aktualisierte Standardumgebungswerte, z.B. $PATH, um nativem Ubuntu besser zu entsprechen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1447">Updated default environment values, such as $PATH to closer match native Ubuntu</span></span>
- <span data-ttu-id="9daaa-1448">Hinzufügen eines wöchentlichen Wartungstasks in Windows zum Aktualisieren des apt-Paketcaches</span><span class="sxs-lookup"><span data-stu-id="9daaa-1448">Added a weekly maintenance task in Windows to update the apt package cache</span></span>
- <span data-ttu-id="9daaa-1449">Korrektur eines Problems bei der Überprüfung von ELF-Headern, WSL unterstützt jetzt alle Melkor-Optionen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1449">Fixed issue with ELF header validation, WSL now supports all Melkor options</span></span>
- <span data-ttu-id="9daaa-1450">Zsh-Shell ist funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="9daaa-1450">Zsh shell is functional</span></span>
- <span data-ttu-id="9daaa-1451">Vorkompilierte Go-Binärdateien werden jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1451">Precompiled Go binaries are now supported</span></span>
- <span data-ttu-id="9daaa-1452">Eingabeaufforderung bei der ersten Ausführung von „bash.exe“ ist nun richtig lokalisiert</span><span class="sxs-lookup"><span data-stu-id="9daaa-1452">Prompting on Bash.exe first run is now localized correctly</span></span>
- <span data-ttu-id="9daaa-1453">/proc/meminfo gibt jetzt richtige Informationen zurück</span><span class="sxs-lookup"><span data-stu-id="9daaa-1453">/proc/meminfo now returns correct information</span></span>
- <span data-ttu-id="9daaa-1454">Sockets werden jetzt in VFS unterstützt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1454">Sockets now supported in VFS</span></span>
- <span data-ttu-id="9daaa-1455">/dev jetzt als tempfs eingebunden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1455">/dev now mounted as tempfs</span></span>
- <span data-ttu-id="9daaa-1456">Fifo wird jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1456">Fifo now supported</span></span>
- <span data-ttu-id="9daaa-1457">Mehrkernsysteme werden nun ordnungsgemäß in /proc/cpuinfo angezeigt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1457">Multi-core systems now showing correctly in /proc/cpuinfo</span></span>
- <span data-ttu-id="9daaa-1458">Weitere Verbesserungen und Fehlermeldungen, die während der ersten Ausführung heruntergeladen werden</span><span class="sxs-lookup"><span data-stu-id="9daaa-1458">Additional improvements and error messages downloading during first run</span></span>
- <span data-ttu-id="9daaa-1459">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1459">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="9daaa-1460">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1460">Supported syscall list below.</span></span>
- <span data-ttu-id="9daaa-1461">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1461">Additional bugfixes and improvements</span></span>

### <a name="known-issues"></a><span data-ttu-id="9daaa-1462">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="9daaa-1462">Known Issues</span></span>
- <span data-ttu-id="9daaa-1463">„.“ wird in einigen Fällen nicht</span><span class="sxs-lookup"><span data-stu-id="9daaa-1463">Not resolving ‘..’</span></span> <span data-ttu-id="9daaa-1464">ordnungsgemäß auf DriveFs aufgelöst</span><span class="sxs-lookup"><span data-stu-id="9daaa-1464">correctly on DriveFs in some cases</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1465">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1465">Syscall Support</span></span>
<span data-ttu-id="9daaa-1466">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1466">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1467">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1467">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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

## <a name="build-14332"></a><span data-ttu-id="9daaa-1468">Build 14332</span><span class="sxs-lookup"><span data-stu-id="9daaa-1468">Build 14332</span></span>

<span data-ttu-id="9daaa-1469">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14332).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1469">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14332).</span></span> <br/>


### <a name="fixed"></a><span data-ttu-id="9daaa-1470">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1470">Fixed</span></span>
- <span data-ttu-id="9daaa-1471">Bessere resolv.conf-Generierung einschließlich Priorisieren von DNS-Einträgen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1471">Better resolv.conf generation including prioritizing DNS entries</span></span>
- <span data-ttu-id="9daaa-1472">Problem beim Verschieben von Dateien und Verzeichnissen zwischen/mnt- und Nicht-/mnt-Laufwerken</span><span class="sxs-lookup"><span data-stu-id="9daaa-1472">Issue with moving files and directories between /mnt and non-/mnt drives</span></span>
- <span data-ttu-id="9daaa-1473">TAR-Dateien können jetzt mit symbolischen Verknüpfungen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1473">Tar files can now be created with symlinks</span></span>
- <span data-ttu-id="9daaa-1474">Hinzufügen des /run/lock-Standardverzeichnisses bei der Instanzerstellung</span><span class="sxs-lookup"><span data-stu-id="9daaa-1474">Added default /run/lock directory on instance creation</span></span>
- <span data-ttu-id="9daaa-1475">Aktualisieren von /dev/null, um die richtigen Statusinformationen zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="9daaa-1475">Update /dev/null to return proper stat info</span></span>
- <span data-ttu-id="9daaa-1476">Weitere Fehler beim Herunterladen während der ersten Ausführung</span><span class="sxs-lookup"><span data-stu-id="9daaa-1476">Additional errors when downloading during first run</span></span>
- <span data-ttu-id="9daaa-1477">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1477">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="9daaa-1478">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1478">Supported syscall list below.</span></span>
- <span data-ttu-id="9daaa-1479">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1479">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1480">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1480">Syscall Support</span></span>
<span data-ttu-id="9daaa-1481">Im folgenden finden Sie den neuen Systemaufruf, der in WSL implementiert ist.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1481">Below is the new syscall that has some implementation in WSL.</span></span> <span data-ttu-id="9daaa-1482">Der Systemaufruf in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1482">The syscall on this list is supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a><span data-ttu-id="9daaa-1483">Build 14328</span><span class="sxs-lookup"><span data-stu-id="9daaa-1483">Build 14328</span></span>

<span data-ttu-id="9daaa-1484">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14328).</span><span class="sxs-lookup"><span data-stu-id="9daaa-1484">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14328).</span></span> <br/>


### <a name="new-features"></a><span data-ttu-id="9daaa-1485">Neue Funktionen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1485">New Features</span></span>
* <span data-ttu-id="9daaa-1486">Jetzt werden Linux-Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1486">Now support Linux users.</span></span>  <span data-ttu-id="9daaa-1487">Bei der Installation von Bash unter Ubuntu unter Windows werden Sie aufgefordert, einen Linux-Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1487">Installing Bash on Ubuntu on Windows will prompt for creation of a Linux user.</span></span>  <span data-ttu-id="9daaa-1488">Weitere Informationen finden Sie unter https://aka.ms/wslusers.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1488">For more information, visit https://aka.ms/wslusers</span></span>
* <span data-ttu-id="9daaa-1489">Der Hostname ist jetzt auf den Windows-Computernamen festgelegt, nicht mehr auf @localhost</span><span class="sxs-lookup"><span data-stu-id="9daaa-1489">Hostname is now set to the Windows computer name, no more @localhost</span></span>
* <span data-ttu-id="9daaa-1490">Weitere Informationen zu Build 14328 finden Sie unter: https://aka.ms/wip14328</span><span class="sxs-lookup"><span data-stu-id="9daaa-1490">For more information on build 14328, visit: https://aka.ms/wip14328</span></span>

### <a name="fixed"></a><span data-ttu-id="9daaa-1491">Fest</span><span class="sxs-lookup"><span data-stu-id="9daaa-1491">Fixed</span></span>
* <span data-ttu-id="9daaa-1492">Verbesserungen von symbolischen Verknüpfungen für Nicht-/mnt/<drive>-Dateien</span><span class="sxs-lookup"><span data-stu-id="9daaa-1492">Symlink improvements for non /mnt/<drive> files</span></span>
    * <span data-ttu-id="9daaa-1493">Die npm-Installation funktioniert jetzt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1493">npm install now works</span></span>
    * <span data-ttu-id="9daaa-1494">jdk/jre kann nun mithilfe der Anweisungen installiert werden, die Sie [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html) finden.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1494">jdk / jre now installable using instructions found [here](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span></span>
    * <span data-ttu-id="9daaa-1495">Bekanntes Problem: Symbolische Verknüpfungen funktionieren für Windows-Einbindungen nicht.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1495">known issue: symlinks do not work for Windows mounts.</span></span>  <span data-ttu-id="9daaa-1496">Diese Funktionen werden in einem späteren Build verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1496">Functionality will be available in a later build</span></span>
* <span data-ttu-id="9daaa-1497">top und htop werden jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="9daaa-1497">top and htop now display</span></span>
* <span data-ttu-id="9daaa-1498">Zusätzliche Fehlermeldungen bei einigen Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="9daaa-1498">Additional error messages for some install failures</span></span>
* <span data-ttu-id="9daaa-1499">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1499">Syscall improvements and bugfixes.</span></span>  <span data-ttu-id="9daaa-1500">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1500">Supported syscall list below.</span></span>
* <span data-ttu-id="9daaa-1501">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1501">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9daaa-1502">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9daaa-1502">Syscall Support</span></span>
<span data-ttu-id="9daaa-1503">Im folgenden finden Sie eine Liste der Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1503">Below is a list of syscalls that have some implementation in WSL.</span></span>  <span data-ttu-id="9daaa-1504">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9daaa-1504">Syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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
