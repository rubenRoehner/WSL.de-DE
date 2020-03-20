---
title: Verwalten von Linux-Distributionen
description: Referenzliste und Konfigurieren mehrerer Linux-Distributionen, die unter dem Windows-Subsystem für Linux ausgeführt werden.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
ms.date: 02/7/2018
ms.topic: article
ms.assetid: 7ca59bd7-d9d3-4f6d-8b92-b8faa9bcf250
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: e69810625d08baf734683ff06231f79132ce1519
ms.sourcegitcommit: e1cc2fe4de0fa03d5aea14f6b328f1bb9d0c59be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/07/2019
ms.locfileid: "71999392"
---
# <a name="manage-and-configure-windows-subsystem-for-linux"></a><span data-ttu-id="5e833-104">Verwalten und Konfigurieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="5e833-104">Manage and configure Windows Subsystem for Linux</span></span>

> <span data-ttu-id="5e833-105">Gilt für Windows 10 Fall Creators Update oder höher.</span><span class="sxs-lookup"><span data-stu-id="5e833-105">Applies to Windows 10 Fall Creators Update and later.</span></span>  <span data-ttu-id="5e833-106">Lesen Sie unseren aktualisierten [Installationsleitfaden](./install_guide.md), um neue Verwaltungsfunktionen auszuprobieren und mehrere Linux-Distributionen aus dem Microsoft Store auszuführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-106">See our updated [installation guide](./install_guide.md) to try new management features and start running multiple Linux distributions from the Microsoft store.</span></span>

## <a name="ways-to-run-wsl"></a><span data-ttu-id="5e833-107">Möglichkeiten zum Ausführen von WSL</span><span class="sxs-lookup"><span data-stu-id="5e833-107">Ways to run WSL</span></span>

<span data-ttu-id="5e833-108">Es gibt viele Möglichkeiten, Linux mit dem Windows-Subsystem für Linux auszuführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-108">There are many ways to run Linux with the Windows Subsystem for Linux.</span></span>

1. <span data-ttu-id="5e833-109">`[distro]`, beispielsweise `ubuntu`</span><span class="sxs-lookup"><span data-stu-id="5e833-109">`[distro]`, for example `ubuntu`</span></span>
1. <span data-ttu-id="5e833-110">`wsl.exe` oder `bash.exe`</span><span class="sxs-lookup"><span data-stu-id="5e833-110">`wsl.exe` or `bash.exe`</span></span>
1. <span data-ttu-id="5e833-111">`wsl [command]` oder `bash -c [command]`</span><span class="sxs-lookup"><span data-stu-id="5e833-111">`wsl [command]` or `bash -c [command]`</span></span>

<span data-ttu-id="5e833-112">Welche Methode Sie verwenden sollten, hängt vom Anwendungsfall ab.</span><span class="sxs-lookup"><span data-stu-id="5e833-112">Which method you should use depends on what you're doing.</span></span>

### <a name="launch-wsl-by-distribution"></a><span data-ttu-id="5e833-113">Starten von WSL nach Distribution</span><span class="sxs-lookup"><span data-stu-id="5e833-113">Launch WSL by distribution</span></span>

<span data-ttu-id="5e833-114">Durch das Ausführen einer Distribution mit ihrer distributionsspezifischen Anwendung wird diese Distribution in einem eigenen Konsolenfenster gestartet.</span><span class="sxs-lookup"><span data-stu-id="5e833-114">Running a distribution using it's distro-specific application launches that distribution in it's own console window.</span></span>

![Starten von WSL aus dem Startmenü](media/start-launch.png)

<span data-ttu-id="5e833-116">Dies entspricht dem Klicken auf „Starten“ im Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="5e833-116">It is the same as clicking "Launch" in the Microsoft store.</span></span>

![Starten von WSL aus dem Microsoft Store](media/store-launch.png)

<span data-ttu-id="5e833-118">Sie können die Distribution auch über die Befehlszeile ausführen, indem Sie `[distribution].exe` ausführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-118">You can also run the distribution from the command line by running `[distribution].exe`.</span></span>

<span data-ttu-id="5e833-119">Der Nachteil, eine Distribution auf diese Weise über die Befehlszeile auszuführen, besteht darin, dass sich Ihr Arbeitsverzeichnis automatisch aus dem aktuellen Verzeichnis in das Startverzeichnis der Distribution ändert.</span><span class="sxs-lookup"><span data-stu-id="5e833-119">The disadvantage of running a distribution from the command line in this way is that it will automatically change your working directory from the current directory to the distribution's home directory.</span></span>

<span data-ttu-id="5e833-120">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-120">**Example:**</span></span>

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

### <a name="wsl-and-wsl-command"></a><span data-ttu-id="5e833-121">wsl und wsl [Befehl]</span><span class="sxs-lookup"><span data-stu-id="5e833-121">wsl and wsl [command]</span></span>

<span data-ttu-id="5e833-122">Die beste Methode zum Ausführen von WSL über die Befehlszeile ist die Verwendung von `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="5e833-122">The best way to run WSL from the command line is using `wsl.exe`.</span></span>

<span data-ttu-id="5e833-123">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-123">**Example:**</span></span>

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> wsl

scooley@scooley-elmer:/mnt/c/Users/sarah$ pwd
/mnt/c/Users/sarah
```

<span data-ttu-id="5e833-124">`wsl` behält nicht nur das aktuelle Arbeitsverzeichnis bei, sondern ermöglicht es auch, einen einzelnen Befehl neben Windows-Befehlen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-124">Not only does `wsl` keep the current working directory in place, it lets you run a single command along side Windows commands.</span></span>

<span data-ttu-id="5e833-125">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-125">**Example:**</span></span>

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

<span data-ttu-id="5e833-126">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-126">**Example:**</span></span>

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


## <a name="managing-multiple-linux-distributions"></a><span data-ttu-id="5e833-127">Verwalten mehrerer Linux-Distributionen</span><span class="sxs-lookup"><span data-stu-id="5e833-127">Managing multiple Linux Distributions</span></span>

### <a name="windows-10-version-1903-and-later"></a><span data-ttu-id="5e833-128">Windows 10, Version 1903 und höher</span><span class="sxs-lookup"><span data-stu-id="5e833-128">Windows 10 Version 1903 and later</span></span>

<span data-ttu-id="5e833-129">Mit `wsl.exe` können Sie Ihre Distributionen im Windows-Subsystem für Linux (WSL) verwalten, einschließlich der Liste der verfügbaren Distributionen, der Festlegung einer Standarddistribution und der Deinstallation von Distributionen.</span><span class="sxs-lookup"><span data-stu-id="5e833-129">You can use `wsl.exe` to manage your distributions in the Windows Subsystem for Linux (WSL), including listing available distributions, setting a default distribution, and uninstalling distributions.</span></span>

<span data-ttu-id="5e833-130">Jede Linux-Distribution verwaltet unabhängig ihre eigenen Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="5e833-130">Each Linux distribution independently manages its own configurations.</span></span> <span data-ttu-id="5e833-131">Führen Sie `[distro.exe] /?` aus, um distributionsspezifische Befehle anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="5e833-131">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="5e833-132">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="5e833-132">For example `ubuntu /?`.</span></span>

#### <a name="list-distributions"></a><span data-ttu-id="5e833-133">Auflisten von Distributionen</span><span class="sxs-lookup"><span data-stu-id="5e833-133">List distributions</span></span>

<span data-ttu-id="5e833-134">`wsl -l`, `wsl --list`</span><span class="sxs-lookup"><span data-stu-id="5e833-134">`wsl -l` , `wsl --list`</span></span>  
<span data-ttu-id="5e833-135">Listet verfügbare Linux-Distributionen für WSL auf.</span><span class="sxs-lookup"><span data-stu-id="5e833-135">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="5e833-136">Wenn eine Distribution aufgeführt wird, ist sie installiert und einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="5e833-136">If a distribution is listed, it's installed and ready to use.</span></span>

`wsl --list --all`   
<span data-ttu-id="5e833-137">Listet alle Distributionen auf, einschließlich derjenigen, die zurzeit nicht verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="5e833-137">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="5e833-138">Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.</span><span class="sxs-lookup"><span data-stu-id="5e833-138">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

`wsl --list --running`   
<span data-ttu-id="5e833-139">Listet alle Distributionen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-139">Lists all distributions that are currently running.</span></span>

#### <a name="set-a-default-distribution"></a><span data-ttu-id="5e833-140">Festlegen einer Standarddistribution</span><span class="sxs-lookup"><span data-stu-id="5e833-140">Set a default distribution</span></span>

<span data-ttu-id="5e833-141">Die WSL-Standarddistribution ist die Distribution, die ausgeführt wird, wenn Sie `wsl` in einer Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-141">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

<span data-ttu-id="5e833-142">`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`</span><span class="sxs-lookup"><span data-stu-id="5e833-142">`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`</span></span>

<span data-ttu-id="5e833-143">Legt die Standarddistribution auf `<DistributionName>` fest.</span><span class="sxs-lookup"><span data-stu-id="5e833-143">Sets the default distribution to `<DistributionName>`.</span></span>

<span data-ttu-id="5e833-144">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-144">**Example:**</span></span>  
<span data-ttu-id="5e833-145">`wsl -s Ubuntu` würde die Standarddistribution auf Ubuntu festlegen.</span><span class="sxs-lookup"><span data-stu-id="5e833-145">`wsl -s Ubuntu` would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="5e833-146">Wenn jetzt `wsl npm init` ausgeführt wird, wird Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5e833-146">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="5e833-147">Wenn `wsl` ausgeführt wird, wird eine Ubuntu-Sitzung geöffnet.</span><span class="sxs-lookup"><span data-stu-id="5e833-147">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="5e833-148">Aufheben der Registrierung und Neuinstallation einer Distribution</span><span class="sxs-lookup"><span data-stu-id="5e833-148">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="5e833-149">Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-149">While Linux distributions can be installed through the Microsoft store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="5e833-150">WSL Config ermöglicht die Aufhebung der Registrierung/Deinstallation von Distributionen.</span><span class="sxs-lookup"><span data-stu-id="5e833-150">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="5e833-151">Durch das Aufheben der Registrierung können Distributionen auch erneut installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-151">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="5e833-152">**Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Softwareanwendungen, die dieser Distribution zugeordnet sind, dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="5e833-152">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="5e833-153">Bei der erneuten Installation aus dem Store wird eine saubere Kopie der Distribution installiert.</span><span class="sxs-lookup"><span data-stu-id="5e833-153">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wsl --unregister <DistributionName>`  
<span data-ttu-id="5e833-154">Hebt die Registrierung der Distribution bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5e833-154">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="5e833-155">Beispiel: `wsl --unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Distributionen entfernen.</span><span class="sxs-lookup"><span data-stu-id="5e833-155">For example: `wsl --unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="5e833-156">Beim Ausführen von `wsl --list` würde diese Distribution nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="5e833-156">When I run `wsl --list` it will not be listed.</span></span>

<span data-ttu-id="5e833-157">Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie dann „Starten“ aus.</span><span class="sxs-lookup"><span data-stu-id="5e833-157">To reinstall, find the distribution in the Microsoft store and select "Launch".</span></span>

#### <a name="run-as-a-specific-user"></a><span data-ttu-id="5e833-158">Ausführen als ein bestimmter Benutzer</span><span class="sxs-lookup"><span data-stu-id="5e833-158">Run as a specific user</span></span>

<span data-ttu-id="5e833-159">`wsl -u <Username>`, `wsl --user <Username>`</span><span class="sxs-lookup"><span data-stu-id="5e833-159">`wsl -u <Username>`, `wsl --user <Username>`</span></span>

<span data-ttu-id="5e833-160">Führen Sie WSL als der angegebene Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="5e833-160">Run WSL as the specified user.</span></span> <span data-ttu-id="5e833-161">Beachten Sie, dass der Benutzer in der WSL-Distribution vorhanden sein muss.</span><span class="sxs-lookup"><span data-stu-id="5e833-161">Please note that user must exist inside of the WSL distribution.</span></span>

#### <a name="run-a-specific-distribution"></a><span data-ttu-id="5e833-162">Ausführen als eine bestimmte Distribution</span><span class="sxs-lookup"><span data-stu-id="5e833-162">Run a specific distribution</span></span>

<span data-ttu-id="5e833-163">`wsl -d <DistributionName>`, `wsl --distribution <DistributionName>`</span><span class="sxs-lookup"><span data-stu-id="5e833-163">`wsl -d <DistributionName>`, `wsl --distribution <DistributionName>`</span></span>

<span data-ttu-id="5e833-164">Führen Sie eine angegebene Distribution von WSL aus. Kann zum Senden von Befehlen an eine bestimmte Distribution verwendet werden, ohne die Standardeinstellung ändern zu müssen.</span><span class="sxs-lookup"><span data-stu-id="5e833-164">Run a specified distribution of WSL, can be used to send commands to a specific distribution without having to change your default.</span></span>

### <a name="versions-earlier-than-windows-10-version-1903"></a><span data-ttu-id="5e833-165">Frühere Versionen als Windows 10, Version 1903</span><span class="sxs-lookup"><span data-stu-id="5e833-165">Versions Earlier than Windows 10 Version 1903</span></span>

<span data-ttu-id="5e833-166">WSL Config (`wslconfig.exe`) ist ein Befehlszeilen Tool zum Verwalten von Linux-Distributionen, die unter dem Windows-Subsystem für Linux (WSL) ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-166">WSL Config (`wslconfig.exe`) is a command-line tool for managing Linux distributions running on the Windows Subsystem for Linux (WSL).</span></span>  <span data-ttu-id="5e833-167">Damit können Sie verfügbare Distributionen auflisten, eine Standarddistribution festlegen und Distributionen deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="5e833-167">It lets you list available distributions, set a default distribution, and uninstall distributions.</span></span>

<span data-ttu-id="5e833-168">Während WSL Config für Einstellungen nützlich ist, die Distributionen umspannen oder koordinieren, verwaltet jede Linux-Distribution unabhängig ihre eigenen Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="5e833-168">While WSL Config is helpful for settings that span or coordinate distributions, each Linux distribution independently manages its own configurations.</span></span>  <span data-ttu-id="5e833-169">Führen Sie `[distro.exe] /?` aus, um distributionsspezifische Befehle anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="5e833-169">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="5e833-170">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="5e833-170">For example `ubuntu /?`.</span></span>

<span data-ttu-id="5e833-171">Um alle verfügbaren Optionen für wslconfig anzuzeigen, führen Sie Folgendes aus: `wslconfig /?`</span><span class="sxs-lookup"><span data-stu-id="5e833-171">To see all available options for wslconfig, run:  `wslconfig /?`</span></span>

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

#### <a name="list-distributions"></a><span data-ttu-id="5e833-172">Auflisten von Distributionen</span><span class="sxs-lookup"><span data-stu-id="5e833-172">List distributions</span></span>

`wslconfig /list`  
<span data-ttu-id="5e833-173">Listet verfügbare Linux-Distributionen für WSL auf.</span><span class="sxs-lookup"><span data-stu-id="5e833-173">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="5e833-174">Wenn eine Distribution aufgeführt wird, ist sie installiert und einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="5e833-174">If a distribution is listed, it's installed and ready to use.</span></span>

`wslconfig /list /all`  
<span data-ttu-id="5e833-175">Listet alle Distributionen auf, einschließlich derjenigen, die zurzeit nicht verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="5e833-175">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="5e833-176">Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.</span><span class="sxs-lookup"><span data-stu-id="5e833-176">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

#### <a name="set-a-default-distribution"></a><span data-ttu-id="5e833-177">Festlegen einer Standarddistribution</span><span class="sxs-lookup"><span data-stu-id="5e833-177">Set a default distribution</span></span>

<span data-ttu-id="5e833-178">Die WSL-Standarddistribution ist die Distribution, die ausgeführt wird, wenn Sie `wsl` in einer Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="5e833-178">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

`wslconfig /setdefault <DistributionName>`

<span data-ttu-id="5e833-179">Legt die Standarddistribution auf `<DistributionName>` fest.</span><span class="sxs-lookup"><span data-stu-id="5e833-179">Sets the default distribution to `<DistributionName>`.</span></span>

<span data-ttu-id="5e833-180">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="5e833-180">**Example:**</span></span>  
<span data-ttu-id="5e833-181">`wslconfig /setdefault Ubuntu` würde die Standarddistribution auf Ubuntu festlegen.</span><span class="sxs-lookup"><span data-stu-id="5e833-181">`wslconfig /setdefault Ubuntu` would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="5e833-182">Wenn jetzt `wsl npm init` ausgeführt wird, wird Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5e833-182">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="5e833-183">Wenn `wsl` ausgeführt wird, wird eine Ubuntu-Sitzung geöffnet.</span><span class="sxs-lookup"><span data-stu-id="5e833-183">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="5e833-184">Aufheben der Registrierung und Neuinstallation einer Distribution</span><span class="sxs-lookup"><span data-stu-id="5e833-184">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="5e833-185">Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-185">While Linux distributions can be installed through the Microsoft store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="5e833-186">WSL Config ermöglicht die Aufhebung der Registrierung/Deinstallation von Distributionen.</span><span class="sxs-lookup"><span data-stu-id="5e833-186">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="5e833-187">Durch das Aufheben der Registrierung können Distributionen auch erneut installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-187">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="5e833-188">**Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Softwareanwendungen, die dieser Distribution zugeordnet sind, dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="5e833-188">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="5e833-189">Bei der erneuten Installation aus dem Store wird eine saubere Kopie der Distribution installiert.</span><span class="sxs-lookup"><span data-stu-id="5e833-189">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wslconfig /unregister <DistributionName>`  
<span data-ttu-id="5e833-190">Hebt die Registrierung der Distribution bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5e833-190">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="5e833-191">Beispiel: `wslconfig /unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Distributionen entfernen.</span><span class="sxs-lookup"><span data-stu-id="5e833-191">For example: `wslconfig /unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="5e833-192">Beim Ausführen von `wslconfig /list` würde diese Distribution nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="5e833-192">When I run `wslconfig /list` it will not be listed.</span></span>

<span data-ttu-id="5e833-193">Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie dann „Starten“ aus.</span><span class="sxs-lookup"><span data-stu-id="5e833-193">To reinstall, find the distribution in the Microsoft store and select "Launch".</span></span>

## <a name="set-wsl-launch-settings"></a><span data-ttu-id="5e833-194">Festlegen der WSL-Starteinstellungen</span><span class="sxs-lookup"><span data-stu-id="5e833-194">Set WSL launch settings</span></span>

> <span data-ttu-id="5e833-195">**Verfügbar in Windows Insider Build 17093 und höher**</span><span class="sxs-lookup"><span data-stu-id="5e833-195">**Available in Windows Insider Build 17093 and later**</span></span>

<span data-ttu-id="5e833-196">Konfigurieren Sie automatisch bestimmte Funktionen in WSL, die jedes Mal angewendet werden, wenn Sie das Subsystem mithilfe von `wsl.conf` starten.</span><span class="sxs-lookup"><span data-stu-id="5e833-196">Automatically configure certain functionality in WSL that will be applied every time you launch the subsystem using `wsl.conf`.</span></span> 

<span data-ttu-id="5e833-197">Zurzeit umfasst dies Optionen für die automatische Einbindung und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5e833-197">Right now, this includes automount options and network configuration.</span></span>

<span data-ttu-id="5e833-198">`wsl.conf` befindet sich in jeder Linux-Distribution in `/etc/wsl.conf`.</span><span class="sxs-lookup"><span data-stu-id="5e833-198">`wsl.conf` is located in each Linux distribution in `/etc/wsl.conf`.</span></span> <span data-ttu-id="5e833-199">Wenn die Datei nicht vorhanden ist, können Sie sie selbst erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e833-199">If the file is not there, you can create it yourself.</span></span> <span data-ttu-id="5e833-200">WSL erkennt das Vorhandensein der Datei und liest ihren Inhalt.</span><span class="sxs-lookup"><span data-stu-id="5e833-200">WSL will detect the existence of the file and will read its contents.</span></span> <span data-ttu-id="5e833-201">Wenn die Datei fehlt oder falsch formatiert ist (d.h. falsche Markupformatierung), wird WSL weiterhin normal gestartet.</span><span class="sxs-lookup"><span data-stu-id="5e833-201">If the file is missing or malformed (that is, improper markup formatting), WSL will continue to launch as normal.</span></span>

<span data-ttu-id="5e833-202">Im folgenden finden Sie eine Beispieldatei `wsl.conf`, die Sie Ihren Distributionen hinzufügen können:</span><span class="sxs-lookup"><span data-stu-id="5e833-202">Here is a sample `wsl.conf` file you could add into your distros:</span></span>

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

### <a name="configuration-options"></a><span data-ttu-id="5e833-203">Konfigurationsoptionen</span><span class="sxs-lookup"><span data-stu-id="5e833-203">Configuration Options</span></span>

<span data-ttu-id="5e833-204">In Übereinstimmung mit INI-Konventionen werden Schlüssel in einem Abschnitt deklariert.</span><span class="sxs-lookup"><span data-stu-id="5e833-204">In keeping with .ini conventions, keys are declared under a section.</span></span> 

<span data-ttu-id="5e833-205">WSL unterstützt zwei Abschnitte: `automount` und `network`.</span><span class="sxs-lookup"><span data-stu-id="5e833-205">WSL supports two sections: `automount` and `network`.</span></span>

#### <a name="automount"></a><span data-ttu-id="5e833-206">automount</span><span class="sxs-lookup"><span data-stu-id="5e833-206">automount</span></span>

<span data-ttu-id="5e833-207">Abschnitt: `[automount]`</span><span class="sxs-lookup"><span data-stu-id="5e833-207">Section: `[automount]`</span></span>


| <span data-ttu-id="5e833-208">key</span><span class="sxs-lookup"><span data-stu-id="5e833-208">key</span></span>        | <span data-ttu-id="5e833-209">value</span><span class="sxs-lookup"><span data-stu-id="5e833-209">value</span></span>                          | <span data-ttu-id="5e833-210">Standard</span><span class="sxs-lookup"><span data-stu-id="5e833-210">default</span></span>      | <span data-ttu-id="5e833-211">notes</span><span class="sxs-lookup"><span data-stu-id="5e833-211">notes</span></span>                                                                                                                                                                                                                                                                                                                          |
|:-----------|:-------------------------------|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5e833-212">enabled</span><span class="sxs-lookup"><span data-stu-id="5e833-212">enabled</span></span>    | <span data-ttu-id="5e833-213">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-213">boolean</span></span>                        | <span data-ttu-id="5e833-214">wahr</span><span class="sxs-lookup"><span data-stu-id="5e833-214">true</span></span>         | <span data-ttu-id="5e833-215">`true` bewirkt, dass lokale Festplattenlaufwerke (d.h.</span><span class="sxs-lookup"><span data-stu-id="5e833-215">`true` causes fixed drives (i.e</span></span> <span data-ttu-id="5e833-216">`C:/` oder `D:/`) mit DrvFs automatisch unter `/mnt` eingebunden werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-216">`C:/` or `D:/`) to be automatically mounted with DrvFs under `/mnt`.</span></span>  <span data-ttu-id="5e833-217">`false` bedeutet, dass Laufwerke nicht automatisch eingebunden werden, aber Sie können sie dennoch manuell oder über `fstab` einbinden.</span><span class="sxs-lookup"><span data-stu-id="5e833-217">`false` means drives won’t be mounted automatically, but you could still mount them manually or via `fstab`.</span></span>                                                                                                             |
| <span data-ttu-id="5e833-218">mountFsTab</span><span class="sxs-lookup"><span data-stu-id="5e833-218">mountFsTab</span></span> | <span data-ttu-id="5e833-219">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-219">boolean</span></span>                        | <span data-ttu-id="5e833-220">wahr</span><span class="sxs-lookup"><span data-stu-id="5e833-220">true</span></span>         | <span data-ttu-id="5e833-221">`true` legt fest, dass `/etc/fstab` beim WSL-Start verarbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="5e833-221">`true` sets `/etc/fstab` to be processed on WSL start.</span></span> <span data-ttu-id="5e833-222">Bei „/etc/fstab“ handelt es sich um eine Datei, in der Sie andere Dateisysteme wie eine SMB-Freigabe deklarieren können.</span><span class="sxs-lookup"><span data-stu-id="5e833-222">/etc/fstab is a file where you can declare other filesystems, like an SMB share.</span></span> <span data-ttu-id="5e833-223">Daher können Sie diese Dateisysteme beim Start automatisch in WSL einbinden.</span><span class="sxs-lookup"><span data-stu-id="5e833-223">Thus, you can mount these filesystems automatically in WSL on start up.</span></span>                                                                                                                |
| <span data-ttu-id="5e833-224">root</span><span class="sxs-lookup"><span data-stu-id="5e833-224">root</span></span>       | <span data-ttu-id="5e833-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e833-225">String</span></span>                         | `/mnt/`      | <span data-ttu-id="5e833-226">Legt das Verzeichnis fest, in dem lokale Festplattenlaufwerke automatisch eingebunden werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-226">Sets the directory where fixed drives will be automatically mounted.</span></span> <span data-ttu-id="5e833-227">Wenn Sie z.B. ein Verzeichnis unter `/windir/` in WSL verwenden und Sie dieses als Stammverzeichnis angeben, erwarten Sie, dass die lokalen Festplattenlaufwerke unter `/windir/c` eingebunden werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-227">For example, if you have a directory in WSL at `/windir/` and you specify that as the root, you would expect to see your fixed drives mounted at `/windir/c`</span></span>                                                                                              |
| <span data-ttu-id="5e833-228">Optionen</span><span class="sxs-lookup"><span data-stu-id="5e833-228">options</span></span>    | <span data-ttu-id="5e833-229">Durch Kommas getrennte Liste mit Werten</span><span class="sxs-lookup"><span data-stu-id="5e833-229">comma-separated list of values</span></span> | <span data-ttu-id="5e833-230">Leere Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e833-230">empty string</span></span> | <span data-ttu-id="5e833-231">Dieser Wert wird an die Standardzeichenfolge der DrvFs-Einbindungsoptionen angefügt.</span><span class="sxs-lookup"><span data-stu-id="5e833-231">This value is appended to the default DrvFs mount options string.</span></span> <span data-ttu-id="5e833-232">**Es können nur DrvFs-spezifische Optionen angegeben werden.**</span><span class="sxs-lookup"><span data-stu-id="5e833-232">**Only DrvFs-specific options can be specified.**</span></span> <span data-ttu-id="5e833-233">Optionen, die die Einbindungsbinärdatei normalerweise in ein Flag analysieren würde, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e833-233">Options that the mount binary would normally parse into a flag are not supported.</span></span> <span data-ttu-id="5e833-234">Wenn Sie diese Optionen explizit angeben möchten, müssen Sie jedes Laufwerk, für das dies gelten soll, in „/etc/fstab“ einschließen.</span><span class="sxs-lookup"><span data-stu-id="5e833-234">If you want to explicitly specify those options, you must include every drive for which you want to do so in /etc/fstab.</span></span> |

<span data-ttu-id="5e833-235">Standardmäßig legt WSL die UID und die GID auf den Wert des Standardbenutzers fest (in der Ubuntu-Distribution wird der Standardbenutzer mit „uid=1000,gid=1000“ erstellt).</span><span class="sxs-lookup"><span data-stu-id="5e833-235">By default, WSL sets the uid and gid to the value of the default user (in Ubuntu distro, the default user is created with uid=1000,gid=1000).</span></span> <span data-ttu-id="5e833-236">Wenn der Benutzer eine GID-oder UID-Option explizit über diesen Schlüssel angibt, wird der zugehörige Wert überschrieben.</span><span class="sxs-lookup"><span data-stu-id="5e833-236">If the user specifies a gid or uid option explicitly via this key, the associated value will be overwritten.</span></span> <span data-ttu-id="5e833-237">Andernfalls wird der Standardwert immer angefügt.</span><span class="sxs-lookup"><span data-stu-id="5e833-237">Otherwise, the default value will always be appended.</span></span>

<span data-ttu-id="5e833-238">**Hinweis:** Diese Optionen werden als Einbindungsoptionen für alle automatisch eingebundenen Laufwerke angewendet.</span><span class="sxs-lookup"><span data-stu-id="5e833-238">**Note:** These options are applied as the mount options for all automatically mounted drives.</span></span> <span data-ttu-id="5e833-239">Verwenden Sie stattdessen „/etc/fstab“, um die Optionen nur für ein bestimmtes Laufwerk zu ändern.</span><span class="sxs-lookup"><span data-stu-id="5e833-239">To change the options for a specific drive only, use /etc/fstab instead.</span></span>

##### <a name="mount-options"></a><span data-ttu-id="5e833-240">Einbindungsoptionen</span><span class="sxs-lookup"><span data-stu-id="5e833-240">Mount options</span></span>

<span data-ttu-id="5e833-241">Durch Festlegen verschiedener Einbindungsoptionen für Windows-Laufwerke (DrvFs) kann gesteuert werden, wie Dateiberechtigungen für Windows-Dateien berechnet werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-241">Setting different mount options for Windows drives (DrvFs) can control how file permissions are calculated for Windows files.</span></span> <span data-ttu-id="5e833-242">Die folgenden Optionen sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="5e833-242">The following options are available:</span></span>

| <span data-ttu-id="5e833-243">Schlüssel</span><span class="sxs-lookup"><span data-stu-id="5e833-243">Key</span></span> | <span data-ttu-id="5e833-244">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e833-244">Description</span></span> | <span data-ttu-id="5e833-245">Standardwert</span><span class="sxs-lookup"><span data-stu-id="5e833-245">Default</span></span> |
|:----|:----|:----|
|<span data-ttu-id="5e833-246">uid</span><span class="sxs-lookup"><span data-stu-id="5e833-246">uid</span></span>| <span data-ttu-id="5e833-247">Die Benutzer-ID, die für den Besitzer aller Dateien verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5e833-247">The User ID used for the owner of all files</span></span> | <span data-ttu-id="5e833-248">Die Standard-Benutzer-ID Ihrer WSL-Distribution (bei der erstmaligen Installation ist der Standardwert 1000)</span><span class="sxs-lookup"><span data-stu-id="5e833-248">The default User ID of your WSL distro (On first installation this defaults to 1000)</span></span>
|<span data-ttu-id="5e833-249">gid</span><span class="sxs-lookup"><span data-stu-id="5e833-249">gid</span></span>| <span data-ttu-id="5e833-250">Die Gruppen-ID, die für den Besitzer aller Dateien verwendet wird</span><span class="sxs-lookup"><span data-stu-id="5e833-250">The Group ID used for the owner of all files</span></span> | <span data-ttu-id="5e833-251">Die Standard-Gruppen-ID Ihrer WSL-Distribution (bei der erstmaligen Installation ist der Standardwert 1000)</span><span class="sxs-lookup"><span data-stu-id="5e833-251">The default group ID of your WSL distro (On first installation this defaults to 1000)</span></span>
|<span data-ttu-id="5e833-252">umask</span><span class="sxs-lookup"><span data-stu-id="5e833-252">umask</span></span> | <span data-ttu-id="5e833-253">Eine oktale Maske mit Berechtigungen, die für alle Dateien und Verzeichnisse ausgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="5e833-253">An octal mask of permissions to exclude for all files and directories</span></span> | <span data-ttu-id="5e833-254">000</span><span class="sxs-lookup"><span data-stu-id="5e833-254">000</span></span>
|<span data-ttu-id="5e833-255">fmask</span><span class="sxs-lookup"><span data-stu-id="5e833-255">fmask</span></span> | <span data-ttu-id="5e833-256">Eine oktale Maske mit Berechtigungen, die für alle Dateien ausgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="5e833-256">An octal mask of permissions to exclude for all files</span></span> | <span data-ttu-id="5e833-257">000</span><span class="sxs-lookup"><span data-stu-id="5e833-257">000</span></span>
|<span data-ttu-id="5e833-258">dmask</span><span class="sxs-lookup"><span data-stu-id="5e833-258">dmask</span></span> | <span data-ttu-id="5e833-259">Eine oktale Maske mit Berechtigungen, die für alle Verzeichnisse ausgeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="5e833-259">An octal mask of permissions to exclude for all directories</span></span> | <span data-ttu-id="5e833-260">000</span><span class="sxs-lookup"><span data-stu-id="5e833-260">000</span></span>

<span data-ttu-id="5e833-261">**Hinweis:** Die Berechtigungsmasken werden durch eine logische ODER-Operation festgelegt, bevor sie auf Dateien oder Verzeichnisse angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="5e833-261">**Note:** The permission masks are put through a logical OR operation before being applied to files or directories.</span></span> 

#### <a name="network"></a><span data-ttu-id="5e833-262">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="5e833-262">network</span></span>

<span data-ttu-id="5e833-263">Abschnittsbezeichnung: `[network]`</span><span class="sxs-lookup"><span data-stu-id="5e833-263">Section label: `[network]`</span></span>

| <span data-ttu-id="5e833-264">key</span><span class="sxs-lookup"><span data-stu-id="5e833-264">key</span></span> | <span data-ttu-id="5e833-265">value</span><span class="sxs-lookup"><span data-stu-id="5e833-265">value</span></span> | <span data-ttu-id="5e833-266">Standard</span><span class="sxs-lookup"><span data-stu-id="5e833-266">default</span></span> | <span data-ttu-id="5e833-267">notes</span><span class="sxs-lookup"><span data-stu-id="5e833-267">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="5e833-268">generateHosts</span><span class="sxs-lookup"><span data-stu-id="5e833-268">generateHosts</span></span> | <span data-ttu-id="5e833-269">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-269">boolean</span></span> | `true` | <span data-ttu-id="5e833-270">`true` legt fest, dass WSL `/etc/hosts` generiert.</span><span class="sxs-lookup"><span data-stu-id="5e833-270">`true` sets WSL to generate `/etc/hosts`.</span></span> <span data-ttu-id="5e833-271">Die Datei `hosts` enthält eine statische Zuordnung der entsprechenden IP-Adresse von Hostnamen.</span><span class="sxs-lookup"><span data-stu-id="5e833-271">The `hosts` file contains a static map of hostnames corresponding IP address.</span></span> |
| <span data-ttu-id="5e833-272">generateResolvConf</span><span class="sxs-lookup"><span data-stu-id="5e833-272">generateResolvConf</span></span> | <span data-ttu-id="5e833-273">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-273">boolean</span></span> | `true` | <span data-ttu-id="5e833-274">`true` legt fest, dass WSL `/etc/resolv.conf` generiert.</span><span class="sxs-lookup"><span data-stu-id="5e833-274">`true` set WSL to generate `/etc/resolv.conf`.</span></span> <span data-ttu-id="5e833-275">`resolv.conf` enthält eine DNS-Liste, mit der ein angegebener Hostnamen in seine IP-Adresse aufgelöst werden kann.</span><span class="sxs-lookup"><span data-stu-id="5e833-275">The `resolv.conf` contains a DNS list that are capable of resolving a given hostname to its IP address.</span></span> | 

#### <a name="interop"></a><span data-ttu-id="5e833-276">interop</span><span class="sxs-lookup"><span data-stu-id="5e833-276">interop</span></span>

<span data-ttu-id="5e833-277">Abschnittsbezeichnung: `[interop]`</span><span class="sxs-lookup"><span data-stu-id="5e833-277">Section label: `[interop]`</span></span>

<span data-ttu-id="5e833-278">Diese Optionen sind in Insider Build 17713 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5e833-278">These options are available in Insider Build 17713 and later.</span></span>

| <span data-ttu-id="5e833-279">key</span><span class="sxs-lookup"><span data-stu-id="5e833-279">key</span></span> | <span data-ttu-id="5e833-280">value</span><span class="sxs-lookup"><span data-stu-id="5e833-280">value</span></span> | <span data-ttu-id="5e833-281">Standard</span><span class="sxs-lookup"><span data-stu-id="5e833-281">default</span></span> | <span data-ttu-id="5e833-282">notes</span><span class="sxs-lookup"><span data-stu-id="5e833-282">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="5e833-283">enabled</span><span class="sxs-lookup"><span data-stu-id="5e833-283">enabled</span></span> | <span data-ttu-id="5e833-284">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-284">boolean</span></span> | `true` | <span data-ttu-id="5e833-285">Durch Festlegen dieses Schlüssels wird festgelegt, ob WSL das Starten von Windows-Prozessen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e833-285">Setting this key will determine whether WSL will support launching Windows processes.</span></span> |
| <span data-ttu-id="5e833-286">appendWindowsPath</span><span class="sxs-lookup"><span data-stu-id="5e833-286">appendWindowsPath</span></span> | <span data-ttu-id="5e833-287">boolean</span><span class="sxs-lookup"><span data-stu-id="5e833-287">boolean</span></span> | `true` | <span data-ttu-id="5e833-288">Durch Festlegen dieses Schlüssels wird festgelegt, ob WSL der $PATH-Umgebungsvariablen Windows-Pfadelemente hinzufügt.</span><span class="sxs-lookup"><span data-stu-id="5e833-288">Setting this key will determine whether WSL will add Windows path elements to the $PATH environment variable.</span></span> | 
