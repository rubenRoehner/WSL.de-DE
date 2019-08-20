---
title: Windows-Subsystem für Linux (Befehlsreferenz)
description: Liste der Befehle, mit denen das Windows-Subsystem für Linux verwaltet wird
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu
author: scooley
ms.author: scooley
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.openlocfilehash: 018b02b43e859476f7ee38f54df8efa0ca0e652b
ms.sourcegitcommit: 62c49d435a91f2e390c3c495f3e09e62b5ada13c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/19/2019
ms.locfileid: "69578836"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a><span data-ttu-id="527d2-104">Befehlsreferenz für Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="527d2-104">Command Reference for Windows Subsystem for Linux</span></span>

<span data-ttu-id="527d2-105">Die beste Möglichkeit, mit dem Windows-Subsystem für Linux zu interagieren, ist `wsl.exe` die Verwendung des-Befehls.</span><span class="sxs-lookup"><span data-stu-id="527d2-105">The best way to interact with the Windows Subsystem for Linux is to use the `wsl.exe` command.</span></span> 


## `wsl.exe`

<span data-ttu-id="527d2-106">Im folgenden finden Sie eine Liste mit allen Optionen `wsl.exe` , wenn Sie ab Windows Version 1903 verwenden.</span><span class="sxs-lookup"><span data-stu-id="527d2-106">Below is a list containing all options when using `wsl.exe` as of Windows Version 1903.</span></span>

<span data-ttu-id="527d2-107">Genutzt`wsl [Argument] [Options...] [CommandLine]`</span><span class="sxs-lookup"><span data-stu-id="527d2-107">Using: `wsl [Argument] [Options...] [CommandLine]`</span></span>

### <a name="arguments-for-running-linux-binaries"></a><span data-ttu-id="527d2-108">Argumente für das Ausführen von Linux-Binärdateien</span><span class="sxs-lookup"><span data-stu-id="527d2-108">Arguments for running Linux binaries</span></span>

* <span data-ttu-id="527d2-109">**Ohne Argumente**</span><span class="sxs-lookup"><span data-stu-id="527d2-109">**Without arguments**</span></span>

  <span data-ttu-id="527d2-110">Wenn keine Befehlszeile angegeben wird, wird die Standardshell von WSL. exe gestartet.</span><span class="sxs-lookup"><span data-stu-id="527d2-110">If no command line is provided, wsl.exe launches the default shell.</span></span>

* <span data-ttu-id="527d2-111">**--Exec,-e \<commandline >**</span><span class="sxs-lookup"><span data-stu-id="527d2-111">**--exec, -e \<CommandLine>**</span></span>
  
  <span data-ttu-id="527d2-112">Führen Sie den angegebenen Befehl ohne die Linux-Standard Shell aus.</span><span class="sxs-lookup"><span data-stu-id="527d2-112">Execute the specified command without using the default Linux shell.</span></span>

* **--**
  
  <span data-ttu-id="527d2-113">Übergeben Sie die verbleibende Befehlszeile unverändert.</span><span class="sxs-lookup"><span data-stu-id="527d2-113">Pass the remaining command line as is.</span></span>

<span data-ttu-id="527d2-114">Die obigen Befehle akzeptieren außerdem die folgenden Optionen:</span><span class="sxs-lookup"><span data-stu-id="527d2-114">The above commands also accept the following options:</span></span>

* <span data-ttu-id="527d2-115">**--Distribution,-d \<Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-115">**--distribution, -d \<Distro>**</span></span>

  <span data-ttu-id="527d2-116">Führt die angegebene Verteilung aus.</span><span class="sxs-lookup"><span data-stu-id="527d2-116">Run the specified distribution.</span></span>

* <span data-ttu-id="527d2-117">**--Benutzer,-u \<Benutzername >**</span><span class="sxs-lookup"><span data-stu-id="527d2-117">**--user, -u \<UserName>**</span></span>

  <span data-ttu-id="527d2-118">Ausführen als angegebener Benutzer.</span><span class="sxs-lookup"><span data-stu-id="527d2-118">Run as the specified user.</span></span>

### <a name="arguments-for-managing-windows-subsystem-for-linux"></a><span data-ttu-id="527d2-119">Argumente für die Verwaltung des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="527d2-119">Arguments for managing Windows Subsystem for Linux</span></span>

* <span data-ttu-id="527d2-120">**--> \< \<Dateiname "Distribution" Exportieren >**</span><span class="sxs-lookup"><span data-stu-id="527d2-120">**--export \<Distro> \<FileName>**</span></span>
  
  <span data-ttu-id="527d2-121">Exportiert die Verteilung in eine tar-Datei.</span><span class="sxs-lookup"><span data-stu-id="527d2-121">Exports the distribution to a tar file.</span></span> <span data-ttu-id="527d2-122">Der Dateiname kann für die Standardausgabe sein.</span><span class="sxs-lookup"><span data-stu-id="527d2-122">The filename can be - for standard output.</span></span>

* <span data-ttu-id="527d2-123">**--> \< \<INSTALLLOCATION > \<Dateinamen importieren >**</span><span class="sxs-lookup"><span data-stu-id="527d2-123">**--import \<Distro> \<InstallLocation> \<FileName>**</span></span>
  
  <span data-ttu-id="527d2-124">Importiert die angegebene tar-Datei als neue Verteilung.</span><span class="sxs-lookup"><span data-stu-id="527d2-124">Imports the specified tar file as a new distribution.</span></span> <span data-ttu-id="527d2-125">Der Dateiname kann für die Standardeingabe sein.</span><span class="sxs-lookup"><span data-stu-id="527d2-125">The filename can be - for standard input.</span></span>

* <span data-ttu-id="527d2-126">**--List,-l [Optionen]**</span><span class="sxs-lookup"><span data-stu-id="527d2-126">**--list, -l [Options]**</span></span>
  
  <span data-ttu-id="527d2-127">Listet Verteilungen auf.</span><span class="sxs-lookup"><span data-stu-id="527d2-127">Lists distributions.</span></span>

  <span data-ttu-id="527d2-128">Optionen:</span><span class="sxs-lookup"><span data-stu-id="527d2-128">Options:</span></span>
  * <span data-ttu-id="527d2-129">**--Alle**</span><span class="sxs-lookup"><span data-stu-id="527d2-129">**--all**</span></span>
      
    <span data-ttu-id="527d2-130">Auflisten aller Verteilungen, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="527d2-130">List all distributions, including distributions that are currently being installed or uninstalled.</span></span>

  * <span data-ttu-id="527d2-131">**--wird ausgeführt**</span><span class="sxs-lookup"><span data-stu-id="527d2-131">**--running**</span></span>
      
    <span data-ttu-id="527d2-132">Listet nur Verteilungen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="527d2-132">List only distributions that are currently running.</span></span>

* <span data-ttu-id="527d2-133">**--Set-Default,-s \<-Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-133">**--set-default, -s \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-134">Legt die Verteilung als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="527d2-134">Sets the distribution as the default.</span></span>

* <span data-ttu-id="527d2-135">**--beenden,-t \<Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-135">**--terminate, -t \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-136">Beendet die angegebene Verteilung.</span><span class="sxs-lookup"><span data-stu-id="527d2-136">Terminates the specified distribution.</span></span>

* <span data-ttu-id="527d2-137">**--Aufheben der \<Registrierung von Distribution->**</span><span class="sxs-lookup"><span data-stu-id="527d2-137">**--unregister \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-138">Hebt die Registrierung der Verteilung auf.</span><span class="sxs-lookup"><span data-stu-id="527d2-138">Unregisters the distribution.</span></span>
   
* <span data-ttu-id="527d2-139">**--Hilfe** Anzeigen von Nutzungsinformationen.</span><span class="sxs-lookup"><span data-stu-id="527d2-139">**--help** Display usage information.</span></span>

## <a name="additional-commands"></a><span data-ttu-id="527d2-140">Weitere Befehle</span><span class="sxs-lookup"><span data-stu-id="527d2-140">Additional Commands</span></span>

<span data-ttu-id="527d2-141">Es gibt auch historische Befehle für die Interaktion mit dem Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="527d2-141">There are also historic commands to interact with the Windows Subsystem for Linux.</span></span> <span data-ttu-id="527d2-142">Ihre Funktionalität ist in `wsl.exe`enthalten, Sie sind jedoch weiterhin zur Verwendung verfügbar.</span><span class="sxs-lookup"><span data-stu-id="527d2-142">Their functionality is encompassed within `wsl.exe`, but they are still available for use.</span></span> 

### `wslconfig.exe`

<span data-ttu-id="527d2-143">Mit diesem Befehl können Sie Ihre WSL-Verteilung konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="527d2-143">This command lets you configure your WSL distribution.</span></span> <span data-ttu-id="527d2-144">Im folgenden finden Sie eine Liste der zugehörigen Optionen.</span><span class="sxs-lookup"><span data-stu-id="527d2-144">Below is a list of its options.</span></span>

<span data-ttu-id="527d2-145">Genutzt`wslconfig [Argument] [Options...]`</span><span class="sxs-lookup"><span data-stu-id="527d2-145">Using: `wslconfig [Argument] [Options...]`</span></span>

#### <a name="arguments"></a><span data-ttu-id="527d2-146">Argumente</span><span class="sxs-lookup"><span data-stu-id="527d2-146">Arguments</span></span>
* <span data-ttu-id="527d2-147">**/l,/List [Optionen]**</span><span class="sxs-lookup"><span data-stu-id="527d2-147">**/l, /list [Options]**</span></span>
  
  <span data-ttu-id="527d2-148">Listet registrierte Verteilungen auf.</span><span class="sxs-lookup"><span data-stu-id="527d2-148">Lists registered distributions.</span></span>
  
  <span data-ttu-id="527d2-149">Optionen:</span><span class="sxs-lookup"><span data-stu-id="527d2-149">Options:</span></span>
    * <span data-ttu-id="527d2-150">**/All**</span><span class="sxs-lookup"><span data-stu-id="527d2-150">**/all**</span></span>
    
      <span data-ttu-id="527d2-151">Optional können Sie alle Distributionen auflisten, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="527d2-151">Optionally list all distributions, including distributions that are currently being installed or uninstalled.</span></span>

    * <span data-ttu-id="527d2-152">**/running**</span><span class="sxs-lookup"><span data-stu-id="527d2-152">**/running**</span></span>
      
      <span data-ttu-id="527d2-153">Listet nur Verteilungen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="527d2-153">List only distributions that are currently running.</span></span>

* <span data-ttu-id="527d2-154">**/s,/SetDefault \<Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-154">**/s, /setdefault \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-155">Legt die Verteilung als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="527d2-155">Sets the distribution as the default.</span></span>

* <span data-ttu-id="527d2-156">**/t,/Terminate \<Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-156">**/t, /terminate \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-157">Beendet die Verteilung.</span><span class="sxs-lookup"><span data-stu-id="527d2-157">Terminates the distribution.</span></span>

* <span data-ttu-id="527d2-158">**/u,/Unregister \<Distribution >**</span><span class="sxs-lookup"><span data-stu-id="527d2-158">**/u, /unregister \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-159">Hebt die Registrierung der Verteilung auf.</span><span class="sxs-lookup"><span data-stu-id="527d2-159">Unregisters the distribution.</span></span>
   
* <span data-ttu-id="527d2-160">**/Upgrade \<Distribution->**</span><span class="sxs-lookup"><span data-stu-id="527d2-160">**/upgrade \<Distro>**</span></span>
  
  <span data-ttu-id="527d2-161">Führt ein Upgrade der Verteilung auf das wslfs-Dateisystem Format durch.</span><span class="sxs-lookup"><span data-stu-id="527d2-161">Upgrades the distribution to the WslFs file system format.</span></span>

### `bash.exe`

<span data-ttu-id="527d2-162">Dieser Befehl wird verwendet, um eine bash-Shell zu starten.</span><span class="sxs-lookup"><span data-stu-id="527d2-162">This command is used to start a bash shell.</span></span> <span data-ttu-id="527d2-163">Im folgenden finden Sie die Optionen, die Sie mit diesem Befehl verwenden können.</span><span class="sxs-lookup"><span data-stu-id="527d2-163">Below are the options you can use with this command.</span></span>

<span data-ttu-id="527d2-164">Genutzt`bash [Options...]`</span><span class="sxs-lookup"><span data-stu-id="527d2-164">Using: `bash [Options...]`</span></span>

* <span data-ttu-id="527d2-165">**Keine Option angegeben.**</span><span class="sxs-lookup"><span data-stu-id="527d2-165">**No Option given**</span></span>
  
  <span data-ttu-id="527d2-166">Starten der bash-Shell im aktuellen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="527d2-166">Launches the Bash shell in the current directory.</span></span> <span data-ttu-id="527d2-167">Wenn die bash-Shell nicht installiert ist, wird automatisch ausgeführt.`lxrun /install`</span><span class="sxs-lookup"><span data-stu-id="527d2-167">If the Bash shell is not installed automatically runs `lxrun /install`</span></span>

* **~**
  
  <span data-ttu-id="527d2-168">`bash ~`Hiermit wird die bash-Shell in das Basisverzeichnis des Benutzers gestartet.</span><span class="sxs-lookup"><span data-stu-id="527d2-168">`bash ~` launches the bash shell into the user's home directory.</span></span>  <span data-ttu-id="527d2-169">Vergleichbar mit dem `cd ~`Ausführen von.</span><span class="sxs-lookup"><span data-stu-id="527d2-169">Similar to running `cd ~`.</span></span>

* <span data-ttu-id="527d2-170">**-c "\<Command >"**</span><span class="sxs-lookup"><span data-stu-id="527d2-170">**-c "\<command>"**</span></span>
  
  <span data-ttu-id="527d2-171">Führt den Befehl aus, druckt die Ausgabe und wird zurück zur Windows-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="527d2-171">Runs the command, prints the output and exits back to the Windows command prompt.</span></span>
    
  <span data-ttu-id="527d2-172">Beispiel: `bash -c "ls"`.</span><span class="sxs-lookup"><span data-stu-id="527d2-172">Example:  `bash -c "ls"`.</span></span>

## <a name="deprecated-commands"></a><span data-ttu-id="527d2-173">Als veraltet markierte Befehle</span><span class="sxs-lookup"><span data-stu-id="527d2-173">Deprecated Commands</span></span>

<span data-ttu-id="527d2-174">`lxrun.exe` War der erste Befehl, der zum Installieren und Verwalten des Windows-Subsystems für Linux verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="527d2-174">The `lxrun.exe` was the first command used to install and manage the Windows Subsystem for Linux.</span></span> <span data-ttu-id="527d2-175">Sie ist ab Windows 10 1803 und höher veraltet.</span><span class="sxs-lookup"><span data-stu-id="527d2-175">It is deprecated as of Windows 10 1803 and later.</span></span>

<span data-ttu-id="527d2-176">Der Befehl `lxrun.exe` kann verwendet werden, um direkt mit dem [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) zu interagieren.</span><span class="sxs-lookup"><span data-stu-id="527d2-176">The command `lxrun.exe` can be used to interact with the [Windows Subsystem for Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) directly.</span></span>  <span data-ttu-id="527d2-177">Diese Befehle werden im `\Windows\System32` Verzeichnis installiert und können in einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="527d2-177">These commands are installed into the `\Windows\System32` directory and may be run within a Windows command prompt or in PowerShell.</span></span>

| <span data-ttu-id="527d2-178">Befehl</span><span class="sxs-lookup"><span data-stu-id="527d2-178">Command</span></span>                     | <span data-ttu-id="527d2-179">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="527d2-179">Description</span></span>                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | <span data-ttu-id="527d2-180">Der lxrun-Befehl wird verwendet, um die WSL-Instanz zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="527d2-180">The lxrun command is used to manage the WSL instance.</span></span> |
| `lxrun /install`            | <span data-ttu-id="527d2-181">Startet den Download-und Installationsvorgang.</span><span class="sxs-lookup"><span data-stu-id="527d2-181">Starts the download and install process.</span></span> <br/> <span data-ttu-id="527d2-182">**/y** kann hinzugefügt werden, um alle Eingabe Aufforderungen zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="527d2-182">**/y** may be added to bypass all prompts.</span></span>  <span data-ttu-id="527d2-183">Die Bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer ist auf root festgelegt.</span><span class="sxs-lookup"><span data-stu-id="527d2-183">The confirmation prompt is automatically accepted and the default user is set to root.</span></span>          |
| `lxrun /uninstall`          | <span data-ttu-id="527d2-184">Deinstalliert und löscht das Ubuntu-Image.</span><span class="sxs-lookup"><span data-stu-id="527d2-184">Uninstalls and deletes the Ubuntu image.</span></span>  <span data-ttu-id="527d2-185">Standardmäßig wird hierdurch nicht das Ubuntu-Basisverzeichnis des Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="527d2-185">By default this does not remove the user's Ubuntu home directory.</span></span> <br/> <span data-ttu-id="527d2-186">**/y** kann hinzugefügt werden, um die Bestätigungsaufforderung automatisch zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="527d2-186">**/y** may be added to automatically accept the confirmation prompt</span></span> <br/><span data-ttu-id="527d2-187">**/Full** deinstalliert und löscht das Ubuntu-Basisverzeichnis des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="527d2-187">**/full** uninstalls and deletes the user's Ubuntu home directory</span></span>         |
| `lxrun /setdefaultuser <userName>`     | <span data-ttu-id="527d2-188">Legt den Standard-bash on Ubuntu-Benutzer fest.</span><span class="sxs-lookup"><span data-stu-id="527d2-188">Sets the default Bash on Ubuntu user.</span></span> <span data-ttu-id="527d2-189">Fordert zur Eingabe eines Kennworts auf, wenn der angegebene Benutzer nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="527d2-189">Will prompt for a password if the specified user does not exist.</span></span>  <span data-ttu-id="527d2-190">Weitere Informationen finden Sie unter https://aka.ms/wslusers:.</span><span class="sxs-lookup"><span data-stu-id="527d2-190">For more information visit: https://aka.ms/wslusers.</span></span> <br/> <span data-ttu-id="527d2-191">**/y** Umgeht das Kennwort.</span><span class="sxs-lookup"><span data-stu-id="527d2-191">**/y** Bypasses promping for the password.</span></span>  <span data-ttu-id="527d2-192">Der Benutzer wird ohne Kennwort erstellt.</span><span class="sxs-lookup"><span data-stu-id="527d2-192">The user will be created without a password.</span></span>|
| `lxrun /update`            | <span data-ttu-id="527d2-193">Aktualisiert den Paket Index des Subsystems.</span><span class="sxs-lookup"><span data-stu-id="527d2-193">Updates the subsystem's package index</span></span>          |
