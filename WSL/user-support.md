---
title: Linux-Benutzerkonto und-Berechtigungen
description: Referenz für Benutzerkonten und Berechtigungs Verwaltung mit dem Windows-Subsystem für Linux.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Benutzerkonten
author: scooley
ms.author: scooley
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.openlocfilehash: 0d00b43d059e72edd4e2a5b9591c29441f461fca
ms.sourcegitcommit: cd239efc5c7c25ffbe5de25b2438d44181a838a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/14/2019
ms.locfileid: "67040825"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a><span data-ttu-id="156bb-104">Benutzerkonten und Berechtigungen für das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="156bb-104">User Accounts and Permissions for Windows Subsystem for Linux</span></span>

<span data-ttu-id="156bb-105">Das Erstellen eines Linux-Benutzers ist der erste Schritt beim Einrichten einer neuen Linux-Distribution auf WSL.</span><span class="sxs-lookup"><span data-stu-id="156bb-105">Creating your Linux user is the first step in setting up a new Linux distribution on WSL.</span></span>  <span data-ttu-id="156bb-106">Das erste Benutzerkonto, das Sie erstellen, wird automatisch mit einigen speziellen Attributen konfiguriert:</span><span class="sxs-lookup"><span data-stu-id="156bb-106">The first user account you create is automatically configured with a few special attributes:</span></span>

1. <span data-ttu-id="156bb-107">Dies ist der Standardbenutzer, der sich beim Start automatisch anmeldet.</span><span class="sxs-lookup"><span data-stu-id="156bb-107">It is your default user -- it signs-in automatically on launch.</span></span>
1. <span data-ttu-id="156bb-108">Standardmäßig ist dies der Linux-Administrator (Mitglied der Gruppe "sudo").</span><span class="sxs-lookup"><span data-stu-id="156bb-108">It is Linux administrator (a member of the sudo group) by default.</span></span>

<span data-ttu-id="156bb-109">Jede Linux-Distribution, die unter dem Windows-Subsystem für Linux ausgeführt wird, verfügt über eigene Linux-Benutzerkonten und Kenn Wörter.</span><span class="sxs-lookup"><span data-stu-id="156bb-109">Each Linux distribution running on the Windows Subsystem for Linux has its own Linux user accounts and passwords.</span></span>  <span data-ttu-id="156bb-110">Sie müssen ein Linux-Benutzerkonto konfigurieren, wenn Sie eine Verteilung hinzufügen, neu installieren oder zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="156bb-110">You will have to configure a Linux user account any time you add a distribution, reinstall, or reset.</span></span>  <span data-ttu-id="156bb-111">Linux-Benutzerkonten sind nicht nur pro Verteilung unabhängig, sondern auch unabhängig von Ihrem Windows-Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="156bb-111">Linux user accounts are not only independent per distribution, they are also independent from your Windows user account.</span></span>

## <a name="resetting-your-linux-password"></a><span data-ttu-id="156bb-112">Zurücksetzen Ihres Linux-Kennworts</span><span class="sxs-lookup"><span data-stu-id="156bb-112">Resetting your Linux password</span></span>

<span data-ttu-id="156bb-113">Wenn Sie Zugriff auf Ihr Linux-Benutzerkonto haben und Ihr aktuelles Kennwort kennen, ändern Sie es mit den Tools für die Linux-Kenn Wort `passwd`Zurücksetzung dieser Verteilung (höchstwahrscheinlich).</span><span class="sxs-lookup"><span data-stu-id="156bb-113">If you have access to your Linux user account and know your current password, change it using Linux password reset tools of that distribution -- most likely `passwd`.</span></span>

<span data-ttu-id="156bb-114">Wenn dies nicht möglich ist, können Sie je nach Verteilung Ihr Kennwort zurücksetzen, indem Sie den Standardbenutzer zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="156bb-114">If that's not an option, depending on the distribution, you may be able to reset your password by resetting the default user.</span></span>

<span data-ttu-id="156bb-115">WSL bietet ein Standard Benutzertag, um zu ermitteln, welches Benutzerkonto beim Starten eines WSL automatisch angemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="156bb-115">WSL offers a default user tag to identify which user account automatically logs in when you start a WSL.</span></span>  <span data-ttu-id="156bb-116">Da viele Verteilungen Befehle enthalten, um den Standardbenutzer auf root festzulegen, und auch ein root-Benutzer ohne Kennwort festgelegt ist, ist das Ändern des Standard Benutzers in root ein praktisches Tool für die Kenn Wort Zurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="156bb-116">Since many distributions include commands to set the default user to root and also a root user with no password set, changing the default user to root is a handy tool for things like password reset.</span></span>

### <a name="for-creators-update-and-earlier"></a><span data-ttu-id="156bb-117">Für Creators Update und früher</span><span class="sxs-lookup"><span data-stu-id="156bb-117">For Creators Update and earlier</span></span>
<span data-ttu-id="156bb-118">Wenn Sie Windows 10 Creators Update oder eine frühere Version ausführen, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="156bb-118">If you're running Windows 10 Creators update or earlier, you can change the default Bash user by running the following commands:</span></span>

1. <span data-ttu-id="156bb-119">Ändern Sie den Standardbenutzer `root`in:</span><span class="sxs-lookup"><span data-stu-id="156bb-119">Change the default user to `root`:</span></span>

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. <span data-ttu-id="156bb-120">Führen `bash.exe` Sie aus, um `root`sich jetzt als anzumelden:</span><span class="sxs-lookup"><span data-stu-id="156bb-120">Run `bash.exe` to now login as `root`:</span></span>

    ```console
    C:\> bash.exe
    ```

1. <span data-ttu-id="156bb-121">Setzen Sie Ihr Kennwort mit dem Kenn Wort Befehl der Verteilung zurück, und schließen Sie die Linux-Konsole:</span><span class="sxs-lookup"><span data-stu-id="156bb-121">Reset your password using the distribution's password command, and close the Linux Console:</span></span>

    ```BASH
    $ passwd username
    $ exit
    ```

1. <span data-ttu-id="156bb-122">Setzen Sie Ihren Standardbenutzer von Windows CMD zurück auf Ihr normales Linux-Benutzerkonto:</span><span class="sxs-lookup"><span data-stu-id="156bb-122">From Windows CMD, reset your default user back to your normal Linux user account:</span></span>

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a><span data-ttu-id="156bb-123">Für Fall Creators Update und höher</span><span class="sxs-lookup"><span data-stu-id="156bb-123">For Fall Creators Update and later</span></span>
<span data-ttu-id="156bb-124">Um anzuzeigen, welche Befehle für eine bestimmte Verteilung verfügbar sind, `[distro.exe] /?`führen Sie aus.</span><span class="sxs-lookup"><span data-stu-id="156bb-124">To see what commands are available for a particular distribution, run `[distro.exe] /?`.</span></span>
    
<span data-ttu-id="156bb-125">Beispielsweise bei installiertem Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="156bb-125">For example, with Ubuntu installed:</span></span>

```console
C:\> ubuntu.exe /?

Launches or configures a linux distribution.

Usage:
    <no args>
      - Launches the distro's default behavior. By default, this launches your default shell.

    run <command line>
      - Run the given command line in that distro, using the default configuration.
      - Everything after `run ` is passed to the linux LaunchProcess cal

    config [setting [value]]
      - Configure certain settings for this distro.
      - Settings are any of the following (by default)
        - `--default-user <username>`: Set the default user for this distro to <username>

    clean
      - Uninstalls the distro. The appx remains on your machine. This can be
        useful for "factory resetting" your instance. This removes the linux
        filesystem from the disk, but not the app from your PC, so you don't
        need to redownload the entire tar.gz again.

    help
      - Print this usage message.
```

<span data-ttu-id="156bb-126">Schritt-für-Schritt-Anleitungen unter Verwendung von Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="156bb-126">Step by step instructions using Ubuntu:</span></span>

1. <span data-ttu-id="156bb-127">Cmd öffnen</span><span class="sxs-lookup"><span data-stu-id="156bb-127">Open CMD</span></span>
1. <span data-ttu-id="156bb-128">Legen Sie den Standard-Linux `root`-Benutzer auf fest:</span><span class="sxs-lookup"><span data-stu-id="156bb-128">Set the default Linux user to `root`:</span></span>

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. <span data-ttu-id="156bb-129">Starten Sie Ihre Linux-`ubuntu`Distribution ().</span><span class="sxs-lookup"><span data-stu-id="156bb-129">Launch your Linux distribution (`ubuntu`).</span></span>  <span data-ttu-id="156bb-130">Sie werden automatisch wie `root`folgt anmelden:</span><span class="sxs-lookup"><span data-stu-id="156bb-130">You will automatically login as `root`:</span></span>

1. <span data-ttu-id="156bb-131">Setzen Sie Ihr Kennwort `passwd` mit dem folgenden Befehl zurück:</span><span class="sxs-lookup"><span data-stu-id="156bb-131">Reset your password using the `passwd` command:</span></span>

    ```BASH
    $ passwd username
    ```

1. <span data-ttu-id="156bb-132">Setzen Sie Ihren Standardbenutzer von Windows cmd auf Ihr normales Linux-Benutzerkonto zurück.</span><span class="sxs-lookup"><span data-stu-id="156bb-132">From Windows CMD, reset your default user back to your normal Linux user account.</span></span>

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a><span data-ttu-id="156bb-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="156bb-133">Permissions</span></span>

<span data-ttu-id="156bb-134">Es gibt zwei wichtige Konzepte, die Sie beachten sollten, wenn es um Berechtigungen in WSL geht:</span><span class="sxs-lookup"><span data-stu-id="156bb-134">There are two important concepts to keep in mind when it comes to permissions in WSL:</span></span>

1. <span data-ttu-id="156bb-135">Mit dem Windows-Berechtigungs Modell wird eine Prozess Berechtigung für Windows-Ressourcen geregelt.</span><span class="sxs-lookup"><span data-stu-id="156bb-135">The Windows permission model governs a process' rights to Windows resources</span></span>
2. <span data-ttu-id="156bb-136">Das Linux-Berechtigungs Modell steuert die Rechte eines Prozesses für Linux-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="156bb-136">The Linux permission model controls a process' rights to Linux resources</span></span>

<span data-ttu-id="156bb-137">Bei der Ausführung von Linux auf WSL hat Linux dieselben Windows-Berechtigungen wie der Prozess, von dem die Anwendung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="156bb-137">When running Linux on WSL, Linux will have the same Windows permissions as the process that launches it.</span></span> <span data-ttu-id="156bb-138">Linux kann mit einer von zwei Berechtigungsstufen gestartet werden:</span><span class="sxs-lookup"><span data-stu-id="156bb-138">Linux can be launched in one of two permission levels:</span></span>

* <span data-ttu-id="156bb-139">Normal (ohne erhöhte Rechte): Linux wird mit den Berechtigungen des angemeldeten Benutzers ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="156bb-139">Normal (non-elevated): Linux runs with the permissions of the logged-in user</span></span>
* <span data-ttu-id="156bb-140">Erhöht/admin: Linux wird mit erhöhten/Administrator-Windows-Berechtigungen ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="156bb-140">Elevated/admin: Linux runs with elevated/admin Windows permissions</span></span>

> <span data-ttu-id="156bb-141">Da erweiterte Prozesse auf systemweite Einstellungen und systemweite/geschützte Daten zugreifen bzw. diese ändern (und dadurch beschädigen) können, **vermeiden** Sie das Starten von erweiterten Prozessen, es sei denn, Sie müssen unbedingt die Windows-oder Linux-Anwendungen/Tools/ Bomben!</span><span class="sxs-lookup"><span data-stu-id="156bb-141">Because elevated processes can access/modify (and therefore damage) system-wide settings and system-wide/protected data, **AVOID** launching elevated processes unless you absolutely have to - whether they're Windows or Linux applications/tools/shells!</span></span>

<span data-ttu-id="156bb-142">Die obigen Windows-Berechtigungen sind unabhängig von den Berechtigungen innerhalb einer Linux-Instanz: Linux-"Root-Berechtigungen" wirken sich nur auf die Rechte des Benutzers in der Linux-Umgebung & File System aus; Sie haben keine Auswirkung auf die gewährten Windows-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="156bb-142">The above Windows permissions are independent of the permissions within a Linux instance: Linux "Root privileges" only impact the user’s rights within the Linux environment & filesystem; they have no impact on the Windows privileges granted.</span></span> <span data-ttu-id="156bb-143">Folglich werden durch das Ausführen eines Linux-Prozesses als Stamm ( `sudo`z. b. via) nur die Administratorrechte innerhalb der Linux-Umgebung erteilt.</span><span class="sxs-lookup"><span data-stu-id="156bb-143">Thus, running a Linux process as root (e.g. via `sudo`) only grants that process admin rights within the Linux environment.</span></span>

<span data-ttu-id="156bb-144">**Beispiel:**   </span><span class="sxs-lookup"><span data-stu-id="156bb-144">**Example:**  </span></span>  
<span data-ttu-id="156bb-145">Eine bash-Sitzung mit Windows-Administrator Berechtigungen `cd /mnt/c/Users/Administrator` kann auf zugreifen, während einer bash-Sitzung ohne Administratorrechte der Fehler "Berechtigung verweigert" angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="156bb-145">A Bash session with Windows admin privileges may access `cd /mnt/c/Users/Administrator` while a Bash session without admin privileges would see a "Permission Denied" error.</span></span>

<span data-ttu-id="156bb-146">Unter Linux gewährt die `sudo cd /mnt/c/Users/Administrator` Eingabe keinen Zugriff auf das Administrator Verzeichnis, da Berechtigungen in Windows von Windows verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="156bb-146">In Linux, typing `sudo cd /mnt/c/Users/Administrator` will not grant access to the Administrator’s directory since permissions within Windows are managed by Windows.</span></span>

<span data-ttu-id="156bb-147">Das Linux-Berechtigungs Modell ist wichtig, wenn der Benutzer in der Linux-Umgebung über Berechtigungen verfügt, die auf dem aktuellen Linux-Benutzer basiert.</span><span class="sxs-lookup"><span data-stu-id="156bb-147">The Linux permission model is important when inside the Linux environment where the user has permissions based on the current Linux user.</span></span>

<span data-ttu-id="156bb-148">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="156bb-148">**Example:**</span></span>  
<span data-ttu-id="156bb-149">Ein Benutzer in der sudo-Gruppe kann `sudo apt update`ausführen.</span><span class="sxs-lookup"><span data-stu-id="156bb-149">A user in the sudo group may run `sudo apt update`.</span></span>
