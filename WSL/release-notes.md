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
ms.openlocfilehash: 31bf975afb202a6cfd9a2879cff29a77b2969fce
ms.sourcegitcommit: 7069b8d452308c32cc7fa31d1158fcb130d42e06
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2020
ms.locfileid: "76911704"
---
# <a name="release-notes-for-windows-subsystem-for-linux"></a><span data-ttu-id="9e6f0-105">Anmerkungen zu dieser Version des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="9e6f0-105">Release Notes for Windows Subsystem for Linux</span></span>

## <a name="build-19555"></a><span data-ttu-id="9e6f0-106">Build 19555</span><span class="sxs-lookup"><span data-stu-id="9e6f0-106">Build 19555</span></span>
<span data-ttu-id="9e6f0-107">Allgemeine Windows-Informationen zu Build 19555 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2020/01/30/announcing-windows-10-insider-preview-build-19555/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-107">For general Windows information on build 19555 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2020/01/30/announcing-windows-10-insider-preview-build-19555/).</span></span>

* <span data-ttu-id="9e6f0-108">[WSL2] Verwenden einer Arbeitsspeicher-cgroup, um den von Installations- und Konvertierungsvorgängen verwendeten Speicherplatz zu begrenzen [GH 4669]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-108">[WSL2] Use a memory cgroup to limit the amount of memory used by install and conversion operations [GH 4669]</span></span>
* <span data-ttu-id="9e6f0-109">Verfügbarmachen von „wsl.exe“, wenn die optionale Komponente „Windows-Subsystem für Linux“ (WSL) nicht aktiviert ist, um die Auffindbarkeit von Features zu verbessern.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-109">Make wsl.exe present when the Windows Subsystem for Linux optional component is not enabled to improve feature discoverability.</span></span>
* <span data-ttu-id="9e6f0-110">Ändern von „wsl.exe“, um Hilfetext auszugeben, wenn die optionale Komponente WSL nicht installiert ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-110">Change wsl.exe to print help text if the WSL optional component is not installed</span></span>
* <span data-ttu-id="9e6f0-111">Fehlerbehebung für die Racebedingung beim Erstellen von Instanzen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-111">Fix race condition when creating instances</span></span>
* <span data-ttu-id="9e6f0-112">Erstellen von „wslclient.dll“ mit allen Befehlszeilenfunktionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-112">Create wslclient.dll that contains all command line functionality</span></span>
* <span data-ttu-id="9e6f0-113">Verhindern eines Absturzes bei angehaltenem LxssManagerUser-Dienst</span><span class="sxs-lookup"><span data-stu-id="9e6f0-113">Prevent crash during LxssManagerUser service stop</span></span>
* <span data-ttu-id="9e6f0-114">Fehlerbehebung für ein wslapi.dll-Fast-Fail, wenn der distroName-Parameter NULL ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-114">Fix wslapi.dll fast fail when distroName parameter is NULL</span></span>

## <a name="build-19041"></a><span data-ttu-id="9e6f0-115">Build 19041</span><span class="sxs-lookup"><span data-stu-id="9e6f0-115">Build 19041</span></span>
<span data-ttu-id="9e6f0-116">Allgemeine Windows-Informationen zu Build 19041 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/12/10/announcing-windows-10-insider-preview-build-19041/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-116">For general Windows information on build 19041 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/12/10/announcing-windows-10-insider-preview-build-19041/).</span></span>

* <span data-ttu-id="9e6f0-117">[WSL2] Löschen der Signalmaske vor dem Starten der Prozesse</span><span class="sxs-lookup"><span data-stu-id="9e6f0-117">[WSL2] Clear the signal mask before launching the processes</span></span>
* <span data-ttu-id="9e6f0-118">[WSL2] Aktualisieren des Linux-Kernels auf 4.19.84</span><span class="sxs-lookup"><span data-stu-id="9e6f0-118">[WSL2] Update Linux kernel to 4.19.84</span></span>
* <span data-ttu-id="9e6f0-119">Verarbeiten der Erstellung der symbolischen Verknüpfung „/etc/resolv.conf“, wenn die symbolische Verknüpfung nicht relativ ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-119">Handle creation of /etc/resolv.conf symlink when the symlink is non-relative</span></span>

## <a name="build-19028"></a><span data-ttu-id="9e6f0-120">Build 19028</span><span class="sxs-lookup"><span data-stu-id="9e6f0-120">Build 19028</span></span>
<span data-ttu-id="9e6f0-121">Allgemeine Windows-Informationen zu Build 19028 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/11/19/announcing-windows-10-insider-preview-build-19028/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-121">For general Windows information on build 19028 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/11/19/announcing-windows-10-insider-preview-build-19028/).</span></span>

* <span data-ttu-id="9e6f0-122">[WSL2] Aktualisieren des Linux-Kernels auf 4.19.81</span><span class="sxs-lookup"><span data-stu-id="9e6f0-122">[WSL2] Update Linux kernel to 4.19.81</span></span>
* <span data-ttu-id="9e6f0-123">[WSL2] Ändern der Standardberechtigung von /dev/net/tun in 0666 [GH 4629]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-123">[WSL2] Change the default permission of /dev/net/tun to 0666 [GH 4629]</span></span>
* <span data-ttu-id="9e6f0-124">[WSL2] Optimieren der Standard-Arbeitsspeichergröße, die dem virtuellen Linux-Computer zugewiesen ist, auf 80% des Hostarbeitsspeichers</span><span class="sxs-lookup"><span data-stu-id="9e6f0-124">[WSL2] Tweak default amount of memory assigned to Linux VM to be 80% of host memory</span></span>
* <span data-ttu-id="9e6f0-125">[WSL2] Fehlerbehebung für den Interop-Server, um Anforderungen mit einem Timeout zu verarbeiten, damit sich der Server bei ungültigen Aufrufern nicht aufhängt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-125">[WSL2] fix interop server to handle requests with a timeout so bad callers cannot hang the server</span></span>

## <a name="build-19018"></a><span data-ttu-id="9e6f0-126">Build 19018</span><span class="sxs-lookup"><span data-stu-id="9e6f0-126">Build 19018</span></span>
<span data-ttu-id="9e6f0-127">Allgemeine Windows-Informationen zu Build 19018 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/11/05/announcing-windows-10-insider-preview-build-19018/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-127">For general Windows information on build 19018 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/11/05/announcing-windows-10-insider-preview-build-19018/).</span></span>

* <span data-ttu-id="9e6f0-128">[WSL2] Verwenden Sie cache=mmap als Standardeinstellung für 9p-Einbindungen, um Probleme mit Dotnet-Apps zu beheben</span><span class="sxs-lookup"><span data-stu-id="9e6f0-128">[WSL2] Use cache=mmap as the default for 9p mounts to fix dotnet apps</span></span>
* <span data-ttu-id="9e6f0-129">[WSL2] Korrekturen für localhost-Relay [GH 4340]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-129">[WSL2] Fixes for localhost relay [GH 4340]</span></span>
* <span data-ttu-id="9e6f0-130">[WSL2] Einführen einer distributionsübergreifenden, gemeinsam genutzten tmpfs-Einbindung für den Freigabezustand zwischen Distributionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-130">[WSL2] Introduce a cross-distro shared tmpfs mount for sharing state between distros</span></span>
* <span data-ttu-id="9e6f0-131">Korrektur der Wiederherstellung des permanenten Netzwerklaufwerks für \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="9e6f0-131">Fix restoring persistent network drive for \\\\wsl$</span></span>

## <a name="build-19013"></a><span data-ttu-id="9e6f0-132">Build 19013</span><span class="sxs-lookup"><span data-stu-id="9e6f0-132">Build 19013</span></span>
<span data-ttu-id="9e6f0-133">Allgemeine Windows-Informationen zu Build 19013 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/10/29/announcing-windows-10-insider-preview-build-19013/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-133">For general Windows information on build 19013 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/10/29/announcing-windows-10-insider-preview-build-19013/).</span></span>

* <span data-ttu-id="9e6f0-134">[WSL2] Verbesserte Arbeitsspeicherleistung der VM des WSL-Hilfsprogramms</span><span class="sxs-lookup"><span data-stu-id="9e6f0-134">[WSL2] Improve memory performance of WSL utility VM.</span></span> <span data-ttu-id="9e6f0-135">Arbeitsspeicher, der nicht mehr verwendet wird, wird an den Host zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-135">Memory that is no longer in use will be freed back to the host.</span></span>
* <span data-ttu-id="9e6f0-136">[WSL2] Aktualisieren der Kernelversion auf 4.19.79</span><span class="sxs-lookup"><span data-stu-id="9e6f0-136">[WSL2] Update kernel version to 4.19.79.</span></span> <span data-ttu-id="9e6f0-137">(CONFIG_HIGH_RES_TIMERS, CONFIG_TASK_XACCT, CONFIG_TASK_IO_ACCOUNTING, CONFIG_SCHED_HRTICK und CONFIG_BRIDGE_VLAN_FILTERING hinzugefügt).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-137">(add CONFIG_HIGH_RES_TIMERS, CONFIG_TASK_XACCT, CONFIG_TASK_IO_ACCOUNTING, CONFIG_SCHED_HRTICK, and CONFIG_BRIDGE_VLAN_FILTERING).</span></span>
* <span data-ttu-id="9e6f0-138">[WSL2] Korrigiertes Eingaberelay zur Behandlung von Fällen, in denen stdin ein nicht geschlossenes Pipehandle ist [GH 4424]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-138">[WSL2] Fix input relay to handle cases where stdin is a pipe handle that is not closed [GH 4424]</span></span>
* <span data-ttu-id="9e6f0-139">Die Überprüfung auf \\\\wsl$ unterscheidet nicht mehr zwischen Groß- und Kleinschreibung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-139">Make the check for \\\\wsl$ case-insensitive.</span></span>
```
[wsl2]
pageReporting = <bool>    # Enable or disable the free memory page reporting feature (default true).
idleThreshold = <integer> # Set the idle threshold for memory compaction, 0 disables the feature (default 1).
```

## <a name="build-19002"></a><span data-ttu-id="9e6f0-140">Build 19002</span><span class="sxs-lookup"><span data-stu-id="9e6f0-140">Build 19002</span></span>
<span data-ttu-id="9e6f0-141">Allgemeine Windows-Informationen zu Build 19002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/10/17/announcing-windows-10-insider-preview-build-19002/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-141">For general Windows information on build 19002 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/10/17/announcing-windows-10-insider-preview-build-19002/).</span></span>

* <span data-ttu-id="9e6f0-142">[WSL] Beheben von Problemen bei der Behandlung einiger Unicode-Zeichen: https://github.com/microsoft/terminal/issues/2770</span><span class="sxs-lookup"><span data-stu-id="9e6f0-142">[WSL] Fix issue with handling of some Unicode characters: https://github.com/microsoft/terminal/issues/2770</span></span>
* <span data-ttu-id="9e6f0-143">[WSL] Korrektur seltener Fälle, in denen die Registrierung von Distributionen aufgehoben werden kann, wenn sie unmittelbar nach einem Build-zu-Build-Upgrade gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-143">[WSL] Fix rare cases where distros could be unregistered if launched immediately after a build-to-build upgrade.</span></span>
* <span data-ttu-id="9e6f0-144">[WSL] Korrektur eines kleinen Problems beim Herunterfahren mit „wsl.exe“, bei dem Leerlaufzeitgeber von Instanzen nicht abgebrochen wurden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-144">[WSL] Fix minor issue with wsl.exe --shutdown where instance idle timers were not cancelled.</span></span>

## <a name="build-18995"></a><span data-ttu-id="9e6f0-145">Build 18995</span><span class="sxs-lookup"><span data-stu-id="9e6f0-145">Build 18995</span></span>
<span data-ttu-id="9e6f0-146">Allgemeine Windows-Informationen zu Build 18995 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/10/03/announcing-windows-10-insider-preview-build-18995/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-146">For general Windows information on build 18995 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/10/03/announcing-windows-10-insider-preview-build-18995/).</span></span>

* <span data-ttu-id="9e6f0-147">[WSL2] Korrektur eines Problems, bei dem DrvFs-Einbindungen nach dem Abbruch eines Vorgangs (z.B. STRG-C) zu funktionieren aufhörten [GH 4377]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-147">[WSL2] Fix an issue where DrvFs mounts stopped working after an operation was interrupted (e.g. ctrl-c) [GH 4377]</span></span>
* <span data-ttu-id="9e6f0-148">[WSL2] Korrektur der Verarbeitung sehr großer hvsocket-Nachrichten [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-148">[WSL2] Fix handling of very large hvsocket messages [GH 4105]</span></span>
* <span data-ttu-id="9e6f0-149">[WSL2] Korrektur eines Interop-Problems, wenn stdin eine Datei ist [GH 4475]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-149">[WSL2] Fix issue with interop when stdin is a file [GH 4475]</span></span>
* <span data-ttu-id="9e6f0-150">[WSL2] Korrektur eines Absturzes, wenn ein unerwarteter Netzwerkstatus festgestellt wird [GH 4474]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-150">[WSL2] Fix service crash when unexpected network state is encountered [GH 4474]</span></span>
* <span data-ttu-id="9e6f0-151">[WSL2] Abfragen des Namens der Distribution beim Interopserver, wenn der aktuelle Prozess nicht über die Umgebungsvariable verfügt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-151">[WSL2] Query the distro name from the interop server if the current process does not have the environment variable</span></span>
* <span data-ttu-id="9e6f0-152">[WSL2] Korrektur eines Interop-Problems, wenn stdin eine Datei ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-152">[WSL2] Fix issue with interop whe stdin is a file</span></span>
* <span data-ttu-id="9e6f0-153">[WSL2] Aktualisieren der Linux-Kernelversion auf 4.19.72</span><span class="sxs-lookup"><span data-stu-id="9e6f0-153">[WSL2] Update Linux kernel version to 4.19.72</span></span>
* <span data-ttu-id="9e6f0-154">[WSL2] Neu hinzugefügte Möglichkeit zum Angeben weiterer Kernelbefehle in der Befehlszeile mithilfe von WSLCONFIG</span><span class="sxs-lookup"><span data-stu-id="9e6f0-154">[WSL2] Add ability to specify additional kernel command line parameters via .wslconfig</span></span>
```
[wsl2]
kernelCommandLine = <string> # Additional kernel command line arguments
```

## <a name="build-18990"></a><span data-ttu-id="9e6f0-155">Build 18990</span><span class="sxs-lookup"><span data-stu-id="9e6f0-155">Build 18990</span></span>
<span data-ttu-id="9e6f0-156">Allgemeine Windows-Informationen zu Build 18990 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-156">For general Windows information on build 18990 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/24/announcing-windows-10-insider-preview-build-18990/).</span></span>

* <span data-ttu-id="9e6f0-157">Verbesserte Leistung für Verzeichnisauflistungen in \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="9e6f0-157">Improve the performance for directory listings in \\\\wsl$</span></span>
* <span data-ttu-id="9e6f0-158">[WSL2] Einführen zusätzlicher Entropie beim Systemstart [GH 4416]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-158">[WSL2] Inject additional boot entropy [GH 4416]</span></span>
* <span data-ttu-id="9e6f0-159">[WSL2] Problembehebung für Windows-Interop bei der Verwendung von „su“ / „sudo“ [GH 4465]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-159">[WSL2] Fix for Windows interop when using su / sudo [GH 4465]</span></span>

## <a name="build-18980"></a><span data-ttu-id="9e6f0-160">Build 18980</span><span class="sxs-lookup"><span data-stu-id="9e6f0-160">Build 18980</span></span>
<span data-ttu-id="9e6f0-161">Allgemeine Windows-Informationen zu Build 18980 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-161">For general Windows information on build 18980 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/11/announcing-windows-10-insider-preview-build-18980/).</span></span>

* <span data-ttu-id="9e6f0-162">Korrektur des Lesen von symbolischen Verknüpfungen, die FILE_READ_DATA verweigern.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-162">Fix reading symlinks that deny FILE_READ_DATA.</span></span> <span data-ttu-id="9e6f0-163">Dies umfasst alle symbolischen Verknüpfungen, die von Windows aus Gründen der Abwärtskompatibilität erstellt werden, z.B. „C:\Dokumente und Einstellungen“ und eine Reihe von symbolischen Verknüpfungen im Benutzerprofilverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-163">This includes all the symlinks Windows creates for backwards compatibility such as "C:\Document and Settings" and a bunch of symlinks in the user profile directory</span></span>
* <span data-ttu-id="9e6f0-164">Festlegen eines unerwarteten Dateisystemzustands als nicht schwerwiegend [GH 4334, 4305]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-164">Make unexpected filesystem state non-fatal [GH 4334, 4305]</span></span>
* <span data-ttu-id="9e6f0-165">[WSL2] Hinzufügen von Unterstützung für arm64, wenn Ihre CPU/Firmware Virtualisierung unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-165">[WSL2] Add support for arm64 if your CPU / firmware supports virtualization</span></span>
* <span data-ttu-id="9e6f0-166">[WSL2] Zulassen der Anzeige von Kernelprotokollen durch nicht berechtigte Benutzer</span><span class="sxs-lookup"><span data-stu-id="9e6f0-166">[WSL2] Allow unprivileged users to view kernel log</span></span>
* <span data-ttu-id="9e6f0-167">[WSL2] Korrigieren des Ausgaberelays, wenn stdout/stderr-Sockets geschlossen wurden [GH 4375]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-167">[WSL2] Fix output relay when stdout / stderr sockets have been closed [GH 4375]</span></span>
* <span data-ttu-id="9e6f0-168">[WSL2] Unterstützung von Akku- und AC-Adapter-Passthrough</span><span class="sxs-lookup"><span data-stu-id="9e6f0-168">[WSL2] Support battery and AC adapter passthrough</span></span>
* <span data-ttu-id="9e6f0-169">[WSL2] Aktualisieren des Linux-Kernels auf 4.19.67</span><span class="sxs-lookup"><span data-stu-id="9e6f0-169">[WSL2] Update Linux kernel to 4.19.67</span></span>
* <span data-ttu-id="9e6f0-170">Hinzufügen der Möglichkeit, den Standardbenutzernamen in „/etc/wsl.conf“ festzulegen:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-170">Add the ability to set default username in /etc/wsl.conf:</span></span>
```
[user]
default=<string>
```

## <a name="build-18975"></a><span data-ttu-id="9e6f0-171">Build 18975</span><span class="sxs-lookup"><span data-stu-id="9e6f0-171">Build 18975</span></span>
<span data-ttu-id="9e6f0-172">Allgemeine Windows-Informationen zu Build 18975 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-172">For general Windows information on build 18975 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/09/06/announcing-windows-10-insider-preview-build-18975/).</span></span>

* <span data-ttu-id="9e6f0-173">[WSL2] Korrektur einer Reihe von Problemen mit der localhost-Zuverlässigkeit [GH 4340]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-173">[WSL2] Fixed a number of localhost reliability issues [GH 4340]</span></span>

## <a name="build-18970"></a><span data-ttu-id="9e6f0-174">Build 18970</span><span class="sxs-lookup"><span data-stu-id="9e6f0-174">Build 18970</span></span>
<span data-ttu-id="9e6f0-175">Allgemeine Windows-Informationen zu Build 18970 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-175">For general Windows information on build 18970 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/08/29/announcing-windows-10-insider-preview-build-18970/).</span></span>

* <span data-ttu-id="9e6f0-176">[WSL2] Synchronisierung der Uhrzeit mit der Hostzeit, wenn das System nach dem Ruhezustand fortgesetzt wird [GH 4245]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-176">[WSL2] Sync time with host time when system resumes from sleep state [GH 4245]</span></span>
* <span data-ttu-id="9e6f0-177">[WSL2] Nach Möglichkeit Erstellen symbolischer NT-Verknüpfungen auf den Windows-Volumes</span><span class="sxs-lookup"><span data-stu-id="9e6f0-177">[WSL2] Create NT symlinks on the Windows volumes when possible.</span></span>
* <span data-ttu-id="9e6f0-178">[WSL2] Erstellen von Distributionen in den UTS-, IPC-, PID- und Mount-Namespaces.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-178">[WSL2] Create distros in UTS, IPC, PID, and Mount namespaces.</span></span>
* <span data-ttu-id="9e6f0-179">[WSL2] Korrigieren des localhost-Portrelays, wenn der Server direkt an localhost gebunden wird [GH 4353]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-179">[WSL2] Fix localhost port relay when server binds to localhost directly [GH 4353]</span></span>
* <span data-ttu-id="9e6f0-180">[WSL2] Korrigieren von Interop, wenn die Ausgabe umgeleitet wird [GH 4337]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-180">[WSL2] Fix interop when output is redirected [GH 4337]</span></span>
* <span data-ttu-id="9e6f0-181">[WSL2] Unterstützung der Übersetzung absoluter symbolischer NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-181">[WSL2] Support translating absolute NT symlinks.</span></span>
* <span data-ttu-id="9e6f0-182">[WSL2] Aktualisieren des Kernels auf 4.19.59</span><span class="sxs-lookup"><span data-stu-id="9e6f0-182">[WSL2] Update kernel to 4.19.59</span></span>
* <span data-ttu-id="9e6f0-183">[WSL2] Ordnungsgemäße Festlegung der Subnetzmaske für eth0.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-183">[WSL2] Properly set subnet mask for eth0.</span></span>
* <span data-ttu-id="9e6f0-184">[WSL2] Ändern der Logik, um die Konsolenworkerschleife zu verlassen, wenn das Beendigungsereignis signalisiert wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-184">[WSL2] Change logic to break out of console worker loop when exit event is signaled.</span></span>
* <span data-ttu-id="9e6f0-185">[WSL2] Auswerfen der Distributions-VHD, wenn die Distribution nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-185">[WSL2] Eject distribution vhd when the distro is not running.</span></span>
* <span data-ttu-id="9e6f0-186">[WSL2] Korrigieren der Analysebibliothek, um leere Werte ordnungsgemäß zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-186">[WSL2] Fix config parsing library to correctly handle empty values.</span></span>
* <span data-ttu-id="9e6f0-187">[WSL2] Unterstützung von Docker Desktop durch Erstellen von distributionsübergreifenden Einbindungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-187">[WSL2] Support Docker Desktop by creating cross distro mounts.</span></span> <span data-ttu-id="9e6f0-188">Dieses Verhalten kann durch eine Distribution übernommen werden, indem die folgende Zeile der Datei „/etc/wsl.conf“ hinzugefügt wird:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-188">A distro can opt-in to this behavior by adding the following line to the /etc/wsl.conf file:</span></span>
```
[automount]
crossDistro = true
```

## <a name="build-18945"></a><span data-ttu-id="9e6f0-189">Build 18945</span><span class="sxs-lookup"><span data-stu-id="9e6f0-189">Build 18945</span></span>
<span data-ttu-id="9e6f0-190">Allgemeine Windows-Informationen zu Build 18945 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-190">For general Windows information on build 18945 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-191">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-191">WSL</span></span>
* <span data-ttu-id="9e6f0-192">[WSL2] Zulassen, dass der Zugriff auf lauschende TCP-Sockets in WSL2 über „localhost:port“ vom Host erfolgen kann.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-192">[WSL2] Allow listening tcp sockets in WSL2 to be accessible from the host by using localhost:port</span></span>
* <span data-ttu-id="9e6f0-193">[WSL2] Korrekturen für Installations- und Konvertierungsfehler und zusätzliche Diagnose zur Nachverfolgung zukünftiger Probleme [GH 4105]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-193">[WSL2] Fixes for install / conversion failures and additional diagnostics to track down future issues [GH 4105]</span></span> 
* <span data-ttu-id="9e6f0-194">[WSL2] Verbessern der Diagnose von WSL2-Netzwerkproblemen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-194">[WSL2] Improve diagnosability of WSL2 network issues</span></span>
* <span data-ttu-id="9e6f0-195">[WSL2] Aktualisieren der Kernelversion auf 4.19.55</span><span class="sxs-lookup"><span data-stu-id="9e6f0-195">[WSL2] Update kernel version to 4.19.55</span></span>
* <span data-ttu-id="9e6f0-196">[WSL2] Aktualisieren des Kernels mit Konfigurationsoptionen, die für Docker erforderlich sind [GH 4165]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-196">[WSL2] Update kernel with config options required for docker [GH 4165]</span></span>
* <span data-ttu-id="9e6f0-197">[WSL2] Erhöhen der Anzahl der CPUs, die der Lightweight Utility-VM zugeordnet sind, um eine mit dem Host identische Anzahl zu erreichen (wurde zuvor durch CONFIG_NR_CPUS in der Kernelkonfiguration auf 8 begrenzt) [GH 4137]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-197">[WSL2] Increase the number of CPUs assigned to the lightweight utility VM to be the same as the host (was previously capped at 8 by CONFIG_NR_CPUS in the kernel config) [GH 4137]</span></span>
* <span data-ttu-id="9e6f0-198">[WSL2] Erstellen einer Auslagerungsdatei für die WSL2-Lightweight-VM</span><span class="sxs-lookup"><span data-stu-id="9e6f0-198">[WSL2] Create a swap file for the WSL2 lightweight VM</span></span>
* <span data-ttu-id="9e6f0-199">[WSL2] Zulassen, dass Benutzereinbindungen über die \\\\wsl$\\-Distribution (z.B. sshfs) sichtbar sind [GH 4172]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-199">[WSL2] Allow user mounts to be visible via \\\\wsl$\\distro (for example sshfs) [GH 4172]</span></span>
* <span data-ttu-id="9e6f0-200">[WSL2] Verbessern der Leistung des 9P-Dateisystems</span><span class="sxs-lookup"><span data-stu-id="9e6f0-200">[WSL2] Improve 9p filesystem performance</span></span>
* <span data-ttu-id="9e6f0-201">[WSL2] Sicherstellen, dass die VHD-ACL nicht unbegrenzt anwächst [GH 4126]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-201">[WSL2] Ensure vhd ACL does not grow unbounded [GH 4126]</span></span>
* <span data-ttu-id="9e6f0-202">[WSL2] Aktualisieren der Kernelkonfiguration für die Unterstützung von squashfs und xt_conntrack [GH 4107, 4123]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-202">[WSL2] Update kernel config to support squashfs and xt_conntrack [GH 4107, 4123]</span></span>
* <span data-ttu-id="9e6f0-203">[WSL2] Korrektur für interopaktivierte „/etc/wsl.conf“-Option [GH 4140]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-203">[WSL2] Fix for interop.enabled /etc/wsl.conf option [GH 4140]</span></span>
* <span data-ttu-id="9e6f0-204">[WSL2] Rückgabe von ENOTSUP, wenn das Dateisystem EAS nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-204">[WSL2] Return ENOTSUP if the file system does not support EAs</span></span>
* <span data-ttu-id="9e6f0-205">[WSL2] Korrigieren von CopyFile-Hänger mit \\\\wsl$</span><span class="sxs-lookup"><span data-stu-id="9e6f0-205">[WSL2] Fix CopyFile hang with \\\\wsl$</span></span>
* <span data-ttu-id="9e6f0-206">Umschalten von Standard-umask in 0022 und Hinzufügen der filesystem.umask-Einstellung zu „/etc/wsl.conf“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-206">Switch default umask to 0022 and add filesystem.umask setting to /etc/wsl.conf</span></span>
* <span data-ttu-id="9e6f0-207">Korrigieren von wslpath, um symbolische Verknüpfungen ordnungsgemäß aufzulösen, dies wurde in 19h1 zurückgesetzt [GH 4078]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-207">Fix wslpath to properly resolve symlinks, this was regressed in 19h1 [GH 4078]</span></span>
* <span data-ttu-id="9e6f0-208">Einführung der Datei „%UserProfile%\\.wslconfig“ für die Optimierung der WSL2-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-208">Introduce %UserProfile%\\.wslconfig file for tweaking WSL2 settings</span></span>
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

## <a name="build-18917"></a><span data-ttu-id="9e6f0-209">Build 18917</span><span class="sxs-lookup"><span data-stu-id="9e6f0-209">Build 18917</span></span>
<span data-ttu-id="9e6f0-210">Allgemeine Windows-Informationen zu Build 18917 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-210">For general Windows information on build 18917 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/06/12/announcing-windows-10-insider-preview-build-18917/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-211">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-211">WSL</span></span>
* <span data-ttu-id="9e6f0-212">WSL 2 ist Jetzt verfügbar!</span><span class="sxs-lookup"><span data-stu-id="9e6f0-212">WSL 2 is now available!</span></span> <span data-ttu-id="9e6f0-213">Weitere Informationen finden Sie im [Blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-213">Please see [blog](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/) for more details.</span></span>
* <span data-ttu-id="9e6f0-214">Korrektur einer Regression, bei der das Starten von Windows-Prozessen über symbolische Verknüpfungen nicht ordnungsgemäß funktioniert hat [GH 3999]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-214">Fix a regression where launching Windows processes via symlinks did not work correctly [GH 3999]</span></span>
* <span data-ttu-id="9e6f0-215">Hinzufügen der Optionen wsl.exe --list --verbose, wsl.exe --list --quiet und wsl.exe --import --version zu „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-215">Add wsl.exe --list --verbose, wsl.exe --list --quiet, and wsl.exe --import --version options to wsl.exe</span></span>
* <span data-ttu-id="9e6f0-216">Hinzufügen der Option wsl.exe --shutdown</span><span class="sxs-lookup"><span data-stu-id="9e6f0-216">Add wsl.exe --shutdown option</span></span>
* <span data-ttu-id="9e6f0-217">Plan 9: Zulassen des Öffnend eines Verzeichnisses für einen erfolgreichen Schreibvorgang</span><span class="sxs-lookup"><span data-stu-id="9e6f0-217">Plan 9: Allow opening a directory for write to succeed</span></span>

## <a name="build-18890"></a><span data-ttu-id="9e6f0-218">Build 18890</span><span class="sxs-lookup"><span data-stu-id="9e6f0-218">Build 18890</span></span>
<span data-ttu-id="9e6f0-219">Allgemeine Windows-Informationen zu Build 18890 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-219">For general Windows information on build 18890 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/05/01/announcing-windows-10-insider-preview-build-18890/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-220">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-220">WSL</span></span>
* <span data-ttu-id="9e6f0-221">Nicht blockierender Socketverlust [GH 2913]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-221">Non-blocking socket leak [GH 2913]</span></span>
* <span data-ttu-id="9e6f0-222">EOF-Eingabe für Terminal kann nachfolgende Lesevorgänge blockieren [GH 3421]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-222">EOF input to terminal can block subsequent reads [GH 3421]</span></span>
* <span data-ttu-id="9e6f0-223">Aktualisieren des resolv.conf-Headers, damit er auf „wsl.conf“ verweist [in GH 3928 beschrieben].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-223">Update resolv.conf header to refer to wsl.conf [discussed in GH 3928]</span></span>
* <span data-ttu-id="9e6f0-224">Deadlock im epoll-Löschcode [GH 3922]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-224">Deadlock in epoll delete code [GH 3922]</span></span>
* <span data-ttu-id="9e6f0-225">Verarbeiten von Leerzeichen in Argumenten für --import und --export [GH 3932]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-225">Handle spaces in arguments to --import and –export [GH 3932]</span></span>
* <span data-ttu-id="9e6f0-226">Erweitern von mit mmap behandelten Dateien funktioniert nicht ordnungsgemäß [GH 3939]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-226">Extending mmap’d files does not work properly [GH 3939]</span></span>
* <span data-ttu-id="9e6f0-227">Korrektur eines Problems mit ARM64 \\\\wsl$-Zugriff funktioniert nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="9e6f0-227">Fix issue with ARM64 \\\\wsl$ access not working properly</span></span>
* <span data-ttu-id="9e6f0-228">Hinzufügen eines besseren Standardsymbols für „wsl.exe“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-228">Add better default icon for wsl.exe</span></span>

## <a name="build-18342"></a><span data-ttu-id="9e6f0-229">Build 18342</span><span class="sxs-lookup"><span data-stu-id="9e6f0-229">Build 18342</span></span>
<span data-ttu-id="9e6f0-230">Allgemeine Windows-Informationen zu Build 18342 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-230">For general Windows information on build 18342 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/20/announcing-windows-10-insider-preview-build-18342/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-231">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-231">WSL</span></span>
* <span data-ttu-id="9e6f0-232">Wir haben für Benutzer die Möglichkeit hinzugefügt, auf Linux-Dateien in einer WSL-Distribution aus Windows zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-232">We've added the ability for users to access Linux files in a WSL distro from Windows.</span></span> <span data-ttu-id="9e6f0-233">Auf diese Dateien kann über die Befehlszeile zugegriffen werden. Außerdem können Windows-Apps wie der Datei-Explorer, VSCode usw. mit diesen Dateien interagieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-233">These files can be accessed through the command line, and also Windows apps, like file explorer, VSCode, etc. can interact with these files.</span></span> <span data-ttu-id="9e6f0-234">Greifen Sie auf Ihre Dateien zu, indem Sie zu \\\\wsl$\\<distributions_name> navigieren, oder zeigen Sie eine Liste der ausgeführten Distributionen an, indem Sie zu \\\\wsl$ navigieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-234">Access your files by navigating to \\\\wsl$\\<distro_name>, or see a list of running distributions by navigating to \\\\wsl$</span></span>
* <span data-ttu-id="9e6f0-235">Hinzufügen zusätzlicher CPU-Infotags und Korrigieren der Cpus_allowed[_list]-Werte [GH 2234]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-235">Add additional CPU info tags and fix Cpus_allowed[_list] values [GH 2234]</span></span>
* <span data-ttu-id="9e6f0-236">Unterstützung der Ausführung aus Nicht-Leaderthread [GH 3800]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-236">Support exec from non-leader thread [GH 3800]</span></span>
* <span data-ttu-id="9e6f0-237">Behandeln von Konfigurationsupdatefehlern als nicht schwerwiegend [GH 3785]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-237">Treat configuration update failures as non-fatal [GH 3785]</span></span>
* <span data-ttu-id="9e6f0-238">Aktualisieren von binfmt für die ordnungsgemäße Verarbeitung von Offsets [GH 3768]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-238">Update binfmt to properly handle offsets [GH 3768]</span></span>
* <span data-ttu-id="9e6f0-239">Aktivieren der Zuordnung von Netzlaufwerken für Plan 9 [GH 3854]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-239">Enable mapping network drives for Plan 9 [GH 3854]</span></span>
* <span data-ttu-id="9e6f0-240">Unterstützung von Windows -> Linux und Linux -> Windows-Pfadübersetzung für Bindungseinbindungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-240">Support Windows -> Linux and Linux -> Windows path translation for bind mounts</span></span>
* <span data-ttu-id="9e6f0-241">Erstellen schreibgeschützter Abschnitte für Zuordnungen für Dateien, die schreibgeschützt geöffnet sind</span><span class="sxs-lookup"><span data-stu-id="9e6f0-241">Create read-only sections for mappings on files opened read-only</span></span>

## <a name="build-18334"></a><span data-ttu-id="9e6f0-242">Build 18334</span><span class="sxs-lookup"><span data-stu-id="9e6f0-242">Build 18334</span></span>
<span data-ttu-id="9e6f0-243">Allgemeine Windows-Informationen zu Build 18334 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-243">For general Windows information on build 18334 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2019/02/08/announcing-windows-10-insider-preview-build-18334/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-244">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-244">WSL</span></span>
* <span data-ttu-id="9e6f0-245">Umgestalten der Art und Weise, in der die Windows-Zeitzone einer Linux-Zeitzone zugeordnet wird [GH 3747]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-245">Redesign the way that Windows time zone is mapped to a  Linux time zone [GH 3747]</span></span>
* <span data-ttu-id="9e6f0-246">Beheben von Speicherverlusten und Hinzufügen neuer Zeichenfolgenübersetzungsfunktionen [GH 3746]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-246">Fix memory leaks and add new string translation functions [GH 3746]</span></span>
* <span data-ttu-id="9e6f0-247">SIGCONT für eine Threadgruppe ohne Threads ist eine Nulloperation [GH 3741]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-247">SIGCONT on a threadgroup with no threads is a no-op [GH 3741]</span></span> 
* <span data-ttu-id="9e6f0-248">Richtige Anzeige von Socket- und Epoll-Dateideskriptoren in „/proc/self/fd“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-248">Correctly display socket and epoll file descriptors in /proc/self/fd</span></span>

## <a name="build-18305"></a><span data-ttu-id="9e6f0-249">Build 18305</span><span class="sxs-lookup"><span data-stu-id="9e6f0-249">Build 18305</span></span>
<span data-ttu-id="9e6f0-250">Allgemeine Windows-Informationen zu Build 18305 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-250">For general Windows information on build 18305 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/12/19/announcing-windows-10-insider-preview-build-18305/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-251">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-251">WSL</span></span>
* <span data-ttu-id="9e6f0-252">pthreads verlieren den Zugriff auf Dateien, wenn der primäre Thread beendet wird [GH 3589]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-252">pthreads lose access to files when the primary thread exits [GH 3589]</span></span>
* <span data-ttu-id="9e6f0-253">TIOCSCTTY sollte den Parameter „force“ ignorieren, wenn er nicht erforderlich ist [GH 3652]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-253">TIOCSCTTY should ignore the “force” parameter unless it is required [GH 3652]</span></span>
* <span data-ttu-id="9e6f0-254">Verbesserungen an der Befehlszeile von „wsl.exe“ und Hinzufügung von Import-/Exportfunktionen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-254">wsl.exe command line improvements and addition of import / export functionality.</span></span>
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

## <a name="build-18277"></a><span data-ttu-id="9e6f0-255">Build 18277</span><span class="sxs-lookup"><span data-stu-id="9e6f0-255">Build 18277</span></span>
<span data-ttu-id="9e6f0-256">Allgemeine Windows-Informationen zu Build 18277 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-256">For general Windows information on build 18277 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/11/07/announcing-windows-10-insider-preview-build-18277/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-257">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-257">WSL</span></span>
* <span data-ttu-id="9e6f0-258">Korrektur des Fehlers „no such interface supported“ in Build 18272 [GH 3645]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-258">Fix "no such interface supported" error introduced in build 18272 [GH 3645]</span></span>
* <span data-ttu-id="9e6f0-259">Ignorieren des MNT_FORCE-Flags für Systemaufruf zum Aufheben der Einbindung [GH 3605]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-259">Ignore the MNT_FORCE flag for umount syscall [GH 3605]</span></span>
* <span data-ttu-id="9e6f0-260">Umschalten von WSL-Interop für die Verwendung der offiziellen CreatePseudoConsole-API</span><span class="sxs-lookup"><span data-stu-id="9e6f0-260">Switch WSL interop to use the official CreatePseudoConsole API</span></span>
* <span data-ttu-id="9e6f0-261">Keinen Timeoutwert beibehalten, wenn FUTEX_WAIT neu gestartet wird</span><span class="sxs-lookup"><span data-stu-id="9e6f0-261">Maintain no timeout value when FUTEX_WAIT restarts</span></span>

## <a name="build-18272"></a><span data-ttu-id="9e6f0-262">Build 18272</span><span class="sxs-lookup"><span data-stu-id="9e6f0-262">Build 18272</span></span>
<span data-ttu-id="9e6f0-263">Allgemeine Windows-Informationen zu Build 18272 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-263">For general Windows information on build 18272 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/31/announcing-windows-10-insider-preview-build-18272/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-264">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-264">WSL</span></span>
* <span data-ttu-id="9e6f0-265">**WARNUNG:** In diesem Build liegt ein Problem vor, durch das WSL nicht funktionsfähig wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-265">**WARNING:** There is an issue in this build that makes WSL inoperable.</span></span> <span data-ttu-id="9e6f0-266">Wenn Sie versuchen, die Distribution zu starten, wird der Fehler „No such interface supported“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-266">When trying to launch your distribution you will see a “No such interface supported” error.</span></span> <span data-ttu-id="9e6f0-267">Das Problem wurde behoben und ist im Insider Fast-Build der nächsten Woche nicht mehr enthalten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-267">The issue has been fixed and will be in next week's Insider Fast build.</span></span> <span data-ttu-id="9e6f0-268">Wenn Sie diesen Build installiert haben, können Sie ein Rollback auf den vorherigen Windows-Build durchführen, indem Sie unter „Einstellungen > Update und Sicherheit > Wiederherstellung“ die Option „Zur vorherigen Version von Windows 10 zurückkehren“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-268">If you've installed this build you can roll back to the previous Windows build using “Go back to the previous version of Windows 10” in Settings->Update & Security->Recovery.</span></span>

## <a name="build-18267"></a><span data-ttu-id="9e6f0-269">Build 18267</span><span class="sxs-lookup"><span data-stu-id="9e6f0-269">Build 18267</span></span>
<span data-ttu-id="9e6f0-270">Allgemeine Windows-Informationen zu Build 18267 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-270">For general Windows information on build 18267 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/24/announcing-windows-10-insider-preview-build-18267/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-271">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-271">WSL</span></span>
* <span data-ttu-id="9e6f0-272">Korrektur eines Problems, bei dem der Zombieprozess möglicherweise nicht beendet und unbegrenzt ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-272">Fix issue where zombie process may not be reaped and remain indefinitely.</span></span>
* <span data-ttu-id="9e6f0-273">WslRegisterDistribution hängt, wenn die Fehlermeldung die maximale Länge überschreitet [GH 3592]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-273">WslRegisterDistribution hangs if error message exceeds max length [GH 3592]</span></span>
* <span data-ttu-id="9e6f0-274">Zulassen der erfolgreichen Ausführung von fsync für schreibgeschützte Dateien auf DrvFs [GH 3556]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-274">Allow fsync to succeed for read-only files on DrvFs [GH 3556]</span></span>
* <span data-ttu-id="9e6f0-275">Sicherstellen, dass die Verzeichnisse „/bin“ und „/sbin“ vorhanden sind, bevor symbolische Verknüpfungen darin erstellt werden [GH 3584]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-275">Ensure that /bin and /sbin directories exist before creating symlinks inside [GH 3584]</span></span>
* <span data-ttu-id="9e6f0-276">Hinzufügen eines Instanztimeoutmechanismus für WSL-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-276">Added an instance termination timeout mechanism for WSL instances.</span></span> <span data-ttu-id="9e6f0-277">Der Timeoutwert ist derzeit auf 15 Sekunden festgelegt. Das bedeutet, dass die Instanz 15 Sekunden nach Beendigung des letzten WSL-Prozesses beendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-277">The timeout is currently set to 15 seconds, meaning the instance will terminate 15 seconds after the last WSL process exits.</span></span> <span data-ttu-id="9e6f0-278">Um eine Distribution sofort zu beenden, verwenden Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-278">To terminate a distribution immediately, use:</span></span>
```
wslconfig.exe /terminate <DistributionName>
```

## <a name="build-17763-1809"></a><span data-ttu-id="9e6f0-279">Build 17763 (1809)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-279">Build 17763 (1809)</span></span>
<span data-ttu-id="9e6f0-280">Allgemeine Windows-Informationen zu Build 17763 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-280">For general Windows information on build 17763 visit the [Windows blog](https://blogs.windows.com/windowsexperience/2018/10/02/how-to-get-the-windows-10-october-2018-update/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-281">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-281">WSL</span></span>
* <span data-ttu-id="9e6f0-282">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-282">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="9e6f0-283">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-283">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="9e6f0-284">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-284">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="9e6f0-285">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-285">Better handling of threadgroup leader file descriptor cleanup.</span></span>
* <span data-ttu-id="9e6f0-286">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-286">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="9e6f0-287">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-287">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="9e6f0-288">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-288">Fix several AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="9e6f0-289">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-289">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>
* <span data-ttu-id="9e6f0-290">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-290">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="9e6f0-291">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-291">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="9e6f0-292">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-292">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="9e6f0-293">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-293">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="9e6f0-294">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-294">Pipe filesystem inadvertently clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9e6f0-295">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-295">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>
* <span data-ttu-id="9e6f0-296">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-296">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="9e6f0-297">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-297">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="9e6f0-298">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-298">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="9e6f0-299">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-299">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="9e6f0-300">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-300">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="9e6f0-301">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-301">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="9e6f0-302">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-302">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="9e6f0-303">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-303">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="9e6f0-304">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-304">Windows UI apps should execute even when launched in the background.</span></span>
* <span data-ttu-id="9e6f0-305">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-305">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="9e6f0-306">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-306">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="9e6f0-307">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-307">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="9e6f0-308">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-308">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="9e6f0-309">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-309">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="9e6f0-310">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-310">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="9e6f0-311">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-311">Add wslconfig /terminate to stop running distributions.</span></span>
* <span data-ttu-id="9e6f0-312">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-312">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="9e6f0-313">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="9e6f0-313">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="9e6f0-314">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-314">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="9e6f0-315">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-315">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="9e6f0-316">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-316">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>
* <span data-ttu-id="9e6f0-317">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-317">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="9e6f0-318">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-318">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="9e6f0-319">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-319">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="9e6f0-320">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-320">Atomically create case sensitive directories in DrvFs.</span></span>
* <span data-ttu-id="9e6f0-321">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-321">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9e6f0-322">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-322">[GH 2712]</span></span>
* <span data-ttu-id="9e6f0-323">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="9e6f0-323">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="9e6f0-324">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-324">[GH 3020]</span></span>
* <span data-ttu-id="9e6f0-325">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-325">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="9e6f0-326">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-326">To use, hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="9e6f0-327">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-327">Fix Unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="9e6f0-328">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-328">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="9e6f0-329">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-329">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="9e6f0-330">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-330">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="9e6f0-331">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-331">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="9e6f0-332">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-332">Add --distribution option for wsl.exe to select a specific distro.</span></span>
* <span data-ttu-id="9e6f0-333">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-333">Limited support for dmesg.</span></span> <span data-ttu-id="9e6f0-334">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-334">Applications can now log to dmesg.</span></span> <span data-ttu-id="9e6f0-335">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-335">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="9e6f0-336">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-336">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="9e6f0-337">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-337">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="9e6f0-338">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-338">`syslog` syscall interface is not yet supported.</span></span> <span data-ttu-id="9e6f0-339">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-339">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="9e6f0-340">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-340">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="9e6f0-341">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-341">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="9e6f0-342">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-342">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="9e6f0-343">Einige Zeichen (etwa „/“, „:“ und „\*“) sind unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-343">Some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-18252-skip-ahead"></a><span data-ttu-id="9e6f0-344">Build 18252 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-344">Build 18252 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-345">Allgemeine Windows-Informationen zu Build 18252 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-345">For general Windows information on build 18252 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/10/03/announcing-windows-10-insider-preview-build-18252/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-346">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-346">WSL</span></span>
* <span data-ttu-id="9e6f0-347">Verschieben von init- und bsdtar-Binärdateien aus der lxssmanager-DLL in einen separaten Toolsordner</span><span class="sxs-lookup"><span data-stu-id="9e6f0-347">Move init and bsdtar binaries out of lxssmanager dll and into a separate tools folder</span></span>
* <span data-ttu-id="9e6f0-348">Korrektur von Racebedingung um schließenden Dateideskriptor bei Verwendung von CLONE_FILES</span><span class="sxs-lookup"><span data-stu-id="9e6f0-348">Fix race around closing file descriptor when using CLONE_FILES</span></span>
* <span data-ttu-id="9e6f0-349">Verarbeiten optionaler Felder in „/proc/pid/mountinfo“ bei der Übersetzung von DrvFs-Pfaden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-349">Handle optional fields in /proc/pid/mountinfo when translating DrvFs paths</span></span>
* <span data-ttu-id="9e6f0-350">Zulassen, dass DrvFs mklod ohne Metadatenunterstützung für S_IFREG erfolgreich ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-350">Allow DrvFs mknod to succeed without metadata support for S_IFREG</span></span>
* <span data-ttu-id="9e6f0-351">Für schreibgeschützte Dateien, die auf DrvFs erstellt wurden, muss das schreibgeschützte Attribut festgelegt werden [GH 3411]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-351">Readonly files created on DrvFs should have the readonly attribute set [GH 3411]</span></span>
* <span data-ttu-id="9e6f0-352">Hinzufügen von /sbin/mount.drvfs-Hilfsprogramm zur Verarbeitung der DrvFs-Einbindung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-352">Add /sbin/mount.drvfs helper to handle DrvFs mounting</span></span>
* <span data-ttu-id="9e6f0-353">Verwenden der POSIX-Umbenennung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-353">Use POSIX rename in DrvFs.</span></span>
* <span data-ttu-id="9e6f0-354">Ermöglichen der Pfadübersetzung für Volumes ohne Volume-GUID.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-354">Allow path translation on volumes without a volume GUID.</span></span>

## <a name="build-17738-fast"></a><span data-ttu-id="9e6f0-355">Build 17738 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-355">Build 17738 (Fast)</span></span>
<span data-ttu-id="9e6f0-356">Allgemeine Windows-Informationen zu Build 17738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-356">For general Windows information on build 17738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/08/14/announcing-windows-10-insider-preview-build-17738/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-357">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-357">WSL</span></span>
* <span data-ttu-id="9e6f0-358">Berechtigungsüberprüfung für Setpriority-Systemaufruf ist zu streng, um die gleiche Threadpriorität zu ändern[GH 1838].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-358">Setpriority syscall permission check too strict for changing same thread priority [GH 1838]</span></span>
* <span data-ttu-id="9e6f0-359">Stellen Sie sicher, dass die unbeeinflusste Interruptzeit für die Startzeit verwendet wird, um zu vermeiden, dass negative Werte für clock_gettime (CLOCK_BOOTTIME) zurückgegeben werden [GH 3434]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-359">Ensure that unbiased interrupt time is used for boot time to avoid returning negative values for clock_gettime(CLOCK_BOOTTIME) [GH 3434]</span></span>
* <span data-ttu-id="9e6f0-360">Verarbeiten von symbolischen Verknüpfungen im WSL-binfmt-Interpreter [GH 3424]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-360">Handle symlinks in the WSL binfmt interpreter [GH 3424]</span></span>
* <span data-ttu-id="9e6f0-361">Bessere Verarbeitung der Bereinigung des Threadgruppen-Leaderdateideskriptors.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-361">Better handling of threadgroup leader file descriptor cleanup.</span></span>

## <a name="build-17728-fast"></a><span data-ttu-id="9e6f0-362">Build 17728 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-362">Build 17728 (Fast)</span></span>
<span data-ttu-id="9e6f0-363">Allgemeine Windows-Informationen zu Build 17728 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-363">For general Windows information on build 17728 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/31/announcing-windows-10-insider-preview-build-17728/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-364">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-364">WSL</span></span>
* <span data-ttu-id="9e6f0-365">Umschalten von WSL für die Verwendung von KeQueryInterruptTimePrecise anstelle von KeQueryPerformanceCounter zur Vermeidung eines Überlaufs [GH 3252].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-365">Switch WSL to use KeQueryInterruptTimePrecise instead of KeQueryPerformanceCounter to avoid overflow [GH 3252]</span></span>
* <span data-ttu-id="9e6f0-366">Ptrace-Anfügevorgang kann zu einem ungültigen Rückgabewert von Systemaufrufen führen [GH 1731]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-366">Ptrace attach may cause bad return value from system calls [GH 1731]</span></span>
* <span data-ttu-id="9e6f0-367">Korrektur mehrerer Probleme, die sich auf AF_UNIX beziehen [GH 3371]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-367">Fix a number of AF_UNIX related issues [GH 3371]</span></span>
* <span data-ttu-id="9e6f0-368">Korrektur eines Problems, das dazu führen kann, dass WSL-Interop fehlschlägt, wenn das aktuelle Arbeitsverzeichnis weniger als 5 Zeichen lang ist [GH 3379]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-368">Fix issue that could cause WSL interop to fail if the current working directory is less than 5 characters long [GH 3379]</span></span>

## <a name="build-18204-skip-ahead"></a><span data-ttu-id="9e6f0-369">Build 18204 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-369">Build 18204 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-370">Allgemeine Windows-Informationen zu Build 18204 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-370">For general Windows information on build 18204 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-371">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-371">WSL</span></span>
* <span data-ttu-id="9e6f0-372">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-372">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9e6f0-373">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-373">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17723-fast"></a><span data-ttu-id="9e6f0-374">Build 17723 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-374">Build 17723 (Fast)</span></span>
<span data-ttu-id="9e6f0-375">Allgemeine Windows-Informationen zu Build 17723 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-375">For general Windows information on build 17723 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/25/announcing-windows-10-insider-preview-build-17723-and-build-18204/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-376">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-376">WSL</span></span>
* <span data-ttu-id="9e6f0-377">Vermeiden von einer Sekunde Verzögerung bei Ausfall von Loopbackverbindungen mit nicht vorhandenen Ports [GH 3286]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-377">Avoid one second delay failing loopback connections to non-existent ports [GH 3286]</span></span>
* <span data-ttu-id="9e6f0-378">Hinzufügen der Stubdatei „/proc/sys/fs/file-max“ [GH 2893]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-378">Add /proc/sys/fs/file-max stub file [GH 2893]</span></span>
* <span data-ttu-id="9e6f0-379">Genauere IPv6-Bereichsinformationen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-379">More accurate IPV6 scope information.</span></span>
* <span data-ttu-id="9e6f0-380">PR_SET_PTRACER-Unterstützung [GH 3053]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-380">PR_SET_PTRACER support [GH 3053]</span></span>
* <span data-ttu-id="9e6f0-381">Versehentliches Löschen eines edge-ausgelösten epoll-Ereignisses durch das Pipedateisystem [GH 3276]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-381">Pipe filesystem inadvertenly clearing edge-triggered epoll event [GH 3276]</span></span>
* <span data-ttu-id="9e6f0-382">Ausführbare Win32-Datei, die über die symbolische NTFS-Verknüpfung gestartet wurde, respektiert den Namen der symbolischen Verknüpfung nicht [GH 2909]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-382">Win32 executable launched via NTFS symlink doesn't respect symlink name [GH 2909]</span></span>

## <a name="build-17713"></a><span data-ttu-id="9e6f0-383">Build 17713</span><span class="sxs-lookup"><span data-stu-id="9e6f0-383">Build 17713</span></span>
<span data-ttu-id="9e6f0-384">Allgemeine Windows-Informationen zu Build 17713 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-384">For general Windows information on build 17713 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/07/11/announcing-windows-10-insider-preview-build-17713/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-385">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-385">WSL</span></span>
* <span data-ttu-id="9e6f0-386">Verbesserte Zombieunterstützung [GH 1353]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-386">Improved zombie support [GH 1353]</span></span>
* <span data-ttu-id="9e6f0-387">Hinzufügen von wsl.conf-Einträgen zum Steuern des Windows-Interop-Verhaltens [GH 1493]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-387">Add wsl.conf entries for controlling Windows interop behavior [GH 1493]</span></span>
  ```
    [interop]

    enabled=false # enable launch of Windows binaries; default is true

    appendWindowsPath=false # append Windows path to $PATH variable; default is true
  ```
* <span data-ttu-id="9e6f0-388">Korrektur des Verhaltens, dass getsockname nicht immer den Porduktfamilientyp des UNIX-Sockets zurückgibt [GH 1774]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-388">Fix for getsockname not always returning UNIX socket family type [GH 1774]</span></span>
* <span data-ttu-id="9e6f0-389">Hinzufügen von Unterstützung für TIOCSTI [GH 1863]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-389">Add support for TIOCSTI [GH 1863]</span></span>
* <span data-ttu-id="9e6f0-390">Nicht blockierende Sockets beim Verbindungsaufbau sollten für Schreibversuche EAGAIN zurückgeben [GH 2846]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-390">Non-blocking sockets in the process of connecting should return EAGAIN for write attempts [GH 2846]</span></span>
* <span data-ttu-id="9e6f0-391">Unterstützung von Interop auf eingebundenen VHDs [GH 3246, 3291]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-391">Support interop on mounted VHDs [GH 3246, 3291]</span></span>
* <span data-ttu-id="9e6f0-392">Korrektur von Problem mit der Berechtigungsüberprüfung im Stammordner [GH 3304]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-392">Fix permission checking issue on root folder [GH 3304]</span></span>
* <span data-ttu-id="9e6f0-393">Eingeschränkte Unterstützung für die TTY-Tastatur-ioctls KDGKBTYPE, KDGKBMODE und KDSKBMODE.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-393">Limited support for TTY keyboard ioctls KDGKBTYPE, KDGKBMODE and KDSKBMODE.</span></span>
* <span data-ttu-id="9e6f0-394">Windows-UI-Apps sollten ausgeführt selbst dann werden, wenn Sie im Hintergrund gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-394">Windows UI apps should execute even when launched in the background.</span></span>

## <a name="build-17704"></a><span data-ttu-id="9e6f0-395">Build 17704</span><span class="sxs-lookup"><span data-stu-id="9e6f0-395">Build 17704</span></span>
<span data-ttu-id="9e6f0-396">Allgemeine Windows-Informationen zu Build 17704 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-396">For general Windows information on build 17704 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/27/announcing-windows-10-insider-preview-build-17704/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-397">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-397">WSL</span></span>
* <span data-ttu-id="9e6f0-398">Hinzufügen der Option wsl -u oder--user [GH 1203]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-398">Add wsl -u or --user option [GH 1203]</span></span>
* <span data-ttu-id="9e6f0-399">Korrektur von WSL-Startproblemen, wenn der Schnellstart aktiviert ist [GH 2576]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-399">Fix WSL launch issues when fast startup is enabled [GH 2576]</span></span>
* <span data-ttu-id="9e6f0-400">Unix-Sockets müssen getrennte Peeranmelde Informationen beibehalten [GH 3183]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-400">Unix sockets need to retain disconnected peer credentials [GH 3183]</span></span>
* <span data-ttu-id="9e6f0-401">Nicht blockierende Unix-Sockets, die unbegrenzt EAGAIN-Fehler ausgeben [GH 3191]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-401">Non-blocking Unix sockets failing indefinitely with EAGAIN [GH 3191]</span></span>
* <span data-ttu-id="9e6f0-402">case=off ist der neue standardmäßige drvfs-Einbindungstyp [GH 2937, 3212, 3328]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-402">case=off is the new default drvfs mount type [GH 2937, 3212, 3328]</span></span>
    * <span data-ttu-id="9e6f0-403">Weitere Informationen finden Sie im [Blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-403">See [blog](https://blogs.msdn.microsoft.com/commandline/2018/06/14/improved-per-directory-case-sensitivity-support-in-wsl/) for more information.</span></span>
* <span data-ttu-id="9e6f0-404">Hinzufügen von wslconfig/terminate zum Beenden ausgeführter Distributionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-404">Add wslconfig /terminate to stop running distributions.</span></span>

## <a name="build-17692"></a><span data-ttu-id="9e6f0-405">Build 17692</span><span class="sxs-lookup"><span data-stu-id="9e6f0-405">Build 17692</span></span>
<span data-ttu-id="9e6f0-406">Allgemeine Windows-Informationen zu Build 17692 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-406">For general Windows information on build 17692 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/14/announcing-windows-10-insider-preview-build-17692).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-407">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-407">WSL</span></span>
* <span data-ttu-id="9e6f0-408">Korrektur des Problems mit den Kontextmenüeinträgen der WSL-Shell, die Pfade mit Leerzeichen nicht ordnungsgemäß behandeln.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-408">Fix issue with the WSL shell context menu entries that do not correctly handle paths with spaces.</span></span>
* <span data-ttu-id="9e6f0-409">Bereitstellen von Unterscheidung von Groß-/Kleinschreibung pro Verzeichnis als erweitertes Attribut</span><span class="sxs-lookup"><span data-stu-id="9e6f0-409">Expose per-directory case sensitivity as an extended attribute</span></span>
* <span data-ttu-id="9e6f0-410">ARM64: Emulieren von Cacheverwaltungsvorgängen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-410">ARM64: Emulate cache maintenance operations.</span></span> <span data-ttu-id="9e6f0-411">Beheben von [dotnet-Problem](https://github.com/dotnet/core/issues/1561).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-411">Resolve [dotnet issue](https://github.com/dotnet/core/issues/1561).</span></span>
* <span data-ttu-id="9e6f0-412">DrvFs: Nur Escapezeichen im privaten Bereich, die einem mit Escapezeichen versehenen Zeichen entsprechen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-412">DrvFs: only unescape characters in the private range that correspond to an escaped character.</span></span>

## <a name="build-17686"></a><span data-ttu-id="9e6f0-413">Build 17686</span><span class="sxs-lookup"><span data-stu-id="9e6f0-413">Build 17686</span></span>
<span data-ttu-id="9e6f0-414">Allgemeine Windows-Informationen zu Build 17686 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-414">For general Windows information on build 17686 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/06/06/announcing-windows-10-insider-preview-build-17686).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-415">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-415">WSL</span></span>
* <span data-ttu-id="9e6f0-416">Korrektur eines Off-by-one-Fehlers in der Längenüberprüfung des ELF Parserinterpreters [GH 3154].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-416">Fix off-by-one error in ELF parser interpreter length validation [GH 3154]</span></span>
* <span data-ttu-id="9e6f0-417">Absolute WSL-Timer mit einer Zeitangabe in der Vergangenheit werden nicht ausgelöst [GH 3091]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-417">WSL absolute timers with a time in the past do not fire [GH 3091]</span></span>
* <span data-ttu-id="9e6f0-418">Sicherstellen, dass neu erstellte Analysepunkte als solche im übergeordneten Verzeichnis aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-418">Ensure newly created reparse points are listed as such in the parent directory.</span></span>
* <span data-ttu-id="9e6f0-419">Atomarisches Erstellen von Verzeichnissen mit Berücksichtigung von Groß- und Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-419">Atomically create case sensitive directories in DrvFs.</span></span>

## <a name="build-17677"></a><span data-ttu-id="9e6f0-420">Build 17677</span><span class="sxs-lookup"><span data-stu-id="9e6f0-420">Build 17677</span></span>
<span data-ttu-id="9e6f0-421">Allgemeine Windows-Informationen zu Build 17677 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-421">For general Windows information on build 17677 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/24/announcing-windows-10-insider-preview-build-17677/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-422">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-422">WSL</span></span>
* <span data-ttu-id="9e6f0-423">Korrektur eines zusätzlichen Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-423">Fixed an additional issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9e6f0-424">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-424">[GH 2712]</span></span>
* <span data-ttu-id="9e6f0-425">Korrektur eines WSL-Startfehlers, wenn UMCI aktiviert ist.-</span><span class="sxs-lookup"><span data-stu-id="9e6f0-425">Fixed WSL launch failure when UMCI is enabled.</span></span> <span data-ttu-id="9e6f0-426">[GH 3020]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-426">[GH 3020]</span></span>

## <a name="build-17666"></a><span data-ttu-id="9e6f0-427">Build 17666</span><span class="sxs-lookup"><span data-stu-id="9e6f0-427">Build 17666</span></span>
<span data-ttu-id="9e6f0-428">Allgemeine Windows-Informationen zu Build 17666 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-428">For general Windows information on build 17666 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/05/09/announcing-windows-10-insider-preview-build-17666/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-429">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-429">WSL</span></span>
#### <a name="warning-there-is-an-issue-preventing-wsl-from-running-on-some-amd-chipsets-gh-3134-a-fix-is-ready-and-making-its-way-to-the-insider-build-branch"></a><span data-ttu-id="9e6f0-430">WARNUNG: Es gibt ein Problem, das das Ausführen von WSL in einigen AMD-Chipsätzen verhindert [GH 3134].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-430">WARNING: There is an issue preventing WSL from running on some AMD chipsets [GH 3134].</span></span> <span data-ttu-id="9e6f0-431">Eine Korrektur ist verfügbar und wird in den Insider Build-Branch integriert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-431">A fix is ready and making its way to the Insider Build branch.</span></span>
* <span data-ttu-id="9e6f0-432">Hinzufügen des Explorer-Kontextmenüs zum Starten von WSL [GH 437, 603, 1836].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-432">Add explorer context menu to launch WSL [GH 437, 603, 1836].</span></span> <span data-ttu-id="9e6f0-433">Halten Sie in einem Explorer-Fenster die UMSCHALTTASTE gedrückt, und klicken Sie mit der rechten Maustaste, um diese Option zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-433">To use hold shift and right-click when in an explorer window.</span></span>
* <span data-ttu-id="9e6f0-434">Korrektur des nicht blockierenden UNIX-Socketverhaltens [GH 2822, 3100]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-434">Fix unix socket non-blocking behavior [GH 2822, 3100]</span></span>
* <span data-ttu-id="9e6f0-435">Korrigieren des hängenden NETLINK-Befehls, wie in GH 2026 gemeldet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-435">Fix hanging NETLINK command as reported in GH 2026.</span></span>
* <span data-ttu-id="9e6f0-436">Hinzufügen von Unterstützung für Einbindungsweitergabeflags [GH 2911]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-436">Add support for mount propagation flags [GH 2911].</span></span>
* <span data-ttu-id="9e6f0-437">Korrektur von Problem mit truncate, das keine inotify-Ereignisse verursacht [GH 2978].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-437">Fix issue with truncate not causing inotify events [GH 2978].</span></span>
* <span data-ttu-id="9e6f0-438">Hinzufügen der Option --exec für „wsl.exe“ zum Aufrufen eine einzelne Binärdatei ohne Shell.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-438">Add --exec option for wsl.exe to invoke a single binary without a shell.</span></span>
* <span data-ttu-id="9e6f0-439">Hinzufügen der Option --distribution für „wsl.exe“, um eine bestimmte Distribution auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-439">Add --distribution option for wsl.exe to select a specific distro.</span></span>

## <a name="build-17655-skip-ahead"></a><span data-ttu-id="9e6f0-440">Build 17655 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-440">Build 17655 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-441">Allgemeine Windows-Informationen zu Build 17655 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-441">For general Windows information on build 17655 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/25/announcing-windows-10-insider-preview-build-17655-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-442">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-442">WSL</span></span>
* <span data-ttu-id="9e6f0-443">Eingeschränkte Unterstützung für dmesg.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-443">Limited support for dmesg.</span></span> <span data-ttu-id="9e6f0-444">Anwendungen können sich jetzt in dmesg protokollieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-444">Applications can now log to dmesg.</span></span> <span data-ttu-id="9e6f0-445">Der WSL-Treiber protokolliert eingeschränkte Informationen in dmesg.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-445">WSL driver logs limited information to dmesg.</span></span> <span data-ttu-id="9e6f0-446">In Zukunft kann dies so erweitert werden, dass andere Informationen/Diagnoseinhalte vom Treiber erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-446">In future, this can be extended to carry other information/diagnostics from the driver.</span></span>
    * <span data-ttu-id="9e6f0-447">Hinweis: dmesg wird derzeit über die `/dev/kmsg`-Geräteschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-447">Note: dmesg is currently supported through the `/dev/kmsg` device interface.</span></span> <span data-ttu-id="9e6f0-448">`syslog`-Systemaufrufschnittstelle wird noch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-448">`syslog` sycall interface is not yet supported.</span></span> <span data-ttu-id="9e6f0-449">Daher funktionieren einige der `dmesg`-Befehlszeilenoptionen (z.B. `-S`, `-C`) nicht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-449">And, so, some of the `dmesg` command line options such as `-S`, `-C` don't work.</span></span>
* <span data-ttu-id="9e6f0-450">Korrektur eines Problems, bei dem Multithreadingvorgänge ENOENT zurückgeben konnten, obwohl die Datei vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-450">Fixed an issue where multithreaded operations could return ENOENT even though the file exists.</span></span> <span data-ttu-id="9e6f0-451">[GH 2712]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-451">[GH 2712]</span></span>

## <a name="build-17639-skip-ahead"></a><span data-ttu-id="9e6f0-452">Build 17639 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-452">Build 17639 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-453">Allgemeine Windows-Informationen zu Build 17639 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-453">For general Windows information on build 17639 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/04/04/announcing-windows-10-insider-preview-build-17639-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-454">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-454">WSL</span></span>
* <span data-ttu-id="9e6f0-455">Änderung der Standard-GID und des Modus von seriellen Geräten entsprechend den nativen Einstellungen [GH 3042]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-455">Change default gid and mode of serial devices to match native [GH 3042]</span></span>
* <span data-ttu-id="9e6f0-456">DrvFs unterstützt jetzt erweiterte Attribute.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-456">DrvFs now supports extended attributes.</span></span>
    * <span data-ttu-id="9e6f0-457">Hinweis: Für DrvFs gelten einige Einschränkungen für den Namen erweiterter Attribute.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-457">Note: DrvFs has some limitations on the name of extended attributes.</span></span> <span data-ttu-id="9e6f0-458">Insbesondere sind einige Zeichen (etwa „/“, „:“ und „\*“) unzulässig, und für Namen erweiterter Attribute wird in DrvFs keine Groß- und Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-458">In particular, some characters (like '/', ':' and '\*') are not allowed, and extended attribute names are not case sensitive on DrvFs</span></span>

## <a name="build-17133-fast"></a><span data-ttu-id="9e6f0-459">Build 17133 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-459">Build 17133 (Fast)</span></span>
<span data-ttu-id="9e6f0-460">Allgemeine Windows-Informationen zu Build 17133 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-460">For general Windows information on build 17133 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/27/announcing-windows-10-insider-preview-build-17133-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-461">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-461">WSL</span></span>
* <span data-ttu-id="9e6f0-462">Fehlerbehebung für Hängen in WSL.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-462">Fix for hang in WSL.</span></span> <span data-ttu-id="9e6f0-463">[GH 3039, 3034]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-463">[GH 3039, 3034]</span></span>

## <a name="build-17128-fast"></a><span data-ttu-id="9e6f0-464">Build 17128 (Fast)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-464">Build 17128 (Fast)</span></span>
<span data-ttu-id="9e6f0-465">Allgemeine Windows-Informationen zu Build 17128 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-465">For general Windows information on build 17128 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/23/announcing-windows-10-insider-preview-build-17128-for-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-466">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-466">WSL</span></span>
* <span data-ttu-id="9e6f0-467">Keine</span><span class="sxs-lookup"><span data-stu-id="9e6f0-467">None</span></span>

## <a name="build-17627-skip-ahead"></a><span data-ttu-id="9e6f0-468">Build 17627 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-468">Build 17627 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-469">Allgemeine Windows-Informationen zu Build 17627 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-469">For general Windows information on build 17627 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/21/announcing-windows-10-insider-preview-build-17627-for-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-470">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-470">WSL</span></span>
* <span data-ttu-id="9e6f0-471">Hinzufügen von Unterstützung für futex-pi-fähige Vorgänge.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-471">Add support for the futex pi-aware operations.</span></span> <span data-ttu-id="9e6f0-472">[GH 1006]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-472">[GH 1006]</span></span>
    * <span data-ttu-id="9e6f0-473">Beachten Sie, dass Prioritäten derzeit keine unterstützte WSL-Funktion sind, sodass Einschränkungen bestehen. Die Standardverwenund sollte jedoch aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-473">Note that priorities are not currently a supported WSL feature so there are limitations, but standard usage should be unblocked.</span></span>
* <span data-ttu-id="9e6f0-474">Windows-Firewallunterstützung für WSL-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-474">Windows firewall support for WSL processes.</span></span> <span data-ttu-id="9e6f0-475">[GH 1852]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-475">[GH 1852]</span></span>
    * <span data-ttu-id="9e6f0-476">Um beispielsweise zuzulassen, dass der WSL python-Prozess an einem beliebigen Port lauschen kann, verwenden Sie Windows-CMD mit erhöhten Rechten: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span><span class="sxs-lookup"><span data-stu-id="9e6f0-476">For example, to allow the WSL python process to listen on any port, use the elevated Windows cmd: ```netsh.exe advfirewall firewall add rule name=wsl_python dir=in action=allow program="C:\users\<username>\appdata\local\packages\canonicalgrouplimited.ubuntuonwindows_79rhkp1fndgsc\localstate\rootfs\usr\bin\python2.7" enable=yes```</span></span>
    * <span data-ttu-id="9e6f0-477">Weitere Informationen zum Hinzufügen von Firewallregeln finden Sie unter [Link.](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-477">For additional details on how to add firewall rules, see [link](https://support.microsoft.com/en-us/help/947709/how-to-use-the-netsh-advfirewall-firewall-context-instead-of-the-netsh)</span></span>
* <span data-ttu-id="9e6f0-478">Beachten der Standardshell des Benutzers bei der Verwendung von „wsl.exe“.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-478">Respect user's default shell when using wsl.exe.</span></span> <span data-ttu-id="9e6f0-479">[GH 2372]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-479">[GH 2372]</span></span>
* <span data-ttu-id="9e6f0-480">Melden aller Netzwerkschnittstellen als Ethernet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-480">Report all network interfaces as ethernet.</span></span> <span data-ttu-id="9e6f0-481">[GH 2996]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-481">[GH 2996]</span></span>
* <span data-ttu-id="9e6f0-482">Bessere Verarbeitung von beschädigten /etc/passwd-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-482">Better handling of corrupt /etc/passwd file.</span></span> <span data-ttu-id="9e6f0-483">[GH 3001]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-483">[GH 3001]</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-484">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-484">Console</span></span>
* <span data-ttu-id="9e6f0-485">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-485">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-486">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-486">LTP Results:</span></span>
<span data-ttu-id="9e6f0-487">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-487">Testing in progress.</span></span>

## <a name="build-17618-skip-ahead"></a><span data-ttu-id="9e6f0-488">Build 17618 (Skip Ahead)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-488">Build 17618 (Skip Ahead)</span></span>
<span data-ttu-id="9e6f0-489">Allgemeine Windows-Informationen zu Build 17618 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-489">For general Windows information on build 17618 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/03/07/announcing-windows-10-insider-preview-build-17618-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-490">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-490">WSL</span></span>
* <span data-ttu-id="9e6f0-491">Einführung in Pseudoconsolenfunktionalität für NT-Interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-491">Introduce pseudoconsole functionality for NT interop [GH 988, 1366, 1433, 1542, 2370, 2406].</span></span>
* <span data-ttu-id="9e6f0-492">Der Legacyinstallationsmechanismus („lxrun.exe“) ist veraltet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-492">The legacy install mechanism (lxrun.exe) has been deprecated.</span></span> <span data-ttu-id="9e6f0-493">Der unterstützte Mechanismus zum Installieren von Distributionen ist der Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-493">The supported mechanism for installing distributions is through the Microsoft Store.</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-494">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-494">Console</span></span>
* <span data-ttu-id="9e6f0-495">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-495">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-496">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-496">LTP Results:</span></span>
<span data-ttu-id="9e6f0-497">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-497">Testing in progress.</span></span>

## <a name="build-17110"></a><span data-ttu-id="9e6f0-498">Build 17110</span><span class="sxs-lookup"><span data-stu-id="9e6f0-498">Build 17110</span></span>
<span data-ttu-id="9e6f0-499">Allgemeine Windows-Informationen zu Build 17110 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-499">For general Windows information on build 17110 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/27/announcing-windows-10-insider-preview-build-17110-fast/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-500">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-500">WSL</span></span>
* <span data-ttu-id="9e6f0-501">Zulassen, dass /init aus Windows beendet wird [GH 2928].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-501">Allow /init to be terminated from Windows [GH 2928].</span></span>
* <span data-ttu-id="9e6f0-502">DrvFs verwendet nun standardmäßig Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis (entspricht der Einbindungsoption „case=dir“).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-502">DrvFs now uses per-directory case sensitivity by default (equivalent to the “case=dir” mount option).</span></span>
    * <span data-ttu-id="9e6f0-503">Wenn Sie „case=force“ verwenden (das alte Verhalten), muss ein Registrierungsschlüssel festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-503">Using “case=force” (the old behavior) requires setting a registry key.</span></span> <span data-ttu-id="9e6f0-504">Führen Sie den folgenden Befehl aus, um „case=force“ zu aktivieren, wenn Sie diese Option verwenden müssen: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span><span class="sxs-lookup"><span data-stu-id="9e6f0-504">Run the following command to enable “case=force” if you need to use it: reg add HKLM\SYSTEM\CurrentControlSet\Services\lxss /v DrvFsAllowForceCaseSensitivity /t REG_DWORD /d 1</span></span>
    * <span data-ttu-id="9e6f0-505">Wenn Sie über vorhandene Verzeichnisse verfügen, die mit WSL in einer älteren Version von Windows erstellt wurden, bei denen die Groß-/Kleinschreibung beachtet werden muss, verwenden Sie „fsutil.exe“, um sie für Unterscheidung von Groß-/Kleinschreibung zu markieren: fsutil.exe file setcasesensitiveinfo <path> enable</span><span class="sxs-lookup"><span data-stu-id="9e6f0-505">If you have existing directories created with WSL in older version of Windows which need to be case sensitive, use fsutil.exe to mark them as case sensitive: fsutil.exe file setcasesensitiveinfo <path> enable</span></span>
* <span data-ttu-id="9e6f0-506">NULL-Beendigungszeichenfolgen werden vom uname-Systemaufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-506">NULL terminate strings returned from the uname syscall.</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-507">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-507">Console</span></span>
* <span data-ttu-id="9e6f0-508">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-508">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-509">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-509">LTP Results:</span></span>
<span data-ttu-id="9e6f0-510">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-510">Testing in progress.</span></span>

## <a name="build-17107"></a><span data-ttu-id="9e6f0-511">Build 17107</span><span class="sxs-lookup"><span data-stu-id="9e6f0-511">Build 17107</span></span>
<span data-ttu-id="9e6f0-512">Allgemeine Windows-Informationen zu Build 17107 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-512">For general Windows information on build 17107 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/23/announcing-windows-10-insider-preview-build-17107-fast-ring/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-513">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-513">WSL</span></span>
* <span data-ttu-id="9e6f0-514">Unterstützung von TCSETSF und TCSETSW für pty-Masterendpunkte [GH 2552].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-514">Support TCSETSF and TCSETSW on master pty endpoints [GH 2552].</span></span>
* <span data-ttu-id="9e6f0-515">Starten von gleichzeitigen Interop-Prozessen kann zu EINVAL führen [GH 2813].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-515">Starting simultaneous interop processes can result in EINVAL [GH 2813].</span></span>
* <span data-ttu-id="9e6f0-516">Korrektur von PTRACE_ATTACH, um den richtigen Ablaufverfolgungsstatus in „/proc/pid/status“ anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-516">Fix PTRACE_ATTACH to show proper tracing status in /proc/pid/status.</span></span>
* <span data-ttu-id="9e6f0-517">Korrektur der Racebedingung, bei der kurzlebige Prozesse, die mit den CLEARTID- und SETTID-Flags geklont wurden, ohne Löschen der TID-Adresse beendet werden konnten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-517">Fix race where short-lived processes cloned with both the CLEARTID and SETTID flags could exit without clearing the TID address.</span></span>
* <span data-ttu-id="9e6f0-518">Anzeigen einer Meldung beim Aktualisieren der Linux-Dateisystemverzeichnisse beim Umstieg von einem Build vor 17093.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-518">Display a message when upgrading the Linux file system directories when moving from a pre-17093 build.</span></span> <span data-ttu-id="9e6f0-519">Weitere Informationen zu den Änderungen für das 17093-Dateisystem finden Sie in den Anmerkungen zur Version für [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-519">For more details on the 17093 file system changes, see the release notes for [17093](https://github.com/MicrosoftDocs/WSL/blob/live/WSL/release-notes.md#build-17093).</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-520">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-520">Console</span></span>
* <span data-ttu-id="9e6f0-521">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-521">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-522">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-522">LTP Results:</span></span>
<span data-ttu-id="9e6f0-523">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-523">Testing in progress.</span></span>

## <a name="build-17101"></a><span data-ttu-id="9e6f0-524">Build 17101</span><span class="sxs-lookup"><span data-stu-id="9e6f0-524">Build 17101</span></span>
<span data-ttu-id="9e6f0-525">Allgemeine Windows-Informationen zu Build 17101 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-525">For general Windows information on build 17101 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/14/announcing-windows-10-insider-preview-build-17101-fast-build-17604-skip-ahead/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-526">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-526">WSL</span></span>
* <span data-ttu-id="9e6f0-527">Unterstützung für signalfd.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-527">Support for signalfd.</span></span> <span data-ttu-id="9e6f0-528">[GH 129]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-528">[GH 129]</span></span>
* <span data-ttu-id="9e6f0-529">Unterstützung von Dateinamen, die ungültige NTFS-Zeichen enthalten, durch Codieren als private Unicode-Zeichen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-529">Support file-names containing illegal NTFS characters by encoding them as private Unicode characters.</span></span> <span data-ttu-id="9e6f0-530">[GH 1514]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-530">[GH 1514]</span></span>
* <span data-ttu-id="9e6f0-531">Automatisches Einbinden greift auf den schreibgeschützten Modus zurück, wenn Schreibvorgänge nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-531">Auto mount will fallback to read-only when write is not supported.</span></span> <span data-ttu-id="9e6f0-532">[GH 2603]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-532">[GH 2603]</span></span>
* <span data-ttu-id="9e6f0-533">Ermöglichen des Einfügens von Unicode-Ersatzzeichenpaaren (z.B. Emojis).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-533">Allow pasting of Unicode surrogate pairs (like emoji characters).</span></span> <span data-ttu-id="9e6f0-534">[GH 2765]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-534">[GH 2765]</span></span>
* <span data-ttu-id="9e6f0-535">Pseudodateien in „/proc“ und „/sys“ sollten „read“ und „write ready“ aus select, poll, epoll, usw. zurückgeben [GH 2838].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-535">Pseudo-files in /proc and /sys should return read and write ready from select, poll, epoll, et al. [GH 2838]</span></span>
* <span data-ttu-id="9e6f0-536">Korrektur eines Problems, das dazu führen kann, dass der Dienst in eine Endlosschleife übergeht, wenn die Registrierung manipuliert wurde oder beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-536">Fix issue that could cause service to go into infinite loop when the registry has been tampered with or is corrupt.</span></span>
* <span data-ttu-id="9e6f0-537">Korrektur von Netlink-Nachrichten, sodass sie mit neueren Versionen von iproute2 (upstream 4.14) funktionieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-537">Fix netlink messages to work with newer (upstream 4.14) version of iproute2.</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-538">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-538">Console</span></span>
* <span data-ttu-id="9e6f0-539">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-539">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-540">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-540">LTP Results:</span></span>
<span data-ttu-id="9e6f0-541">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-541">Testing in progress.</span></span>

## <a name="build-17093"></a><span data-ttu-id="9e6f0-542">Build 17093</span><span class="sxs-lookup"><span data-stu-id="9e6f0-542">Build 17093</span></span>
<span data-ttu-id="9e6f0-543">Allgemeine Windows-Informationen zu Build 17093 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-543">For general Windows information on build 17093 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/02/07/announcing-windows-10-insider-preview-build-17093-pc/).</span></span>

#### <a name="important"></a><span data-ttu-id="9e6f0-544">Wichtig:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-544">Important:</span></span>
<span data-ttu-id="9e6f0-545">Wenn Sie WSL zum ersten Mal nach dem Upgrade auf diesen Build starten, müssen Sie einige Aufgaben durchführen, um die Linux-Dateisystemverzeichnisse zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-545">When starting WSL for the first time after upgrading to this build, it needs to perform some work upgrading the Linux file system directories.</span></span> <span data-ttu-id="9e6f0-546">Dieser Vorgang kann einige Minuten in Anspruch nehmen, sodass WSL möglicherweise langsam zu starten scheint.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-546">This may take up to several minutes, so WSL may appear to start slowly.</span></span> <span data-ttu-id="9e6f0-547">Dies sollte nur ein Mal für jede Distribution erfolgen, die Sie aus dem Store installiert haben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-547">This should only happen once for each distribution you have installed from the store.</span></span>
* <span data-ttu-id="9e6f0-548">Verbesserte Unterscheidung von Groß-/Kleinschreibung in DrvFs.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-548">Improved case sensitivity support in DrvFs.</span></span>
    * <span data-ttu-id="9e6f0-549">DrvFs unterstützt jetzt Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-549">DrvFs now supports per-directory case sensitivity.</span></span> <span data-ttu-id="9e6f0-550">Dies ist ein neues Flag, das für Verzeichnisse festgelegt werden kann, um anzugeben, dass alle Vorgänge in diesen Verzeichnissen mit Unterscheidung zwischen Groß-/Kleinschreibung behandelt werden sollen, sodass sogar Windows-Anwendungen Dateien ordnungsgemäß öffnen können, bei denen sich nur die Groß-/Kleinschreibung unterscheidet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-550">This is a new flag that can be set on directories to indicate all operations in those directories should be treated as case sensitive, which allows even Windows applications to correctly open files that differ only by case.</span></span>
    * <span data-ttu-id="9e6f0-551">DrvFs verfügt über neue Einbindungsoptionen, die die Berücksichtigung von Groß-/Kleinschreibung pro Verzeichnis steuern.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-551">DrvFs has new mount options controlling case sensitivity on a per-directory basis</span></span>
        * <span data-ttu-id="9e6f0-552">case=force: Für alle Verzeichnisse wird zwischen Groß-/Kleinschreibung unterschieden (mit Ausnahme des Laufwerkstamms).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-552">case=force: all directories are treated as case sensitive (except for the drive root).</span></span> <span data-ttu-id="9e6f0-553">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-553">New directories created with WSL are marked as case sensitive.</span></span> <span data-ttu-id="9e6f0-554">Dies ist das Legacyverhalten (ausgenommen, wenn neue Verzeichnisse für Unterscheidung zwischen Groß-/Kleinschreibung markiert werden).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-554">This is the legacy behavior except for marking new directories case sensitive.</span></span>
        * <span data-ttu-id="9e6f0-555">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-555">case=dir: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="9e6f0-556">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-556">New directories created with WSL are marked as case sensitive.</span></span>
        * <span data-ttu-id="9e6f0-557">case=dir: Nur für Verzeichnisse mit dem Flag für Unterscheidung zwischen Groß-/Kleinschreibung pro Verzeichnis wird Groß-/Kleinschreibung beachtet, für alle anderen Verzeichnisse nicht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-557">case=off: only directories with the per-directory case sensitivity flag are treated as case sensitive; other directories are case insensitive.</span></span> <span data-ttu-id="9e6f0-558">Für neue Verzeichnisse, die mit WSL erstellt werden, wird Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-558">New directories created with WSL are marked as case insensitive.</span></span>
    * <span data-ttu-id="9e6f0-559">Hinweis: Für Verzeichnisse, die in früheren Versionen von WSL erstellt wurden, ist dieses Flag nicht festgelegt, sodass bei Verwendung der Option „case=dir“ keine Groß-/Kleinschreibung beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-559">Note: directories created by WSL in previous releases do not have this flag set, so will not be treated as case sensitive if you use the “case=dir” option.</span></span> <span data-ttu-id="9e6f0-560">Eine Möglichkeit, dieses Flag für vorhandene Verzeichnisse festzulegen, ist in Kürze verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-560">A way to set this flag on existing directories is coming soon.</span></span>
    * <span data-ttu-id="9e6f0-561">Beispiel für die Einbindung mit diesen Optionen (für vorhandene Laufwerke müssen Sie zuerst die Einbindung aufheben, bevor Sie die Einbindung mit anderen Optionen ausführen können): sudo mount -t drvfs C: /mnt/c -o case=dir</span><span class="sxs-lookup"><span data-stu-id="9e6f0-561">Example of mounting with these options (for existing drives, you must first unmount before you can mount with different options): sudo mount -t drvfs C: /mnt/c -o case=dir</span></span>
    * <span data-ttu-id="9e6f0-562">Momentan ist case=force immer noch die Standardoption.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-562">For now, case=force is still the default option.</span></span> <span data-ttu-id="9e6f0-563">Dies wird in Zukunft in case=dir geändert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-563">This will be changed to case=dir in the future.</span></span>
* <span data-ttu-id="9e6f0-564">Sie können jetzt Schrägstriche in Windows-Pfaden verwenden, wenn Sie DrvFs einbinden, z.B. sudo mount -t drvfs //server/share /mnt/share</span><span class="sxs-lookup"><span data-stu-id="9e6f0-564">You can now use forward slashes in Windows paths when mounting DrvFs, e.g.: sudo mount -t drvfs //server/share /mnt/share</span></span>
* <span data-ttu-id="9e6f0-565">WSL verarbeitet nun die /etc/fstab-Datei während des Instanzstarts [GH 2636].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-565">WSL now processes the /etc/fstab file during instance start [GH 2636].</span></span>
    * <span data-ttu-id="9e6f0-566">Dies erfolgt vor der automatischen Einbindung von DrvFs-Laufwerken. Alle Laufwerke, die bereits von fstab eingebunden wurden, werden nicht automatisch erneut eingebunden, sodass Sie den Einbindungspunkt für bestimmte Laufwerke ändern können.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-566">This is done prior to automatically mounting DrvFs drives; any drives that were already mounted by fstab will not be remounted automatically, allowing you to change the mount point for specific drives.</span></span>
    * <span data-ttu-id="9e6f0-567">Dieses Verhalten kann mithilfe von „wsl.conf“ deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-567">This behavior can be turned off using wsl.conf.</span></span>
* <span data-ttu-id="9e6f0-568">Die mount, mountinfo- und mountstats-Dateien in „/proc“ versehen Sonderzeichen wie umgekehrte Schrägstriche und Leerzeichen ordnungsgemäß mit Escapezeichen [GH 2799]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-568">The mount, mountinfo and mountstats files in /proc properly escape special characters like backslashes and spaces [GH 2799]</span></span>
* <span data-ttu-id="9e6f0-569">Spezielle Dateien, die mit DrvFs erstellt werden (z.B. symbolische WSL-Verknüpfungen oder Fifos und Sockets, wenn Metadaten aktiviert sind), können nun aus Windows kopiert und verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-569">Special files created with DrvFs such as WSL symbolic links, or fifos and sockets when metadata is enabled, can now be copied and moved from Windows.</span></span>

#### <a name="wsl-is-more-configurable-with-wslconf"></a><span data-ttu-id="9e6f0-570">WSL ist mit „wsl.conf“ besser konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-570">WSL is more configurable with wsl.conf</span></span>
<span data-ttu-id="9e6f0-571">Es wurde eine Methode zum automatischen Konfigurieren bestimmter Funktionen in WSL hinzugefügt, die jedes Mal angewendet wird, wenn Sie das Subsystem starten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-571">We added a method for you to automatically configure certain functionality in WSL that will be applied every time you launch the subsystem.</span></span> <span data-ttu-id="9e6f0-572">Dies umfasst Optionen für die automatische Einbindung und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-572">This includes automount options and network configuration.</span></span> <span data-ttu-id="9e6f0-573">Weitere Informationen hierzu finden Sie in unserem Blogbeitrag unter: https://aka.ms/wslconf</span><span class="sxs-lookup"><span data-stu-id="9e6f0-573">Learn more about it in our blog post at: https://aka.ms/wslconf</span></span>

#### <a name="af_unix-allows-socket-connections-between-linux-processes-on-wsl-and-windows-native-processes"></a><span data-ttu-id="9e6f0-574">AF_UNIX ermöglicht Socketverbindungen zwischen Linux-Prozessen für WSL- und native Windows-Prozesse.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-574">AF_UNIX allows socket connections between Linux processes on WSL and Windows native processes</span></span>
<span data-ttu-id="9e6f0-575">WSL- und Windows-Anwendungen können nun über Unix-Sockets miteinander kommunizieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-575">WSL and Windows applications can now communicate with each other over Unix sockets.</span></span> <span data-ttu-id="9e6f0-576">Stellen Sie sich vor, Sie möchten einen Dienst in Windows ausführen und sowohl für Windows- als auch für WSL-Apps verfügbar machen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-576">Imagine you want to run a service in Windows and make it available to both Windows and WSL apps.</span></span> <span data-ttu-id="9e6f0-577">Das ist nun mit UNIX-Sockets möglich.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-577">Now, that’s possible with Unix sockets.</span></span> <span data-ttu-id="9e6f0-578">Weitere Informationen finden Sie in unserem Blogbeitrag unter https://aka.ms/afunixinterop.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-578">Read more in our blog post at https://aka.ms/afunixinterop</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-579">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-579">WSL</span></span>
* <span data-ttu-id="9e6f0-580">Unterstützung von mmap() mit MAP_NORESERVE [GH 121, 2784]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-580">Support mmap() with MAP_NORESERVE [GH 121, 2784]</span></span>
* <span data-ttu-id="9e6f0-581">Unterstützung von CLONE_PTRACE und CLONE_UNTRACED [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-581">Support CLONE_PTRACE and CLONE_UNTRACED [GH 121, 2781]</span></span>
* <span data-ttu-id="9e6f0-582">Verarbeiten eines Nicht-SIGCHLD-Beendigungssignals im Klon [GH 121, 2781]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-582">Handle non-SIGCHLD termination signal in clone [GH 121, 2781]</span></span>
* <span data-ttu-id="9e6f0-583">Stub für /proc/sys/fs/inotify/max_user_instances und /proc/sys/fs/inotify/max_user_watches [GH 1705]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-583">Stub /proc/sys/fs/inotify/max_user_instances and /proc/sys/fs/inotify/max_user_watches [GH 1705]</span></span>
* <span data-ttu-id="9e6f0-584">Fehler beim Laden von ELF-Binärdateien, die Ladeheader mit Offsets ungleich NULL enthalten [GH 1884]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-584">Error loading ELF binaries that contain load headers with non-zero offsets [GH 1884]</span></span>
* <span data-ttu-id="9e6f0-585">Eliminieren von nachfolgenden Seitenbytes beim Laden von Images.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-585">Zero out trailing page bytes when loading images.</span></span>
* <span data-ttu-id="9e6f0-586">Verringern der Fälle, in denen execve den Prozess automatisch beendet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-586">Reduce cases where execve silently terminates process</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-587">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-587">Console</span></span>
* <span data-ttu-id="9e6f0-588">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-588">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-589">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-589">LTP Results:</span></span>
<span data-ttu-id="9e6f0-590">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-590">Testing in progress.</span></span>

## <a name="build-17083"></a><span data-ttu-id="9e6f0-591">Build 17083</span><span class="sxs-lookup"><span data-stu-id="9e6f0-591">Build 17083</span></span>
<span data-ttu-id="9e6f0-592">Allgemeine Windows-Informationen zu Build 17083 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-592">For general Windows information on build 17083 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/24/announcing-windows-10-insider-preview-build-17083-for-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-593">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-593">WSL</span></span>
* <span data-ttu-id="9e6f0-594">Korrektur der Fehlerüberprüfung für epoll [GH 2798, 2801, 2857]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-594">Fixed bugcheck related to epoll [GH 2798, 2801, 2857]</span></span>
* <span data-ttu-id="9e6f0-595">Korrektur von Hängern beim Deaktivieren von ASLR [GH 1185, 2870]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-595">Fixed hangs when turning off ASLR [GH 1185, 2870]</span></span>
* <span data-ttu-id="9e6f0-596">Sicherstellen, dass mmap-Vorgänge atomarisch erscheinen [GH 2732]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-596">Ensure mmap operations appear atomic [GH 2732]</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-597">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-597">Console</span></span>
* <span data-ttu-id="9e6f0-598">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-598">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-599">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-599">LTP Results:</span></span>
<span data-ttu-id="9e6f0-600">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-600">Testing in progress.</span></span>

## <a name="build-17074"></a><span data-ttu-id="9e6f0-601">Build 17074</span><span class="sxs-lookup"><span data-stu-id="9e6f0-601">Build 17074</span></span>
<span data-ttu-id="9e6f0-602">Allgemeine Windows-Informationen zu Build 17074 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-602">For general Windows information on build 17074 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2018/01/11/announcing-windows-10-insider-preview-build-17074-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-603">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-603">WSL</span></span>
* <span data-ttu-id="9e6f0-604">Festes Speicherformat von DrvFs-Metadaten [GH 2777]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-604">Fixed storage format of DrvFs metadata [GH 2777]</span></span> </br>
<span data-ttu-id="9e6f0-605">**Wichtig:** Die vor diesem Build erstellten DrvFs-Metadaten werden falsch oder überhaupt nicht angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-605">**Important:** DrvFs metadata created before this build will show up incorrectly or not at all.</span></span> <span data-ttu-id="9e6f0-606">Um betroffene Dateien zu korrigieren, verwenden Sie chmod und chown zum erneuten Anwenden der Metadaten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-606">To fix affected files, use chmod and chown to re-apply the metadata.</span></span>
* <span data-ttu-id="9e6f0-607">Korrektur eines Problems mit mehreren Signalen und neu startbaren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-607">Fixed issue with multiple signals and restartable syscalls.</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-608">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-608">Console</span></span>
* <span data-ttu-id="9e6f0-609">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-609">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-610">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-610">LTP Results:</span></span>
<span data-ttu-id="9e6f0-611">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-611">Testing in progress.</span></span>

## <a name="build-17063"></a><span data-ttu-id="9e6f0-612">Build 17063</span><span class="sxs-lookup"><span data-stu-id="9e6f0-612">Build 17063</span></span>
<span data-ttu-id="9e6f0-613">Allgemeine Windows-Informationen zu Build 17063 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-613">For general Windows information on build 17063 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/12/19/announcing-windows-10-insider-preview-build-17063-pc/).</span></span>

### <a name="wsl"></a><span data-ttu-id="9e6f0-614">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-614">WSL</span></span>
* <span data-ttu-id="9e6f0-615">DrvFs unterstützt zusätzliche Linux-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-615">DrvFs supports additional Linux metadata.</span></span> <span data-ttu-id="9e6f0-616">Dies ermöglicht das Festlegen des Besitzers und des Dateimodus mit chmod/chown sowie das Erstellen spezieller Dateien, etwa Fifos, Unix-Sockets und Gerätedateien.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-616">This allows setting the owner and mode of files using chmod/chown, and also the creation of special files such as fifos, unix sockets and device files.</span></span> <span data-ttu-id="9e6f0-617">Diese Option ist zurzeit standardmäßig deaktiviert, da Sie noch experimentell ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-617">This is disabled by default for now since it's still experimental.</span></span>
<span data-ttu-id="9e6f0-618">**Hinweis:**  Wir haben einen Fehler im Metadatenformat behoben, das von DrvFs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-618">**Note:**  We fixed a bug in the metadata format used by DrvFs.</span></span> <span data-ttu-id="9e6f0-619">Obwohl Metadaten in diesem Build für Experimente funktionieren, lesen zukünftige Builds die von diesem Build erstellten Metadaten nicht ordnungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-619">While metadata works on this build for experimentation, future builds will not correctly read metadata created by this build.</span></span>  <span data-ttu-id="9e6f0-620">Möglicherweise müssen Sie den Besitzer für geänderte Dateien manuell aktualisieren, und Geräte mit einer benutzerdefinierten Geräte-ID müssen neu erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-620">You might need to manually update owner for modified files and devices with a custom device ID will have to be recreated.</span></span>

  <span data-ttu-id="9e6f0-621">Um diese Funktion zu aktivieren, binden Sie DrvFs mit der Metadatenoption ein (um sie für eine vorhandene Einbindung zu aktivieren, müssen Sie die Einbindung zunächst aufheben):</span><span class="sxs-lookup"><span data-stu-id="9e6f0-621">To enable, mount DrvFs with the metadata option (to enable it on an existing mount, you must first unmount it):</span></span>

  ```bash
  mount -t drvfs C: /mnt/c -o metadata
  ```

  <span data-ttu-id="9e6f0-622">Linux-Berechtigungen werden der Datei als zusätzliche Metadaten hinzugefügt. Sie wirken sich nicht auf die Windows-Berechtigungen aus.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-622">Linux permissions are added as additional metadata to the file; they do not affect the Windows permissions.</span></span>  <span data-ttu-id="9e6f0-623">Beachten Sie, dass beim Bearbeiten einer Datei mithilfe eines Windows-Editors die Metadaten möglicherweise entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-623">Remember, editing a file using a Windows editor may remove the metadata.</span></span> <span data-ttu-id="9e6f0-624">In diesem Fall wird die Datei auf die Standardberechtigungen zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-624">In this case, the file will revert to its default permissions.</span></span>

* <span data-ttu-id="9e6f0-625">Hinzufügen von Einbindungsoptionen zu DrvFs, um Dateien ohne Metadaten zu steuern.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-625">Added mount options to DrvFs to control files without metadata.</span></span>
  * <span data-ttu-id="9e6f0-626">uid: die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-626">uid: the user ID used for the owner of all files.</span></span>
  * <span data-ttu-id="9e6f0-627">gid: die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-627">gid: the group ID used for the owner of all files.</span></span>
  * <span data-ttu-id="9e6f0-628">umask: Eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-628">umask: an octal mask of permissions to exclude for all files and directories.</span></span>
  * <span data-ttu-id="9e6f0-629">fmask: Eine oktale Maske mit Berechtigungen, die für alle regulären Dateien ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-629">fmask: an octal mask of permissions to exclude for all regular files.</span></span>
  * <span data-ttu-id="9e6f0-630">dmask: Eine oktale Maske mit Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-630">dmask: an octal mask of permissions to exclude for all directories.</span></span>

  <span data-ttu-id="9e6f0-631">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-631">For example:</span></span>
  ```
  mount -t drvfs C: /mnt/c -o uid=1000,gid=1000,umask=22,fmask=111
  ```

  <span data-ttu-id="9e6f0-632">Kombinieren Sie dies mit der Metadatenoption, um Standardberechtigungen für Dateien ohne Metadaten anzugeben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-632">Combine with the metadata option to specify default permissions for files without metadata.</span></span>

* <span data-ttu-id="9e6f0-633">Wird in einer neuen Umgebungsvariablen (`WSLENV`) eingeführt, um zu konfigurieren, wie Umgebungsvariablen zwischen WSL und Win32 ausgetauscht werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-633">Introduced a new environment variable, `WSLENV`, to configure how environment variables flow between WSL and Win32.</span></span>

  <span data-ttu-id="9e6f0-634">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-634">For example:</span></span>

  ``` bash
  WSLENV=GOPATH/l:USERPROFILE/pu:DISPLAY
  ```

  <span data-ttu-id="9e6f0-635">`WSLENV` eine durch Doppelpunkte getrennte Liste von Umgebungsvariablen, die beim Starten von WSL-Prozessen aus Win32 oder Win32-Prozessen aus WSL eingeschlossen werden können.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-635">`WSLENV` is a colon-delimited list of environment variables that can be included when launching WSL processes from Win32 or Win32 processes from WSL.</span></span>  <span data-ttu-id="9e6f0-636">Jeder Variablen kann ein Schrägstrich als Suffix vorangestellt werden, gefolgt von Flags, um anzugeben, wie sie übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-636">Each variable can be suffixed with a slash followed by flags to specify how it is translated.</span></span>
  * <span data-ttu-id="9e6f0-637">p: Der Wert ist ein Pfad, der zwischen WSL-Pfaden und Win32-Pfaden übersetzt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-637">p: The value is a path that should be translated between WSL paths and Win32 paths.</span></span>
  * <span data-ttu-id="9e6f0-638">l: Der Wert ist eine Liste von Pfaden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-638">l: The value is a list of paths.</span></span> <span data-ttu-id="9e6f0-639">In WSL ist es eine durch Doppelpunkte getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-639">In WSL, it is a colon-delimited list.</span></span> <span data-ttu-id="9e6f0-640">In Win32 ist es eine durch Semikolons getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-640">In Win32, it is a semicolon-delimited list.</span></span>
  * <span data-ttu-id="9e6f0-641">u: Der Wert sollte nur beim Aufrufen von WSL aus Win32 eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-641">u: The value should only be included when invoking WSL from Win32</span></span>
  * <span data-ttu-id="9e6f0-642">w: Der Wert sollte nur beim Aufrufen von Win32 aus WSL eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-642">w: The value should only be included when invoking Win32 from WSL</span></span>

  <span data-ttu-id="9e6f0-643">Sie können `WSLENV` in der BASHRC-Datei oder in der benutzerdefinierten Windows-Umgebung für Ihren Benutzer festlegen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-643">You can set `WSLENV` in .bashrc or in the custom Windows environment for your user.</span></span>

* <span data-ttu-id="9e6f0-644">drvfs wird ordnungsgemäß eingebunden und behält Zeitstempel aus from tar, cp -p bei (GH 1939)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-644">drvfs mounts correctly preserves timestamps from tar, cp -p (GH 1939)</span></span>
* <span data-ttu-id="9e6f0-645">Symbolische drvfs-Verknüpfungen geben die richtige Größe an (GH 2641)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-645">drvfs symlinks report the correct size (GH 2641)</span></span>
* <span data-ttu-id="9e6f0-646">Lese-/Schreibvorgänge funktionieren für sehr große E/A-Größen (GH 2653)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-646">read/write works for very large IO sizes (GH 2653)</span></span>
* <span data-ttu-id="9e6f0-647">waitpid funktioniert mit Prozessgruppen-IDs (GH 2534)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-647">waitpid works with process group IDs (GH 2534)</span></span>
* <span data-ttu-id="9e6f0-648">Erheblich verbesserte mmap-Leistung für große reserve-Regionen, Verbesserung der ghc-Leistung (GH 1671)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-648">significantly improved mmap performance for large reserve regions; improves ghc performance (GH 1671)</span></span>
* <span data-ttu-id="9e6f0-649">personality unterstützt READ_IMPLIES_EXEC, Korrekturen maxima und clisp (GH 1185)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-649">personality supports for READ_IMPLIES_EXEC; fixes maxima and clisp (GH 1185)</span></span>
* <span data-ttu-id="9e6f0-650">mprotect unterstützt PROT_GROWSDOWN,;Korrekturen clisp (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-650">mprotect supports PROT_GROWSDOWN; fixes clisp (GH 1128)</span></span>
* <span data-ttu-id="9e6f0-651">Seitenfehlerkorrekturen im Overcommitmodus, Korrekturen sbcl (GH 1128)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-651">page fault fixes in overcommit mode; fixes sbcl (GH 1128)</span></span>
* <span data-ttu-id="9e6f0-652">clone unterstützt weitere Flagkombinationen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-652">clone supports more flags combinations</span></span>
* <span data-ttu-id="9e6f0-653">Unterstützung von select/epoll von epoll-Dateien (zuvor eine Nulloperation).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-653">Support select/epoll of epoll files (previously a no-op).</span></span>
* <span data-ttu-id="9e6f0-654">Benachrichtigen von ptrace über nicht implementierte Systemaufrufe.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-654">Notify ptrace of unimplemented syscalls.</span></span>
* <span data-ttu-id="9e6f0-655">Ignorieren von Schnittstellen, die nicht aktiv sind, beim Generieren von resolv.conf-Namenservern [GH 2694]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-655">Ignore interfaces that are not up when generating resolv.conf nameservers [GH 2694]</span></span>
* <span data-ttu-id="9e6f0-656">Aufzählen von Netzwerkschnittstellen ohne physische Adresse.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-656">Enumerate network interfaces with no physical address.</span></span> <span data-ttu-id="9e6f0-657">[GH 2685]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-657">[GH 2685]</span></span>
* <span data-ttu-id="9e6f0-658">Zusätzliche Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-658">Additional bug fixes and improvements.</span></span>

### <a name="linux-tools-available-to-developers-on-windows"></a><span data-ttu-id="9e6f0-659">Linux-Tools für Entwickler unter Windows verfügbar</span><span class="sxs-lookup"><span data-stu-id="9e6f0-659">Linux tools available to developers on Windows</span></span>

* <span data-ttu-id="9e6f0-660">Windows-Befehlszeilen-Toolkette enthält bsdtar (tar) und curl.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-660">Windows Command line Toolchain includes bsdtar (tar) and curl.</span></span>
  <span data-ttu-id="9e6f0-661">Lesen Sie [diesen Blog](https://aka.ms/tarcurlwindows), um mehr über das Hinzufügen dieser beiden neuen Tools zu erfahren, und sehen Sie, wie Sie das Entwicklererlebnis unter Windows formen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-661">Read [this blog](https://aka.ms/tarcurlwindows) to learn more about the addition of these two new tools and see how they’re shaping the developer experience on Windows.</span></span>

*   <span data-ttu-id="9e6f0-662">`AF_UNIX` ist im Windows Insider SDK (17061 und höher) verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-662">`AF_UNIX` is available in the Windows Insider SDK (17061+).</span></span>
  <span data-ttu-id="9e6f0-663">Lesen Sie [diesen Blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/), um weitere Informationen zu `AF_UNIX` zu erhalten und mehr über die Verwendung in Windows durch Entwickler zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-663">Read [this blog](https://blogs.msdn.microsoft.com/commandline/2017/12/19/af_unix-comes-to-windows/) to learn more about `AF_UNIX` and how developers on Windows can use it.</span></span>

### <a name="console"></a><span data-ttu-id="9e6f0-664">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-664">Console</span></span>
* <span data-ttu-id="9e6f0-665">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-665">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-666">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-666">LTP Results:</span></span>
<span data-ttu-id="9e6f0-667">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-667">Testing in progress.</span></span>


## <a name="build-17046"></a><span data-ttu-id="9e6f0-668">Build 17046</span><span class="sxs-lookup"><span data-stu-id="9e6f0-668">Build 17046</span></span>

<span data-ttu-id="9e6f0-669">Allgemeine Windows-Informationen zu Build 17046 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-669">For general Windows information on build 17046 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/22/announcing-windows-10-insider-preview-build-17046-pc).</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-670">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-670">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-671">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-671">WSL</span></span>
- <span data-ttu-id="9e6f0-672">Ermöglicht das Ausführen von Prozessen ohne ein aktives Terminal.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-672">Allow processes to run without an active terminal.</span></span> <span data-ttu-id="9e6f0-673">[GH 709, 1007, 1511, 2252, 2391 usw.]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-673">[GH 709, 1007, 1511, 2252, 2391, et al.]</span></span>
- <span data-ttu-id="9e6f0-674">Bessere Unterstützung von CLONE_VFORK und CLONE_VM.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-674">Better support of CLONE_VFORK and CLONE_VM.</span></span> <span data-ttu-id="9e6f0-675">[GH 1878, 2615]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-675">[GH 1878, 2615]</span></span>
- <span data-ttu-id="9e6f0-676">Überspringen der TDI-Filtertreiber für WSL-Netzwerkvorgänge.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-676">Skip TDI filter drivers for WSL networking operations.</span></span> <span data-ttu-id="9e6f0-677">[GH 1554]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-677">[GH 1554]</span></span>
- <span data-ttu-id="9e6f0-678">DrvFs erstellt symbolische NT-Verknüpfungen, wenn bestimmte Bedingungen erfüllt sind.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-678">DrvFs creates NT symlinks when certain conditions are met.</span></span> <span data-ttu-id="9e6f0-679">[GH 353, 1475, 2602]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-679">[GH 353, 1475, 2602]</span></span>
    - <span data-ttu-id="9e6f0-680">Das Verknüpfungsziel muss relativ sein, darf keine Einbindungspunkte oder symbolische Verknüpfungen kreuzen und muss vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-680">The link target must be relative, must not cross any mount points or symlinks, and must exist.</span></span>
    - <span data-ttu-id="9e6f0-681">Der Benutzer muss über SE_CREATE_SYMBOLIC_LINK_PRIVILEGE verfügen (dies erfordert normalerweise, dass Sie „wsl.exe“ mit erhöhten Rechten starten), sofern der Entwicklermodus nicht aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-681">The user must have SE_CREATE_SYMBOLIC_LINK_PRIVILEGE (this normally requires you to launch wsl.exe elevated), unless Developer Mode is turned on.</span></span>
    - <span data-ttu-id="9e6f0-682">Unter allen anderen Umständen erstellt DrvFs weiterhin symbolische WSL-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-682">In all other situations, DrvFs still creates WSL symlinks.</span></span>
- <span data-ttu-id="9e6f0-683">Ermöglichen der gleichzeitigen Ausführung von WSL-Instanzen mit und ohne erhöhten Rechten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-683">Allow running elevated and non-elevated WSL instances simultaneously.</span></span>
- <span data-ttu-id="9e6f0-684">Unterstützung von /proc/sys/kernel/Yama/ptrace_scope</span><span class="sxs-lookup"><span data-stu-id="9e6f0-684">Support /proc/sys/kernel/yama/ptrace_scope</span></span>
- <span data-ttu-id="9e6f0-685">Hinzufügen von wslpath zum Durchführen von Konvertierungen von WSL-<- >Windows-Pfaden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-685">Add wslpath to do WSL<->Windows path conversions.</span></span> <span data-ttu-id="9e6f0-686">[GH 522, 1243, 1834, 2327 usw.]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-686">[GH 522, 1243, 1834, 2327, et al.]</span></span>
  ```
    wslpath usage:
      -a    force result to absolute path format
      -u    translate from a Windows path to a WSL path (default)
      -w    translate from a WSL path to a Windows path
      -m    translate from a WSL path to a Windows path, with ‘/’ instead of ‘\\’

      EX: wslpath ‘c:\users’
  ```
  #### <a name="console"></a><span data-ttu-id="9e6f0-687">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-687">Console</span></span>
- <span data-ttu-id="9e6f0-688">Keine Korrekturen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-688">No fixes.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-689">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-689">LTP Results:</span></span>
<span data-ttu-id="9e6f0-690">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-690">Testing in progress.</span></span>


## <a name="build-17040"></a><span data-ttu-id="9e6f0-691">Build 17040</span><span class="sxs-lookup"><span data-stu-id="9e6f0-691">Build 17040</span></span>

<span data-ttu-id="9e6f0-692">Allgemeine Windows-Informationen zu Build 17040 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-692">For general Windows information on build 17040 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/16/announcing-windows-10-insider-preview-build-17040-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-693">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-693">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-694">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-694">WSL</span></span>
- <span data-ttu-id="9e6f0-695">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-695">No fixes since 17035.</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-696">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-696">Console</span></span>
- <span data-ttu-id="9e6f0-697">Keine Korrekturen seit 17035.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-697">No fixes since 17035.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-698">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-698">LTP Results:</span></span>
<span data-ttu-id="9e6f0-699">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-699">Testing in progress.</span></span>

## <a name="build-17035"></a><span data-ttu-id="9e6f0-700">Build 17035</span><span class="sxs-lookup"><span data-stu-id="9e6f0-700">Build 17035</span></span>

<span data-ttu-id="9e6f0-701">Allgemeine Windows-Informationen zu Build 17035 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-701">For general Windows information on build 17035 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/11/08/announcing-windows-10-insider-preview-build-17035-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-702">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-702">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-703">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-703">WSL</span></span>
- <span data-ttu-id="9e6f0-704">Der Zugriff auf Dateien auf DrvFs kann gelegentlich mit EINVAL fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-704">Accessing files on DrvFs could occasionally fail with EINVAL.</span></span> <span data-ttu-id="9e6f0-705">[GH 2448]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-705">[GH 2448]</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-706">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-706">Console</span></span>
- <span data-ttu-id="9e6f0-707">Farbverlust beim Einfügen/Löschen von Zeilen im VT-Modus.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-707">Some color loss when inserting/deleting lines in VT mode.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-708">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-708">LTP Results:</span></span>
<span data-ttu-id="9e6f0-709">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-709">Testing in progress.</span></span>

## <a name="build-17025"></a><span data-ttu-id="9e6f0-710">Build 17025</span><span class="sxs-lookup"><span data-stu-id="9e6f0-710">Build 17025</span></span>

<span data-ttu-id="9e6f0-711">Allgemeine Windows-Informationen zu Build 17025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-711">For general Windows information on build 17025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/25/announcing-windows-10-insider-preview-build-17025-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-712">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-712">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-713">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-713">WSL</span></span>
- <span data-ttu-id="9e6f0-714">Starten anfänglicher Prozesse in einer neuen Vordergrundprozessgruppe [GH 1653, 2510].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-714">Start initial processes in a new foreground process group [GH 1653, 2510].</span></span>
- <span data-ttu-id="9e6f0-715">Korrekturen der SIGHUP-Übermittlung [GH 2496].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-715">SIGHUP delivery fixes [GH 2496].</span></span>
- <span data-ttu-id="9e6f0-716">Generieren eines Standardnamens für virtuelle Bridge generieren, wenn keine Angabe erfolgt [GH 2497].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-716">Generate default virtual bridge name if none provided [GH 2497].</span></span>
- <span data-ttu-id="9e6f0-717">Implementieren von /proc/sys/kernel/Random/boot_id [GH 2518].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-717">Implement /proc/sys/kernel/random/boot_id [GH 2518].</span></span>
- <span data-ttu-id="9e6f0-718">Weitere Interop-Pipekorrekturen für stdout/stderr.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-718">More interop stdout/stderr pipe fixes.</span></span>
- <span data-ttu-id="9e6f0-719">Stub für syncfs-Systemaufruf.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-719">Stub syncfs system call.</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-720">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-720">Console</span></span>
- <span data-ttu-id="9e6f0-721">Korrektur der VT-Eingabeübersetzung für Drittanbieterkonsolen [GH 111]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-721">Fix input VT translation for third party consoles [GH 111]</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-722">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-722">LTP Results:</span></span>
<span data-ttu-id="9e6f0-723">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-723">Testing in progress.</span></span>

## <a name="build-17017"></a><span data-ttu-id="9e6f0-724">Build 17017</span><span class="sxs-lookup"><span data-stu-id="9e6f0-724">Build 17017</span></span>

<span data-ttu-id="9e6f0-725">Allgemeine Windows-Informationen zu Build 17017 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-725">For general Windows information on build 17017 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/10/13/announcing-windows-10-insider-preview-build-17017-pc).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-726">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-726">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-727">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-727">WSL</span></span>
- <span data-ttu-id="9e6f0-728">Ignorieren leerer ELF-Programmheader [GH 330].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-728">Ignore empty ELF program headers [GH 330].</span></span>
- <span data-ttu-id="9e6f0-729">Ermöglichen, dass LxssManager WSL-Instanzen für nicht interaktive Benutzer erstellt (Unterstützung für SSH und geplante Aufgaben) [GH 777, 1602].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-729">Allow LxssManager to create WSL instances for non-interactive users (ssh and scheduled task support) [GH 777, 1602].</span></span>
- <span data-ttu-id="9e6f0-730">Unterstützung von WSL->Win32->WSL-Szenarien („Inception“) [GH 1228].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-730">Support WSL->Win32->WSL ("inception") scenarios [GH 1228].</span></span>
- <span data-ttu-id="9e6f0-731">Eingeschränkte Unterstützung für das Beenden von Konsolen-Apps, die über Interop aufgerufen wurden [GH 1614].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-731">Limited support for termination of console apps invoked via interop [GH 1614].</span></span>
- <span data-ttu-id="9e6f0-732">Unterstützung von Einbindungsoptionen für devpts [GH 1948].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-732">Support mount options for devpts [GH 1948].</span></span>
- <span data-ttu-id="9e6f0-733">Ptrace blockiert den Start untergeordneter Prozesse [GH 2333].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-733">Ptrace blocking child startup [GH 2333].</span></span>
- <span data-ttu-id="9e6f0-734">EPOLLET fehlen einige Ereignisse [GH 2462].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-734">EPOLLET missing some events [GH 2462].</span></span>
- <span data-ttu-id="9e6f0-735">Rückgabe einer größeren Anzahl von Daten für PTRACE_GETSIGINFO.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-735">Return more data for PTRACE_GETSIGINFO.</span></span>
- <span data-ttu-id="9e6f0-736">Getdents mit lseek liefert falsche Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-736">Getdents with lseek gives incorrect results.</span></span>
- <span data-ttu-id="9e6f0-737">Korrektur einiger Hänger von Win32-Interop-Apps, die auf Eingaben in einer Pipe warten, die keine weiteren Daten enthält.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-737">Fix some Win32 interop app hangs, waiting for input on a pipe that has no more data.</span></span>
- <span data-ttu-id="9e6f0-738">O_ASYNC-Unterstützung für tty/pty-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-738">O_ASYNC support for tty/pty files.</span></span>
- <span data-ttu-id="9e6f0-739">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-739">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-740">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-740">Console</span></span>
- <span data-ttu-id="9e6f0-741">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-741">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-742">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-742">LTP Results:</span></span>
<span data-ttu-id="9e6f0-743">Tests werden zurzeit ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-743">Testing in progress.</span></span>

## <a name="fall-creators-update"></a><span data-ttu-id="9e6f0-744">Fall Creators Update</span><span class="sxs-lookup"><span data-stu-id="9e6f0-744">Fall Creators Update</span></span>

## <a name="build-16288"></a><span data-ttu-id="9e6f0-745">Build 16288</span><span class="sxs-lookup"><span data-stu-id="9e6f0-745">Build 16288</span></span>

<span data-ttu-id="9e6f0-746">Allgemeine Windows-Informationen zu Build 16288 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-746">For general Windows information on build 16288 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/09/12/announcing-windows-10-insider-preview-build-16288-pc-build-15250-mobile/#7pLWQbj23JisfzV5.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-747">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-747">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-748">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-748">WSL</span></span>
- <span data-ttu-id="9e6f0-749">Ordnungsgemäße Initialisierung und Meldung von uid, gid und Modus für Socketdateideskriptoren [GH 2490]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-749">Correctly initialize and report uid, gid, and mode for socket file descriptors [GH 2490]</span></span>
- <span data-ttu-id="9e6f0-750">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-750">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-751">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-751">Console</span></span>
- <span data-ttu-id="9e6f0-752">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-752">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-753">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-753">LTP Results:</span></span>
<span data-ttu-id="9e6f0-754">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9e6f0-754">No change since 16273</span></span>

## <a name="build-16278"></a><span data-ttu-id="9e6f0-755">Build 16278</span><span class="sxs-lookup"><span data-stu-id="9e6f0-755">Build 16278</span></span>

<span data-ttu-id="9e6f0-756">Allgemeine Windows-Informationen zu Build 162738 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-756">For general Windows information on build 162738 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/29/announcing-windows-10-insider-preview-build-16278-pc/#HMz6Xq7Su68WKi0t.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-757">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-757">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-758">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-758">WSL</span></span>
- <span data-ttu-id="9e6f0-759">Explizite Aufhebung der Zuordnung zugeordneter Ansichten von dateigestützten Abschnitten beim Beenden des LX MM-Status [GH 2415]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-759">Explicitly unmap mapped views of file backed sections when tearing down LX MM state [GH 2415]</span></span>
- <span data-ttu-id="9e6f0-760">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-760">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-761">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-761">Console</span></span>
- <span data-ttu-id="9e6f0-762">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-762">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-763">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-763">LTP Results:</span></span>
<span data-ttu-id="9e6f0-764">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9e6f0-764">No change since 16273</span></span>

## <a name="build-16275"></a><span data-ttu-id="9e6f0-765">Build 16275</span><span class="sxs-lookup"><span data-stu-id="9e6f0-765">Build 16275</span></span>

<span data-ttu-id="9e6f0-766">Allgemeine Windows-Informationen zu Build 162735 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-766">For general Windows information on build 162735 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/25/announcing-windows-10-insider-preview-build-16275-pc-build-15245-mobile/#8QkxWqQbY37yZslV.97/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-767">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-767">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-768">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-768">WSL</span></span>
- <span data-ttu-id="9e6f0-769">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-769">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-770">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-770">Console</span></span>
- <span data-ttu-id="9e6f0-771">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-771">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-772">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-772">LTP Results:</span></span>
<span data-ttu-id="9e6f0-773">Keine Änderung seit 16273</span><span class="sxs-lookup"><span data-stu-id="9e6f0-773">No change since 16273</span></span>

## <a name="build-16273"></a><span data-ttu-id="9e6f0-774">Build 16273</span><span class="sxs-lookup"><span data-stu-id="9e6f0-774">Build 16273</span></span>

<span data-ttu-id="9e6f0-775">Allgemeine Windows-Informationen zu Build 16273 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-775">For general Windows information on build 16273 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/23/announcing-windows-10-insider-preview-build-16273-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-776">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-776">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-777">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-777">WSL</span></span>
- <span data-ttu-id="9e6f0-778">Korrektur eines Problems, bei dem DrvFs manchmal den falschen Dateityp für Verzeichnisse gemeldet hat [GH 2392]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-778">Fixed an issue where DrvFs sometimes reported the wrong file type for directories [GH 2392]</span></span>
- <span data-ttu-id="9e6f0-779">Ermöglichen der Erstellung von NETLINK_KOBJECT_UEVENT-Sockets zum Entsperren von Programmen, die uevent verwenden [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-779">Allow creation of NETLINK_KOBJECT_UEVENT sockets to unblock programs that use uevent [GH 1121, 2293, 2242, 2295, 2235, 648, 637]</span></span>
- <span data-ttu-id="9e6f0-780">Hinzufügen von Unterstützung für nicht blockierende Verbindungen [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-780">Add support for non-blocking connect [GH 903, 1391, 1584, 1585, 1829, 2290, 2314]</span></span>
- <span data-ttu-id="9e6f0-781">Implementieren des CLONE_FS-Klonsystem-Aufrufflags [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-781">Implement CLONE_FS clone system call flag [GH 2242]</span></span>
- <span data-ttu-id="9e6f0-782">Korrektur von Problemen im Zusammenhang mit der nicht ordnungsgemäßen Behandlung von Registerkarten oder Anführungszeichen in NT-Interop [GH 1625, 2164]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-782">Fix issues around not handling tabs or quotes correctly in NT interop [GH 1625, 2164]</span></span>
- <span data-ttu-id="9e6f0-783">Beheben des Fehlers „Zugriff verweigert“ beim Versuch, WSL-Instanzen erneut zu starten [GH 651, 2095]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-783">Resolve access denied error when trying to re-launch WSL instances [GH 651, 2095]</span></span>
- <span data-ttu-id="9e6f0-784">Implementieren von Futex-Vorgängen FUTEX_REQUEUE und FUTEX_CMP_REQUEUE [GH 2242]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-784">Implement futex FUTEX_REQUEUE and FUTEX_CMP_REQUEUE operations [GH 2242]</span></span>
- <span data-ttu-id="9e6f0-785">Korrigieren von Berechtigungen für verschiedene SysFs-Dateien [GH 2214]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-785">Fix permissions for various SysFs files [GH 2214]</span></span>
- <span data-ttu-id="9e6f0-786">Korrigieren des Hängens des Haskell-Stapels während des Setups [GH 2290]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-786">Fix Haskell stack hang during setup [GH 2290]</span></span>
- <span data-ttu-id="9e6f0-787">Implementieren der Flags „C“, „O“ und „P“ von binfmt_misc [GH 2103]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-787">Implement binfmt_misc 'C' 'O' and 'P' flags [GH 2103]</span></span>
- <span data-ttu-id="9e6f0-788">Hinzufügen von /proc/sys/kernel/shmmax/shmmni und /threads-max [GH 1753]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-788">Add /proc/sys/kernel /shmmax /shmmni & /threads-max [GH 1753]</span></span>
- <span data-ttu-id="9e6f0-789">Hinzufügen partieller Unterstützung für den ioprio_set-Systemaufruf [GH 498]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-789">Add partial support for ioprio_set system call [GH 498]</span></span>
- <span data-ttu-id="9e6f0-790">Stub für SO_REUSEPORT und Hinzufügen von Unterstützung für SO_PASSCRED für netlink-Sockets [GH 69]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-790">Stub SO_REUSEPORT & adding support for SO_PASSCRED for netlink sockets [GH 69]</span></span>
- <span data-ttu-id="9e6f0-791">Rückgabe anderer Fehlercodes aus RegisterDistribuiton, wenn zurzeit eine Distribution installiert oder deinstalliert wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-791">Return different error codes from RegisterDistribuiton if a distribution is currently being installed or uninstalled.</span></span>
- <span data-ttu-id="9e6f0-792">Ermöglichen des Aufhebens der Registrierung von teilweise installierten WSL-Distributionen über „wslconfig.exe“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-792">Allow unregistration of partially installed WSL distributions via wslconfig.exe</span></span>
- <span data-ttu-id="9e6f0-793">Korrektur des Hängens des Python-Sockettests von udp::msg_peek</span><span class="sxs-lookup"><span data-stu-id="9e6f0-793">Fix python socket test hang from udp::msg_peek</span></span>
- <span data-ttu-id="9e6f0-794">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-794">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-795">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-795">Console</span></span>
- <span data-ttu-id="9e6f0-796">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-796">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-797">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-797">LTP Results:</span></span>
<span data-ttu-id="9e6f0-798">Tests gesamt: 1904</span><span class="sxs-lookup"><span data-stu-id="9e6f0-798">Total Tests: 1904</span></span><br/>
<span data-ttu-id="9e6f0-799">Übersprungene Tests gesamt: 209</span><span class="sxs-lookup"><span data-stu-id="9e6f0-799">Total Skipped Tests: 209</span></span><br/>
<span data-ttu-id="9e6f0-800">Fehler gesamt: 229</span><span class="sxs-lookup"><span data-stu-id="9e6f0-800">Total Failures: 229</span></span><br/>
[<span data-ttu-id="9e6f0-801">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-801">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16273)<br/>

## <a name="build-16257"></a><span data-ttu-id="9e6f0-802">Build 16257</span><span class="sxs-lookup"><span data-stu-id="9e6f0-802">Build 16257</span></span>

<span data-ttu-id="9e6f0-803">Allgemeine Windows-Informationen zu Build 16257 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-803">For general Windows information on build 16257 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/08/02/announcing-windows-10-insider-preview-build-16257-pc-build-15237-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-804">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-804">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-805">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-805">WSL</span></span>
- <span data-ttu-id="9e6f0-806">Implementieren des prlimit64-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-806">Implement prlimit64 system call</span></span>
- <span data-ttu-id="9e6f0-807">Hinzufügen von Unterstützung für ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-807">Add support for ulimit -n (setrlimit RLIMIT_NOFILE) [GH 1688]</span></span>
- <span data-ttu-id="9e6f0-808">Stub für MSG_MORE für TCP-Sockets [GH 2351]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-808">Stub MSG_MORE for TCP sockets [GH 2351]</span></span>
- <span data-ttu-id="9e6f0-809">Korrektur des ungültigen Verhaltens des AT_EXECFN-Hilfsvektors [GH 2133]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-809">Fix invalid AT_EXECFN auxiliary vector behavior [GH 2133]</span></span>
- <span data-ttu-id="9e6f0-810">Korrektur des Kopier-/Einfügeverhalten für Konsole/TTY und Hinzufügen einer besseren Verarbeitung voller Puffer [GH 2204, 2131]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-810">Fix copy/paste behavior for console/tty, and add better full buffer handling [GH 2204, 2131]</span></span>
- <span data-ttu-id="9e6f0-811">Festlegen von T_SECURE im Hilfsvektor für set-user-ID- und set-group-ID-Programme [GH 2031]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-811">Set AT_SECURE in auxiliary vector for set-user-ID and set-group-ID programs [GH 2031]</span></span>
- <span data-ttu-id="9e6f0-812">Psuedoterminal-Masterendpunkt verarbeitet TIOCPGRP nicht [GH 1063]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-812">Psuedo-terminal master endpoint not handling TIOCPGRP [GH 1063]</span></span>
- <span data-ttu-id="9e6f0-813">Korrektur des Nichtzurückspulens von Verzeichnissen in LxFs durch lseek [GH 2310]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-813">Fix lseek does to rewind directories in LxFs [GH 2310]</span></span>
- <span data-ttu-id="9e6f0-814">/dev/ptmx wird nach hoher Auslastung gesperrt [GH 1882]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-814">/dev/ptmx locks up after heavy usage [GH 1882]</span></span>
- <span data-ttu-id="9e6f0-815">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-815">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-816">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-816">Console</span></span>
- <span data-ttu-id="9e6f0-817">Korrektur für horizontale Linien/Unterstriche überall [GH 2168]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-817">Fix for horizontal Lines/Underscores Everywhere [GH 2168]</span></span>
- <span data-ttu-id="9e6f0-818">Korrektur der Änderung der Prozessreihenfolge, wodurch das Schließen von NPM erschwert wird [GH 2170]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-818">Fix for process order changed making NPM harder to close [GH 2170]</span></span>
- <span data-ttu-id="9e6f0-819">Hinzufügen des neuen Farbschemas: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span><span class="sxs-lookup"><span data-stu-id="9e6f0-819">Added our new color scheme: https://blogs.msdn.microsoft.com/commandline/2017/08/02/updating-the-windows-console-colors/</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-820">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-820">LTP Results:</span></span>
<span data-ttu-id="9e6f0-821">Keine Änderung seit 16251</span><span class="sxs-lookup"><span data-stu-id="9e6f0-821">No change since 16251</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-822">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-822">Syscall Support</span></span>
<span data-ttu-id="9e6f0-823">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-823">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-824">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-824">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`prlimit64`<br/>

### <a name="known-issues"></a><span data-ttu-id="9e6f0-825">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="9e6f0-825">Known Issues</span></span>
#### <a name="github-issue-2392-windows-folders-not-recognized-by-wsl-"></a><span data-ttu-id="9e6f0-826">[GitHub-Issue 2392: Windows-Ordner werden von WSL nicht erkannt (](https://github.com/Microsoft/BashOnWindows/issues/2392))</span><span class="sxs-lookup"><span data-stu-id="9e6f0-826">[GitHub Issue 2392: Windows Folders not recognized by WSL ...](https://github.com/Microsoft/BashOnWindows/issues/2392)</span></span>
<span data-ttu-id="9e6f0-827">In Build 16257 hat WSL beim Aufzählen von Windows-Dateien/-Ordnern über `/mnt/c/...` Probleme.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-827">In build 16257, WSL has issues when enumerating Windows files/folders via `/mnt/c/...`.</span></span>
<span data-ttu-id="9e6f0-828">Dieses Problem wurde behoben und sollte im Insider-Builds in der Woche ab dem 14.08.2017 veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-828">This issue has been fixed and should be released in Insiders build during week commencing 8/14/2017.</span></span>

<br/>

## <a name="build-16251"></a><span data-ttu-id="9e6f0-829">Build 16251</span><span class="sxs-lookup"><span data-stu-id="9e6f0-829">Build 16251</span></span>

<span data-ttu-id="9e6f0-830">Allgemeine Windows-Informationen zu Build 16251 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-830">For general Windows information on build 16251 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/26/announcing-windows-10-insider-preview-build-16251-pc-build-15235-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-831">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-831">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-832">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-832">WSL</span></span>
- <span data-ttu-id="9e6f0-833">Entfernen des Beta-Tags aus der optionalen WSL-Komponente. Weitere Informationen finden Sie im [Blogbeitrag](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-833">Remove beta tag from WSL optional component, see [blog post](https://blogs.msdn.microsoft.com/commandline/2017/07/28/windows-subsystem-for-linux-out-of-beta/) for details.</span></span>
- <span data-ttu-id="9e6f0-834">Ordnungsgemäße Initialisierung der saved-set uid und gid für set-user-ID- and set-group-ID-Binärdateien bei der Ausführung [GH 962, 1415, 2072]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-834">Correctly initialize saved-set uid and gid for set-user-ID and set-group-ID binaries on exec [GH 962, 1415, 2072]</span></span>
- <span data-ttu-id="9e6f0-835">Hinzufügen von Unterstützung für PTRACE_O_TRACEEXIT [GH 555]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-835">Added support for ptrace PTRACE_O_TRACEEXIT [GH 555]</span></span>
- <span data-ttu-id="9e6f0-836">Hinzufügen von Unterstützung für PTRACE_GETFPREGS und PTRACE_GETREGSET mit NT_FPREGSET [GH 555]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-836">Added support for ptrace PTRACE_GETFPREGS and PTRACE_GETREGSET with NT_FPREGSET [GH 555]</span></span>
- <span data-ttu-id="9e6f0-837">Korrektur von ptrace, um bei ignorierten Signalen anzuhalten</span><span class="sxs-lookup"><span data-stu-id="9e6f0-837">Fixed ptrace to stop on ignored signals</span></span>
- <span data-ttu-id="9e6f0-838">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-838">Additional improvements and bug fixes</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-839">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-839">Console</span></span>
- <span data-ttu-id="9e6f0-840">Keine konsolenbezogenen Änderungen in diesem Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-840">No Console related changes in this release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-841">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-841">LTP Results:</span></span>
<span data-ttu-id="9e6f0-842">Anzahl bestandener Tests: 768</span><span class="sxs-lookup"><span data-stu-id="9e6f0-842">Number of Passing Tests: 768</span></span></br>
<span data-ttu-id="9e6f0-843">Anzahl fehlgeschlagener Tests: 244</span><span class="sxs-lookup"><span data-stu-id="9e6f0-843">Number of Failing Tests: 244</span></span></br>
<span data-ttu-id="9e6f0-844">Anzahl übersprungener Tests: 96</span><span class="sxs-lookup"><span data-stu-id="9e6f0-844">Number of Skipped Tests: 96</span></span></br>
[<span data-ttu-id="9e6f0-845">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-845">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/16251)<br/>

</br>

## <a name="build-16241"></a><span data-ttu-id="9e6f0-846">Build 16241</span><span class="sxs-lookup"><span data-stu-id="9e6f0-846">Build 16241</span></span>

<span data-ttu-id="9e6f0-847">Allgemeine Windows-Informationen zu Build 16241 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-847">For general Windows information on build 16241 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/13/announcing-windows-10-insider-preview-build-16241-pc-build-15230-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-848">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-848">Fixed</span></span>
#### <a name="wsl"></a><span data-ttu-id="9e6f0-849">WSL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-849">WSL</span></span>
- <span data-ttu-id="9e6f0-850">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-850">No WSL related changes in this release.</span></span>

#### <a name="console"></a><span data-ttu-id="9e6f0-851">Konsole</span><span class="sxs-lookup"><span data-stu-id="9e6f0-851">Console</span></span>
- <span data-ttu-id="9e6f0-852">Korrektur für die Ausgabe des falschen Zeichens für Schnittlinien-DEC, ursprünglich [hier](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/) gemeldet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-852">Fix for outputting the wrong character for the crossing-lines DEC, originally reported [here](https://www.reddit.com/r/Windows10/comments/6in82t/i_believe_ive_found_the_most_obscure_bug_ever/)</span></span>
- <span data-ttu-id="9e6f0-853">Korrektur, dass kein Ausgabetext in Codepage 65001 (UTF8) angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="9e6f0-853">Fix for no output text being displayed in codepage 65001 (utf8)</span></span>
- <span data-ttu-id="9e6f0-854">Übertragen Sie an den RGB-Werten einer Farbe vorgenommene Änderungen nicht an andere Teile der Palette bei Änderungen der Auswahl.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-854">Do not transfer changes made to one color's RGB values to other parts of the palette on selection change.</span></span> <span data-ttu-id="9e6f0-855">Dadurch wird die Verwendung des Konsoleneigenschaftenblatts erheblich vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-855">This will make the console properties sheet a lot easier to use.</span></span>
- <span data-ttu-id="9e6f0-856">STRG+S funktioniert anscheinend nicht ordnungsgemäß</span><span class="sxs-lookup"><span data-stu-id="9e6f0-856">Ctrl+S doesn't appear to work correctly</span></span>
- <span data-ttu-id="9e6f0-857">Un-Bold/-Dim fehlt in ANSI-Escapecodes vollständig [GH 2174]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-857">Un-Bold/-Dim completely absent from ANSI escape codes [GH 2174]</span></span>
- <span data-ttu-id="9e6f0-858">Die Konsole unterstützt VIM-Farbdesigns nicht ordnungsgemäß [GH 1706]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-858">Console doesn't correctly support Vim color themes [GH 1706]</span></span>
- <span data-ttu-id="9e6f0-859">Bestimmte Zeichen können nicht eingefügt werden [GH 2149]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-859">Cannot paste particular characters [GH 2149]</span></span>
- <span data-ttu-id="9e6f0-860">Die Größenänderung von dynamischem Umbruch interagiert seltsam mit der Größenänderung eines Bash-Fensters, wenn sich die Inhalte in der Bearbeitungs-/Befehlszeile befinden [GH-Verbindung 1123]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-860">Reflow resize interacts strangely with resizing a bash window when stuff is on the edit/command line [GH ConEmu 1123]</span></span>
- <span data-ttu-id="9e6f0-861">STRG+L hinterlässt Fragmente auf dem Bildschirm [GH 1978]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-861">Ctrl-L leaves the screen dirty [GH 1978]</span></span>
- <span data-ttu-id="9e6f0-862">Konsolenrenderingfehler bei der Anzeige von VT für HDPI [GH 1907]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-862">Console rendering bug when displaying VT on HDPI [GH 1907]</span></span>
- <span data-ttu-id="9e6f0-863">Japanische Zeichen sehen mit dem Unicode-Zeichen U+30FB seltsam aus [GH 2146]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-863">Japansese characters look strange with Unicode Character U+30FB [GH 2146]</span></span>
- <span data-ttu-id="9e6f0-864">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-864">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16237"></a><span data-ttu-id="9e6f0-865">Build 16237</span><span class="sxs-lookup"><span data-stu-id="9e6f0-865">Build 16237</span></span>

<span data-ttu-id="9e6f0-866">Allgemeine Windows-Informationen zu Build 16237 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-866">For general Windows information on build 16237 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/07/07/announcing-windows-10-insider-preview-build-16237-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-867">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-867">Fixed</span></span>
- <span data-ttu-id="9e6f0-868">Verwenden von Standardattributen für Dateien ohne E/As in lxfs (root, root, 0000)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-868">Use default attributes for files without EAs in lxfs (root, root, 0000)</span></span>
- <span data-ttu-id="9e6f0-869">Hinzufügen von Unterstützung für Distributionen, die erweiterte Attribute verwenden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-869">Added support for distributions that use extended attributes</span></span>
- <span data-ttu-id="9e6f0-870">Korrektur des Auffüllens für von getdents und getdents64 zurückgegebene Einträge</span><span class="sxs-lookup"><span data-stu-id="9e6f0-870">Fix padding for entries returned by getdents and getdents64</span></span>
- <span data-ttu-id="9e6f0-871">Korrektur der Berechtigungsüberprüfung für den SHM_STAT-Systemaufruf [GH 2068]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-871">Fix permissions check for the shmctl SHM_STAT system call [GH 2068]</span></span>
- <span data-ttu-id="9e6f0-872">Korrektur des falschen anfänglichen epoll-Zustands für ttys [GH 2231]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-872">Fixed incorrect initial epoll state for ttys [GH 2231]</span></span>
- <span data-ttu-id="9e6f0-873">Korrektur, dass DrvFs readdir nicht alle Einträge zurückgibt [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-873">Fix DrvFs readdir not returning all entries [GH 2077]</span></span>
- <span data-ttu-id="9e6f0-874">Korrektur von LxFs readdir, wenn Dateien nicht verknüpft sind [GH 2077]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-874">Fix LxFs readdir when files are unlinked [GH 2077]</span></span>
- <span data-ttu-id="9e6f0-875">Ermöglichen des erneuten Öffnens von nicht verknüpfter drvfs-Dateien über procfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-875">Allow unlinked drvfs files to be reopened through procfs</span></span>
- <span data-ttu-id="9e6f0-876">Hinzufügen einer Außerkraftsetzung des globalen Registrierungsschlüssels zum Deaktivieren von WSL-Features (Interop/Laufwerkeinbindung)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-876">Added global registry key override for disabling WSL features (interop / drive mounting)</span></span>
- <span data-ttu-id="9e6f0-877">Korrektur falscher Blockanzahl in „stat“ für DrvFs (und LxFs) [GH 1894]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-877">Fix incorrect block count in "stat" for DrvFs (and LxFs) [GH 1894]</span></span>
- <span data-ttu-id="9e6f0-878">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-878">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16232"></a><span data-ttu-id="9e6f0-879">Build 16232</span><span class="sxs-lookup"><span data-stu-id="9e6f0-879">Build 16232</span></span>

<span data-ttu-id="9e6f0-880">Allgemeine Windows-Informationen zu Build 16232 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-880">For general Windows information on build 16232 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/28/announcing-windows-10-insider-preview-build-16232-pc-build-15228-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-881">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-881">Fixed</span></span>
- <span data-ttu-id="9e6f0-882">In diesem Release gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-882">No WSL related changes in this release.</span></span>

</br>

## <a name="build-16226"></a><span data-ttu-id="9e6f0-883">Build 16226</span><span class="sxs-lookup"><span data-stu-id="9e6f0-883">Build 16226</span></span>

<span data-ttu-id="9e6f0-884">Allgemeine Windows-Informationen zu Build 16226 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-884">For general Windows information on build 16226 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/21/announcing-windows-10-insider-preview-build-16226-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-885">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-885">Fixed</span></span>
- <span data-ttu-id="9e6f0-886">Unterstützung von auf xattr bezogenen Systemaufrufen (getxattr, setxattr, listxattr, removexattr).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-886">xattr related syscalls support (getxattr, setxattr, listxattr, removexattr).</span></span>
- <span data-ttu-id="9e6f0-887">xattr-Unterstützung für security.capablity.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-887">security.capablity xattr support.</span></span>
- <span data-ttu-id="9e6f0-888">Verbesserte Kompatibilität mit bestimmten Dateisystemen und Filtern, einschließlich Nicht-MS-SMB-Servern.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-888">Improved compatibility with certain file systems and filters, including non-MS SMB servers.</span></span> <span data-ttu-id="9e6f0-889">[GH #1952]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-889">[GH #1952]</span></span>
- <span data-ttu-id="9e6f0-890">Verbesserte Unterstützung für OneDrive-Platzhalter, GVFS-Platzhalter und komprimierte Compact OS-Dateien.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-890">Improved support for OneDrive placeholders, GVFS placeholders, and Compact OS compressed files.</span></span>
- <span data-ttu-id="9e6f0-891">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-891">Additional improvements and bug fixes</span></span>

</br>

## <a name="build-16215"></a><span data-ttu-id="9e6f0-892">Build 16215</span><span class="sxs-lookup"><span data-stu-id="9e6f0-892">Build 16215</span></span>

<span data-ttu-id="9e6f0-893">Allgemeine Windows-Informationen zu Build 16215 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-893">For general Windows information on build 16215 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/06/08/announcing-windows-10-insider-preview-build-16215-pc-build-15222-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-894">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-894">Fixed</span></span>
- <span data-ttu-id="9e6f0-895">Für WSL ist der Entwicklermodus nicht mehr erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-895">WSL no longer requires developer mode.</span></span>
- <span data-ttu-id="9e6f0-896">Unterstützung von Verzeichnisverbindungen in drvfs.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-896">Support directory junctions in drvfs.</span></span>
- <span data-ttu-id="9e6f0-897">Verarbeiten der Deinstallation von appx-Paketen der WSL-Distribution.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-897">Handle uninstalling of WSL distribution appx packages.</span></span>
- <span data-ttu-id="9e6f0-898">Aktualisieren von procfs, um private und freigegebene Zuordnungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-898">Update procfs to show private and shared mappings.</span></span>
- <span data-ttu-id="9e6f0-899">Hinzufügen einer Möglichkeit für „wslconfig.exe“ zum Bereinigen von Distributionen, die teilweise installiert oder deinstalliert wurden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-899">Add ability for wslconfig.exe to clean up distributions that are partially installed or uninstalled.</span></span>
- <span data-ttu-id="9e6f0-900">Hinzufügen von Unterstützung für IP_MTU_DISCOVER für TCP-Sockets.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-900">Added support for IP_MTU_DISCOVER for TCP sockets.</span></span> <span data-ttu-id="9e6f0-901">[GH 1639, 2115, 2205]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-901">[GH 1639, 2115, 2205]</span></span>
- <span data-ttu-id="9e6f0-902">Ableiten der Protokollfamilie für Routen zu AF_INADDR.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-902">Infer protocol family for routes to AF_INADDR.</span></span>
- <span data-ttu-id="9e6f0-903">Verbesserungen an seriellen Geräten [GH 1929].</span><span class="sxs-lookup"><span data-stu-id="9e6f0-903">Serial device improvements [GH 1929].</span></span>

</br>

## <a name="build-16199"></a><span data-ttu-id="9e6f0-904">Build 16199</span><span class="sxs-lookup"><span data-stu-id="9e6f0-904">Build 16199</span></span>

<span data-ttu-id="9e6f0-905">Allgemeine Windows-Informationen zu Build 16199 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-905">For general Windows information on build 16199 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/17/announcing-windows-10-insider-preview-build-16199-pc-build-15215-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-906">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-906">Fixed</span></span>
- <span data-ttu-id="9e6f0-907">In diesen Releases gibt es keine WSL-bezogenen Änderungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-907">No WSL related changes in these releases.</span></span>

</br>

## <a name="build-16193"></a><span data-ttu-id="9e6f0-908">Build 16193</span><span class="sxs-lookup"><span data-stu-id="9e6f0-908">Build 16193</span></span>

<span data-ttu-id="9e6f0-909">Allgemeine Windows-Informationen zu Build 16193 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-909">For general Windows information on build 16193 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/05/11/announcing-windows-10-insider-preview-build-16193-pc-build-15213-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-910">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-910">Fixed</span></span>
- <span data-ttu-id="9e6f0-911">Racebedingung zwischen dem Senden von SIGCONT und einer Threadgruppe, die beendet wird [GH 1973]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-911">Race condition between sending SIGCONT and a threadgroup terminating [GH 1973]</span></span>
- <span data-ttu-id="9e6f0-912">Ändern von TTY-und PTY-Geräten zum Melden von FILE_DEVICE_NAMED_PIPE anstelle von FILE_DEVICE_CONSOLE [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-912">change tty and pty devices to report FILE_DEVICE_NAMED_PIPE instead of FILE_DEVICE_CONSOLE [GH 1840]</span></span>
- <span data-ttu-id="9e6f0-913">SSH-Korrektur für IP_OPTIONS</span><span class="sxs-lookup"><span data-stu-id="9e6f0-913">SSH fix for IP_OPTIONS</span></span>
- <span data-ttu-id="9e6f0-914">Verschieben der DrvFs-Einbindung in den init-Daemon [GH 1862, 1968, 1767, 1933]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-914">Moved DrvFs mounting to init daemon [GH 1862, 1968, 1767, 1933]</span></span>
- <span data-ttu-id="9e6f0-915">Hinzufügen von Unterstützung in DrvFs für die folgenden symbolischen NT-Verknüpfungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-915">Added support in DrvFs for following NT symlinks.</span></span>

</br>

## <a name="build-16184"></a><span data-ttu-id="9e6f0-916">Build 16184</span><span class="sxs-lookup"><span data-stu-id="9e6f0-916">Build 16184</span></span>

<span data-ttu-id="9e6f0-917">Allgemeine Windows-Informationen zu Build 16184 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-917">For general Windows information on build 16184 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/28/announcing-windows-10-insider-preview-build-16184-pc-build-15208-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-918">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-918">Fixed</span></span>
- <span data-ttu-id="9e6f0-919">Entfernen des apt-Paketverwaltungstasks (lxrun.exe /update) wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-919">Removed apt package maintenance task (lxrun.exe /update)</span></span>
- <span data-ttu-id="9e6f0-920">Korrektur der Nichtanzeige der Ausgabe aus Windows-Prozessen in node.js [GH 1840]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-920">Fixed output not showing up in from Windows processes in node.js [GH 1840]</span></span>
- <span data-ttu-id="9e6f0-921">Lockern der Ausrichtungsanforderungen in lxcore [GH 1794]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-921">Relax alignment requirements in lxcore [GH 1794]</span></span>
- <span data-ttu-id="9e6f0-922">Korrektur der Verarbeitung des AT_EMPTY_PATH-Flags in mehreren Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-922">Fixed handling of the AT_EMPTY_PATH flag in a numer of system calls.</span></span>
- <span data-ttu-id="9e6f0-923">Korrektur eines Problems, bei dem das Löschen von DrvFs-Dateien mit geöffneten Handles bewirkt, dass die Datei nicht definiertes Verhalten aufweist [GH 544, 966, 1357, 1535, 1615]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-923">Fixed issue where deleting DrvFs files with open handles will cause the file to exhibit undefined behavior [GH 544,966,1357,1535,1615]</span></span>
- <span data-ttu-id="9e6f0-924">„/etc/hosts“ erbt nun Einträge von der Windows-Hostdatei (%windir%\system32\drivers\etc\hosts) [GH 1495]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-924">/etc/hosts will now inherit entries from the Windows hosts file (%windir%\system32\drivers\etc\hosts) [GH 1495]</span></span>

</br>

## <a name="build-16179"></a><span data-ttu-id="9e6f0-925">Build 16179</span><span class="sxs-lookup"><span data-stu-id="9e6f0-925">Build 16179</span></span>

<span data-ttu-id="9e6f0-926">Allgemeine Windows-Informationen zu Build 16179 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-926">For general Windows information on build 16179 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/19/announcing-windows-10-insider-preview-build-16179-pc-build-15205-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-927">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-927">Fixed</span></span>
- <span data-ttu-id="9e6f0-928">Keine WSL-Änderungen in dieser Woche.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-928">No WSL changes this week.</span></span>

</br>

## <a name="build-16176"></a><span data-ttu-id="9e6f0-929">Build 16176</span><span class="sxs-lookup"><span data-stu-id="9e6f0-929">Build 16176</span></span>

<span data-ttu-id="9e6f0-930">Allgemeine Windows-Informationen zu Build 16176 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-930">For general Windows information on build 16176 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/14/announcing-windows-10-insider-preview-build-16176-pc-build-15204-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-931">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-931">Fixed</span></span>

- [<span data-ttu-id="9e6f0-932">Aktivierte serielle Unterstützung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-932">Enabled serial support</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/14/serial-support-on-the-windows-subsystem-for-linux/)
- <span data-ttu-id="9e6f0-933">Hinzufügen der IP-Socketoption IP_OPTIONS [GH 1116]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-933">Added IP socket option IP_OPTIONS [GH 1116]</span></span>
- <span data-ttu-id="9e6f0-934">Implementierung der pwritev-Funktion (beim Hochladen der Datei nach nginx/PHP-FPM) [GH 1506]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-934">Implemented pwritev function (while uploading file to nginx/PHP-FPM) [GH 1506]</span></span>
- <span data-ttu-id="9e6f0-935">Hinzufügen der IP-Socket-Optionen IP_MULTICAST_IF und IPV6_MULTICAST_IF [GH 990]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-935">Added IP socket options IP_MULTICAST_IF & IPV6_MULTICAST_IF [GH 990]</span></span>
- <span data-ttu-id="9e6f0-936">Unterstützung für Socketoption IP_MULTICAST_LOOP und IPV6_MULTICAST_LOOP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-936">Support for socket option IP_MULTICAST_LOOP & IPV6_MULTICAST_LOOP [GH 1678]</span></span>
- <span data-ttu-id="9e6f0-937">Hinzufügen von IP(V6)_MTU-Socketoption für den Knoten apps, traceroute, dig, nslookup, host</span><span class="sxs-lookup"><span data-stu-id="9e6f0-937">Added IP(V6)_MTU socket option for apps node, traceroute, dig, nslookup, host</span></span>
- <span data-ttu-id="9e6f0-938">Hinzufügen der IP-Socketoption IPV6_UNICAST_HOPS</span><span class="sxs-lookup"><span data-stu-id="9e6f0-938">Added IP socket option IPV6_UNICAST_HOPS</span></span>
- [<span data-ttu-id="9e6f0-939">Verbesserungen des Dateisystems</span><span class="sxs-lookup"><span data-stu-id="9e6f0-939">Filesystem Improvements</span></span>](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)
    * <span data-ttu-id="9e6f0-940">Ermöglichen der Einbindung von UNC-Pfaden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-940">Allow mounting of UNC paths</span></span>
    * <span data-ttu-id="9e6f0-941">Ermöglichen von CDFS-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-941">Enable CDFS support in drvfs</span></span>
    * <span data-ttu-id="9e6f0-942">Ordnungsgemäße Verarbeitung von Berechtigungen für Netzwerkdateisysteme in drvfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-942">Correctly handle permissions for network file systems in drvfs</span></span>
    * <span data-ttu-id="9e6f0-943">Hinzufügen von Unterstützung für Remotelaufwerke zu drvfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-943">Add support for remote drives to drvfs</span></span>
    * <span data-ttu-id="9e6f0-944">Ermöglichen von FAT-Unterstützung in drvfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-944">Enable FAT support in drvfs</span></span>
- <span data-ttu-id="9e6f0-945">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-945">Additional fixes and Improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-946">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="9e6f0-946">LTP Results</span></span>
<span data-ttu-id="9e6f0-947">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="9e6f0-947">No changes since 15042</span></span>

</br>

## <a name="build-16170"></a><span data-ttu-id="9e6f0-948">Build 16170</span><span class="sxs-lookup"><span data-stu-id="9e6f0-948">Build 16170</span></span>

<span data-ttu-id="9e6f0-949">Allgemeine Windows-Informationen zu Build 16170 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-949">For general Windows information on build 16170 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/04/07/announcing-windows-10-insider-preview-build-16170-pc/).</span></span><br/>

<span data-ttu-id="9e6f0-950">Wir haben einen neuen [Blogbeitrag](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) veröffentlicht, in dem unsere Anstrengungen beim Testen von WSL erläutert werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-950">We released a new [blog post](https://blogs.msdn.microsoft.com/wsl/2017/04/11/testing-the-windows-subsystem-for-linux/) discussing our efforts to test WSL.</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-951">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-951">Fixed</span></span>

- <span data-ttu-id="9e6f0-952">Unterstützung für Socketoption IP_ADD_MEMBERSHIP und IPV6_ADD_MEMBERSHIP [GH 1678]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-952">Support socket option IP_ADD_MEMBERSHIP & IPV6_ADD_MEMBERSHIP [GH 1678]</span></span>
- <span data-ttu-id="9e6f0-953">Hinzufügen von Unterstützung für PTRACE_OLDSETOPTIONS.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-953">Add support for PTRACE_OLDSETOPTIONS.</span></span> <span data-ttu-id="9e6f0-954">[GH 1692]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-954">[GH 1692]</span></span>
- <span data-ttu-id="9e6f0-955">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-955">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-956">LTP-Ergebnisse</span><span class="sxs-lookup"><span data-stu-id="9e6f0-956">LTP Results</span></span>
<span data-ttu-id="9e6f0-957">Keine Änderungen seit 15042</span><span class="sxs-lookup"><span data-stu-id="9e6f0-957">No changes since 15042</span></span>

</br>

## <a name="build-15046-to-windows-10-creators-update"></a><span data-ttu-id="9e6f0-958">Build 15046 für Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="9e6f0-958">Build 15046 to Windows 10 Creators Update</span></span>
<span data-ttu-id="9e6f0-959">Es gibt keine weiteren WSL-Korrekturen oder-Funktionen, die für die Einbindung in das Creators Update in Windows 10 geplant sind.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-959">There are no more WSL fixes or features planned for inclusion in the Creators Update to Windows 10.</span></span> <span data-ttu-id="9e6f0-960">Die Anmerkungen zu dieser Version von WSL werden in den kommenden Wochen fortgesetzt, um Ergänzungen für das nächste Hauptupdate von Windows aufzuführen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-960">Release notes for WSL will resume in the coming weeks for additions targeting the next major Windows Update.</span></span> <span data-ttu-id="9e6f0-961">Allgemeine Windows-Informationen zu Build 15046 und zukünftigen Insider Releases finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-961">For general Windows information on build 15046 and future Insider releases visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/28/announcing-windows-10-insider-preview-build-15046-pc/).</span></span> <br/><br/>
 <br/>

## <a name="build-15042"></a><span data-ttu-id="9e6f0-962">Build 15042</span><span class="sxs-lookup"><span data-stu-id="9e6f0-962">Build 15042</span></span>

<span data-ttu-id="9e6f0-963">Allgemeine Windows-Informationen zu Build 15042 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-963">For general Windows information on build 15042 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/24/announcing-windows-10-insider-preview-build-15042-pc-build-15043-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-964">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-964">Fixed</span></span>

- <span data-ttu-id="9e6f0-965">Korrektur eines Deadlocks beim Entfernen eines Pfades, der auf „..“ endet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-965">Fix for a deadlock when removing a path ending in ".."</span></span>
- <span data-ttu-id="9e6f0-966">Korrektur eines Problems, bei dem FIONBIO bei Erfolg 0 zurückgibt [GH 1683]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-966">Fixed an issue where FIONBIO not returning 0 on success [GH 1683]</span></span>
- <span data-ttu-id="9e6f0-967">Korrektur eines Problems bei Lesevorgängen mit einer Länge von Null von Internetdatagrammsockets</span><span class="sxs-lookup"><span data-stu-id="9e6f0-967">Fixed issue with zero-length reads of inet datagram sockets</span></span>
- <span data-ttu-id="9e6f0-968">Korrektur eines möglichen Deadlocks aufgrund einer Racebedingung bei der drvfs inode-Suche [GH 1675]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-968">Fix possible deadlock due to race condition in drvfs inode lookup [GH 1675]</span></span>
- <span data-ttu-id="9e6f0-969">Erweiterte Unterstützung für Hilfsdaten von Unix-Sockets, SCM_CREDENTIALS und SCM_RIGHTS [GH 514, 613, 1326]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-969">Extended support for unix socket ancillary data; SCM_CREDENTIALS and SCM_RIGHTS [GH 514, 613, 1326]</span></span>
- <span data-ttu-id="9e6f0-970">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-970">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-971">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-971">LTP Results:</span></span>
<span data-ttu-id="9e6f0-972">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="9e6f0-972">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="9e6f0-973">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9e6f0-973">Number of non-Passing (failing, skipped, etc…): 255</span></span>

</br>

## <a name="build-15031"></a><span data-ttu-id="9e6f0-974">Build 15031</span><span class="sxs-lookup"><span data-stu-id="9e6f0-974">Build 15031</span></span>

<span data-ttu-id="9e6f0-975">Allgemeine Windows-Informationen zu Build 15031 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-975">For general Windows information on build 15031 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/08/announcing-windows-10-insider-preview-build-15031-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-976">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-976">Fixed</span></span>

- <span data-ttu-id="9e6f0-977">Korrektur eines Fehlers, bei dem sich time(2) sporadisch falsch verhielt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-977">Fixed a bug where time(2) would sporadically misbehave.</span></span>
- <span data-ttu-id="9e6f0-978">Korrektur eines Problems, bei dem \*SIGPROCMASK-Systemaufrufe die Signalmaske beschädigen konnten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-978">Fixed and issue where \*SIGPROCMASK syscalls could corrupt signal mask.</span></span>
- <span data-ttu-id="9e6f0-979">Jetzt Rückgabe der vollständigen Länge der Befehlszeile in WSL-Benachrichtigung zur Prozesserstellung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-979">Now return full command line length in WSL process creation notification.</span></span> <span data-ttu-id="9e6f0-980">[GH 1632]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-980">[GH 1632]</span></span>
- <span data-ttu-id="9e6f0-981">WSL meldet jetzt die Threadbeendigung über ptrace für GDB-Hänger.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-981">WSL now reports thread exit through ptrace for GDB hangs.</span></span> <span data-ttu-id="9e6f0-982">[GH 1196]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-982">[GH 1196]</span></span>
- <span data-ttu-id="9e6f0-983">Korrektur eines Fehlers, bei dem ptys nach hoher tmux-E/A nicht mehr reagiert</span><span class="sxs-lookup"><span data-stu-id="9e6f0-983">Fixed bug where ptys would hang after heavy tmux IO.</span></span> <span data-ttu-id="9e6f0-984">[GH 1358]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-984">[GH 1358]</span></span>
- <span data-ttu-id="9e6f0-985">Korrektur der Timeoutüberprüfung in zahlreichen Systemaufrufen (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-985">Fixed timeout validation in many system calls (futex, semtimedop, ppoll, sigtimedwait, itimer, timer_create)</span></span>
- <span data-ttu-id="9e6f0-986">Hinzufügen von eventfd EFD_SEMAPHORE-Unterstützung [GH 452]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-986">Added eventfd EFD_SEMAPHORE support [GH 452]</span></span>
- <span data-ttu-id="9e6f0-987">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-987">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-988">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-988">LTP Results:</span></span>
<span data-ttu-id="9e6f0-989">Anzahl bestandener Tests: 737</span><span class="sxs-lookup"><span data-stu-id="9e6f0-989">Number of Passing Test: 737</span></span></br>
<span data-ttu-id="9e6f0-990">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9e6f0-990">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9e6f0-991">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-991">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15031)<br/>

<br/>

## <a name="build-15025"></a><span data-ttu-id="9e6f0-992">Build 15025</span><span class="sxs-lookup"><span data-stu-id="9e6f0-992">Build 15025</span></span>

<span data-ttu-id="9e6f0-993">Allgemeine Windows-Informationen zu Build 15025 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-993">For general Windows information on build 15025 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/02/01/announcing-windows-10-insider-preview-build-15025-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-994">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-994">Fixed</span></span>

- <span data-ttu-id="9e6f0-995">Korrektur eines Fehlers, bei dem grep 2.27 nicht mehr funktioniert [GH 1578]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-995">Fix for bug that broke grep 2.27 [GH 1578]</span></span>
- <span data-ttu-id="9e6f0-996">Implementierung des EFD_SEMAPHORE-Flags für den eventfd2-Systemaufruf [GH 452]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-996">Implemented EFD_SEMAPHORE flag for eventfd2 syscall [GH 452]</span></span>
- <span data-ttu-id="9e6f0-997">Implementierung von /proc/[pid]/net/ipv6_route [GH 1608]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-997">Implemented /proc/[pid]/net/ipv6_route [GH 1608]</span></span>
- <span data-ttu-id="9e6f0-998">Signalgestützte E/A-Unterstützung für Unix-Streamsockets [GH 393, 68]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-998">Signal driven IO support for unix stream sockets [GH 393, 68]</span></span>
- <span data-ttu-id="9e6f0-999">Unterstützung für F_GETPIPE_SZ und F_SETPIPE_SZ [GH 1012]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-999">Support F_GETPIPE_SZ and F_SETPIPE_SZ [GH 1012]</span></span>
- <span data-ttu-id="9e6f0-1000">Implementierung des recvmmsg()-Systemaufrufs [GH 1531]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1000">Implement recvmmsg() syscall [GH 1531]</span></span>
- <span data-ttu-id="9e6f0-1001">Korrektur eines Fehlers, bei dem epoll_wait() nicht gewartet hat [GH 1609]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1001">Fixed bug where epoll_wait() wasn't waiting [GH 1609]</span></span>
- <span data-ttu-id="9e6f0-1002">Implementierung von /proc/version_signature</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1002">Implement /proc/version_signature</span></span>
- <span data-ttu-id="9e6f0-1003">Tee-Systemaufruf gibt jetzt einen Fehler zurück, wenn beide Dateideskriptoren auf dieselbe Pipe verweisen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1003">Tee syscall now returns failure if both file descriptors refer to the same pipe</span></span>
- <span data-ttu-id="9e6f0-1004">Implementierung des richtigen Verhaltens für SO_PEERCRED für Unix-Sockets</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1004">Implemented correct behavior for SO_PEERCRED for Unix sockets</span></span>
- <span data-ttu-id="9e6f0-1005">Korrektur der Verarbeitung ungültiger Parameter des tkill-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1005">Fixed tkill syscall invalid parameter handling</span></span>
- <span data-ttu-id="9e6f0-1006">Änderungen zum Verbessern der Leistung von drvfs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1006">Changes to increase the preformace of drvfs</span></span>
- <span data-ttu-id="9e6f0-1007">Kleinere Korrektur für Ruby-E/A-Blockierung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1007">Minor fix for Ruby IO blocking</span></span>
- <span data-ttu-id="9e6f0-1008">Korrektur von recvmsg() beim Zurückgeben von EINVAL für das MSG_DONTWAIT-Flag für Inet-Sockets [GH 1296]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1008">Fixed recvmsg() returning EINVAL for the MSG_DONTWAIT flag for inet sockets [GH 1296]</span></span>
- <span data-ttu-id="9e6f0-1009">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1009">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1010">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1010">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1011">Anzahl bestandener Tests: 732</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1011">Number of Passing Test: 732</span></span></br>
<span data-ttu-id="9e6f0-1012">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1012">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9e6f0-1013">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1013">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15025)<br/>

<br/>

## <a name="build-15019"></a><span data-ttu-id="9e6f0-1014">Build 15019</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1014">Build 15019</span></span>

<span data-ttu-id="9e6f0-1015">Allgemeine Windows-Informationen zu Build 15019 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1015">For general Windows information on build 15019 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/27/announcing-windows-10-insider-preview-build-15019-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1016">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1016">Fixed</span></span>

- <span data-ttu-id="9e6f0-1017">Korrektur eines Fehlers, der fälschlicherweise die CPU-Auslastung in procfs für Tools wie htop gemeldet hat [GH 823, 945, 971]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1017">Fixed bug that incorrectly reported CPU usage in procfs for tools like htop (GH 823, 945, 971)</span></span>
- <span data-ttu-id="9e6f0-1018">Beim Aufrufen von open() mit O_TRUNC für eine vorhandene Datei „inotify“ wird nun IN_MODIFY vor IN_OPEN generiert</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1018">When calling open() with O_TRUNC on an existing file inotify now generates IN_MODIFY before IN_OPEN</span></span>
- <span data-ttu-id="9e6f0-1019">Korrekturen für den Unix-Socket getsockopt SO_ERROR zum Aktivieren von Postgress [GH 61, 1354]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1019">Fixes to unix socket getsockopt SO_ERROR to enable postgress [GH 61, 1354]</span></span>
- <span data-ttu-id="9e6f0-1020">Implementierung von /proc/sys/net/core/somaxconn für die Sprache GO</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1020">Implement /proc/sys/net/core/somaxconn for the GO language</span></span>
- <span data-ttu-id="9e6f0-1021">Der Apt-get-Packageupdate-Hintergrundtask wird jetzt aus der Ansicht ausgeblendet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1021">Apt-get package update background task now runs hidden from view</span></span>
- <span data-ttu-id="9e6f0-1022">Löschen des Bereichs für ipv6 localhost (Fehler Spring-Framework (Java)).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1022">Clear scope for ipv6 localhost (Spring-Framework(Java) failure).</span></span>
- <span data-ttu-id="9e6f0-1023">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1023">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1024">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1024">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1025">Anzahl bestandener Tests: 714</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1025">Number of Passing Test: 714</span></span> </br>
<span data-ttu-id="9e6f0-1026">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 249</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1026">Number of non-Passing (failing, skipped, etc…): 249</span></span> </br>
[<span data-ttu-id="9e6f0-1027">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1027">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15019)<br/>

<br/>

## <a name="build-15014"></a><span data-ttu-id="9e6f0-1028">Build 15014</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1028">Build 15014</span></span>

<span data-ttu-id="9e6f0-1029">Allgemeine Windows-Informationen zu Build 15014 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1029">For general Windows information on build 15014 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/19/announcing-windows-10-insider-preview-build-15014-for-pc-and-mobile-hello-windows-insiders-today-we-are-excited-to-be-releasing-windows-10-insider-preview-build-15014-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1030">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1030">Fixed</span></span>

- <span data-ttu-id="9e6f0-1031">STRG+C funktioniert nun wie beabsichtigt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1031">Ctrl+C now works as intended</span></span>
- <span data-ttu-id="9e6f0-1032">htop und ps auxw zeigen jetzt die richtige Ressourcenverwendung an (GH #516)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1032">htop and ps auxw now show correct resource utilization (GH #516)</span></span>
- <span data-ttu-id="9e6f0-1033">Grundlegende Übersetzung von NT-Ausnahmen in Signale.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1033">Basic translation of NT exceptions to signals.</span></span> <span data-ttu-id="9e6f0-1034">(GH #513)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1034">(GH #513)</span></span>
- <span data-ttu-id="9e6f0-1035">fallocate schlägt nun mit ENOSPC anstatt mit EINVAL fehl, wenn nicht genügend Speicherplatz verfügbar ist (GH #1571)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1035">fallocate now fails with ENOSPC  when running out of space instead of EINVAL (GH #1571)</span></span>
- <span data-ttu-id="9e6f0-1036">Hinzufügen von /proc/sys/kernel/sem.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1036">Added /proc/sys/kernel/sem.</span></span>
- <span data-ttu-id="9e6f0-1037">Implementierung der semop- und semtimedop-Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1037">Implemented semop and semtimedop system calls</span></span>
- <span data-ttu-id="9e6f0-1038">Korrektur von nslookup-Fehlern mit der IP_RECVTOS- und IPV6_RECVTCLASS-Socketoption (GH 69)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1038">Fixed nslookup errors with IP_RECVTOS & IPV6_RECVTCLASS socket option (GH 69)</span></span>
- <span data-ttu-id="9e6f0-1039">Unterstützung für Socketoptionen IP_RECVTTL und IPV6_RECVHOPLIMIT</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1039">Support for socket options IP_RECVTTL and IPV6_RECVHOPLIMIT</span></span>
- <span data-ttu-id="9e6f0-1040">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1040">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1041">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1041">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1042">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1042">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="9e6f0-1043">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1043">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9e6f0-1044">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1044">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014)<br/>

### <a name="syscall-summary"></a><span data-ttu-id="9e6f0-1045">Zusammenfassung der Systemaufrufe</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1045">Syscall Summary</span></span>
<span data-ttu-id="9e6f0-1046">Systemaufrufe gesamt: 384</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1046">Total Syscalls: 384</span></span> </br>
<span data-ttu-id="9e6f0-1047">Implementiert gesamt: 235</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1047">Total Implemented: 235</span></span> </br>
<span data-ttu-id="9e6f0-1048">Mit Stub versehen gesamt: 22</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1048">Total Stubbed: 22</span></span> </br>
<span data-ttu-id="9e6f0-1049">Nicht implementiert gesamt: 127</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1049">Total Unimplemented: 127</span></span> </br>
[<span data-ttu-id="9e6f0-1050">Ausführliche Aufschlüsselung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1050">Detailed Breakdown</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15014/Syscalls.txt)<br/>

<br/>

## <a name="build-15007"></a><span data-ttu-id="9e6f0-1051">Build 15007</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1051">Build 15007</span></span>

<span data-ttu-id="9e6f0-1052">Allgemeine Windows-Informationen zu Build 15007 finden Sie im [Windows-Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1052">For general Windows information on build 15007 visit the [Windows Blog]( https://blogs.windows.com/windowsexperience/2017/01/12/announcing-windows-10-insider-preview-build-15007-pc-mobile).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="9e6f0-1053">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1053">Known Issue</span></span>

- <span data-ttu-id="9e6f0-1054">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1054">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="9e6f0-1055">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1055">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="9e6f0-1056">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1056">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="9e6f0-1057">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1057">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="9e6f0-1058">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1058">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="9e6f0-1059">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1059">Users can explore the option to include this in their `.bashrc`</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1060">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1060">Fixed</span></span>

- <span data-ttu-id="9e6f0-1061">Korrektur eines Problems, bei dem die Ausführung von WSL 100 % eines CPU-Kerns verbraucht</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1061">Corrected the issue where running WSL would consume 100% of a CPU core</span></span>
- <span data-ttu-id="9e6f0-1062">Socketoption IP_PKTINFO, IPV6_RECVPKTINFO wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1062">Socket option IP_PKTINFO, IPV6_RECVPKTINFO now supported.</span></span> <span data-ttu-id="9e6f0-1063">(GH #851, 987)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1063">(GH #851, 987)</span></span>
- <span data-ttu-id="9e6f0-1064">Abschneiden der physischen Adresse der Netzwerkschnittstelle auf 16 Bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1064">Truncate network interface physical address to 16 bytes in lxcore (GH #1452, 1414, 1343, 468, 308)</span></span>
- <span data-ttu-id="9e6f0-1065">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1065">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1066">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1066">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1067">Anzahl bestandener Tests: 709</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1067">Number of Passing Test: 709</span></span> </br>
<span data-ttu-id="9e6f0-1068">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 255</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1068">Number of non-Passing (failing, skipped, etc…): 255</span></span> </br>
[<span data-ttu-id="9e6f0-1069">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1069">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15007)<br/>

<br/>

## <a name="build-15002"></a><span data-ttu-id="9e6f0-1070">Build 15002</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1070">Build 15002</span></span>

<span data-ttu-id="9e6f0-1071">Allgemeine Windows-Informationen zu Build 15002 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1071">For general Windows information on build 15002 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2017/01/09/announcing-windows-10-insider-preview-build-15002-pc/).</span></span><br/>


### <a name="known-issue"></a><span data-ttu-id="9e6f0-1072">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1072">Known Issue</span></span>

<span data-ttu-id="9e6f0-1073">Zwei bekannte Probleme:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1073">Two known issues:</span></span>
- <span data-ttu-id="9e6f0-1074">Es gibt einen bekannten Fehler, bei dem die Konsole einige Eingaben über STRG+<key> nicht erkennt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1074">There is a known bug where the console does not recognize some Ctrl + <key> input.</span></span>  <span data-ttu-id="9e6f0-1075">Dies schließt den Befehl STRG+C ein, der als normaler C-Tastendruck fungiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1075">This includes the ctrl-c command which will act as a normal ‘c’ keypress.</span></span>

  - <span data-ttu-id="9e6f0-1076">Problemumgehung: Ordnen Sie STRG+C eine alternative Taste zu.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1076">Workaround: Map an alternate key to Ctrl+C.</span></span> <span data-ttu-id="9e6f0-1077">Gehen Sie beispielsweise folgendermaßen vor, um STRG+K der Tastenkombination STRG+C zuzuordnen: `stty intr \^k`.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1077">For example, to map Ctrl+K to Ctrl+C do: `stty intr \^k`.</span></span>  <span data-ttu-id="9e6f0-1078">Diese Zuordnung erfolgt pro Terminal und muss *jedes* Mal ausgeführt werden, wenn Bash gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1078">This mapping is per terminal and will have to be done *every* time bash is launched.</span></span> <span data-ttu-id="9e6f0-1079">Benutzer können die Option zum Einbeziehen in ihre `.bashrc`-Datei untersuchen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1079">Users can explore the option to include this in their `.bashrc`</span></span>

- <span data-ttu-id="9e6f0-1080">Während der Ausführung von WSL werden von einem Systemthread 100 % eines CPU-Kerns beansprucht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1080">While WSL is running a system thread will consume 100% of a CPU core.</span></span>  <span data-ttu-id="9e6f0-1081">Die Ursache wurde untersucht und intern behoben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1081">The root cause has been addressed and fixed internally.</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1082">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1082">Fixed</span></span>

- <span data-ttu-id="9e6f0-1083">Alle Bash-Sitzungen müssen jetzt auf derselben Berechtigungsebene erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1083">All bash sessions must now be created at the same permission level.</span></span>  <span data-ttu-id="9e6f0-1084">Der Versuch, eine Sitzung auf einer anderen Ebene zu starten, wird blockiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1084">Attempting to start a session at a different level will be blocked.</span></span>  <span data-ttu-id="9e6f0-1085">Dies bedeutet, dass Administrator-und Nicht-Administratorkonsolen nicht gleichzeitig ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1085">This means admin and non-admin consoles cannot run at the same time.</span></span> <span data-ttu-id="9e6f0-1086">(GH #626)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1086">(GH #626)</span></span>
<br/>
- <span data-ttu-id="9e6f0-1087">Implementierung der folgenden NETLINK_ROUTE-Meldungen (erfordert Windows-Administrator)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1087">Implemented the following NETLINK_ROUTE messages (requires Windows admin)</span></span>
     - <span data-ttu-id="9e6f0-1088">RTM_NEWADDR (unterstützt `ip addr add`)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1088">RTM_NEWADDR (supports `ip addr add`)</span></span>
     - <span data-ttu-id="9e6f0-1089">RTM_NEWROUTE (unterstützt `ip route add`)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1089">RTM_NEWROUTE (supports `ip route add`)</span></span>
     - <span data-ttu-id="9e6f0-1090">RTM_DELADDR (unterstützt `ip addr del`)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1090">RTM_DELADDR (supports `ip addr del`)</span></span>
     - <span data-ttu-id="9e6f0-1091">RTM_DELROUTE (unterstützt `ip route del`)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1091">RTM_DELROUTE (supports `ip route del`)</span></span>
- <span data-ttu-id="9e6f0-1092">Die geplante Tasküberprüfung für zu aktualisierende Pakete wird nicht mehr über eine getaktete Verbindung ausgeführt (GH #1371)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1092">Scheduled task checking for packages to update will no longer run on a metered connection (GH #1371)</span></span>
- <span data-ttu-id="9e6f0-1093">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1093">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="9e6f0-1094">Implementierung der TCP_KEEPCNT-Socketoption (GH #843)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1094">Implemented TCP_KEEPCNT socket option (GH #843)</span></span>
- <span data-ttu-id="9e6f0-1095">Implementierung der IP_MTU_DISCOVER INET-Socketoption (GH #720, 717, 170, 69)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1095">Implemented IP_MTU_DISCOVER INET socket option (GH #720, 717, 170, 69)</span></span>
- <span data-ttu-id="9e6f0-1096">Entfernen der Legacyfnktionalität zum Ausführen von NT-Binärdateien aus init mit NT-Pfadsuche.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1096">Removed legacy functionality to run NT binaries from init with NT path lookup.</span></span> <span data-ttu-id="9e6f0-1097">(GH #1325)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1097">(GH #1325)</span></span>
- <span data-ttu-id="9e6f0-1098">Korrektur des Modus von /dev/kmsg zum Zulassen von Gruppen-/sonstigem Lesezugriff (0644) (GH #1321)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1098">Fix mode of /dev/kmsg to allow group / other read access (0644) (GH #1321)</span></span>
- <span data-ttu-id="9e6f0-1099">Implementierung von /proc/sys/kernel/random/uuid (GH #1092)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1099">Implemented /proc/sys/kernel/random/uuid  (GH #1092)</span></span>
- <span data-ttu-id="9e6f0-1100">Korrektur eines Fehlers, bei dem die Startzeit des Prozesses als Jahr 2432 angezeigt wurde (GH #974)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1100">Corrected error where process start time was showing as year 2432 (GH #974)</span></span>
- <span data-ttu-id="9e6f0-1101">Wechseln der TERM-Standardumgebungsvariablen in xterm-256color (GH #1446)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1101">Switched default TERM environment variable to xterm-256color (GH #1446)</span></span>
- <span data-ttu-id="9e6f0-1102">Änderung der Art und Weise, in der der Prozesscommit während des Prozessforks berechnet wird.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1102">Modified the way that process commit is calculated during process fork.</span></span> <span data-ttu-id="9e6f0-1103">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1103">(GH #1286)</span></span>
- <span data-ttu-id="9e6f0-1104">Implementierung von /proc/sys/vm/overcommit_memory.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1104">Implemented /proc/sys/vm/overcommit_memory.</span></span> <span data-ttu-id="9e6f0-1105">(GH #1286)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1105">(GH #1286)</span></span>
- <span data-ttu-id="9e6f0-1106">Implementierung der /proc/net/route-Datei (GH #69)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1106">Implemented /proc/net/route file (GH #69)</span></span>
- <span data-ttu-id="9e6f0-1107">Korrektur eines Fehlers, bei dem der Verknüpfungsname falsch lokalisiert wurde (GH #696)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1107">Fixed error where shortcut name was incorrectly localized (GH #696)</span></span>
- <span data-ttu-id="9e6f0-1108">Korrektur der fehlerhaften ELF-Verarbeitungslogik, die die Programmheader nicht ordnungsgemäß so überprüft, dass sie kleiner als (oder gleich) PATH_MAX sein müssen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1108">Fixed elf parsing logic that is incorrectly validating the program headers must be less than (or equal to) PATH_MAX.</span></span> <span data-ttu-id="9e6f0-1109">(GH #1048)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1109">(GH #1048)</span></span>
- <span data-ttu-id="9e6f0-1110">Implementierung des statfs-Rückrufs für procfs, sysfs, cgroupfs und binfmts (GH #1378)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1110">Implemented statfs callback for procfs, sysfs, cgroupfs, and binfmtfs (GH #1378)</span></span>
- <span data-ttu-id="9e6f0-1111">Korrektur der AptPackageIndexUpdate-Fenster, die nicht geschlossen werden (GH #1184, auch in GH #1193 beschrieben)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1111">Fixed AptPackageIndexUpdate windows that won’t close (GH #1184, also discussed in GH #1193)</span></span>
- <span data-ttu-id="9e6f0-1112">Hinzufügen von ASLR-Personality, ADDR_NO_RANDOMIZE-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1112">Added ASLR personality  ADDR_NO_RANDOMIZE support.</span></span> <span data-ttu-id="9e6f0-1113">[GH #1148, 1128]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1113">(GH #1148, 1128)</span></span>
- <span data-ttu-id="9e6f0-1114">Verbesserung von PTRACE_GETSIGINFO, SIGSEGV für ordnungsgemäße gdb-Stapelüberwachungen während AV (GH #875)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1114">Improved PTRACE_GETSIGINFO, SIGSEGV, for proper gdb stack traces during AV (GH #875)</span></span>
- <span data-ttu-id="9e6f0-1115">Elf-Verarbeitung schlägt für patchelf-Binärdateien nicht mehr fehl.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1115">Elf parsing no longer fails for patchelf binaries.</span></span> <span data-ttu-id="9e6f0-1116">[GH #471]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1116">(GH #471)</span></span>
- <span data-ttu-id="9e6f0-1117">VPN DNS-Weitergabe an /etc/resolv.conf (GH #416, 1350)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1117">VPN DNS propagated to /etc/resolv.conf (GH #416, 1350)</span></span>
- <span data-ttu-id="9e6f0-1118">Verbesserungen an TCP Close für eine zuverlässigere Datenübertragung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1118">Improvements to TCP close for more reliable data transfer.</span></span> <span data-ttu-id="9e6f0-1119">(GH #610, 616, 1025, 1335)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1119">(GH #610, 616, 1025, 1335)</span></span>
- <span data-ttu-id="9e6f0-1120">Jetzt Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden (EMFILE).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1120">Now return correct error code when too many files are opened (EMFILE).</span></span> <span data-ttu-id="9e6f0-1121">(GH #1126, 2090)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1121">(GH #1126, 2090)</span></span>
- <span data-ttu-id="9e6f0-1122">Windows-Überwachungsprotokoll erfasst jetzt den Imagenamen in Process Create Audit.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1122">Windows Audit log now reports the image name in process create audit.</span></span>
- <span data-ttu-id="9e6f0-1123">Jetzt normaler Fehler beim Starten von „bash.exe“ in einem Bash-Fenster.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1123">Now gracefully fail when launching bash.exe from within a bash window</span></span>
- <span data-ttu-id="9e6f0-1124">Hinzufügen einer Fehlermeldung, wenn Interop nicht auf ein Arbeitsverzeichnis unter LxFs zugreifen kann (z.B. BASHRC-Datei von „notepad.exe“).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1124">Added error message when interop is unable to access a working directory under LxFs (i.e. notepad.exe .bashrc)</span></span>
- <span data-ttu-id="9e6f0-1125">Korrektur eines Problems, bei dem der Windows-Pfad in WSL abgeschnitten wurde</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1125">Fixed issue where Windows path was truncated in WSL</span></span>
- <span data-ttu-id="9e6f0-1126">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1126">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1127">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1127">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1128">Anzahl bestandener Tests: 690</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1128">Number of Passing Test: 690</span></span> </br>
<span data-ttu-id="9e6f0-1129">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 274</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1129">Number of non-Passing (failing, skipped, etc…): 274</span></span> </br>
[<span data-ttu-id="9e6f0-1130">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1130">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/15002)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1131">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1131">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1132">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1132">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1133">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1133">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`shmctl`<br/>
`shmget`<br/>
`shmdt`<br/>
`shmat`<br/>
<br/>

## <a name="build-14986"></a><span data-ttu-id="9e6f0-1134">Build 14986</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1134">Build 14986</span></span>

<span data-ttu-id="9e6f0-1135">Allgemeine Windows-Informationen zu Build 14986 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1135">For general Windows information on build 14986 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/12/07/announcing-windows-10-insider-preview-build-14986-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1136">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1136">Fixed</span></span>

- <span data-ttu-id="9e6f0-1137">Korrektur von Fehlerüberprüfungen mit Netlink und Pty IOCTLs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1137">Fixed bugchecks with Netlink and Pty IOCTLs</span></span>
- <span data-ttu-id="9e6f0-1138">Kernel Version meldet nun 4.4.0-43 aus Gründen der Konsistenz mit Xenial</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1138">Kernel version now reports 4.4.0-43 for consistency with Xenial</span></span>
- <span data-ttu-id="9e6f0-1139">„Bash.exe“ wird jetzt gestartet, wenn die Eingabe an „nul:“ gerichtet ist (GH #1259)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1139">Bash.exe now launches when input directed to 'nul:' (GH #1259)</span></span>
- <span data-ttu-id="9e6f0-1140">Thread-IDs werden nun ordnungsgemäß in procfs erfasst (GH #967)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1140">Thread IDs now reported correctly in procfs (GH #967)</span></span>
- <span data-ttu-id="9e6f0-1141">Flags IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR werden jetzt in inotify_add_watch() unterstützt (GH #1280)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1141">IN_UNMOUNT | IN_Q_OVERFLOW | IN_IGNORED | IN_ISDIR flags now supported in inotify_add_watch() (GH #1280)</span></span>
- <span data-ttu-id="9e6f0-1142">Implementierung von timer_create und verwandten Systemaufrufen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1142">Implement timer_create and related system calls.</span></span>  <span data-ttu-id="9e6f0-1143">Dies ermöglicht die GHC-Unterstützung (GH #307).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1143">This enables GHC support (GH #307)</span></span>
- <span data-ttu-id="9e6f0-1144">Korrektur eines Problems, bei dem Ping eine Zeitangabe von 0,000 ms zurückgab (GH #1296)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1144">Fixed issue where ping returned a time of 0.000ms (GH #1296)</span></span>
- <span data-ttu-id="9e6f0-1145">Rückgabe des richtigen Fehlercodes, wenn zu viele Dateien geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1145">Return correct error code when too many files are opened.</span></span>
- <span data-ttu-id="9e6f0-1146">Korrektur eines Problems in WSL, bei dem die Netlink-Anforderung für Netzwerkschnittstellendaten mit EINVAL fehlschlägt, wenn die Hardwareadresse der Schnittstelle 32 Bytes groß ist (z.B. die Teredo-Schnittstelle)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1146">Fixed issue in WSL where Netlink request for network interface data would fail with EINVAL if the interface's hardware address is 32-bytes (such as the Teredo interface)</span></span>
   - <span data-ttu-id="9e6f0-1147">Beachten Sie, dass das Linux-Hilfsprogramm „ip“ einen Fehler enthält, bei dem ein Absturz erfolgt, wenn WSL eine 32-Byte-Hardwareadresse meldet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1147">Note that the Linux "ip" utility contains a bug where it will crash if WSL reports a 32-byte hardware address.</span></span> <span data-ttu-id="9e6f0-1148">Dies ist ein Fehler in „ip“, nicht in WSL.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1148">This is a bug in "ip", not WSL.</span></span> <span data-ttu-id="9e6f0-1149">Mit dem Hilfsprogramm „ip“ wird die Länge des Zeichenfolgenpuffers fest codiert, der zum Ausgeben der Hardwareadresse verwendet wird, und dieser Puffer ist zu klein, um eine 32-Byte-Hardwareadresse auszugeben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1149">The “ip” utility hard-codes the length of the string buffer used to print the hardware address, and that buffer is too small to print a 32-byte hardware address.</span></span>
- <span data-ttu-id="9e6f0-1150">Zusätzliche Korrekturen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1150">Additional fixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1151">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1151">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1152">Anzahl bestandener Tests: 669</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1152">Number of Passing Test: 669</span></span> </br>
<span data-ttu-id="9e6f0-1153">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1153">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="9e6f0-1154">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1154">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14986)<br/>

<br/>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1155">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1155">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1156">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1156">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1157">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1157">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`timer_create`<br/>
`timer_delete`<br/>
`timer_gettime`<br/>
`timer_settime`<br/>
<br/>

## <a name="build-14971"></a><span data-ttu-id="9e6f0-1158">Build 14971</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1158">Build 14971</span></span>

<span data-ttu-id="9e6f0-1159">Allgemeine Windows-Informationen zu Build 14971 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1159">For general Windows information on build 14971 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/17/announcing-windows-10-insider-preview-build-14971-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1160">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1160">Fixed</span></span>

 - <span data-ttu-id="9e6f0-1161">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1161">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9e6f0-1162">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1162">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1163">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1163">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1164">Keine Änderungen seit 14965</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1164">Unchanged from 14965</span></span> </br>
<span data-ttu-id="9e6f0-1165">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1165">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9e6f0-1166">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1166">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1167">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1167">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14965"></a><span data-ttu-id="9e6f0-1168">Build 14965</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1168">Build 14965</span></span>

<span data-ttu-id="9e6f0-1169">Allgemeine Windows-Informationen zu Build 14965 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1169">For general Windows information on build 14965 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/09/announcing-windows-10-insider-preview-build-14965-for-mobile-and-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1170">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1170">Fixed</span></span>

- <span data-ttu-id="9e6f0-1171">Unterstützung für Netlink-Sockets RTM_GETLINK und RTM_GETADDR des NETLINK_ROUTE-Protokolls (GH #468)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1171">Support for Netlink sockets NETLINK_ROUTE protocol's RTM_GETLINK and RTM_GETADDR (GH #468)</span></span>
  - <span data-ttu-id="9e6f0-1172">Aktiviert ifconfig- und ip-Befehle für die Netzwerkenumeration.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1172">Enables ifconfig and ip commands for network enumeration</span></span>
  - <span data-ttu-id="9e6f0-1173">Weitere Informationen finden Sie in unserem [Blogbeitrag zu WSL-Netzwerken](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1173">More information can be found in our [WSL Networking blog post](https://blogs.msdn.microsoft.com/wsl/2016/11/08/225/).</span></span>

- <span data-ttu-id="9e6f0-1174">„/sbin“ befindet sich jetzt standardmäßig im Pfad des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1174">/sbin is now in the user's path by default</span></span>
- <span data-ttu-id="9e6f0-1175">Der NT-Benutzerpfad wird jetzt standardmäßig an den WSL-Pfad angefügt (Sie können nun also „notepad.exe“ eingeben, ohne dem Linux-Pfad System32 hinzuzufügen).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1175">NT user path now appended to the WSL path by default (i.e. you can now type notepad.exe without adding System32 to the Linux path)</span></span>
- <span data-ttu-id="9e6f0-1176">Hinzufügen von Unterstützung für /proc/sys/kernel/cap_last_cap</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1176">Added support for /proc/sys/kernel/cap_last_cap</span></span>
- <span data-ttu-id="9e6f0-1177">NT-Binärdateien können nun aus WSL gestartet werden, wenn das aktuelle Arbeitsverzeichnis Nicht-ANSI-Zeichen enthält (GH #1254)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1177">NT Binaries can now be launched from WSL when the current working directory contains non-ansi characters (GH #1254)</span></span>
- <span data-ttu-id="9e6f0-1178">Ermöglichen des Herunterfahrens für getrennten UNIX-Streamsocket</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1178">Allow shutdown on disconnected unix stream socket.</span></span>
- <span data-ttu-id="9e6f0-1179">Hinzufügen von Unterstützung für PR_GET_PDEATHSIG.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1179">Added support for PR_GET_PDEATHSIG.</span></span>
- <span data-ttu-id="9e6f0-1180">Hinzufügen von Unterstützung für CLONE_PARENT</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1180">Added support for CLONE_PARENT</span></span>
- <span data-ttu-id="9e6f0-1181">Korrektur eines Fehlers, bei dem die Weiterleitung unterbrochen wird. Beispiel: bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1181">Fixed error where piping gets stuck i.e. bash -c "ls -alR /" | bash -c "cat" (GH #1214)</span></span>
- <span data-ttu-id="9e6f0-1182">Verarbeiten von Anforderungen zum Herstellen einer Verbindung mit dem aktuellen Terminal.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1182">Handle requests to connect to the current terminal.</span></span>
- <span data-ttu-id="9e6f0-1183">Markieren von /proc/<pid>/oom_score_adj als beschreibbar.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1183">Mark /proc/<pid>/oom_score_adj as writable.</span></span>
- <span data-ttu-id="9e6f0-1184">Hinzufügen des Ordners „/sys/fs/cgroup“.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1184">Add /sys/fs/cgroup folder.</span></span>
- <span data-ttu-id="9e6f0-1185">sched_setaffinity sollte den Wert der Affinitätsbitsmaske zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1185">sched_setaffinity should return number of affinity bits mask</span></span>
- <span data-ttu-id="9e6f0-1186">Korrektur der ELF-Validierungslogik, die fälschlicherweise annimmt, dass Interpreterpfade weniger als 64 Zeichen lang sein müssen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1186">Fix ELF validation logic which incorrectly assumes interpreter paths must be less than 64 characters long.</span></span> <span data-ttu-id="9e6f0-1187">(GH #743)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1187">(GH #743)</span></span>
- <span data-ttu-id="9e6f0-1188">Geöffnete Dateideskriptoren können das Konsolenfenster geöffnet lassen (GH #1187)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1188">Open file descriptors can keep console window open (GH #1187)</span></span>
- <span data-ttu-id="9e6f0-1189">Korrektur eines Fehlers, bei dem rename() mit einem nachgestellten Schrägstrich für den Zielnamen fehlschlägt (GH #1008)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1189">Fixeed error where rename() failed with trailing slash on target name (GH #1008)</span></span>
- <span data-ttu-id="9e6f0-1190">Implementierung der/proc/net/dev-Datei</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1190">Implement /proc/net/dev file</span></span>
- <span data-ttu-id="9e6f0-1191">Korrektur von Pings mit 0,000 ms aufgrund der Timerauflösung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1191">Fixed 0.000ms pings due to timer resolution.</span></span>
- <span data-ttu-id="9e6f0-1192">Implementierung von /proc/self/environ (GH #730)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1192">Implemented /proc/self/environ (GH #730)</span></span>
- <span data-ttu-id="9e6f0-1193">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1193">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1194">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1194">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1195">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1195">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9e6f0-1196">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1196">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1197">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1197">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14965)<br/>

<br/>

## <a name="build-14959"></a><span data-ttu-id="9e6f0-1198">Build 14959</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1198">Build 14959</span></span>

<span data-ttu-id="9e6f0-1199">Allgemeine Windows-Informationen zu Build 14959 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1199">For general Windows information on build 14959 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/11/03/announcing-windows-10-insider-preview-build-14959-for-mobile-and-pc/#iI82GufJxMF3POU1.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1200">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1200">Fixed</span></span>

- <span data-ttu-id="9e6f0-1201">Verbesserte Pico-Prozessbenachrichtigung für Windows.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1201">Improved Pico Process notification for Windows.</span></span>  <span data-ttu-id="9e6f0-1202">Weitere Informationen finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1202">Additional information found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/).</span></span>
- <span data-ttu-id="9e6f0-1203">Verbesserte Stabilität mit Windows-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1203">Improved stability with Windows interoperability</span></span>
- <span data-ttu-id="9e6f0-1204">Korrektur von Fehler 0x80070057 beim Starten von „bash.exe“, wenn der Enterprise Data Protection (EDP) aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1204">Fixed error 0x80070057 when launching bash.exe when Enterprise Data Protection (EDP) is enabled</span></span>
- <span data-ttu-id="9e6f0-1205">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1205">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1206">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1206">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1207">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1207">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9e6f0-1208">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1208">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1209">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1209">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14959)<br/>

<br/>

## <a name="build-14955"></a><span data-ttu-id="9e6f0-1210">Build 14955</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1210">Build 14955</span></span>

<span data-ttu-id="9e6f0-1211">Allgemeine Windows-Informationen zu Build 14955 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1211">For general Windows information on build 14955 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/25/announcing-windows-10-insider-preview-build-14955-for-mobile-and-pc/#guGXQzKVFrZIDUYR.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1212">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1212">Fixed</span></span>

 - <span data-ttu-id="9e6f0-1213">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1213">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9e6f0-1214">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1214">Regularly scheduled updates will resume on the next release.</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1215">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1215">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1216">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1216">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9e6f0-1217">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1217">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1218">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1218">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14955)<br/>

<br/>

## <a name="build-14951"></a><span data-ttu-id="9e6f0-1219">Build 14951</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1219">Build 14951</span></span>

<span data-ttu-id="9e6f0-1220">Allgemeine Windows-Informationen zu Build 14951 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1220">For general Windows information on build 14951 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/19/announcing-windows-10-insider-preview-build-14951-for-mobile-and-pc/).</span></span><br/>


### <a name="new-feature-windows--ubuntu-interoperability"></a><span data-ttu-id="9e6f0-1221">Neues Feature: Windows-/Ubuntu-Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1221">New Feature: Windows / Ubuntu Interoperability</span></span>
<span data-ttu-id="9e6f0-1222">Windows-Binärdateien können jetzt direkt über die WSL-Befehlszeile aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1222">Windows binaries can now be invoked directly from the WSL command line.</span></span>  <span data-ttu-id="9e6f0-1223">Dadurch haben Benutzer die Möglichkeit, mit Ihrer Windows-Umgebung und dem -System auf eine Weise zu interagieren, die bisher nicht möglich war.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1223">This gives users the ability to interact with their Windows environment and system in a way that has not been possible.</span></span>  <span data-ttu-id="9e6f0-1224">Als kurzes Beispiel können Benutzer nun die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1224">As a quick example, it is now possible for users to run the following commands:</span></span>

    ```
    $ export PATH=$PATH:/mnt/c/Windows/System32
    $ notepad.exe
    $ ipconfig.exe | grep IPv4 | cut -d: -f2
    $ ls -la | findstr.exe foo.txt
    $ cmd.exe /c dir
    ```

<span data-ttu-id="9e6f0-1225">Weitere Informationen finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1225">More information can be found at:</span></span>

- [<span data-ttu-id="9e6f0-1226">WSL-Teamblog für Interop</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1226">WSL Team Blog for Interop</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)<br/>
- [<span data-ttu-id="9e6f0-1227">MSDN-Interop-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1227">MSDN Interop Documentation</span></span>](https://msdn.microsoft.com/en-us/commandline/wsl/interop)<br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1228">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1228">Fixed</span></span>

- <span data-ttu-id="9e6f0-1229">Ubuntu 16.04 (Xenial) wird jetzt für alle neuen WSL-Instanzen installiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1229">Ubuntu 16.04 (Xenial) is now installed for all new WSL instances.</span></span>  <span data-ttu-id="9e6f0-1230">Benutzer mit vorhandenen 14.04-Instanzen (Trusty) erhalten kein automatisches Upgrade.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1230">Users with existing 14.04 (Trusty) instances will not be automatically upgraded.</span></span>
- <span data-ttu-id="9e6f0-1231">Das während der Installation festgelegte Gebietsschema wird jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1231">Locale set during install is now displayed</span></span>
- <span data-ttu-id="9e6f0-1232">Terminalverbesserungen, einschließlich des Fehlers bei der Umleitung eines WSL-Prozesses an eine Datei, funktionieren nicht immer</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1232">Terminal improvements including bug where redirecting a WSL process to a file does not always work</span></span>
- <span data-ttu-id="9e6f0-1233">Die Konsolenlebensdauer muss an die Lebensdauer von „bash.exe“ gebunden sein</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1233">Console lifetime should be tied to bash.exe lifetime</span></span>
- <span data-ttu-id="9e6f0-1234">Die Größe des Konsolenfensters sollte die sichtbare Größe und nicht die Puffergröße verwenden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1234">Console window size should use visible size, not buffer size</span></span>
- <span data-ttu-id="9e6f0-1235">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1235">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1236">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1236">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1237">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1237">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9e6f0-1238">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1238">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1239">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1239">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14951)<br/>

<br/>

## <a name="build-14946"></a><span data-ttu-id="9e6f0-1240">Build 14946</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1240">Build 14946</span></span>

<span data-ttu-id="9e6f0-1241">Allgemeine Windows-Informationen zu Build 14946 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1241">For general Windows information on build 14946 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/10/13/announcing-windows-10-insider-preview-build-14946-for-pc-and-mobile/#xj8GdVooEqo4H7H7.97).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1242">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1242">Fixed</span></span>

- <span data-ttu-id="9e6f0-1243">Korrektur eines Problems, das das Erstellen von WSL-Benutzerkonten für Benutzer mit NT-Benutzernamen verhindert hat, die Leerzeichen oder Anführungszeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1243">Fixed an issue that prevented creating WSL user accounts for users with NT usernames that contain spaces or quotes.</span></span> 
- <span data-ttu-id="9e6f0-1244">Änderung von VolFs und DrvFs, damit 0 für die Verknüpfungsanzahl des Verzeichnisses im Status zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1244">Change VolFs and DrvFs to return 0 for directory's link count in stat</span></span>
- <span data-ttu-id="9e6f0-1245">Unterstützung der IPV6_MULTICAST_HOPS-Socketoption.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1245">Support IPV6_MULTICAST_HOPS socket option.</span></span>
- <span data-ttu-id="9e6f0-1246">Einschränkung auf eine einzige Konsolen-E/A-Schleife pro TTY.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1246">Limit to a single console I/O loop per tty.</span></span> <span data-ttu-id="9e6f0-1247">Der folgende Befehl ist beispielsweise möglich:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1247">Example: the following command is possible:</span></span>
  - <span data-ttu-id="9e6f0-1248">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1248">bash -c "echo data" | bash -c "ssh user@example.com 'cat > foo.txt'"</span></span>

- <span data-ttu-id="9e6f0-1249">Ersetzen von Leerzeichen durch Tabstoppzeichen in /proc/cpuinfo (GH #1115)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1249">replace spaces with tabs in /proc/cpuinfo (GH #1115)</span></span>
- <span data-ttu-id="9e6f0-1250">DrvFs wird jetzt in den Einbindungsinformationen mit einem Namen angezeigt, der dem eingebundenen Windows-Volume entspricht</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1250">DrvFs now appears in mountinfo with a name that matches mounted Windows volume</span></span>
- <span data-ttu-id="9e6f0-1251">/home und/root werden nun in den Einbindungsinformationen mit den richtigen Namen angezeigt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1251">/home and /root now appear in mountinfo with correct names</span></span>
- <span data-ttu-id="9e6f0-1252">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1252">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1253">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1253">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1254">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1254">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9e6f0-1255">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1255">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1256">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1256">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14946)<br/>

<br/>

## <a name="build-14942"></a><span data-ttu-id="9e6f0-1257">Build 14942</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1257">Build 14942</span></span>

<span data-ttu-id="9e6f0-1258">Allgemeine Windows-Informationen zu Build 14942 finden Sie im [Windows-Blog](https://aka.ms/onefourninefourtwoooooo).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1258">For general Windows information on build 14942 visit the [Windows Blog](https://aka.ms/onefourninefourtwoooooo).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1259">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1259">Fixed</span></span>

- <span data-ttu-id="9e6f0-1260">Eine Reihe von Fehlerüberprüfungen, einschließlich des Netzwerkabsturzes durch „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“, der SSH blockiert hat</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1260">A number of bugchecks addressed, including the “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY” networking crash which was blocking SSH</span></span>
- <span data-ttu-id="9e6f0-1261">inotify-Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1261">inotifiy support for notifications generated from Windows applications on DrvFs is now in</span></span>
- <span data-ttu-id="9e6f0-1262">Implementierung von TCP_KEEPIDLE und TCP_KEEPINTVL für mongod.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1262">Implement TCP_KEEPIDLE and TCP_KEEPINTVL for mongod.</span></span> <span data-ttu-id="9e6f0-1263">(GH #695)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1263">(GH #695)</span></span>
- <span data-ttu-id="9e6f0-1264">Implementierung des pivot_root-Systemaufrufs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1264">Implement the pivot_root system call</span></span>
- <span data-ttu-id="9e6f0-1265">Implementierung der Socketoption für SO_DONTROUTE</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1265">Implement socket option for SO_DONTROUTE</span></span>
- <span data-ttu-id="9e6f0-1266">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1266">Additional bugfixes and improvements</span></span>


### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1267">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1267">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1268">Anzahl bestandener Tests: 665</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1268">Number of Passing Test: 665</span></span> </br>
<span data-ttu-id="9e6f0-1269">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 263</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1269">Number of non-Passing (failing, skipped, etc…): 263</span></span> </br>
[<span data-ttu-id="9e6f0-1270">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1270">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14942)<br/>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1271">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1271">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1272">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1272">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1273">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1273">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`pivot_root`<br/>
<br/>

## <a name="build-14936"></a><span data-ttu-id="9e6f0-1274">Build 14936</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1274">Build 14936</span></span>

<span data-ttu-id="9e6f0-1275">Allgemeine Windows-Informationen zu Build 14936 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1275">For general Windows information on build 14936 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/28/announcing-windows-10-insider-preview-build-14936-for-pc/).</span></span><br/>


<span data-ttu-id="9e6f0-1276">Hinweis: WSL wird in einem zukünftigen Release Ubuntu Version 16.04 (Xenial) anstelle von Ubuntu 14.04 (Trusty) installieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1276">Note: WSL will install Ubuntu version 16.04 (Xenial) instead of Ubuntu 14.04 (Trusty) in an upcoming release.</span></span>  <span data-ttu-id="9e6f0-1277">Diese Änderung gilt für Insider, die neue Instanzen installieren (lxrun.exe /install oder erste Ausführung von „bash.exe“).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1277">This change will apply to Insiders installing new instances (lxrun.exe /install or first run of bash.exe).</span></span>  <span data-ttu-id="9e6f0-1278">Vorhandene Instanzen mit Trusty werden nicht automatisch aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1278">Existing instances with Trusty will not be upgraded automatically.</span></span> <span data-ttu-id="9e6f0-1279">Benutzer können mit dem Befehl „do-release-upgrade“ Ihr Trusty-Image auf Xenial aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1279">Users can upgrade their Trusty image to Xenial using the do-release-upgrade command.</span></span>

### <a name="known-issue"></a><span data-ttu-id="9e6f0-1280">Bekanntes Problem</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1280">Known Issue</span></span>
<span data-ttu-id="9e6f0-1281">Bei WSL treten Probleme mit einigen Socketimplementierungen auf.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1281">WSL is experiencing an issue with some socket implementations.</span></span>  <span data-ttu-id="9e6f0-1282">Die Fehlerüberprüfung manifestiert sich als Absturz mit dem Fehler „ATTEMPTED EXECUTE OF NOEXECUTE MEMORY“.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1282">The bugcheck manifests itself as a crash with the error “ATTEMPTED EXECUTE OF NOEXECUTE MEMORY”.</span></span>  <span data-ttu-id="9e6f0-1283">Die häufigste Variante dieses Problems ist ein Absturz bei der Verwendung von SSH.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1283">The most common manifestation of this issue is a crash when using ssh.</span></span>  <span data-ttu-id="9e6f0-1284">Die Ursache ist bei internen Builds korrigiert und wird so bald wie möglich in Insider gepusht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1284">The root cause is fixed on internal builds and will be pushed to Insiders at the earliest opportunity.</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1285">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1285">Fixed</span></span>

- <span data-ttu-id="9e6f0-1286">Der chroot-Systemaufruf wurde implementiert.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1286">Implemented the chroot system call</span></span>
- <span data-ttu-id="9e6f0-1287">Verbesserungen in inotify ~~einschließlich Unterstützung für Benachrichtigungen, die von Windows-Anwendungen auf DrvFs generiert werden~~</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1287">Improvements in inotify ~~including support for notifications generated from Windows applications on DrvFs~~</span></span>
  - <span data-ttu-id="9e6f0-1288">Korrektur: Inotify-Unterstützung von Änderungen, die von Windows-Anwendungen stammen, ist zurzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1288">Correction: Inotify support for changes originating from Windows applications not available at this time.</span></span>
- <span data-ttu-id="9e6f0-1289">Die Socketbindung an IPv6::<port n> unterstützt jetzt IPV6_V6ONLY (GH #68, #157, #393, #460, #674, #740, #982, #996)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1289">Socket binding to IPV6::<port n> now supports IPV6_V6ONLY  (GH #68, #157, #393, #460, #674, #740, #982, #996)</span></span>
- <span data-ttu-id="9e6f0-1290">Implementierung des WNOWAIT-Verhaltens für den waitid-Systemaufruf (GH #638)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1290">WNOWAIT behavior for waitid systemcall implemented (GH #638)</span></span>
- <span data-ttu-id="9e6f0-1291">Unterstützung für IP-Socketoptionen IP_HDRINCL und IP_TTL</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1291">Support for IP socket options IP_HDRINCL and IP_TTL</span></span>
- <span data-ttu-id="9e6f0-1292">read() der Länge Null sollte sofort zurückgegeben werden (GH #975)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1292">Zero-length read() should return immediately (GH #975)</span></span>
- <span data-ttu-id="9e6f0-1293">Ordnungsgemäße Verarbeitung von Dateinamen und Dateinamenpräfixen, die keinen NULL-Terminator in einer TAR-Datei enthalten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1293">Correctly handle filenames and filename prefixes that don't include a NULL terminator in a .tar file.</span></span>
- <span data-ttu-id="9e6f0-1294">epoll-Unterstützung für/dev/null</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1294">epoll support for /dev/null</span></span>
- <span data-ttu-id="9e6f0-1295">Korrektur der /dev/alarm-Zeitquelle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1295">Fix /dev/alarm time source</span></span>
- <span data-ttu-id="9e6f0-1296">Bash -c kann nun in eine Datei umgeleitet werden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1296">Bash -c now able to redirect to a file</span></span>
- <span data-ttu-id="9e6f0-1297">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1297">Additional bugfixes and improvements</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1298">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1298">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1299">Anzahl bestandener Tests: 664</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1299">Number of Passing Test: 664</span></span> </br>
<span data-ttu-id="9e6f0-1300">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 264</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1300">Number of non-Passing (failing, skipped, etc…): 264</span></span> </br>
[<span data-ttu-id="9e6f0-1301">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1301">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14936)<br/>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1302">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1302">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1303">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1303">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1304">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1304">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`chroot`<br/>
<br/>

## <a name="build-14931"></a><span data-ttu-id="9e6f0-1305">Build 14931</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1305">Build 14931</span></span>

<span data-ttu-id="9e6f0-1306">Allgemeine Windows-Informationen zu Build 14931 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1306">For general Windows information on build 14931 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/21/announcing-windows-10-insider-preview-build-14931-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1307">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1307">Fixed</span></span>

 - <span data-ttu-id="9e6f0-1308">Aufgrund von Umständen, die sich unserer Kontrolle entziehen, gibt es in diesem Build keine Updates für das Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1308">Due to circumstances beyond our control there are no updates in this build for the Windows Subsystem for Linux.</span></span>  <span data-ttu-id="9e6f0-1309">Regelmäßig geplante Updates werden mit dem nächsten Release fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1309">Regularly scheduled updates will resume in the next release.</span></span>

<br/>

## <a name="build-14926"></a><span data-ttu-id="9e6f0-1310">Build 14926</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1310">Build 14926</span></span>

<span data-ttu-id="9e6f0-1311">Allgemeine Windows-Informationen zu Build 14926 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1311">For general Windows information on build 14926 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/09/14/announcing-windows-10-insider-preview-build-14926-for-pc-and-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1312">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1312">Fixed</span></span>

- <span data-ttu-id="9e6f0-1313">Ping funktioniert nun in Konsolen, die nicht über Administratorberechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1313">Ping now works in consoles which do not have administrator privileges</span></span>
- <span data-ttu-id="9e6f0-1314">Ping6 wird jetzt auch ohne Administratorberechtigungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1314">Ping6 now supported, also without administrator privileges</span></span>
- <span data-ttu-id="9e6f0-1315">Inotify-Unterstützung für Dateien, die über WSL geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1315">Inotify support for files modified through WSL.</span></span> <span data-ttu-id="9e6f0-1316">(GH #216)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1316">(GH #216)</span></span>
  - <span data-ttu-id="9e6f0-1317">Unterstützte Flags:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1317">Flags supported:</span></span>
    - <span data-ttu-id="9e6f0-1318">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1318">inotify_init1: LX_O_CLOEXEC, LX_O_NONBLOCK</span></span>
    - <span data-ttu-id="9e6f0-1319">inotify_add_watchEreignisse: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1319">inotify_add_watch events: LX_IN_ACCESS, LX_IN_MODIFY, LX_IN_ATTRIB, LX_IN_CLOSE_WRITE, LX_IN_CLOSE_NOWRITE, LX_IN_OPEN, LX_IN_MOVED_FROM, LX_IN_MOVED_TO, LX_IN_CREATE, LX_IN_DELETE, LX_IN_DELETE_SELF, LX_IN_MOVE_SELF</span></span>
    - <span data-ttu-id="9e6f0-1320">inotify_add_watch-Attribute: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1320">inotify_add_watch attributes: LX_IN_DONT_FOLLOW, LX_IN_EXCL_UNLINK, LX_IN_MASK_ADD, LX_IN_ONESHOT, LX_IN_ONLYDIR</span></span>
    - <span data-ttu-id="9e6f0-1321">Lesen der Ausgabe: LX_IN_ISDIR, LX_IN_IGNORED</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1321">read output: LX_IN_ISDIR, LX_IN_IGNORED</span></span>
  - <span data-ttu-id="9e6f0-1322">Bekanntes Problem: Durch das Ändern von Dateien aus Windows-Anwendungen werden keine Ereignisse generiert</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1322">Known issue: Modifying files from Windows applications does not generate any events</span></span>
- <span data-ttu-id="9e6f0-1323">Unix-Socket unterstützt jetzt SCM_CREDENTIALS</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1323">Unix socket now supports SCM_CREDENTIALS</span></span>

### <a name="ltp-results"></a><span data-ttu-id="9e6f0-1324">LTP-Ergebnisse:</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1324">LTP Results:</span></span>
<span data-ttu-id="9e6f0-1325">Anzahl bestandener Tests: 651</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1325">Number of Passing Test: 651</span></span> </br>
<span data-ttu-id="9e6f0-1326">Anzahl nicht bestandener Tests (fehlerhaft, übersprungen usw.): 258</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1326">Number of non-Passing (failing, skipped, etc…): 258</span></span> </br>
[<span data-ttu-id="9e6f0-1327">LTP-Testlaufprotokolle</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1327">LTP Test Run Logs</span></span>](https://github.com/Microsoft/CommandLine-Documentation/tree/live/LTP_Results/14926)<br/>

<br/>

## <a name="build-14915"></a><span data-ttu-id="9e6f0-1328">Build 14915</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1328">Build 14915</span></span>

<span data-ttu-id="9e6f0-1329">Allgemeine Windows-Informationen zu Build 14915 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1329">For general Windows information on build 14915 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/31/announcing-windows-10-insider-preview-build-14915-for-pc-and-mobile).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1330">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1330">Fixed</span></span>
-  <span data-ttu-id="9e6f0-1331">Socketpair für Unix-Datagrammsockets (GH #262)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1331">Socketpair for unix datagram sockets (GH #262)</span></span>
- <span data-ttu-id="9e6f0-1332">Unix-Socketunterstützung für SO_REUSEADDR</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1332">Unix socket support for SO_REUSEADDR</span></span>
- <span data-ttu-id="9e6f0-1333">Unix-Socketunterstützung für SO_BROADCAST (GH #568)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1333">UNIX socket support for SO_BROADCAST (GH #568)</span></span>
- <span data-ttu-id="9e6f0-1334">Unix-Socketunterstützung für SOCK_SEQPACKET (GH #758, #546)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1334">Unix socket support for SOCK_SEQPACKET (GH #758, #546)</span></span>
- <span data-ttu-id="9e6f0-1335">Hinzufügen von Unterstützung für unix datagram socket send, recv und shutdown</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1335">Adding support for unix datagram socket send, recv and shutdown</span></span>
- <span data-ttu-id="9e6f0-1336">Korrektur einer Fehlerüberprüfung aufgrund einer ungültigen Überprüfung des mmap-Parameters für nicht feste Adressen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1336">Fix bugcheck due to invalid mmap parameter validation for non-fixed addresses.</span></span> <span data-ttu-id="9e6f0-1337">(GH #847)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1337">(GH #847)</span></span>
- <span data-ttu-id="9e6f0-1338">Unterstützung für das Anhalten/Fortsetzen von Terminalzuständen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1338">Support for suspend / resume of terminal states</span></span>
- <span data-ttu-id="9e6f0-1339">Unterstützung für TIOCPKT ioctl zum Entsperren des Bildschirmhilfsprogramms (GH #774)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1339">Support for TIOCPKT ioctl to unblock the Screen utility (GH #774)</span></span>
    - <span data-ttu-id="9e6f0-1340">Bekanntes Problem: Funktionstasten sind nicht funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1340">Known issue: Function keys not operational</span></span>
- <span data-ttu-id="9e6f0-1341">Korrektur einer Racebedingung in TimerFd, die dazu führen konnte, dass auf einen freigegebenen Member „ReaderReady“ durch LxpTimerFdWorkerRoutine zugegriffen wurde (GH #814)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1341">Corrected a race in TimerFd that could cause a freed member 'ReaderReady' to be accessed by LxpTimerFdWorkerRoutine (GH #814)</span></span>
- <span data-ttu-id="9e6f0-1342">Aktivieren der Unterstützung für erneut startbaren Systemaufruf für futex, poll und clock_nanosleep</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1342">Enable restartable system call support for futex, poll, and clock_nanosleep</span></span>
- <span data-ttu-id="9e6f0-1343">Hinzufügen von Unterstützung für Bindungseinbindung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1343">Added bind mount support</span></span>
- <span data-ttu-id="9e6f0-1344">Unterstützung für Aufheben der Freigabe für Einbindungsnamespace</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1344">unshare for mount namespace support</span></span>
    - <span data-ttu-id="9e6f0-1345">Bekanntes Problem: Beim Erstellen eines neuen Einbindngsnamespace mit `unshare(CLONE_NEWNS)` zeigt das aktuelle Arbeitsverzeichnis weiterhin auf den alten Namespace</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1345">Known issue: When creating a new mount namespace with `unshare(CLONE_NEWNS)` the current working directory will continue to point to the old namespace</span></span>
- <span data-ttu-id="9e6f0-1346">Weitere Verbesserungen und Fehlerbehebungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1346">Additional improvements and bug fixes</span></span>

<br/>

## <a name="build-14905"></a><span data-ttu-id="9e6f0-1347">Build 14905</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1347">Build 14905</span></span>

<span data-ttu-id="9e6f0-1348">Allgemeine Windows-Informationen zu Build 14905 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1348">For general Windows information on build 14905 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/17/announcing-windows-10-insider-preview-build-14905-for-pc-mobile/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1349">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1349">Fixed</span></span>
- <span data-ttu-id="9e6f0-1350">Erneut startbare Systemaufrufe werden jetzt unterstützt (GH #349, GH #520)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1350">Restartable system calls are now supported (GH #349, GH #520)</span></span>
- <span data-ttu-id="9e6f0-1351">Symbolische Verknüpfungen mit Verzeichnissen, die auf / wenden, sind jetzt funktionstüchtig (GH #650)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1351">Symlinks to directories ending in / now operational (GH #650)</span></span>
- <span data-ttu-id="9e6f0-1352">Implementierung von RNDGETENTCNT ioctl für „/dev/random“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1352">Implemented RNDGETENTCNT ioctl for /dev/random</span></span>
- <span data-ttu-id="9e6f0-1353">Implementierung der /proc/[pid]/mounts, /proc/[pid]/mountinfo- und /proc/[pid]/mountstats-Dateien</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1353">Implemented the /proc/[pid]/mounts, /proc/[pid]/mountinfo and /proc/[pid]/mountstats files</span></span>
- <span data-ttu-id="9e6f0-1354">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1354">Additional bugfixes and improvements</span></span>

</br>

## <a name="build-14901"></a><span data-ttu-id="9e6f0-1355">Build 14901</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1355">Build 14901</span></span>
<span data-ttu-id="9e6f0-1356">Der erste Insider-Build für das Windows 10 Anniversary Update-Release.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1356">First Insider build for the post Windows 10 Anniversary Update release.</span></span>

<span data-ttu-id="9e6f0-1357">Allgemeine Windows-Informationen zu Build 14901 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1357">For general Windows information on build 14901 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/08/11/announcing-windows-10-insider-preview-build-14901-for-pc/).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1358">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1358">Fixed</span></span>
- <span data-ttu-id="9e6f0-1359">Korrektur eines Problems mit nachfolgenden Schrägstrichen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1359">Fixed trailing slash issue</span></span>
    - <span data-ttu-id="9e6f0-1360">Befehle wie `$ mv a/c/ a/b/` funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1360">Commands such as `$ mv a/c/ a/b/` now work</span></span>
- <span data-ttu-id="9e6f0-1361">Installation von Eingabeaufforderungen, wenn das Ubuntu-Gebietsschema auf das Windows-Gebietsschema festgelegt werden soll</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1361">Installing now prompts if Ubuntu locale should be set to Windows locale</span></span>
- <span data-ttu-id="9e6f0-1362">Procfs-Unterstützung für den Ordner „ns“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1362">Procfs support for ns folder</span></span>
- <span data-ttu-id="9e6f0-1363">Hinzufügen von „mount“ und „unmount“ für tmpfs-, procfs-und sysfs-Dateisysteme</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1363">Added mount and unmount for tmpfs, procfs and sysfs file systems</span></span>
- <span data-ttu-id="9e6f0-1364">Korrektur der 32-Bit-ABI-Signatur von mklod [at]</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1364">Fix mknod[at] 32-bit ABI signature</span></span>
- <span data-ttu-id="9e6f0-1365">Verschieben von Unix-Sockets in Dispatchmodell</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1365">Unix sockets moved to dispatch model</span></span>
- <span data-ttu-id="9e6f0-1366">Mit setsockopt festgelegte recv-Puffergröße von INET-Socket muss berücksichtigt werden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1366">INET socket recv buffer size set using the setsockopt should be honored</span></span>
- <span data-ttu-id="9e6f0-1367">Implementierung des MSG_CMSG_CLOEXEC-Unis-Socket-Empfangsnachrichtenflags</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1367">Implement MSG_CMSG_CLOEXEC unix socket receive message flag</span></span>
- <span data-ttu-id="9e6f0-1368">stdin/stdout-Pipeumleitung des Linux-Prozesses (GH #2)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1368">Linux process stdin/stdout pipe redirection (GH #2)</span></span>
    - <span data-ttu-id="9e6f0-1369">Ermöglicht das Weiterleiten von bash -c-Befehlen in CMD.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1369">Allows for piping of bash -c commands in CMD.</span></span>  <span data-ttu-id="9e6f0-1370">Beispiel: >dir | bash -c "grep foo"</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1370">Example:  >dir | bash -c "grep foo"</span></span>
- <span data-ttu-id="9e6f0-1371">Bash kann nun auf Systemen mit mehreren Auslagerungsdateien installiert werden (GH #538, #358)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1371">Bash can now be installed on systems with multiple pagefiles (GH #538, #358)</span></span>
- <span data-ttu-id="9e6f0-1372">Standardpuffergröße des INET-Sockets sollte mit der Größe des Ubuntu- Standardsetups übereinstimmen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1372">Default INET Socket buffer size should match that of default Ubuntu setup</span></span>
- <span data-ttu-id="9e6f0-1373">Ausrichten von xattr-Systemaufrufen an listxattr</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1373">Align xattr syscalls to listxattr</span></span>
- <span data-ttu-id="9e6f0-1374">Nur Rückgabe von Schnittstellen mit einer gültigen IPv4-Adresse von SIOCGIFCONF</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1374">Only return interfaces with a valid IPv4 address from SIOCGIFCONF</span></span>
- <span data-ttu-id="9e6f0-1375">Korrektur der Signalatandardaktion, wenn von ptrace eingefügt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1375">Fix signal default action when injected by ptrace</span></span>
- <span data-ttu-id="9e6f0-1376">Implementierung von /proc/sys/vm/min_free_kbytes</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1376">implement /proc/sys/vm/min_free_kbytes</span></span>
- <span data-ttu-id="9e6f0-1377">Verwenden der Computerkontext-Registerwerte beim Wiederherstellen von Kontext in sigreturn</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1377">Use machine context register values when restoring context in sigreturn</span></span>
    - <span data-ttu-id="9e6f0-1378">Dadurch wird das Problem behoben, dass Java und javac bei einigen Benutzern nicht mehr reagiert haben</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1378">This resolves the issue where java and javac were hanging for some users</span></span>
- <span data-ttu-id="9e6f0-1379">Implementierung von /proc/sys/kernel/hostname</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1379">Implement /proc/sys/kernel/hostname</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1380">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1380">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1381">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1381">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1382">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1382">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`waitid`<br/>
`epoll_pwait`<br/>

<br/>

## <a name="build-14388-to-windows-10-anniversary-update"></a><span data-ttu-id="9e6f0-1383">Update von Build 14388 auf Windows 10 Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1383">Build 14388 to Windows 10 Anniversary Update</span></span>
<span data-ttu-id="9e6f0-1384">Allgemeine Windows-Informationen zu Build 14388 finden Sie im [Windows-Blog](https://aka.ms/14388wip).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1384">For general Windows information on build 14388 visit the [Windows Blog](https://aka.ms/14388wip).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1385">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1385">Fixed</span></span>
- <span data-ttu-id="9e6f0-1386">Korrekturen als Vorbereitung auf das Windows 10 Anniversary Update am 02.08.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1386">Fixes to prepare for the Windows 10 Anniversary Update on 8/2</span></span>
  - <span data-ttu-id="9e6f0-1387">Weitere Informationen zu WSL im Anniversary Update finden Sie in unserem [Blog](https://blogs.msdn.microsoft.com/wsl/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1387">More information about WSL in the Anniversary Update can be found on our [blog](https://blogs.msdn.microsoft.com/wsl/)</span></span>

<br/>

## <a name="build-14376"></a><span data-ttu-id="9e6f0-1388">Build 14376</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1388">Build 14376</span></span>
<span data-ttu-id="9e6f0-1389">Allgemeine Windows-Informationen zu Build 14376 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1389">For general Windows information on build 14376 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/28/announcing-windows-10-insider-preview-build-14376-for-pc-and-mobile/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1390">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1390">Fixed</span></span>
- <span data-ttu-id="9e6f0-1391">Entfernen einiger Instanzen, in denen apt-get nicht mehr reagiert (GH #493)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1391">Removed some instances where apt-get hangs (GH #493)</span></span>
- <span data-ttu-id="9e6f0-1392">Korrektur eines Problems, bei dem leere Einbindungen nicht ordnungsgemäß verarbeitet wurden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1392">Fixed an issue where empty mounts were not handled correctly</span></span>
- <span data-ttu-id="9e6f0-1393">Korrektur eines Problems, bei dem Ramdisks nicht ordnungsgemäß eingebunden wurden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1393">Fixed an issue where ramdisks were not mounted correctly</span></span>
- <span data-ttu-id="9e6f0-1394">Änderung von „unix socket accept“ für die Unterstützung von Flags (Teil von GH #451)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1394">Change unix socket accept to support flags (partial GH #451)</span></span>
- <span data-ttu-id="9e6f0-1395">Korrektur eines allgemeinen netzwerkbezogenen Bluescreens</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1395">Fixed common network related bluescreen</span></span>
- <span data-ttu-id="9e6f0-1396">Korrektur des Bluescreens beim Zugriff auf /proc/[pid]/task (GH #523)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1396">Fixed bluescreen when accessing /proc/[pid]/task (GH #523)</span></span>
- <span data-ttu-id="9e6f0-1397">Korrektur hoher CPU-Auslastung für einige Pty-Szenarien (GH #488, #504)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1397">Fixed high CPU utilization for some pty scenarios (GH #488, #504)</span></span>
- <span data-ttu-id="9e6f0-1398">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1398">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14371"></a><span data-ttu-id="9e6f0-1399">Build 14371</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1399">Build 14371</span></span>
<span data-ttu-id="9e6f0-1400">Allgemeine Windows-Informationen zu Build 14371 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1400">For general Windows information on build 14371 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/22/announcing-windows-10-insider-preview-build-14371-for-pc/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1401">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1401">Fixed</span></span>
- <span data-ttu-id="9e6f0-1402">Korrektur der Timingracebedingung mit SIGCHLD und wait() bei Verwendung von ptrace</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1402">Corrected timing race with SIGCHLD and wait() when using ptrace</span></span>
- <span data-ttu-id="9e6f0-1403">Korrektur von Verhalten, wenn Pfade ein nachfolgendes Zeichen / aufweisen (GH #432)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1403">Corrected some behavior when paths have a trailing /  (GH #432)</span></span>
- <span data-ttu-id="9e6f0-1404">Korrektur eines Problems, bei dem Umbenennen/Aufheben der Verknüpfung aufgrund von geöffneten Handles für untergeordnete Elemente fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1404">Fixed issue with rename/unlink failing due to open handles to children</span></span>
- <span data-ttu-id="9e6f0-1405">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1405">Additional bugfixes and improvements</span></span>

<br/>

## <a name="build-14366"></a><span data-ttu-id="9e6f0-1406">Build 14366</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1406">Build 14366</span></span>
<span data-ttu-id="9e6f0-1407">Allgemeine Windows-Informationen zu Build 14366 finden Sie im [Windows-Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1407">For general Windows information on build 14366 visit the [Windows Blog](https://blogs.windows.com/windowsexperience/2016/06/14/announcing-windows-10-insider-preview-build-14366-mobile-build-14364/).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1408">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1408">Fixed</span></span>
- <span data-ttu-id="9e6f0-1409">Korrektur der Dateierstellung durch symbolische Verknüpfungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1409">Fix in file creation through symlinks</span></span>
-   <span data-ttu-id="9e6f0-1410">Hinzugefügter von listxattr für Python (GH 385)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1410">Added listxattr for Python (GH 385)</span></span>
-   <span data-ttu-id="9e6f0-1411">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1411">Additional bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1412">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1412">Syscall Support</span></span>
-   <span data-ttu-id="9e6f0-1413">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1413">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1414">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1414">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`listxattr`<br/>
<br/>

## <a name="build-14361"></a><span data-ttu-id="9e6f0-1415">Build 14361</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1415">Build 14361</span></span>
<span data-ttu-id="9e6f0-1416">Allgemeine Windows-Informationen zu Build 14361 finden Sie im [Windows-Blog](https://aka.ms/wip14361).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1416">For general Windows information on build 14361 visit the [Windows Blog](https://aka.ms/wip14361).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1417">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1417">Fixed</span></span>
- <span data-ttu-id="9e6f0-1418">Für DrvFs wird nun bei der Ausführung in Bash unter Ubuntu unter Windows die Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1418">DrvFs is now case sensitive when running in Bash on Ubuntu on Windows.</span></span>
  - <span data-ttu-id="9e6f0-1419">Benutzer können case.txt und CASE.TXT auf Ihren /mnt/c-Laufwerken verwenden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1419">Users may case.txt and CASE.TXT on their /mnt/c drives</span></span>
  - <span data-ttu-id="9e6f0-1420">Die Beachtung von Groß-/Kleinschreibung wird nur in Bash unter Ubuntu unter Windows unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1420">Case sensitivity is only supported within Bash on Ubuntu on Windows.</span></span> <span data-ttu-id="9e6f0-1421">Außerhalb von Bash zeigt NTFS die Dateien richtig an, aber es kann zu unerwartetem Verhalten bei der Interaktion mit den Dateien von Windows kommen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1421">When outside of Bash NTFS will report the files correctly, but unexpected behavior may occur interacting with the files from Windows.</span></span>
  - <span data-ttu-id="9e6f0-1422">Für den Stamm der einzelnen Volumes (d.h. /mnt/c) wird die Groß-/Kleinschreibung nicht beachtet.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1422">The root of each volume (i.e. /mnt/c) is not case sensitive</span></span>
  - <span data-ttu-id="9e6f0-1423">Weitere Informationen zum Verarbeiten dieser Dateien in Windows finden Sie [hier](https://support.microsoft.com/en-us/kb/100625).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1423">More information on handling these files in Windows can be found [here](https://support.microsoft.com/en-us/kb/100625).</span></span>
- <span data-ttu-id="9e6f0-1424">Stark verbesserte PTY-/TTY-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1424">Greatly enhanced pty / tty support.</span></span>  <span data-ttu-id="9e6f0-1425">Anwendungen wie TMUX werden jetzt unterstützt (GH #40)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1425">Applications like TMUX now supported (GH #40)</span></span>
- <span data-ttu-id="9e6f0-1426">Korrektur eines Installationsproblems, bei dem Benutzerkonten nicht immer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1426">Fixed install issue where user accounts not always created</span></span>
- <span data-ttu-id="9e6f0-1427">Optimierte Befehlszeilen-Argumentstruktur, die eine extrem lange Argumentliste zulässt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1427">Optimized command line arg structure allowing for extremely long argument list.</span></span> <span data-ttu-id="9e6f0-1428">(GH #153)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1428">(GH #153)</span></span>
- <span data-ttu-id="9e6f0-1429">Jetzt können chmod read_only-Dateien aus DrvFs gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1429">Now able to delete and chmod read_only files from DrvFs</span></span>
- <span data-ttu-id="9e6f0-1430">Korrektur einiger Instanzen, bei denen das Terminal beim Trennen nicht mehr reagiert (GH #43)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1430">Fixed some instances where the terminal hangs on disconnect (GH #43)</span></span>
- <span data-ttu-id="9e6f0-1431">chmod und chown funktionieren jetzt auf TTY-Geräten</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1431">chmod and chown now work on tty devices</span></span>
- <span data-ttu-id="9e6f0-1432">Verbindung mit 0.0.0.0 und :: as localhost zulassen (GH #388)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1432">Allow connection to 0.0.0.0 and :: as localhost (GH #388)</span></span>
- <span data-ttu-id="9e6f0-1433">Sendmsg/recvmsg verarbeitet nun eine E/A-Vektorlänge > 1 (Teil von GH #376)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1433">Sendmsg/recvmsg now handle an IO vector length of >1 (partial GH #376)</span></span>
- <span data-ttu-id="9e6f0-1434">Benutzer können jetzt die automatisch generierte Hostdatei ablehnen (GH #398)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1434">Users can now opt-out of auto-generated hosts file (GH #398)</span></span>
- <span data-ttu-id="9e6f0-1435">Automatisches Zuordnen des Linux-Gebietsschemas zum NT-Gebietsschema während der Installation (GH #11)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1435">Automatically match Linux locale to the NT locale during install (GH #11)</span></span>
- <span data-ttu-id="9e6f0-1436">Hinzufügen der /proc/sys/vm/swappiness-Datei (GH #306)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1436">Added the /proc/sys/vm/swappiness file (GH #306)</span></span>
- <span data-ttu-id="9e6f0-1437">strace wird jetzt ordnungsgemäß beendet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1437">strace now exits correctly</span></span>
- <span data-ttu-id="9e6f0-1438">Ermöglichen des erneuten Öffnens von Pipes über /proc/self/fd (GH #222)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1438">Allow pipes to be reopened through /proc/self/fd (GH #222)</span></span>
- <span data-ttu-id="9e6f0-1439">Ausblenden von Verzeichnissen unter „%LOCALAPPDATA%\lxss“ aus DrvFs (GH #270)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1439">Hide directories under %LOCALAPPDATA%\lxss from DrvFs (GH #270)</span></span>
- <span data-ttu-id="9e6f0-1440">Bessere Verarbeitung von bash.exe ~.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1440">Better handling of bash.exe ~.</span></span>  <span data-ttu-id="9e6f0-1441">Befehle wie „bash ~ -c ls“ werden jetzt unterstützt (GH #467)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1441">Commands like “bash ~ -c ls” now supported (GH #467)</span></span>
- <span data-ttu-id="9e6f0-1442">Sockets benachrichtigen nun darüber, dass epoll read beim Herunterfahren verfügbar ist (GH #271)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1442">Sockets now notify epoll read available during shutdown (GH #271)</span></span>
- <span data-ttu-id="9e6f0-1443">lxrun/uninstall arbeitet besser beim Löschen der Dateien und Ordner.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1443">lxrun /uninstall does a better job of deleting the files and folders</span></span>
- <span data-ttu-id="9e6f0-1444">Korrektur für ps-f (GH #246)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1444">Corrected ps -f (GH #246)</span></span>
- <span data-ttu-id="9e6f0-1445">Verbesserte Unterstützung für X11-Apps, z.B. xEmacs (GH #481)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1445">Improved support for x11 apps such as xEmacs (GH #481)</span></span>
- <span data-ttu-id="9e6f0-1446">Aktualisierte anfängliche Threadstapelgröße, um der standardmäßigen Ubuntu-Einstellung zu entsprechen und die Größe ordnungsgemäß an den get_rlimit-Systemaufruf zu melden (GH #172, #258)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1446">Updated initial thread stack size to match default Ubuntu setting and reporting the size correctly to the get_rlimit syscall (GH #172, #258)</span></span>
- <span data-ttu-id="9e6f0-1447">Verbesserte Berichterstellung von Pico-Prozessimagenamen (z.B. für die Überwachung)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1447">Improved reporting of pico process image names (e.g., for auditing)</span></span>
- <span data-ttu-id="9e6f0-1448">Implementierung von /proc/mountinfo für df-Befehl</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1448">Implemented /proc/mountinfo for df command</span></span>
- <span data-ttu-id="9e6f0-1449">Korrektur des Fehlercodes der symbolischen Verknüpfung für den untergeordneten Namen .</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1449">Fixed symlink error code for child name .</span></span> <span data-ttu-id="9e6f0-1450">und .</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1450">and ..</span></span>
- <span data-ttu-id="9e6f0-1451">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1451">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1452">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1452">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1453">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1453">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1454">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1454">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`GETTIMER`<br/>
`MKNODAT`<br/>
`RENAMEAT`<br/>
`SENDFILE`<br/>
`SENDFILE64`<br/>
`SYNC_FILE_RANGE`<br/>
<br/>

## <a name="build-14352"></a><span data-ttu-id="9e6f0-1455">Build 14352</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1455">Build 14352</span></span>
<span data-ttu-id="9e6f0-1456">Allgemeine Windows-Informationen zu Build 14352 finden Sie im [Windows-Blog](https://aka.ms/wip14352).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1456">For general Windows information on build 14352 visit the [Windows Blog](https://aka.ms/wip14352).</span></span><br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1457">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1457">Fixed</span></span>
- <span data-ttu-id="9e6f0-1458">Korrektur eines Problems, bei dem große Dateien nicht ordnungsgemäß heruntergeladen bzw. ordnungsgemäß erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1458">Fixed issue where large files were not downloaded / created correctly.</span></span>  <span data-ttu-id="9e6f0-1459">Dadurch sollte die Blockierung von npm und anderen Szenarien aufgehoben werden (GH #3, GH #313)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1459">This should unblock npm and other scenarios (GH #3, GH #313)</span></span>
- <span data-ttu-id="9e6f0-1460">Entfernen einiger Instanzen, in denen Sockets nicht mehr reagieren</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1460">Removed some instances where sockets hang</span></span>
- <span data-ttu-id="9e6f0-1461">Korrektur einiger ptrace-Fehler</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1461">Corrected some ptrace errors</span></span>
- <span data-ttu-id="9e6f0-1462">Korrektur eines Problems, bei dem WSL Dateinamen mit mehr als 255 Zeichen zuließ</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1462">Fixed issue with WSL allowing filenames longer than 255 characters</span></span>
- <span data-ttu-id="9e6f0-1463">Verbesserte Unterstützung nicht-englischer Zeichen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1463">Improved support for non-English characters</span></span>
- <span data-ttu-id="9e6f0-1464">Hinzufügen aktueller Windows-Zeitzonendaten und Festlegen als Standard</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1464">Add current Windows timezone data and set as default</span></span>
- <span data-ttu-id="9e6f0-1465">Eindeutige Geräte-IDs für jeden Einbindungspunkt (jre-Korrektur – GH #49)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1465">Unique device id’s for each mount point (jre fix – GH #49)</span></span>
- <span data-ttu-id="9e6f0-1466">Korrektur eines Problems mit Pfaden, die „.“</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1466">Correct issue with paths containing “.”</span></span> <span data-ttu-id="9e6f0-1467">und „..“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1467">and “..”</span></span>
- <span data-ttu-id="9e6f0-1468">Hinzufügen von FIFO-Unterstützung (GH #71)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1468">Added Fifo support (GH #71)</span></span>
- <span data-ttu-id="9e6f0-1469">Aktualisiertes Format von „resolv.conf“ entsprechend dem nativen Ubuntu-Format</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1469">Updated format of resolv.conf to match native Ubuntu format</span></span>
- <span data-ttu-id="9e6f0-1470">procfs-Bereinigung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1470">Some procfs cleanup</span></span>
- <span data-ttu-id="9e6f0-1471">Aktivierten von Ping für Administratorkonsolen (GH #18)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1471">Enabled ping for Administrator consoles (GH #18)</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1472">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1472">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1473">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1473">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1474">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1474">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`FALLOCATE`<br/>
`EXECVE`<br/>
`LGETXATTR`<br/>
`FGETXATTR`<br/>
<br/>

## <a name="build-14342"></a><span data-ttu-id="9e6f0-1475">Build 14342</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1475">Build 14342</span></span>
<span data-ttu-id="9e6f0-1476">Allgemeine Windows-Informationen zu Build 14342 finden Sie im [Windows-Blog](https://aka.ms/wip14342).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1476">For general Windows information on build 14342 the [Windows Blog](https://aka.ms/wip14342).</span></span> <br/>

<span data-ttu-id="9e6f0-1477">Informationen zu VolFs und DriveFs finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1477">Information on VolFs and DriveFs can be found on the [WSL Blog](https://blogs.msdn.microsoft.com/wsl).</span></span> <br/>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1478">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1478">Fixed</span></span>
- <span data-ttu-id="9e6f0-1479">Korrektur eines Installationsproblems, wenn der Windows-Benutzer Unicode-Zeichen im Benutzernamen enthielt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1479">Fixed install issue when the Windows user had Unicode characters in the username</span></span>
- <span data-ttu-id="9e6f0-1480">Die Problemumgehung „apt-get update udev“ in den FAQ wird jetzt standardmäßig bei der ersten Ausführung bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1480">The apt-get update udev workaround in the FAQ is now provided by default on first run</span></span>
- <span data-ttu-id="9e6f0-1481">Aktivierte symbolische Verknüpfungen in DriveFs-Verzeichnissen (/mnt/<drive>)</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1481">Enabled symlinks in DriveFs (/mnt/<drive>) directories</span></span>
- <span data-ttu-id="9e6f0-1482">Symbolische Verknüpfungen funktionieren nun zwischen DriveFs und VolFs</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1482">Symlinks now work between DriveFs and VolFs</span></span>
- <span data-ttu-id="9e6f0-1483">Korrektur des Pfadanalyseproblems auf oberster Ebene: ls .// funktioniert jetzt wie erwartet</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1483">Addressed top level path parsing issue: ls .// will now work as expected</span></span>
- <span data-ttu-id="9e6f0-1484">npm install auf DriveFs und die -g-Optionen funktionieren jetzt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1484">npm install on DriveFs and the -g options are now working</span></span>
- <span data-ttu-id="9e6f0-1485">Korrektur eines Problems, das den Start des PHP-Servers verhinderte</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1485">Fixed issue preventing PHP server from launching</span></span>
- <span data-ttu-id="9e6f0-1486">Aktualisierte Standardumgebungswerte, z.B. $PATH, um nativem Ubuntu besser zu entsprechen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1486">Updated default environment values, such as $PATH to closer match native Ubuntu</span></span>
- <span data-ttu-id="9e6f0-1487">Hinzufügen eines wöchentlichen Wartungstasks in Windows zum Aktualisieren des apt-Paketcaches</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1487">Added a weekly maintenance task in Windows to update the apt package cache</span></span>
- <span data-ttu-id="9e6f0-1488">Korrektur eines Problems bei der Überprüfung von ELF-Headern, WSL unterstützt jetzt alle Melkor-Optionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1488">Fixed issue with ELF header validation, WSL now supports all Melkor options</span></span>
- <span data-ttu-id="9e6f0-1489">Zsh-Shell ist funktionsfähig</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1489">Zsh shell is functional</span></span>
- <span data-ttu-id="9e6f0-1490">Vorkompilierte Go-Binärdateien werden jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1490">Precompiled Go binaries are now supported</span></span>
- <span data-ttu-id="9e6f0-1491">Eingabeaufforderung bei der ersten Ausführung von „bash.exe“ ist nun richtig lokalisiert</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1491">Prompting on Bash.exe first run is now localized correctly</span></span>
- <span data-ttu-id="9e6f0-1492">/proc/meminfo gibt jetzt richtige Informationen zurück</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1492">/proc/meminfo now returns correct information</span></span>
- <span data-ttu-id="9e6f0-1493">Sockets werden jetzt in VFS unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1493">Sockets now supported in VFS</span></span>
- <span data-ttu-id="9e6f0-1494">/dev jetzt als tempfs eingebunden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1494">/dev now mounted as tempfs</span></span>
- <span data-ttu-id="9e6f0-1495">Fifo wird jetzt unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1495">Fifo now supported</span></span>
- <span data-ttu-id="9e6f0-1496">Mehrkernsysteme werden nun ordnungsgemäß in /proc/cpuinfo angezeigt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1496">Multi-core systems now showing correctly in /proc/cpuinfo</span></span>
- <span data-ttu-id="9e6f0-1497">Weitere Verbesserungen und Fehlermeldungen, die während der ersten Ausführung heruntergeladen werden</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1497">Additional improvements and error messages downloading during first run</span></span>
- <span data-ttu-id="9e6f0-1498">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1498">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="9e6f0-1499">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1499">Supported syscall list below.</span></span>
- <span data-ttu-id="9e6f0-1500">Weitere Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1500">Additional bugfixes and improvements</span></span>

### <a name="known-issues"></a><span data-ttu-id="9e6f0-1501">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1501">Known Issues</span></span>
- <span data-ttu-id="9e6f0-1502">„.“ wird in einigen Fällen nicht</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1502">Not resolving ‘..’</span></span> <span data-ttu-id="9e6f0-1503">ordnungsgemäß auf DriveFs aufgelöst</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1503">correctly on DriveFs in some cases</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1504">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1504">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1505">Im folgenden finden Sie eine Liste der neuen oder verbesserten Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1505">Below are a list of new or enhanced syscalls that have some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1506">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1506">The syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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

## <a name="build-14332"></a><span data-ttu-id="9e6f0-1507">Build 14332</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1507">Build 14332</span></span>

<span data-ttu-id="9e6f0-1508">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14332).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1508">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14332).</span></span> <br/>


### <a name="fixed"></a><span data-ttu-id="9e6f0-1509">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1509">Fixed</span></span>
- <span data-ttu-id="9e6f0-1510">Bessere resolv.conf-Generierung einschließlich Priorisieren von DNS-Einträgen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1510">Better resolv.conf generation including prioritizing DNS entries</span></span>
- <span data-ttu-id="9e6f0-1511">Problem beim Verschieben von Dateien und Verzeichnissen zwischen/mnt- und Nicht-/mnt-Laufwerken</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1511">Issue with moving files and directories between /mnt and non-/mnt drives</span></span>
- <span data-ttu-id="9e6f0-1512">TAR-Dateien können jetzt mit symbolischen Verknüpfungen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1512">Tar files can now be created with symlinks</span></span>
- <span data-ttu-id="9e6f0-1513">Hinzufügen des /run/lock-Standardverzeichnisses bei der Instanzerstellung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1513">Added default /run/lock directory on instance creation</span></span>
- <span data-ttu-id="9e6f0-1514">Aktualisieren von /dev/null, um die richtigen Statusinformationen zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1514">Update /dev/null to return proper stat info</span></span>
- <span data-ttu-id="9e6f0-1515">Weitere Fehler beim Herunterladen während der ersten Ausführung</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1515">Additional errors when downloading during first run</span></span>
- <span data-ttu-id="9e6f0-1516">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1516">Syscall improvements and bugfixes.</span></span> <span data-ttu-id="9e6f0-1517">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1517">Supported syscall list below.</span></span>
- <span data-ttu-id="9e6f0-1518">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1518">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1519">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1519">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1520">Im folgenden finden Sie den neuen Systemaufruf, der in WSL implementiert ist.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1520">Below is the new syscall that has some implementation in WSL.</span></span> <span data-ttu-id="9e6f0-1521">Der Systemaufruf in dieser Liste wird in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1521">The syscall on this list is supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

`READLINKAT`<br/>
<br/>

## <a name="build-14328"></a><span data-ttu-id="9e6f0-1522">Build 14328</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1522">Build 14328</span></span>

<span data-ttu-id="9e6f0-1523">Allgemeine Windows-Informationen zu Build 14332 finden Sie im [Windows-Blog](https://aka.ms/wip14328).</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1523">For general Windows information on build 14332 visit the [Windows Blog](https://aka.ms/wip14328).</span></span> <br/>


### <a name="new-features"></a><span data-ttu-id="9e6f0-1524">Neue Funktionen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1524">New Features</span></span>
* <span data-ttu-id="9e6f0-1525">Jetzt werden Linux-Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1525">Now support Linux users.</span></span>  <span data-ttu-id="9e6f0-1526">Bei der Installation von Bash unter Ubuntu unter Windows werden Sie aufgefordert, einen Linux-Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1526">Installing Bash on Ubuntu on Windows will prompt for creation of a Linux user.</span></span>  <span data-ttu-id="9e6f0-1527">Weitere Informationen finden Sie unter https://aka.ms/wslusers.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1527">For more information, visit https://aka.ms/wslusers</span></span>
* <span data-ttu-id="9e6f0-1528">Der Hostname ist jetzt auf den Windows-Computernamen festgelegt, nicht mehr auf @localhost</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1528">Hostname is now set to the Windows computer name, no more @localhost</span></span>
* <span data-ttu-id="9e6f0-1529">Weitere Informationen zu Build 14328 finden Sie unter: https://aka.ms/wip14328</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1529">For more information on build 14328, visit: https://aka.ms/wip14328</span></span>

### <a name="fixed"></a><span data-ttu-id="9e6f0-1530">Fest</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1530">Fixed</span></span>
* <span data-ttu-id="9e6f0-1531">Verbesserungen von symbolischen Verknüpfungen für Nicht-/mnt/<drive>-Dateien</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1531">Symlink improvements for non /mnt/<drive> files</span></span>
    * <span data-ttu-id="9e6f0-1532">Die npm-Installation funktioniert jetzt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1532">npm install now works</span></span>
    * <span data-ttu-id="9e6f0-1533">jdk/jre kann nun mithilfe der Anweisungen installiert werden, die Sie [hier](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html) finden.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1533">jdk / jre now installable using instructions found [here](https://xubuntugeek.blogspot.com/2012/09/how-to-install-oracle-jdk-7-manually-in.html).</span></span>
    * <span data-ttu-id="9e6f0-1534">Bekanntes Problem: Symbolische Verknüpfungen funktionieren für Windows-Einbindungen nicht.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1534">known issue: symlinks do not work for Windows mounts.</span></span>  <span data-ttu-id="9e6f0-1535">Diese Funktionen werden in einem späteren Build verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1535">Functionality will be available in a later build</span></span>
* <span data-ttu-id="9e6f0-1536">top und htop werden jetzt angezeigt</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1536">top and htop now display</span></span>
* <span data-ttu-id="9e6f0-1537">Zusätzliche Fehlermeldungen bei einigen Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1537">Additional error messages for some install failures</span></span>
* <span data-ttu-id="9e6f0-1538">Systemaufrufverbesserungen und -fehlerbehebungen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1538">Syscall improvements and bugfixes.</span></span>  <span data-ttu-id="9e6f0-1539">Unterstützte Systemaufrufliste unten.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1539">Supported syscall list below.</span></span>
* <span data-ttu-id="9e6f0-1540">Weitere optimierende Fehlerbehebungen und Verbesserungen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1540">Additional improvements bugfixes and improvements</span></span>

### <a name="syscall-support"></a><span data-ttu-id="9e6f0-1541">Unterstützung von Systemaufrufen</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1541">Syscall Support</span></span>
<span data-ttu-id="9e6f0-1542">Im folgenden finden Sie eine Liste der Systemaufrufe, die einige Implementierungen in WSL aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1542">Below is a list of syscalls that have some implementation in WSL.</span></span>  <span data-ttu-id="9e6f0-1543">Die Systemaufrufe in dieser Liste werden in mindestens einem Szenario unterstützt, aber möglicherweise werden zurzeit nicht alle Parameter unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e6f0-1543">Syscalls on this list are supported in at least one scenario, but may not have all parameters supported at this time.</span></span>

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
