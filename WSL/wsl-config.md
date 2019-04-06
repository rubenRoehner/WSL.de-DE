---
title: Verwalten von Linux-Distributionen
description: Verweisen auf auflisten und Konfigurieren von mehreren Linux-Distributionen, die auf dem Windows-Subsystem für Linux ausführen.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
author: scooley
ms.author: scooley
ms.date: 02/7/2018
ms.topic: article
ms.assetid: 7ca59bd7-d9d3-4f6d-8b92-b8faa9bcf250
ms.custom: seodec18
ms.openlocfilehash: c806552750f413fcb75f989d868a57cc939af64a
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063498"
---
# <a name="manage-and-configure-windows-subsystem-for-linux"></a><span data-ttu-id="93c5d-104">Verwalten und Konfigurieren von Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="93c5d-104">Manage and configure Windows Subsystem for Linux</span></span>

> <span data-ttu-id="93c5d-105">Gilt für Windows 10 Fall Creators Update und höher.</span><span class="sxs-lookup"><span data-stu-id="93c5d-105">Applies to Windows 10 Fall Creators Update and later.</span></span>  <span data-ttu-id="93c5d-106">Finden Sie in unserer aktualisierten [Installationshandbuch](./install_guide.md) , neue Features zu starten, Ausführen von mehreren Linux-Distributionen aus dem Windows Store.</span><span class="sxs-lookup"><span data-stu-id="93c5d-106">See our updated [installation guide](./install_guide.md) to try new management features and start running multiple Linux distributions from the Windows Store.</span></span>

## <a name="ways-to-run-wsl"></a><span data-ttu-id="93c5d-107">Möglichkeiten zum Ausführen von WSL</span><span class="sxs-lookup"><span data-stu-id="93c5d-107">Ways to run WSL</span></span>

<span data-ttu-id="93c5d-108">Es gibt viele Möglichkeiten zum Ausführen von Linux mit dem Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="93c5d-108">There are many ways to run Linux with the Windows Subsystem for Linux.</span></span>

1. `[distro]` <span data-ttu-id="93c5d-109">IE</span><span class="sxs-lookup"><span data-stu-id="93c5d-109">ie</span></span> `ubuntu`
1. `wsl.exe` <span data-ttu-id="93c5d-110">oder</span><span class="sxs-lookup"><span data-stu-id="93c5d-110">or</span></span> `bash.exe`
1. `wsl [command]` <span data-ttu-id="93c5d-111">oder</span><span class="sxs-lookup"><span data-stu-id="93c5d-111">or</span></span> `bash -c [command]`

<span data-ttu-id="93c5d-112">Welche Methode Sie verwenden sollten, hängt davon ab, was Sie tun.</span><span class="sxs-lookup"><span data-stu-id="93c5d-112">Which method you should use depends on what you're doing.</span></span>

### <a name="launch-wsl-by-distribution"></a><span data-ttu-id="93c5d-113">Starten Sie von der Verteilung von WSL</span><span class="sxs-lookup"><span data-stu-id="93c5d-113">Launch WSL by distribution</span></span>

<span data-ttu-id="93c5d-114">Eine Distribution mit distributionsspezifische Anwendung ausführt, wird dieser Verteilung in seinem eigenen Konsolenfenster gestartet.</span><span class="sxs-lookup"><span data-stu-id="93c5d-114">Running a distribution using it's distro-specific application launches that distribution in it's own console window.</span></span>

![Starten Sie im Startmenü WSL](media/start-launch.png)

<span data-ttu-id="93c5d-116">Es ist identisch mit dem "Start" klicken, in der Windows Store.</span><span class="sxs-lookup"><span data-stu-id="93c5d-116">It is the same as clicking "Launch" in the Windows Store.</span></span>

![Starten Sie die WSL aus dem Windows Store](media/store-launch.png)

<span data-ttu-id="93c5d-118">Sie können auch die Verteilung über die Befehlszeile ausführen, mit `[distribution].exe`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-118">You can also run the distribution from the command line by running `[distribution].exe`.</span></span>

<span data-ttu-id="93c5d-119">Der Nachteil der Ausführung einer Verteilungs über die Befehlszeile auf diese Weise ist, dass es automatisch Ihrem Arbeitsverzeichnis aus dem aktuellen Verzeichnis in der Distribution-Basisverzeichnis ändert.</span><span class="sxs-lookup"><span data-stu-id="93c5d-119">The disadvantage of running a distribution from the command line in this way is that it will automatically change your working directory from the current directory to the distribution's home directory.</span></span>

**<span data-ttu-id="93c5d-120">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-120">Example:</span></span>**

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> ubuntu

scooley@scooley-elmer:~$ pwd
/home/scooley
scooley@scooley-elmer:~$ exit
logout

PS C:\Users\sarah>
```

### <a name="wsl-and-wsl-command"></a><span data-ttu-id="93c5d-121">Wsl und Wsl [Befehl]</span><span class="sxs-lookup"><span data-stu-id="93c5d-121">wsl and wsl [command]</span></span>

<span data-ttu-id="93c5d-122">Die beste Möglichkeit zum Ausführen von WSL über die Befehlszeile verwendet `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-122">The best way to run WSL from the command line is using `wsl.exe`.</span></span>

**<span data-ttu-id="93c5d-123">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-123">Example:</span></span>**

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> wsl

scooley@scooley-elmer:/mnt/c/Users/sarah$ pwd
/mnt/c/Users/sarah
```

<span data-ttu-id="93c5d-124">Nicht nur `wsl` behalten Sie das aktuelle Arbeitsverzeichnis vorhanden, sie können einen einzelnen Befehl auf der Seite Windows-Befehle ausführen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-124">Not only does `wsl` keep the current working directory in place, it lets you run a single command along side Windows commands.</span></span>

**<span data-ttu-id="93c5d-125">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-125">Example:</span></span>**

```console
PS C:\Users\sarah> Get-Date

Sunday, March 11, 2018 7:54:05 PM

PS C:\Users\sarah> wsl
scooley@scooley-elmer:/mnt/c/Users/sarah$ date
Sun Mar 11 19:56:57 DST 2018
scooley@scooley-elmer:/mnt/c/Users/sarah$ exit
logout

PS C:\Users\sarah> wsl date
Sun Mar 11 19:55:47 DST 2018
```

**<span data-ttu-id="93c5d-126">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-126">Example:</span></span>**

```console
PS C:\Users\sarah> Get-VM

Name            State CPUUsage(%) MemoryAssigned(M) Uptime   Status
----            ----- ----------- ----------------- ------   ------
Server17093     Off   0           0                 00:00:00 Opera...
Ubuntu          Off   0           0                 00:00:00 Opera...
Ubuntu (bionic) Off   0           0                 00:00:00 Opera...
Windows         Off   0           0                 00:00:00 Opera...


PS C:\Users\sarah> Get-VM | wsl grep "Ubuntu"
Ubuntu          Off   0           0                 00:00:00 Opera...
Ubuntu (bionic) Off   0           0                 00:00:00 Opera...
PS C:\Users\sarah>
```


## <a name="managing-multiple-linux-distributions"></a><span data-ttu-id="93c5d-127">Verwalten von mehreren Linux-Distributionen</span><span class="sxs-lookup"><span data-stu-id="93c5d-127">Managing multiple Linux Distributions</span></span>

### <a name="windows-10-version-1903-and-later"></a><span data-ttu-id="93c5d-128">Windows 10-Version 1903 und höher</span><span class="sxs-lookup"><span data-stu-id="93c5d-128">Windows 10 Version 1903 and later</span></span>

<span data-ttu-id="93c5d-129">Sie können `wsl.exe` Ihre Distributionen im Windows-Subsystem für Linux (WSL), einschließlich der verfügbare Distributionen auflisten, Festlegen von einer standardverteilung und Deinstallieren von Verteilungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="93c5d-129">You can use `wsl.exe` to manage your distributions in the Windows Subsystem for Linux (WSL), including listing available distributions, setting a default distribution, and uninstalling distributions.</span></span>

<span data-ttu-id="93c5d-130">Jede Linux-Distribution verwaltet unabhängig voneinander eine eigene Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-130">Each Linux distribution independently manages its own configurations.</span></span> <span data-ttu-id="93c5d-131">Führen Sie zum Anzeigen der Verteilung spezifischen Befehle `[distro.exe] /?`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-131">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="93c5d-132">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-132">For example `ubuntu /?`.</span></span>

#### <a name="list-distributions"></a><span data-ttu-id="93c5d-133">Liste von Verteilungen</span><span class="sxs-lookup"><span data-stu-id="93c5d-133">List distributions</span></span>

`wsl -l` <span data-ttu-id="93c5d-134">,</span><span class="sxs-lookup"><span data-stu-id="93c5d-134">,</span></span> `wsl --list`  
<span data-ttu-id="93c5d-135">Listet die verfügbaren Linux-Distributionen für WSL verfügbar.</span><span class="sxs-lookup"><span data-stu-id="93c5d-135">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="93c5d-136">Wenn eine Verteilung aufgeführt ist, wird installiert und bereit für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="93c5d-136">If a distribution is listed, it's installed and ready to use.</span></span>

`wsl --list --all`   
<span data-ttu-id="93c5d-137">Listet alle Verteilungen, einschließlich jener, die nicht derzeit verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="93c5d-137">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="93c5d-138">Sie möglicherweise während der Installation, Deinstallation oder in einem fehlerhaften Zustand befinden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-138">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

`wsl --list --running`   
<span data-ttu-id="93c5d-139">Listet alle Verteilungen, die derzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-139">Lists all distributions that are currently running.</span></span>

#### <a name="set-a-default-distribution"></a><span data-ttu-id="93c5d-140">Legen Sie eine standardverteilung</span><span class="sxs-lookup"><span data-stu-id="93c5d-140">Set a default distribution</span></span>

<span data-ttu-id="93c5d-141">Die standardverteilung von WSL ist diejenige, die ausgeführt, beim Ausführen von wird `wsl` in einer Befehlszeile.</span><span class="sxs-lookup"><span data-stu-id="93c5d-141">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

`wsl -s <DistributionName>`<span data-ttu-id="93c5d-142">,</span><span class="sxs-lookup"><span data-stu-id="93c5d-142">,</span></span> `wsl --setdefault <DistributionName>`

<span data-ttu-id="93c5d-143">Legt die standardverteilung auf `<DistributionName>`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-143">Sets the default distribution to `<DistributionName>`.</span></span>

**<span data-ttu-id="93c5d-144">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-144">Example:</span></span>**  
`wsl -s Ubuntu` <span data-ttu-id="93c5d-145">Meine standardverteilung würde auf Ubuntu festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-145">would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="93c5d-146">Wenn ich jetzt ausführen `wsl npm init` wird es in Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-146">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="93c5d-147">Wenn ich ausführe `wsl` eine Ubuntu-Sitzung wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="93c5d-147">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="93c5d-148">Aufheben der Registrierung, und installieren Sie eine Verteilung neu.</span><span class="sxs-lookup"><span data-stu-id="93c5d-148">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="93c5d-149">Speichern bei Linux, auf die Verteilungen, die durch die Windows installiert werden können, sie können nicht deinstalliert werden, über den Store.</span><span class="sxs-lookup"><span data-stu-id="93c5d-149">While Linux distributions can be installed through the Windows store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="93c5d-150">WSL Config können Verteilungen, deren Registrierung aufgehoben/deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-150">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="93c5d-151">Aufheben der Registrierung können auch Distributionen neu installiert werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-151">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="93c5d-152">**Vorsicht:** Nach deren Registrierung aufgehoben wird, werden alle Daten, Einstellungen und Software, die dieser Verteilung zugeordneten dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="93c5d-152">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="93c5d-153">Neu aus dem Store installieren, installieren Sie eine Neuinstallation der Verteilung.</span><span class="sxs-lookup"><span data-stu-id="93c5d-153">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wsl --unregister <DistributionName>`  
<span data-ttu-id="93c5d-154">Hebt die Registrierung auf der Verteilung von WSL, damit sie neu installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="93c5d-154">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="93c5d-155">Zum Beispiel: `wsl -unregister Ubuntu` Ubuntu die Verteilungen in WSL verfügbar entfernt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-155">For example: `wsl -unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="93c5d-156">Beim Ausführen `wsl --list` wird es nicht aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-156">When I run `wsl --list` it will not be listed.</span></span>

<span data-ttu-id="93c5d-157">Suchen Sie die Verteilung in der Windows Store, und wählen Sie die "Start", um erneut zu installieren.</span><span class="sxs-lookup"><span data-stu-id="93c5d-157">To reinstall, find the distribution in the Windows Store and select "Launch".</span></span>

#### <a name="run-as-a-specific-user"></a><span data-ttu-id="93c5d-158">Führen Sie als ein bestimmter Benutzer</span><span class="sxs-lookup"><span data-stu-id="93c5d-158">Run as a specific user</span></span>

`wsl -u <Username>`<span data-ttu-id="93c5d-159">,</span><span class="sxs-lookup"><span data-stu-id="93c5d-159">,</span></span> `wsl --user <Username>`

<span data-ttu-id="93c5d-160">Führen Sie WSL, als der angegebene Benutzer.</span><span class="sxs-lookup"><span data-stu-id="93c5d-160">Run WSL as the specified user.</span></span> <span data-ttu-id="93c5d-161">Beachten Sie, dass dieser Benutzer in der Verteilung WSL vorhanden sein muss.</span><span class="sxs-lookup"><span data-stu-id="93c5d-161">Please note that user must exist inside of the WSL distribution.</span></span>

#### <a name="run-a-specific-distribution"></a><span data-ttu-id="93c5d-162">Führen Sie eine bestimmte Verteilung</span><span class="sxs-lookup"><span data-stu-id="93c5d-162">Run a specific distribution</span></span>

`wsl --d <DistributionName>`<span data-ttu-id="93c5d-163">,</span><span class="sxs-lookup"><span data-stu-id="93c5d-163">,</span></span> `wsl --distribution <DistributionName>`

<span data-ttu-id="93c5d-164">Führen Sie eine angegebene Verteilung von WSL, können verwendet werden, um Befehle an einer bestimmten Verteilung zu senden, ohne den Standardwert zu ändern.</span><span class="sxs-lookup"><span data-stu-id="93c5d-164">Run a specified distribution of WSL, can be used to send commands to a specific distribution without having to change your default.</span></span>

### <a name="versions-earlier-than-windows-10-version-1903"></a><span data-ttu-id="93c5d-165">Versionen vor Windows 10, Version 1903</span><span class="sxs-lookup"><span data-stu-id="93c5d-165">Versions Earlier than Windows 10 Version 1903</span></span>

<span data-ttu-id="93c5d-166">WSL Config (`wslconfig.exe`) ist ein Befehlszeilentool zum Verwalten von Linux-Distributionen, die auf dem Windows-Subsystem für Linux (WSL) ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="93c5d-166">WSL Config (`wslconfig.exe`) is a command-line tool for managing Linux distributions running on the Windows Subsystem for Linux (WSL).</span></span>  <span data-ttu-id="93c5d-167">Sie können Sie die Liste der verfügbaren Distributionen, legen Sie eine standardverteilung und Deinstallieren von Verteilungen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-167">It lets you list available distributions, set a default distribution, and uninstall distributions.</span></span>

<span data-ttu-id="93c5d-168">Während die WSL-Konfiguration für Einstellungen hilfreich ist, umfassen oder Verteilungen zu koordinieren, verwaltet jede Linux-Distribution unabhängig eigene Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-168">While WSL Config is helpful for settings that span or coordinate distributions, each Linux distribution independently manages its own configurations.</span></span>  <span data-ttu-id="93c5d-169">Führen Sie zum Anzeigen der Verteilung spezifischen Befehle `[distro.exe] /?`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-169">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="93c5d-170">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-170">For example `ubuntu /?`.</span></span>

<span data-ttu-id="93c5d-171">Um alle verfügbaren Optionen für Wslconfig anzuzeigen, führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="93c5d-171">To see all available options for wslconfig, run:</span></span>  `wslconfig /?`

```console
wslconfig.exe
Performs administrative operations on Windows Subsystem for Linux

Usage:
    /l, /list [/all] - Lists registered distributions.
        /all - Optionally list all distributions, including distributions that
               are currently being installed or uninstalled.
    /s, /setdefault <DistributionName> - Sets the specified distribution as the default.
    /u, /unregister <DistributionName> - Unregisters a distribution.
```

#### <a name="list-distributions"></a><span data-ttu-id="93c5d-172">Liste von Verteilungen</span><span class="sxs-lookup"><span data-stu-id="93c5d-172">List distributions</span></span>

`wslconfig /list`  
<span data-ttu-id="93c5d-173">Listet die verfügbaren Linux-Distributionen für WSL verfügbar.</span><span class="sxs-lookup"><span data-stu-id="93c5d-173">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="93c5d-174">Wenn eine Verteilung aufgeführt ist, wird installiert und bereit für die Verwendung.</span><span class="sxs-lookup"><span data-stu-id="93c5d-174">If a distribution is listed, it's installed and ready to use.</span></span>

`wslconfig /list /all`  
<span data-ttu-id="93c5d-175">Listet alle Verteilungen, einschließlich jener, die nicht derzeit verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="93c5d-175">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="93c5d-176">Sie möglicherweise während der Installation, Deinstallation oder in einem fehlerhaften Zustand befinden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-176">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

#### <a name="set-a-default-distribution"></a><span data-ttu-id="93c5d-177">Legen Sie eine standardverteilung</span><span class="sxs-lookup"><span data-stu-id="93c5d-177">Set a default distribution</span></span>

<span data-ttu-id="93c5d-178">Die standardverteilung von WSL ist diejenige, die ausgeführt, beim Ausführen von wird `wsl` in einer Befehlszeile.</span><span class="sxs-lookup"><span data-stu-id="93c5d-178">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

`wslconfig /setdefault <DistributionName>`

<span data-ttu-id="93c5d-179">Legt die standardverteilung auf `<DistributionName>`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-179">Sets the default distribution to `<DistributionName>`.</span></span>

**<span data-ttu-id="93c5d-180">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="93c5d-180">Example:</span></span>**  
`wslconfig /setdefault Ubuntu` <span data-ttu-id="93c5d-181">Meine standardverteilung würde auf Ubuntu festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-181">would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="93c5d-182">Wenn ich jetzt ausführen `wsl npm init` wird es in Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-182">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="93c5d-183">Wenn ich ausführe `wsl` eine Ubuntu-Sitzung wird geöffnet.</span><span class="sxs-lookup"><span data-stu-id="93c5d-183">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="93c5d-184">Aufheben der Registrierung, und installieren Sie eine Verteilung neu.</span><span class="sxs-lookup"><span data-stu-id="93c5d-184">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="93c5d-185">Speichern bei Linux, auf die Verteilungen, die durch die Windows installiert werden können, sie können nicht deinstalliert werden, über den Store.</span><span class="sxs-lookup"><span data-stu-id="93c5d-185">While Linux distributions can be installed through the Windows store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="93c5d-186">WSL Config können Verteilungen, deren Registrierung aufgehoben/deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-186">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="93c5d-187">Aufheben der Registrierung können auch Distributionen neu installiert werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-187">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="93c5d-188">**Vorsicht:** Nach deren Registrierung aufgehoben wird, werden alle Daten, Einstellungen und Software, die dieser Verteilung zugeordneten dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="93c5d-188">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="93c5d-189">Neu aus dem Store installieren, installieren Sie eine Neuinstallation der Verteilung.</span><span class="sxs-lookup"><span data-stu-id="93c5d-189">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wslconfig /unregister <DistributionName>`  
<span data-ttu-id="93c5d-190">Hebt die Registrierung auf der Verteilung von WSL, damit sie neu installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="93c5d-190">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="93c5d-191">Zum Beispiel: `wslconfig /unregister Ubuntu` Ubuntu die Verteilungen in WSL verfügbar entfernt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-191">For example: `wslconfig /unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="93c5d-192">Beim Ausführen `wslconfig /list` wird es nicht aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-192">When I run `wslconfig /list` it will not be listed.</span></span>

<span data-ttu-id="93c5d-193">Suchen Sie die Verteilung in der Windows Store, und wählen Sie die "Start", um erneut zu installieren.</span><span class="sxs-lookup"><span data-stu-id="93c5d-193">To reinstall, find the distribution in the Windows Store and select "Launch".</span></span>

## <a name="set-wsl-launch-settings"></a><span data-ttu-id="93c5d-194">Starteinstellungen für den WSL festlegen</span><span class="sxs-lookup"><span data-stu-id="93c5d-194">Set WSL launch settings</span></span>

> **<span data-ttu-id="93c5d-195">In Windows-Insider-Build-17093 und höher verfügbar</span><span class="sxs-lookup"><span data-stu-id="93c5d-195">Available in Windows Insider Build 17093 and later</span></span>**

<span data-ttu-id="93c5d-196">Konfigurieren Sie automatisch bestimmte Funktionen in WSL, die jedes Mal, wenn Sie das Subsystem mit starten angewendet werden `wsl.conf`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-196">Automatically configure certain functionality in WSL that will be applied every time you launch the subsystem using `wsl.conf`.</span></span> 

<span data-ttu-id="93c5d-197">Rechts umfasst dies nun, automatische Optionen und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="93c5d-197">Right now, this includes automount options and network configuration.</span></span>

`wsl.conf` <span data-ttu-id="93c5d-198">befindet sich im einzelnen Linux-Distribution `/etc/wsl.conf`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-198">is located in each Linux distribution in `/etc/wsl.conf`.</span></span> <span data-ttu-id="93c5d-199">Wenn die Datei nicht vorhanden ist, können Sie ihn selbst erstellen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-199">If the file is not there, you can create it yourself.</span></span> <span data-ttu-id="93c5d-200">WSL erkennt, dass das Vorhandensein der Datei und liest den Inhalt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-200">WSL will detect the existence of the file and will read its contents.</span></span> <span data-ttu-id="93c5d-201">Wenn die Datei fehlt oder ist falsch formatiert ist (d. h. eine ungültige Markup formatieren), WSL weiterhin normal zu starten.</span><span class="sxs-lookup"><span data-stu-id="93c5d-201">If the file is missing or malformed (that is, improper markup formatting), WSL will continue to launch as normal.</span></span>

<span data-ttu-id="93c5d-202">Hier ist ein Beispiel `wsl.conf` Datei, die Sie in Ihrem Distributionen hinzufügen können:</span><span class="sxs-lookup"><span data-stu-id="93c5d-202">Here is a sample `wsl.conf` file you could add into your distros:</span></span>

```console
# Enable extra metadata options by default
[automount]
enabled = true
root = /windir/
options = "metadata,umask=22,fmask=11"
mountFsTab = false

# Enable DNS – even though these are turned on by default, we’ll specify here just to be explicit.
[network]
generateHosts = true
generateResolvConf = true
```

### <a name="configuration-options"></a><span data-ttu-id="93c5d-203">Konfigurationsoptionen</span><span class="sxs-lookup"><span data-stu-id="93c5d-203">Configuration Options</span></span>

<span data-ttu-id="93c5d-204">Gemäß der INI-Konventionen werden die Schlüssel unter einem Abschnitt deklariert.</span><span class="sxs-lookup"><span data-stu-id="93c5d-204">In keeping with .ini conventions, keys are declared under a section.</span></span> 

<span data-ttu-id="93c5d-205">WSL unterstützt zwei Abschnitte: `automount` und `network`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-205">WSL supports two sections: `automount` and `network`.</span></span>

#### <a name="automount"></a><span data-ttu-id="93c5d-206">Automatische Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="93c5d-206">automount</span></span>

<span data-ttu-id="93c5d-207">Abschnitt:</span><span class="sxs-lookup"><span data-stu-id="93c5d-207">Section:</span></span> `[automount]`


| <span data-ttu-id="93c5d-208">key</span><span class="sxs-lookup"><span data-stu-id="93c5d-208">key</span></span>        | <span data-ttu-id="93c5d-209">Wert</span><span class="sxs-lookup"><span data-stu-id="93c5d-209">value</span></span>                          | <span data-ttu-id="93c5d-210">default</span><span class="sxs-lookup"><span data-stu-id="93c5d-210">default</span></span>      | <span data-ttu-id="93c5d-211">Anmerkungen zu dieser Version</span><span class="sxs-lookup"><span data-stu-id="93c5d-211">notes</span></span>                                                                                                                                                                                                                                                                                                                          |
|:-----------|:-------------------------------|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="93c5d-212">enabled</span><span class="sxs-lookup"><span data-stu-id="93c5d-212">enabled</span></span>    | <span data-ttu-id="93c5d-213">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-213">boolean</span></span>                        | <span data-ttu-id="93c5d-214">true</span><span class="sxs-lookup"><span data-stu-id="93c5d-214">true</span></span>         | `true` <span data-ttu-id="93c5d-215">bewirkt, dass Festplattenlaufwerke (d.h.)</span><span class="sxs-lookup"><span data-stu-id="93c5d-215">causes fixed drives (i.e</span></span> `C:/` <span data-ttu-id="93c5d-216">oder `D:/`) mit DrvFs unter automatisch eingebunden werden `/mnt`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-216">or `D:/`) to be automatically mounted with DrvFs under `/mnt`.</span></span>  `false` <span data-ttu-id="93c5d-217">bedeutet, dass Laufwerke wird nicht automatisch bereitgestellt werden, aber Sie dennoch bereitstellen können, manuell oder über `fstab`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-217">means drives won’t be mounted automatically, but you could still mount them manually or via `fstab`.</span></span>                                                                                                             |
| <span data-ttu-id="93c5d-218">mountFsTab</span><span class="sxs-lookup"><span data-stu-id="93c5d-218">mountFsTab</span></span> | <span data-ttu-id="93c5d-219">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-219">boolean</span></span>                        | <span data-ttu-id="93c5d-220">true</span><span class="sxs-lookup"><span data-stu-id="93c5d-220">true</span></span>         | `true` <span data-ttu-id="93c5d-221">Legt `/etc/fstab` zu verarbeitenden WSL starten.</span><span class="sxs-lookup"><span data-stu-id="93c5d-221">sets `/etc/fstab` to be processed on WSL start.</span></span> <span data-ttu-id="93c5d-222">/ etc/fstab handelt es sich um eine Datei, in dem Sie andere Dateisysteme, wie eine SMB-Freigabe deklarieren können.</span><span class="sxs-lookup"><span data-stu-id="93c5d-222">/etc/fstab is a file where you can declare other filesystems, like an SMB share.</span></span> <span data-ttu-id="93c5d-223">Daher können Sie diese Dateisysteme in WSL beim Start automatisch nach oben bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="93c5d-223">Thus, you can mount these filesystems automatically in WSL on start up.</span></span>                                                                                                                |
| <span data-ttu-id="93c5d-224">Stammverzeichnis</span><span class="sxs-lookup"><span data-stu-id="93c5d-224">root</span></span>       | <span data-ttu-id="93c5d-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93c5d-225">String</span></span>                         | `/mnt/`      | <span data-ttu-id="93c5d-226">Legt das Verzeichnis, in denen feste Laufwerke automatisch eingebunden werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-226">Sets the directory where fixed drives will be automatically mounted.</span></span> <span data-ttu-id="93c5d-227">Für, wenn Sie z. B. ein Verzeichnis in WSL am `/windir/` und angeben, dass als Wurzel an, Sie Ihre Festplattenlaufwerke bereitgestellt erwarten:</span><span class="sxs-lookup"><span data-stu-id="93c5d-227">For example, if you have a directory in WSL at `/windir/` and you specify that as the root, you would expect to see your fixed drives mounted at</span></span> `/windir/c`                                                                                              |
| <span data-ttu-id="93c5d-228">Optionen</span><span class="sxs-lookup"><span data-stu-id="93c5d-228">options</span></span>    | <span data-ttu-id="93c5d-229">durch Trennzeichen getrennte Liste von Werten</span><span class="sxs-lookup"><span data-stu-id="93c5d-229">comma-separated list of values</span></span> | <span data-ttu-id="93c5d-230">Leere Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93c5d-230">empty string</span></span> | <span data-ttu-id="93c5d-231">Dieser Wert wird an die standardmäßige DrvFs Mount-Optionen-Zeichenfolge angefügt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-231">This value is appended to the default DrvFs mount options string.</span></span> **<span data-ttu-id="93c5d-232">Nur DrvFs-spezifische Optionen können angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="93c5d-232">Only DrvFs-specific options can be specified.</span></span>** <span data-ttu-id="93c5d-233">Optionen, die die Bereitstellung, die binäre normalerweise in einem Flag analysieren würde, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-233">Options that the mount binary would normally parse into a flag are not supported.</span></span> <span data-ttu-id="93c5d-234">Wenn Sie diese Optionen explizit angeben möchten, müssen Sie alle Laufwerke einschließen, die für die Sie dazu in/etc/fstab möchten.</span><span class="sxs-lookup"><span data-stu-id="93c5d-234">If you want to explicitly specify those options, you must include every drive for which you want to do so in /etc/fstab.</span></span> |

<span data-ttu-id="93c5d-235">Standardmäßig legt WSL die Uid und Gid auf den Wert des Standardbenutzers (im Ubuntu-Distribution, die Standardbenutzer ist mit einer Uid zwischen erstellt = 1000, Gid = 1000).</span><span class="sxs-lookup"><span data-stu-id="93c5d-235">By default, WSL sets the uid and gid to the value of the default user (in Ubuntu distro, the default user is created with uid=1000,gid=1000).</span></span> <span data-ttu-id="93c5d-236">Wenn der Benutzer eine Gruppen-ID oder die Uid-Option explizit über diesen Schlüssel angegeben ist, wird der zugehörige Wert überschrieben.</span><span class="sxs-lookup"><span data-stu-id="93c5d-236">If the user specifies a gid or uid option explicitly via this key, the associated value will be overwritten.</span></span> <span data-ttu-id="93c5d-237">Andernfalls wird der Standardwert immer angefügt.</span><span class="sxs-lookup"><span data-stu-id="93c5d-237">Otherwise, the default value will always be appended.</span></span>

<span data-ttu-id="93c5d-238">**Hinweis**: Diese Optionen werden als die Bereitstellungsoption für alle automatisch bereitgestellte Laufwerke angewendet.</span><span class="sxs-lookup"><span data-stu-id="93c5d-238">**Note:** These options are applied as the mount options for all automatically mounted drives.</span></span> <span data-ttu-id="93c5d-239">Um die Optionen für die nur ein bestimmtes Laufwerk ändern möchten, verwenden Sie stattdessen/etc/fstab.</span><span class="sxs-lookup"><span data-stu-id="93c5d-239">To change the options for a specific drive only, use /etc/fstab instead.</span></span>

#### <a name="network"></a><span data-ttu-id="93c5d-240">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="93c5d-240">network</span></span>

<span data-ttu-id="93c5d-241">Abschnittsbeschriftung:</span><span class="sxs-lookup"><span data-stu-id="93c5d-241">Section label:</span></span> `[network]`

| <span data-ttu-id="93c5d-242">key</span><span class="sxs-lookup"><span data-stu-id="93c5d-242">key</span></span> | <span data-ttu-id="93c5d-243">Wert</span><span class="sxs-lookup"><span data-stu-id="93c5d-243">value</span></span> | <span data-ttu-id="93c5d-244">default</span><span class="sxs-lookup"><span data-stu-id="93c5d-244">default</span></span> | <span data-ttu-id="93c5d-245">Anmerkungen zu dieser Version</span><span class="sxs-lookup"><span data-stu-id="93c5d-245">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="93c5d-246">generateHosts</span><span class="sxs-lookup"><span data-stu-id="93c5d-246">generateHosts</span></span> | <span data-ttu-id="93c5d-247">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-247">boolean</span></span> | `true` | `true` <span data-ttu-id="93c5d-248">Legt die WSL generieren `/etc/hosts`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-248">sets WSL to generate `/etc/hosts`.</span></span> <span data-ttu-id="93c5d-249">Die `hosts` -Datei enthält von Hostnamen entsprechende IP-Adresse eine statische Karte.</span><span class="sxs-lookup"><span data-stu-id="93c5d-249">The `hosts` file contains a static map of hostnames corresponding IP address.</span></span> |
| <span data-ttu-id="93c5d-250">generateResolvConf</span><span class="sxs-lookup"><span data-stu-id="93c5d-250">generateResolvConf</span></span> | <span data-ttu-id="93c5d-251">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-251">boolean</span></span> | `true` | `true` <span data-ttu-id="93c5d-252">Legen Sie die WSL generieren `/etc/resolv.conf`.</span><span class="sxs-lookup"><span data-stu-id="93c5d-252">set WSL to generate `/etc/resolv.conf`.</span></span> <span data-ttu-id="93c5d-253">Die `resolv.conf` enthält eine DNS-Serverliste, die einen bestimmten Hostnamen in seine IP-Adresse auflösen können.</span><span class="sxs-lookup"><span data-stu-id="93c5d-253">The `resolv.conf` contains a DNS list that are capable of resolving a given hostname to its IP address.</span></span> | 

#### <a name="interop"></a><span data-ttu-id="93c5d-254">Interop</span><span class="sxs-lookup"><span data-stu-id="93c5d-254">interop</span></span>

<span data-ttu-id="93c5d-255">Abschnittsbeschriftung:</span><span class="sxs-lookup"><span data-stu-id="93c5d-255">Section label:</span></span> `[interop]`

<span data-ttu-id="93c5d-256">Diese Optionen sind in Insider-Build 17713 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="93c5d-256">These options are available in Insider Build 17713 and later.</span></span>

| <span data-ttu-id="93c5d-257">key</span><span class="sxs-lookup"><span data-stu-id="93c5d-257">key</span></span> | <span data-ttu-id="93c5d-258">Wert</span><span class="sxs-lookup"><span data-stu-id="93c5d-258">value</span></span> | <span data-ttu-id="93c5d-259">default</span><span class="sxs-lookup"><span data-stu-id="93c5d-259">default</span></span> | <span data-ttu-id="93c5d-260">Anmerkungen zu dieser Version</span><span class="sxs-lookup"><span data-stu-id="93c5d-260">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="93c5d-261">enabled</span><span class="sxs-lookup"><span data-stu-id="93c5d-261">enabled</span></span> | <span data-ttu-id="93c5d-262">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-262">boolean</span></span> | `true` | <span data-ttu-id="93c5d-263">Einstellung, die diesem Schlüssel bestimmen, ob WSL beim Starten von Windows-Prozesse unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="93c5d-263">Setting this key will determine whether WSL will support launching Windows processes.</span></span> |
| <span data-ttu-id="93c5d-264">appendWindowsPath</span><span class="sxs-lookup"><span data-stu-id="93c5d-264">appendWindowsPath</span></span> | <span data-ttu-id="93c5d-265">boolean</span><span class="sxs-lookup"><span data-stu-id="93c5d-265">boolean</span></span> | `true` | <span data-ttu-id="93c5d-266">Einstellung, die diesem Schlüssel bestimmen, ob WSL Windows Pfadelemente die Umgebungsvariable $PATH hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="93c5d-266">Setting this key will determine whether WSL will add Windows path elements to the $PATH environment variable.</span></span> | 
