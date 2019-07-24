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
ms.openlocfilehash: 465f55f8ba210cd366adc66d433f1873e295136f
ms.sourcegitcommit: ead64b13501d6cb7170adafbb5624f4984a0af16
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/21/2019
ms.locfileid: "67307654"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a><span data-ttu-id="9751a-104">Befehlsreferenz für Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="9751a-104">Command Reference for Windows Subsystem for Linux</span></span>

<span data-ttu-id="9751a-105">Die beste Möglichkeit, mit dem Windows-Subsystem für Linux zu interagieren, ist `wsl.exe` die Verwendung des-Befehls.</span><span class="sxs-lookup"><span data-stu-id="9751a-105">The best way to interact with the Windows Subsystem for Linux is to use the `wsl.exe` command.</span></span> 

## `wsl.exe` 

<span data-ttu-id="9751a-106">Im folgenden finden Sie eine Liste mit allen Optionen `wsl.exe` , wenn Sie ab Windows Version 1903 verwenden.</span><span class="sxs-lookup"><span data-stu-id="9751a-106">Below is a list containing all options when using `wsl.exe` as of Windows Version 1903.</span></span>

* <span data-ttu-id="9751a-107">Argumente für das Ausführen von Linux-Binärdateien:</span><span class="sxs-lookup"><span data-stu-id="9751a-107">Arguments for running Linux binaries:</span></span>

    * <span data-ttu-id="9751a-108">Wenn keine Befehlszeile angegeben wird, wird die Standardshell von WSL. exe gestartet.</span><span class="sxs-lookup"><span data-stu-id="9751a-108">If no command line is provided, wsl.exe launches the default shell.</span></span>

    * <span data-ttu-id="9751a-109">--Exec,-e<CommandLine></span><span class="sxs-lookup"><span data-stu-id="9751a-109">--exec, -e <CommandLine></span></span>
        * <span data-ttu-id="9751a-110">Führen Sie den angegebenen Befehl ohne die Linux-Standard Shell aus.</span><span class="sxs-lookup"><span data-stu-id="9751a-110">Execute the specified command without using the default Linux shell.</span></span>

    * --
        * <span data-ttu-id="9751a-111">Übergeben Sie die verbleibende Befehlszeile unverändert.</span><span class="sxs-lookup"><span data-stu-id="9751a-111">Pass the remaining command line as is.</span></span>

* <span data-ttu-id="9751a-112">Optionen:</span><span class="sxs-lookup"><span data-stu-id="9751a-112">Options:</span></span>
    * <span data-ttu-id="9751a-113">--Distribution,-d<Distro></span><span class="sxs-lookup"><span data-stu-id="9751a-113">--distribution, -d <Distro></span></span>
        * <span data-ttu-id="9751a-114">Führt die angegebene Verteilung aus.</span><span class="sxs-lookup"><span data-stu-id="9751a-114">Run the specified distribution.</span></span>

    * <span data-ttu-id="9751a-115">--Benutzer,-u<UserName></span><span class="sxs-lookup"><span data-stu-id="9751a-115">--user, -u <UserName></span></span>
        * <span data-ttu-id="9751a-116">Ausführen als angegebener Benutzer.</span><span class="sxs-lookup"><span data-stu-id="9751a-116">Run as the specified user.</span></span>

* <span data-ttu-id="9751a-117">Argumente für die Verwaltung des Windows-Subsystems für Linux:</span><span class="sxs-lookup"><span data-stu-id="9751a-117">Arguments for managing Windows Subsystem for Linux:</span></span>

    * <span data-ttu-id="9751a-118">--Export <Distro><FileName></span><span class="sxs-lookup"><span data-stu-id="9751a-118">--export <Distro> <FileName></span></span>
        * <span data-ttu-id="9751a-119">Exportiert die Verteilung in eine tar-Datei.</span><span class="sxs-lookup"><span data-stu-id="9751a-119">Exports the distribution to a tar file.</span></span>
        <span data-ttu-id="9751a-120">Der Dateiname kann für die Standardausgabe sein.</span><span class="sxs-lookup"><span data-stu-id="9751a-120">The filename can be - for standard output.</span></span>

    * <span data-ttu-id="9751a-121">--Import <Distro> <InstallLocation>[Optionen <FileName> ]</span><span class="sxs-lookup"><span data-stu-id="9751a-121">--import <Distro> <InstallLocation> <FileName> [Options]</span></span>
        * <span data-ttu-id="9751a-122">Importiert die angegebene tar-Datei als neue Verteilung.</span><span class="sxs-lookup"><span data-stu-id="9751a-122">Imports the specified tar file as a new distribution.</span></span>
        <span data-ttu-id="9751a-123">Der Dateiname kann für die Standardeingabe sein.</span><span class="sxs-lookup"><span data-stu-id="9751a-123">The filename can be - for standard input.</span></span>

        * <span data-ttu-id="9751a-124">Optionen:</span><span class="sxs-lookup"><span data-stu-id="9751a-124">Options:</span></span>
            * <span data-ttu-id="9751a-125">--Version <Version> gibt die Version an, die für die neue Verteilung verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9751a-125">--version <Version> Specifies the version to use for the new distribution.</span></span>

    * <span data-ttu-id="9751a-126">--List,-l [Optionen]</span><span class="sxs-lookup"><span data-stu-id="9751a-126">--list, -l [Options]</span></span>
        * <span data-ttu-id="9751a-127">Listet Verteilungen auf.</span><span class="sxs-lookup"><span data-stu-id="9751a-127">Lists distributions.</span></span>

        * <span data-ttu-id="9751a-128">Optionen:</span><span class="sxs-lookup"><span data-stu-id="9751a-128">Options:</span></span>
            * <span data-ttu-id="9751a-129">--Alle</span><span class="sxs-lookup"><span data-stu-id="9751a-129">--all</span></span>
                * <span data-ttu-id="9751a-130">Auflisten aller Verteilungen, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="9751a-130">List all distributions, including distributions that are currently being installed or uninstalled.</span></span>

            * <span data-ttu-id="9751a-131">--wird ausgeführt</span><span class="sxs-lookup"><span data-stu-id="9751a-131">--running</span></span>
                * <span data-ttu-id="9751a-132">Listet nur Verteilungen auf, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="9751a-132">List only distributions that are currently running.</span></span>

    * <span data-ttu-id="9751a-133">--Set-Default,-s<Distro></span><span class="sxs-lookup"><span data-stu-id="9751a-133">--set-default, -s <Distro></span></span>
        * <span data-ttu-id="9751a-134">Legt die Verteilung als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="9751a-134">Sets the distribution as the default.</span></span>

    * <span data-ttu-id="9751a-135">--Set-Default-Version<Version></span><span class="sxs-lookup"><span data-stu-id="9751a-135">--set-default-version <Version></span></span>
        * <span data-ttu-id="9751a-136">Ändert die Standard Installationsversion für neue Verteilungen.</span><span class="sxs-lookup"><span data-stu-id="9751a-136">Changes the default install version for new distributions.</span></span>

    * <span data-ttu-id="9751a-137">--Set-Version <Distro><Version></span><span class="sxs-lookup"><span data-stu-id="9751a-137">--set-version <Distro> <Version></span></span>
        * <span data-ttu-id="9751a-138">Ändert die Version der angegebenen Verteilung.</span><span class="sxs-lookup"><span data-stu-id="9751a-138">Changes the version of the specified distribution.</span></span>

    * <span data-ttu-id="9751a-139">--beenden,-t<Distro></span><span class="sxs-lookup"><span data-stu-id="9751a-139">--terminate, -t <Distro></span></span>
        * <span data-ttu-id="9751a-140">Beendet die angegebene Verteilung.</span><span class="sxs-lookup"><span data-stu-id="9751a-140">Terminates the specified distribution.</span></span>

    * <span data-ttu-id="9751a-141">--Registrierung aufheben<Distro></span><span class="sxs-lookup"><span data-stu-id="9751a-141">--unregister <Distro></span></span>
        * <span data-ttu-id="9751a-142">Hebt die Registrierung der Verteilung auf.</span><span class="sxs-lookup"><span data-stu-id="9751a-142">Unregisters the distribution.</span></span>

    * <span data-ttu-id="9751a-143">--help</span><span class="sxs-lookup"><span data-stu-id="9751a-143">--help</span></span>
        * <span data-ttu-id="9751a-144">Anzeigen von Nutzungsinformationen.</span><span class="sxs-lookup"><span data-stu-id="9751a-144">Display usage information.</span></span>

## <a name="additional-commands"></a><span data-ttu-id="9751a-145">Weitere Befehle</span><span class="sxs-lookup"><span data-stu-id="9751a-145">Additional Commands</span></span>

<span data-ttu-id="9751a-146">Es gibt auch historische Befehle für die Interaktion mit dem Windows-Subsystem für Linux.</span><span class="sxs-lookup"><span data-stu-id="9751a-146">There are also historic commands to interact with the Windows Subsystem for Linux.</span></span> <span data-ttu-id="9751a-147">Ihre Funktionalität ist in `wsl.exe`enthalten, Sie sind jedoch weiterhin zur Verwendung verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9751a-147">Their functionality is encompassed within `wsl.exe`, but they are still available for use.</span></span> 

### `wslconfig.exe`

<span data-ttu-id="9751a-148">Mit diesem Befehl können Sie Ihre WSL-Verteilung konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="9751a-148">This command lets you configure your WSL distribution.</span></span> <span data-ttu-id="9751a-149">Im folgenden finden Sie eine Liste der zugehörigen Optionen.</span><span class="sxs-lookup"><span data-stu-id="9751a-149">Below is a list of its options.</span></span>

* <span data-ttu-id="9751a-150">/l,/List [Option]</span><span class="sxs-lookup"><span data-stu-id="9751a-150">/l, /list [Option]</span></span>
    * <span data-ttu-id="9751a-151">Listet registrierte Verteilungen auf.</span><span class="sxs-lookup"><span data-stu-id="9751a-151">Lists registered distributions.</span></span>
        * <span data-ttu-id="9751a-152">/All: Optional können Sie alle Distributionen auflisten, einschließlich Verteilungen, die zurzeit installiert oder deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="9751a-152">/all - Optionally list all distributions, including distributions that       are currently being installed or uninstalled.</span></span>

        * <span data-ttu-id="9751a-153">/Running: nur Verteilungen auflisten, die zurzeit ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="9751a-153">/running - List only distributions that are currently running.</span></span>

* <span data-ttu-id="9751a-154">/s,/SetDefault<DistributionName></span><span class="sxs-lookup"><span data-stu-id="9751a-154">/s, /setdefault <DistributionName></span></span>
    * <span data-ttu-id="9751a-155">Legt die Verteilung als Standard fest.</span><span class="sxs-lookup"><span data-stu-id="9751a-155">Sets the distribution as the default.</span></span>

* <span data-ttu-id="9751a-156">/t,/Terminate<DistributionName></span><span class="sxs-lookup"><span data-stu-id="9751a-156">/t, /terminate <DistributionName></span></span>
    * <span data-ttu-id="9751a-157">Beendet die Verteilung.</span><span class="sxs-lookup"><span data-stu-id="9751a-157">Terminates the distribution.</span></span>

* <span data-ttu-id="9751a-158">/u,/Unregister<DistributionName></span><span class="sxs-lookup"><span data-stu-id="9751a-158">/u, /unregister <DistributionName></span></span>
    * <span data-ttu-id="9751a-159">Hebt die Registrierung der Verteilung auf.</span><span class="sxs-lookup"><span data-stu-id="9751a-159">Unregisters the distribution.</span></span>

### `bash.exe`

<span data-ttu-id="9751a-160">Dieser Befehl wird verwendet, um eine bash-Shell zu starten.</span><span class="sxs-lookup"><span data-stu-id="9751a-160">This command is used to start a bash shell.</span></span> <span data-ttu-id="9751a-161">Im folgenden finden Sie die Optionen, die Sie mit diesem Befehl verwenden können.</span><span class="sxs-lookup"><span data-stu-id="9751a-161">Below are the options you can use with this command.</span></span>

* <span data-ttu-id="9751a-162">Keine Option angegeben.</span><span class="sxs-lookup"><span data-stu-id="9751a-162">No Option given</span></span>
    * <span data-ttu-id="9751a-163">Starten der bash-Shell im aktuellen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="9751a-163">Launches the Bash shell in the current directory.</span></span> <span data-ttu-id="9751a-164">Wenn die bash-Shell nicht installiert ist, wird automatisch ausgeführt.`lxrun /install`</span><span class="sxs-lookup"><span data-stu-id="9751a-164">If the Bash shell is not installed automatically runs `lxrun /install`</span></span>

* <span data-ttu-id="9751a-165">bash ~</span><span class="sxs-lookup"><span data-stu-id="9751a-165">bash ~</span></span>
    * <span data-ttu-id="9751a-166">Hiermit wird die bash-Shell in das Basisverzeichnis des Benutzers gestartet.</span><span class="sxs-lookup"><span data-stu-id="9751a-166">Launches the bash shell into the user's home directory.</span></span>  <span data-ttu-id="9751a-167">Vergleichbar mit dem `cd ~`Ausführen von.</span><span class="sxs-lookup"><span data-stu-id="9751a-167">Similar to running `cd ~`.</span></span>

* <span data-ttu-id="9751a-168">bash-c "&lt;Befehl&gt;"</span><span class="sxs-lookup"><span data-stu-id="9751a-168">bash -c "&lt;command&gt;"</span></span>
    * <span data-ttu-id="9751a-169">Führt den Befehl aus, druckt die Ausgabe und wird zurück zur Windows-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="9751a-169">Runs the command, prints the output and exits back to the Windows command prompt.</span></span> <br/> <br/> <span data-ttu-id="9751a-170">Beispiel`bash -c "ls"`</span><span class="sxs-lookup"><span data-stu-id="9751a-170">Example:  `bash -c "ls"`</span></span>

## <a name="deprecated-commands"></a><span data-ttu-id="9751a-171">Als veraltet markierte Befehle</span><span class="sxs-lookup"><span data-stu-id="9751a-171">Deprecated Commands</span></span>

<span data-ttu-id="9751a-172">`lxrun.exe` War der erste Befehl, der zum Installieren und Verwalten des Windows-Subsystems für Linux verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="9751a-172">The `lxrun.exe` was the first command used to install and manage the Windows Subsystem for Linux.</span></span> <span data-ttu-id="9751a-173">Sie ist ab Windows 10 1803 und höher veraltet.</span><span class="sxs-lookup"><span data-stu-id="9751a-173">It is deprecated as of Windows 10 1803 and later.</span></span>

<span data-ttu-id="9751a-174">Der Befehl `lxrun.exe` kann verwendet werden, um direkt mit dem [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) zu interagieren.</span><span class="sxs-lookup"><span data-stu-id="9751a-174">The command `lxrun.exe` can be used to interact with the [Windows Subsystem for Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) directly.</span></span>  <span data-ttu-id="9751a-175">Diese Befehle werden im `\Windows\System32` Verzeichnis installiert und können in einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="9751a-175">These commands are installed into the `\Windows\System32` directory and may be run within a Windows command prompt or in PowerShell.</span></span>

| <span data-ttu-id="9751a-176">Befehl</span><span class="sxs-lookup"><span data-stu-id="9751a-176">Command</span></span>                     | <span data-ttu-id="9751a-177">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9751a-177">Description</span></span>                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | <span data-ttu-id="9751a-178">Der lxrun-Befehl wird verwendet, um die WSL-Instanz zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="9751a-178">The lxrun command is used to manage the WSL instance.</span></span> |
| `lxrun /install`            | <span data-ttu-id="9751a-179">Startet den Download-und Installationsvorgang.</span><span class="sxs-lookup"><span data-stu-id="9751a-179">Starts the download and install process.</span></span> <br/> <span data-ttu-id="9751a-180">**/y** kann hinzugefügt werden, um alle Eingabe Aufforderungen zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="9751a-180">**/y** may be added to bypass all prompts.</span></span>  <span data-ttu-id="9751a-181">Die Bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer ist auf root festgelegt.</span><span class="sxs-lookup"><span data-stu-id="9751a-181">The confirmation prompt is automatically accepted and the default user is set to root.</span></span>          |
| `lxrun /uninstall`          | <span data-ttu-id="9751a-182">Deinstalliert und löscht das Ubuntu-Image.</span><span class="sxs-lookup"><span data-stu-id="9751a-182">Uninstalls and deletes the Ubuntu image.</span></span>  <span data-ttu-id="9751a-183">Standardmäßig wird hierdurch nicht das Ubuntu-Basisverzeichnis des Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="9751a-183">By default this does not remove the user's Ubuntu home directory.</span></span> <br/> <span data-ttu-id="9751a-184">**/y** kann hinzugefügt werden, um die Bestätigungsaufforderung automatisch zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="9751a-184">**/y** may be added to automatically accept the confirmation prompt</span></span> <br/><span data-ttu-id="9751a-185">**/Full** deinstalliert und löscht das Ubuntu-Basisverzeichnis des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9751a-185">**/full** uninstalls and deletes the user's Ubuntu home directory</span></span>         |
| `lxrun /setdefaultuser <userName>`     | <span data-ttu-id="9751a-186">Legt den Standard-bash on Ubuntu-Benutzer fest.</span><span class="sxs-lookup"><span data-stu-id="9751a-186">Sets the default Bash on Ubuntu user.</span></span> <span data-ttu-id="9751a-187">Fordert zur Eingabe eines Kennworts auf, wenn der angegebene Benutzer nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="9751a-187">Will prompt for a password if the specified user does not exist.</span></span>  <span data-ttu-id="9751a-188">Weitere Informationen finden Sie unter https://aka.ms/wslusers:.</span><span class="sxs-lookup"><span data-stu-id="9751a-188">For more information visit: https://aka.ms/wslusers.</span></span> <br/> <span data-ttu-id="9751a-189">**/y** Umgeht das Kennwort.</span><span class="sxs-lookup"><span data-stu-id="9751a-189">**/y** Bypasses promping for the password.</span></span>  <span data-ttu-id="9751a-190">Der Benutzer wird ohne Kennwort erstellt.</span><span class="sxs-lookup"><span data-stu-id="9751a-190">The user will be created without a password.</span></span>|
| `lxrun /update`            | <span data-ttu-id="9751a-191">Aktualisiert den Paket Index des Subsystems.</span><span class="sxs-lookup"><span data-stu-id="9751a-191">Updates the subsystem's package index</span></span>          |
