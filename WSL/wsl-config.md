---
title: Verwalten von Linux-Distributionen
description: Referenz zum Auflisten und Konfigurieren mehrerer Linux-Distributionen, die auf dem Windows-Subsystem für Linux ausgeführt werden.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, WSL. conf, wslconfig
author: scooley
ms.author: scooley
ms.date: 02/7/2018
ms.topic: article
ms.assetid: 7ca59bd7-d9d3-4f6d-8b92-b8faa9bcf250
ms.custom: seodec18
ms.openlocfilehash: 0c9f9315b17d5156aa111e7619ee25534653b27e
ms.sourcegitcommit: 5844c6dbf692780b86b30bd65e11820fff43b3bd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2019
ms.locfileid: "67499276"
---
# <a name="manage-and-configure-windows-subsystem-for-linux"></a><span data-ttu-id="2ca12-104">Verwalten und Konfigurieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="2ca12-104">Manage and configure Windows Subsystem for Linux</span></span>

> <span data-ttu-id="2ca12-105">Gilt für Windows 10 Fall Creators Update und höher.</span><span class="sxs-lookup"><span data-stu-id="2ca12-105">Applies to Windows 10 Fall Creators Update and later.</span></span>  <span data-ttu-id="2ca12-106">Weitere Informationen zu neuen Verwaltungs Features und zum Ausführen mehrerer Linux-Distributionen aus dem Microsoft Store finden Sie in unserem aktualisierten [Installationshandbuch](./install_guide.md) .</span><span class="sxs-lookup"><span data-stu-id="2ca12-106">See our updated [installation guide](./install_guide.md) to try new management features and start running multiple Linux distributions from the Microsoft store.</span></span>

## <a name="ways-to-run-wsl"></a><span data-ttu-id="2ca12-107">Möglichkeiten zum Ausführen von WSL</span><span class="sxs-lookup"><span data-stu-id="2ca12-107">Ways to run WSL</span></span>

<span data-ttu-id="2ca12-108">Es gibt viele Möglichkeiten, Linux mit dem Windows-Subsystem für Linux auszuführen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-108">There are many ways to run Linux with the Windows Subsystem for Linux.</span></span>

1. <span data-ttu-id="2ca12-109">`[distro]`Zum Beispiel`ubuntu`</span><span class="sxs-lookup"><span data-stu-id="2ca12-109">`[distro]`, for example `ubuntu`</span></span>
1. <span data-ttu-id="2ca12-110">`wsl.exe` oder `bash.exe`</span><span class="sxs-lookup"><span data-stu-id="2ca12-110">`wsl.exe` or `bash.exe`</span></span>
1. <span data-ttu-id="2ca12-111">`wsl [command]` oder `bash -c [command]`</span><span class="sxs-lookup"><span data-stu-id="2ca12-111">`wsl [command]` or `bash -c [command]`</span></span>

<span data-ttu-id="2ca12-112">Welche Methode Sie verwenden sollten, hängt davon ab, was Sie gerade tun.</span><span class="sxs-lookup"><span data-stu-id="2ca12-112">Which method you should use depends on what you're doing.</span></span>

### <a name="launch-wsl-by-distribution"></a><span data-ttu-id="2ca12-113">Starten von WSL nach Verteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-113">Launch WSL by distribution</span></span>

<span data-ttu-id="2ca12-114">Durch das Ausführen einer Verteilung mit der IT-spezifischen Anwendung wird diese Distribution im eigenen Konsolenfenster gestartet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-114">Running a distribution using it's distro-specific application launches that distribution in it's own console window.</span></span>

![Starten von WSL über das Startmenü](media/start-launch.png)

<span data-ttu-id="2ca12-116">Dies entspricht dem Klicken auf "starten" im Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="2ca12-116">It is the same as clicking "Launch" in the Microsoft store.</span></span>

![Starten von WSL aus dem Microsoft Store](media/store-launch.png)

<span data-ttu-id="2ca12-118">Sie können die Verteilung auch über die Befehlszeile ausführen, indem `[distribution].exe`Sie ausführen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-118">You can also run the distribution from the command line by running `[distribution].exe`.</span></span>

<span data-ttu-id="2ca12-119">Der Nachteil der Ausführung einer Verteilung von der Befehlszeile auf diese Weise besteht darin, dass das Arbeitsverzeichnis automatisch vom aktuellen Verzeichnis in das Basisverzeichnis der Distribution geändert wird.</span><span class="sxs-lookup"><span data-stu-id="2ca12-119">The disadvantage of running a distribution from the command line in this way is that it will automatically change your working directory from the current directory to the distribution's home directory.</span></span>

<span data-ttu-id="2ca12-120">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-120">**Example:**</span></span>

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

### <a name="wsl-and-wsl-command"></a><span data-ttu-id="2ca12-121">WSL und WSL [Befehl]</span><span class="sxs-lookup"><span data-stu-id="2ca12-121">wsl and wsl [command]</span></span>

<span data-ttu-id="2ca12-122">Die beste Methode zum Ausführen von WSL von der Befehlszeile aus `wsl.exe`ist die Verwendung von.</span><span class="sxs-lookup"><span data-stu-id="2ca12-122">The best way to run WSL from the command line is using `wsl.exe`.</span></span>

<span data-ttu-id="2ca12-123">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-123">**Example:**</span></span>

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> wsl

scooley@scooley-elmer:/mnt/c/Users/sarah$ pwd
/mnt/c/Users/sarah
```

<span data-ttu-id="2ca12-124">Das aktuelle Arbeits `wsl` Verzeichnis wird nicht nur auf dem neuesten Stand gehalten, sondern Sie können auch einen einzelnen Befehl entlang von Windows-Befehlszeilen ausführen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-124">Not only does `wsl` keep the current working directory in place, it lets you run a single command along side Windows commands.</span></span>

<span data-ttu-id="2ca12-125">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-125">**Example:**</span></span>

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

<span data-ttu-id="2ca12-126">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-126">**Example:**</span></span>

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


## <a name="managing-multiple-linux-distributions"></a><span data-ttu-id="2ca12-127">Verwalten mehrerer Linux-Distributionen</span><span class="sxs-lookup"><span data-stu-id="2ca12-127">Managing multiple Linux Distributions</span></span>

### <a name="windows-10-version-1903-and-later"></a><span data-ttu-id="2ca12-128">Windows 10, Version 1903 und höher</span><span class="sxs-lookup"><span data-stu-id="2ca12-128">Windows 10 Version 1903 and later</span></span>

<span data-ttu-id="2ca12-129">Sie können verwenden `wsl.exe` , um die Verteilungen im Windows-Subsystem für Linux (WSL) zu verwalten, einschließlich der Auflistung verfügbarer Verteilungen, dem Festlegen einer Standardverteilung und der Deinstallieren von Verteilungen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-129">You can use `wsl.exe` to manage your distributions in the Windows Subsystem for Linux (WSL), including listing available distributions, setting a default distribution, and uninstalling distributions.</span></span>

<span data-ttu-id="2ca12-130">Jede Linux-Distribution verwaltet unabhängig seine eigenen Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-130">Each Linux distribution independently manages its own configurations.</span></span> <span data-ttu-id="2ca12-131">Führen `[distro.exe] /?`Sie aus, um Verteilungs spezifische Befehle anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-131">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="2ca12-132">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="2ca12-132">For example `ubuntu /?`.</span></span>

#### <a name="list-distributions"></a><span data-ttu-id="2ca12-133">Verteilungen auflisten</span><span class="sxs-lookup"><span data-stu-id="2ca12-133">List distributions</span></span>

<span data-ttu-id="2ca12-134">`wsl -l`,`wsl --list`</span><span class="sxs-lookup"><span data-stu-id="2ca12-134">`wsl -l` , `wsl --list`</span></span>  
<span data-ttu-id="2ca12-135">Listet verfügbare Linux-Distributionen für WSL auf.</span><span class="sxs-lookup"><span data-stu-id="2ca12-135">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="2ca12-136">Wenn eine Distribution aufgeführt ist, ist Sie installiert und einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="2ca12-136">If a distribution is listed, it's installed and ready to use.</span></span>

`wsl --list --all`   
<span data-ttu-id="2ca12-137">Listet alle Verteilungen auf, einschließlich derjenigen, die derzeit nicht verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="2ca12-137">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="2ca12-138">Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-138">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

`wsl --list --running`   
<span data-ttu-id="2ca12-139">Listet alle Verteilungen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-139">Lists all distributions that are currently running.</span></span>

#### <a name="set-a-default-distribution"></a><span data-ttu-id="2ca12-140">Festlegen einer Standardverteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-140">Set a default distribution</span></span>

<span data-ttu-id="2ca12-141">Die standardmäßige WSL-Verteilung ist die, die ausgeführt wird `wsl` , wenn Sie in einer Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-141">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

<span data-ttu-id="2ca12-142">`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`</span><span class="sxs-lookup"><span data-stu-id="2ca12-142">`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`</span></span>

<span data-ttu-id="2ca12-143">Legt die Standardverteilung auf `<DistributionName>`fest.</span><span class="sxs-lookup"><span data-stu-id="2ca12-143">Sets the default distribution to `<DistributionName>`.</span></span>

<span data-ttu-id="2ca12-144">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-144">**Example:**</span></span>  
<span data-ttu-id="2ca12-145">`wsl -s Ubuntu`legt die Standardverteilung auf Ubuntu fest.</span><span class="sxs-lookup"><span data-stu-id="2ca12-145">`wsl -s Ubuntu` would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="2ca12-146">Wenn die Anwendung ausgeführt `wsl npm init` wird, wird Sie jetzt in Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-146">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="2ca12-147">Wenn ich das `wsl` ausführen, wird eine Ubuntu-Sitzung geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-147">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="2ca12-148">Aufheben der Registrierung und Neuinstallation einer Verteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-148">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="2ca12-149">Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-149">While Linux distributions can be installed through the Microsoft store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="2ca12-150">Die WSL-Konfiguration ermöglicht die Registrierung/Deinstallieren von Distributionen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-150">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="2ca12-151">Durch die Aufhebung der Registrierung können auch Verteilungen erneut installiert werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-151">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="2ca12-152">**Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Software, die dieser Verteilung zugeordnet sind, dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="2ca12-152">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="2ca12-153">Bei der erneuten Installation aus dem Speicher wird eine saubere Kopie der Verteilung installiert.</span><span class="sxs-lookup"><span data-stu-id="2ca12-153">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wsl --unregister <DistributionName>`  
<span data-ttu-id="2ca12-154">Hebt die Registrierung der Verteilung bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2ca12-154">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="2ca12-155">Beispiel: `wsl --unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Verteilungen entfernen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-155">For example: `wsl --unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="2ca12-156">Beim Ausführen `wsl --list` wird der Dienst nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-156">When I run `wsl --list` it will not be listed.</span></span>

<span data-ttu-id="2ca12-157">Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie "starten" aus.</span><span class="sxs-lookup"><span data-stu-id="2ca12-157">To reinstall, find the distribution in the Microsoft store and select "Launch".</span></span>

#### <a name="run-as-a-specific-user"></a><span data-ttu-id="2ca12-158">Ausführen als bestimmter Benutzer</span><span class="sxs-lookup"><span data-stu-id="2ca12-158">Run as a specific user</span></span>

<span data-ttu-id="2ca12-159">`wsl -u <Username>`, `wsl --user <Username>`</span><span class="sxs-lookup"><span data-stu-id="2ca12-159">`wsl -u <Username>`, `wsl --user <Username>`</span></span>

<span data-ttu-id="2ca12-160">Führen Sie WSL als den angegebenen Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="2ca12-160">Run WSL as the specified user.</span></span> <span data-ttu-id="2ca12-161">Beachten Sie, dass der Benutzer in der WSL-Distribution vorhanden sein muss.</span><span class="sxs-lookup"><span data-stu-id="2ca12-161">Please note that user must exist inside of the WSL distribution.</span></span>

#### <a name="run-a-specific-distribution"></a><span data-ttu-id="2ca12-162">Ausführen einer bestimmten Verteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-162">Run a specific distribution</span></span>

<span data-ttu-id="2ca12-163">`wsl --d <DistributionName>`, `wsl --distribution <DistributionName>`</span><span class="sxs-lookup"><span data-stu-id="2ca12-163">`wsl --d <DistributionName>`, `wsl --distribution <DistributionName>`</span></span>

<span data-ttu-id="2ca12-164">Führen Sie eine angegebene Distribution von WSL aus, die zum Senden von Befehlen an eine bestimmte Distribution verwendet werden kann, ohne den Standardwert ändern zu müssen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-164">Run a specified distribution of WSL, can be used to send commands to a specific distribution without having to change your default.</span></span>

### <a name="versions-earlier-than-windows-10-version-1903"></a><span data-ttu-id="2ca12-165">Frühere Versionen als Windows 10, Version 1903</span><span class="sxs-lookup"><span data-stu-id="2ca12-165">Versions Earlier than Windows 10 Version 1903</span></span>

<span data-ttu-id="2ca12-166">WSL config (`wslconfig.exe`) ist ein Befehlszeilen Tool zum Verwalten von Linux-Distributionen, die unter dem Windows-Subsystem für Linux (WSL) ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-166">WSL Config (`wslconfig.exe`) is a command-line tool for managing Linux distributions running on the Windows Subsystem for Linux (WSL).</span></span>  <span data-ttu-id="2ca12-167">Damit können Sie verfügbare Distributionen auflisten, eine Standardverteilung festlegen und Verteilungen deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="2ca12-167">It lets you list available distributions, set a default distribution, and uninstall distributions.</span></span>

<span data-ttu-id="2ca12-168">Während die WSL-Konfiguration für Einstellungen nützlich ist, die Verteilungen überspannen oder koordinieren, verwaltet jede Linux-Distribution unabhängig seine eigenen Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-168">While WSL Config is helpful for settings that span or coordinate distributions, each Linux distribution independently manages its own configurations.</span></span>  <span data-ttu-id="2ca12-169">Führen `[distro.exe] /?`Sie aus, um Verteilungs spezifische Befehle anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-169">To see distribution-specific commands, run `[distro.exe] /?`.</span></span>  <span data-ttu-id="2ca12-170">Beispiel: `ubuntu /?`.</span><span class="sxs-lookup"><span data-stu-id="2ca12-170">For example `ubuntu /?`.</span></span>

<span data-ttu-id="2ca12-171">Um alle verfügbaren Optionen für wslconfig anzuzeigen, führen Sie Folgendes aus:`wslconfig /?`</span><span class="sxs-lookup"><span data-stu-id="2ca12-171">To see all available options for wslconfig, run:  `wslconfig /?`</span></span>

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

#### <a name="list-distributions"></a><span data-ttu-id="2ca12-172">Verteilungen auflisten</span><span class="sxs-lookup"><span data-stu-id="2ca12-172">List distributions</span></span>

`wslconfig /list`  
<span data-ttu-id="2ca12-173">Listet verfügbare Linux-Distributionen für WSL auf.</span><span class="sxs-lookup"><span data-stu-id="2ca12-173">Lists available Linux distributions available to WSL.</span></span>  <span data-ttu-id="2ca12-174">Wenn eine Distribution aufgeführt ist, ist Sie installiert und einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="2ca12-174">If a distribution is listed, it's installed and ready to use.</span></span>

`wslconfig /list /all`  
<span data-ttu-id="2ca12-175">Listet alle Verteilungen auf, einschließlich derjenigen, die derzeit nicht verwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="2ca12-175">Lists all distributions, including ones that aren't currently usable.</span></span>  <span data-ttu-id="2ca12-176">Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-176">They may be in the process of installing, uninstalling, or are in a broken state.</span></span>  

#### <a name="set-a-default-distribution"></a><span data-ttu-id="2ca12-177">Festlegen einer Standardverteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-177">Set a default distribution</span></span>

<span data-ttu-id="2ca12-178">Die standardmäßige WSL-Verteilung ist die, die ausgeführt wird `wsl` , wenn Sie in einer Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-178">The default WSL distribution is the one that runs when you run `wsl` on a command line.</span></span>

`wslconfig /setdefault <DistributionName>`

<span data-ttu-id="2ca12-179">Legt die Standardverteilung auf `<DistributionName>`fest.</span><span class="sxs-lookup"><span data-stu-id="2ca12-179">Sets the default distribution to `<DistributionName>`.</span></span>

<span data-ttu-id="2ca12-180">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="2ca12-180">**Example:**</span></span>  
<span data-ttu-id="2ca12-181">`wslconfig /setdefault Ubuntu`legt die Standardverteilung auf Ubuntu fest.</span><span class="sxs-lookup"><span data-stu-id="2ca12-181">`wslconfig /setdefault Ubuntu` would set my default distribution to Ubuntu.</span></span>  <span data-ttu-id="2ca12-182">Wenn die Anwendung ausgeführt `wsl npm init` wird, wird Sie jetzt in Ubuntu ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-182">Now when I run `wsl npm init` it will run in Ubuntu.</span></span>  <span data-ttu-id="2ca12-183">Wenn ich das `wsl` ausführen, wird eine Ubuntu-Sitzung geöffnet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-183">If I run `wsl` it will open an Ubuntu session.</span></span>

#### <a name="unregister-and-reinstall-a-distribution"></a><span data-ttu-id="2ca12-184">Aufheben der Registrierung und Neuinstallation einer Verteilung</span><span class="sxs-lookup"><span data-stu-id="2ca12-184">Unregister and reinstall a distribution</span></span>

<span data-ttu-id="2ca12-185">Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-185">While Linux distributions can be installed through the Microsoft store, they can't be uninstalled through the store.</span></span>  <span data-ttu-id="2ca12-186">Die WSL-Konfiguration ermöglicht die Registrierung/Deinstallieren von Distributionen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-186">WSL Config allows distributions to be unregistered/uninstalled.</span></span>

<span data-ttu-id="2ca12-187">Durch die Aufhebung der Registrierung können auch Verteilungen erneut installiert werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-187">Unregistering also allows distributions to be reinstalled.</span></span>

> <span data-ttu-id="2ca12-188">**Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Software, die dieser Verteilung zugeordnet sind, dauerhaft verloren.</span><span class="sxs-lookup"><span data-stu-id="2ca12-188">**Caution:** Once unregistered, all data, settings, and software associated with that distribution will be permanently lost.</span></span>  <span data-ttu-id="2ca12-189">Bei der erneuten Installation aus dem Speicher wird eine saubere Kopie der Verteilung installiert.</span><span class="sxs-lookup"><span data-stu-id="2ca12-189">Reinstalling from the store will install a clean copy of the distribution.</span></span>

`wslconfig /unregister <DistributionName>`  
<span data-ttu-id="2ca12-190">Hebt die Registrierung der Verteilung bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2ca12-190">Unregisters the distribution from WSL so it can be reinstalled or cleaned up.</span></span>

<span data-ttu-id="2ca12-191">Beispiel: `wslconfig /unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Verteilungen entfernen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-191">For example: `wslconfig /unregister Ubuntu` would remove Ubuntu from the distributions available in WSL.</span></span>  <span data-ttu-id="2ca12-192">Beim Ausführen `wslconfig /list` wird der Dienst nicht aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-192">When I run `wslconfig /list` it will not be listed.</span></span>

<span data-ttu-id="2ca12-193">Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie "starten" aus.</span><span class="sxs-lookup"><span data-stu-id="2ca12-193">To reinstall, find the distribution in the Microsoft store and select "Launch".</span></span>

## <a name="set-wsl-launch-settings"></a><span data-ttu-id="2ca12-194">Festlegen der WSL-Start Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2ca12-194">Set WSL launch settings</span></span>

> <span data-ttu-id="2ca12-195">**Verfügbar in Windows Insider Build 17093 und höher**</span><span class="sxs-lookup"><span data-stu-id="2ca12-195">**Available in Windows Insider Build 17093 and later**</span></span>

<span data-ttu-id="2ca12-196">Konfigurieren Sie automatisch bestimmte Funktionen in WSL, die jedes Mal angewendet werden, wenn Sie das `wsl.conf`Subsystem mithilfe von starten.</span><span class="sxs-lookup"><span data-stu-id="2ca12-196">Automatically configure certain functionality in WSL that will be applied every time you launch the subsystem using `wsl.conf`.</span></span> 

<span data-ttu-id="2ca12-197">Zurzeit umfasst dies automatische Optionen und Netzwerkkonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ca12-197">Right now, this includes automount options and network configuration.</span></span>

<span data-ttu-id="2ca12-198">`wsl.conf`befindet sich in jeder Linux-Distribution `/etc/wsl.conf`in.</span><span class="sxs-lookup"><span data-stu-id="2ca12-198">`wsl.conf` is located in each Linux distribution in `/etc/wsl.conf`.</span></span> <span data-ttu-id="2ca12-199">Wenn die Datei nicht vorhanden ist, können Sie Sie selbst erstellen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-199">If the file is not there, you can create it yourself.</span></span> <span data-ttu-id="2ca12-200">WSL erkennt das vorhanden sein der Datei und liest ihren Inhalt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-200">WSL will detect the existence of the file and will read its contents.</span></span> <span data-ttu-id="2ca12-201">Wenn die Datei fehlt oder falsch formatiert ist (d. h. eine falsche Markup Formatierung), wird WSL weiterhin normal gestartet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-201">If the file is missing or malformed (that is, improper markup formatting), WSL will continue to launch as normal.</span></span>

<span data-ttu-id="2ca12-202">Im folgenden finden Sie `wsl.conf` eine Beispieldatei, die Sie ihren Distributionen hinzufügen können:</span><span class="sxs-lookup"><span data-stu-id="2ca12-202">Here is a sample `wsl.conf` file you could add into your distros:</span></span>

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

### <a name="configuration-options"></a><span data-ttu-id="2ca12-203">Konfigurationsoptionen</span><span class="sxs-lookup"><span data-stu-id="2ca12-203">Configuration Options</span></span>

<span data-ttu-id="2ca12-204">In Übereinstimmung mit ini-Konventionen werden Schlüssel in einem Abschnitt deklariert.</span><span class="sxs-lookup"><span data-stu-id="2ca12-204">In keeping with .ini conventions, keys are declared under a section.</span></span> 

<span data-ttu-id="2ca12-205">WSL unterstützt zwei Abschnitte `automount` : `network`und.</span><span class="sxs-lookup"><span data-stu-id="2ca12-205">WSL supports two sections: `automount` and `network`.</span></span>

#### <a name="automount"></a><span data-ttu-id="2ca12-206">automatischen Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="2ca12-206">automount</span></span>

<span data-ttu-id="2ca12-207">Sektions`[automount]`</span><span class="sxs-lookup"><span data-stu-id="2ca12-207">Section: `[automount]`</span></span>


| <span data-ttu-id="2ca12-208">Key</span><span class="sxs-lookup"><span data-stu-id="2ca12-208">key</span></span>        | <span data-ttu-id="2ca12-209">Wert</span><span class="sxs-lookup"><span data-stu-id="2ca12-209">value</span></span>                          | <span data-ttu-id="2ca12-210">default</span><span class="sxs-lookup"><span data-stu-id="2ca12-210">default</span></span>      | <span data-ttu-id="2ca12-211">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="2ca12-211">notes</span></span>                                                                                                                                                                                                                                                                                                                          |
|:-----------|:-------------------------------|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2ca12-212">aktiviert</span><span class="sxs-lookup"><span data-stu-id="2ca12-212">enabled</span></span>    | <span data-ttu-id="2ca12-213">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-213">boolean</span></span>                        | <span data-ttu-id="2ca12-214">true</span><span class="sxs-lookup"><span data-stu-id="2ca12-214">true</span></span>         | <span data-ttu-id="2ca12-215">`true`verursacht Festplattenlaufwerke (d. h.</span><span class="sxs-lookup"><span data-stu-id="2ca12-215">`true` causes fixed drives (i.e</span></span> <span data-ttu-id="2ca12-216">`C:/`oder `D:/`) für die automatische Bereitstellung mit drvfs `/mnt`unter.</span><span class="sxs-lookup"><span data-stu-id="2ca12-216">`C:/` or `D:/`) to be automatically mounted with DrvFs under `/mnt`.</span></span>  <span data-ttu-id="2ca12-217">`false`bedeutet, dass Laufwerke nicht automatisch bereitgestellt werden, aber Sie können Sie trotzdem manuell `fstab`oder über bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-217">`false` means drives won’t be mounted automatically, but you could still mount them manually or via `fstab`.</span></span>                                                                                                             |
| <span data-ttu-id="2ca12-218">mountfstab</span><span class="sxs-lookup"><span data-stu-id="2ca12-218">mountFsTab</span></span> | <span data-ttu-id="2ca12-219">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-219">boolean</span></span>                        | <span data-ttu-id="2ca12-220">true</span><span class="sxs-lookup"><span data-stu-id="2ca12-220">true</span></span>         | <span data-ttu-id="2ca12-221">`true`auf `/etc/fstab` dem WSL-Start zu verarbeitende Sätze.</span><span class="sxs-lookup"><span data-stu-id="2ca12-221">`true` sets `/etc/fstab` to be processed on WSL start.</span></span> <span data-ttu-id="2ca12-222">bei "/etc/fstab" handelt es sich um eine Datei, in der Sie andere Dateisysteme wie eine SMB-Freigabe deklarieren können.</span><span class="sxs-lookup"><span data-stu-id="2ca12-222">/etc/fstab is a file where you can declare other filesystems, like an SMB share.</span></span> <span data-ttu-id="2ca12-223">Daher können Sie diese Dateisysteme beim Start automatisch in WSL einbinden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-223">Thus, you can mount these filesystems automatically in WSL on start up.</span></span>                                                                                                                |
| <span data-ttu-id="2ca12-224">fasst</span><span class="sxs-lookup"><span data-stu-id="2ca12-224">root</span></span>       | <span data-ttu-id="2ca12-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ca12-225">String</span></span>                         | `/mnt/`      | <span data-ttu-id="2ca12-226">Legt das Verzeichnis fest, in dem Festplattenlaufwerke automatisch bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="2ca12-226">Sets the directory where fixed drives will be automatically mounted.</span></span> <span data-ttu-id="2ca12-227">Wenn Sie z. b. ein Verzeichnis in WSL bei `/windir/` haben und Sie als Stammverzeichnis angeben, erwarten Sie, dass die Festplattenlaufwerke unter`/windir/c`</span><span class="sxs-lookup"><span data-stu-id="2ca12-227">For example, if you have a directory in WSL at `/windir/` and you specify that as the root, you would expect to see your fixed drives mounted at `/windir/c`</span></span>                                                                                              |
| <span data-ttu-id="2ca12-228">options</span><span class="sxs-lookup"><span data-stu-id="2ca12-228">options</span></span>    | <span data-ttu-id="2ca12-229">durch Trennzeichen getrennte Liste von Werten</span><span class="sxs-lookup"><span data-stu-id="2ca12-229">comma-separated list of values</span></span> | <span data-ttu-id="2ca12-230">leere Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ca12-230">empty string</span></span> | <span data-ttu-id="2ca12-231">Dieser Wert wird an die Standard Zeichenfolge der drvfs-Einfügeoptionen angehängt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-231">This value is appended to the default DrvFs mount options string.</span></span> <span data-ttu-id="2ca12-232">**Es können nur drvfs-spezifische Optionen angegeben werden.**</span><span class="sxs-lookup"><span data-stu-id="2ca12-232">**Only DrvFs-specific options can be specified.**</span></span> <span data-ttu-id="2ca12-233">Optionen, die die Einbindungs Binärdatei normalerweise in ein Flag analysieren würde, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-233">Options that the mount binary would normally parse into a flag are not supported.</span></span> <span data-ttu-id="2ca12-234">Wenn Sie diese Optionen explizit angeben möchten, müssen Sie jedes Laufwerk, für das Sie dies tun möchten, in "/etc/fstab" einschließen.</span><span class="sxs-lookup"><span data-stu-id="2ca12-234">If you want to explicitly specify those options, you must include every drive for which you want to do so in /etc/fstab.</span></span> |

<span data-ttu-id="2ca12-235">Standardmäßig legt WSL die UID und die gid auf den Wert des Standard Benutzers fest (in Ubuntu-Distribution wird der Standardbenutzer mit UID = 1000, gid = 1000 erstellt).</span><span class="sxs-lookup"><span data-stu-id="2ca12-235">By default, WSL sets the uid and gid to the value of the default user (in Ubuntu distro, the default user is created with uid=1000,gid=1000).</span></span> <span data-ttu-id="2ca12-236">Wenn der Benutzer eine GID-oder UID-Option explizit über diesen Schlüssel angibt, wird der zugehörige Wert überschrieben.</span><span class="sxs-lookup"><span data-stu-id="2ca12-236">If the user specifies a gid or uid option explicitly via this key, the associated value will be overwritten.</span></span> <span data-ttu-id="2ca12-237">Andernfalls wird der Standardwert immer angefügt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-237">Otherwise, the default value will always be appended.</span></span>

<span data-ttu-id="2ca12-238">**Hinweis**: Diese Optionen werden als Einstellungsoptionen für alle automatisch bereitgestellten Laufwerke angewendet.</span><span class="sxs-lookup"><span data-stu-id="2ca12-238">**Note:** These options are applied as the mount options for all automatically mounted drives.</span></span> <span data-ttu-id="2ca12-239">Verwenden Sie stattdessen "/etc/fstab", um die Optionen für ein bestimmtes Laufwerk zu ändern.</span><span class="sxs-lookup"><span data-stu-id="2ca12-239">To change the options for a specific drive only, use /etc/fstab instead.</span></span>

#### <a name="network"></a><span data-ttu-id="2ca12-240">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="2ca12-240">network</span></span>

<span data-ttu-id="2ca12-241">Abschnitts Bezeichnung:`[network]`</span><span class="sxs-lookup"><span data-stu-id="2ca12-241">Section label: `[network]`</span></span>

| <span data-ttu-id="2ca12-242">Key</span><span class="sxs-lookup"><span data-stu-id="2ca12-242">key</span></span> | <span data-ttu-id="2ca12-243">Wert</span><span class="sxs-lookup"><span data-stu-id="2ca12-243">value</span></span> | <span data-ttu-id="2ca12-244">default</span><span class="sxs-lookup"><span data-stu-id="2ca12-244">default</span></span> | <span data-ttu-id="2ca12-245">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="2ca12-245">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="2ca12-246">generatehosts</span><span class="sxs-lookup"><span data-stu-id="2ca12-246">generateHosts</span></span> | <span data-ttu-id="2ca12-247">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-247">boolean</span></span> | `true` | <span data-ttu-id="2ca12-248">`true`legt fest, dass WSL generiert `/etc/hosts`wird.</span><span class="sxs-lookup"><span data-stu-id="2ca12-248">`true` sets WSL to generate `/etc/hosts`.</span></span> <span data-ttu-id="2ca12-249">Die `hosts` Datei enthält eine statische Zuordnung der Hostnamen der entsprechenden IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="2ca12-249">The `hosts` file contains a static map of hostnames corresponding IP address.</span></span> |
| <span data-ttu-id="2ca12-250">generateresolvconf</span><span class="sxs-lookup"><span data-stu-id="2ca12-250">generateResolvConf</span></span> | <span data-ttu-id="2ca12-251">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-251">boolean</span></span> | `true` | <span data-ttu-id="2ca12-252">`true`Legen Sie WSL auf `/etc/resolv.conf`Generate fest.</span><span class="sxs-lookup"><span data-stu-id="2ca12-252">`true` set WSL to generate `/etc/resolv.conf`.</span></span> <span data-ttu-id="2ca12-253">Die `resolv.conf` enthält eine DNS-Liste, die einen angegebenen Hostnamen in seine IP-Adresse auflösen können.</span><span class="sxs-lookup"><span data-stu-id="2ca12-253">The `resolv.conf` contains a DNS list that are capable of resolving a given hostname to its IP address.</span></span> | 

#### <a name="interop"></a><span data-ttu-id="2ca12-254">Interop</span><span class="sxs-lookup"><span data-stu-id="2ca12-254">interop</span></span>

<span data-ttu-id="2ca12-255">Abschnitts Bezeichnung:`[interop]`</span><span class="sxs-lookup"><span data-stu-id="2ca12-255">Section label: `[interop]`</span></span>

<span data-ttu-id="2ca12-256">Diese Optionen sind in Insider Build 17713 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2ca12-256">These options are available in Insider Build 17713 and later.</span></span>

| <span data-ttu-id="2ca12-257">Key</span><span class="sxs-lookup"><span data-stu-id="2ca12-257">key</span></span> | <span data-ttu-id="2ca12-258">Wert</span><span class="sxs-lookup"><span data-stu-id="2ca12-258">value</span></span> | <span data-ttu-id="2ca12-259">default</span><span class="sxs-lookup"><span data-stu-id="2ca12-259">default</span></span> | <span data-ttu-id="2ca12-260">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="2ca12-260">notes</span></span>|
|:----|:----|:----|:----|
| <span data-ttu-id="2ca12-261">aktiviert</span><span class="sxs-lookup"><span data-stu-id="2ca12-261">enabled</span></span> | <span data-ttu-id="2ca12-262">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-262">boolean</span></span> | `true` | <span data-ttu-id="2ca12-263">Durch Festlegen dieses Schlüssels wird festgelegt, ob WSL das Starten von Windows-Prozessen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-263">Setting this key will determine whether WSL will support launching Windows processes.</span></span> |
| <span data-ttu-id="2ca12-264">appendwindowspath</span><span class="sxs-lookup"><span data-stu-id="2ca12-264">appendWindowsPath</span></span> | <span data-ttu-id="2ca12-265">boolean</span><span class="sxs-lookup"><span data-stu-id="2ca12-265">boolean</span></span> | `true` | <span data-ttu-id="2ca12-266">Wenn dieser Schlüssel festgelegt wird, wird festgelegt, ob WSL der $PATH-Umgebungsvariablen Windows-Pfad Elemente hinzufügt.</span><span class="sxs-lookup"><span data-stu-id="2ca12-266">Setting this key will determine whether WSL will add Windows path elements to the $PATH environment variable.</span></span> | 
