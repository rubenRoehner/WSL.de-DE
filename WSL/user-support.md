---
title: Linux-Benutzerkonto und Berechtigungen
description: Referenz für die Benutzer- und berechtigungsverwaltung mit dem Windows-Subsystem für Linux.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Benutzerkonten
author: scooley
ms.author: scooley
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.openlocfilehash: 5820d701d5c0e22f14bf76e3dc6fe70bacb5213a
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063598"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a><span data-ttu-id="bb7ef-104">Benutzerkonten und Berechtigungen für Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="bb7ef-104">User Accounts and Permissions for Windows Subsystem for Linux</span></span>

<span data-ttu-id="bb7ef-105">Erstellen Ihre Linux-Benutzer ist der erste Schritt zum Einrichten einer neuen Linux-Distribution für WSL.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-105">Creating your Linux user is the first step in setting up a new Linux distribution on WSL.</span></span>  <span data-ttu-id="bb7ef-106">Das erste Benutzerkonto an, die, das Sie erstellen, wird automatisch mit ein paar spezielle Attribute konfiguriert:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-106">The first user account you create is automatically configured with a few special attributes:</span></span>

1. <span data-ttu-id="bb7ef-107">Es ist Ihre Standardbenutzer – es meldet sich automatisch beim Start.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-107">It is your default user -- it signs-in automatically on launch.</span></span>
1. <span data-ttu-id="bb7ef-108">Linux-Administrator (Mitglied der Gruppe "Sudo") in der Standardeinstellung ist.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-108">It is Linux administrator (a member of the sudo group) by default.</span></span>

<span data-ttu-id="bb7ef-109">Jede Linux-Distribution, die das Windows-Subsystem für Linux unter verfügt über einen eigenen Linux-Benutzerkonten und Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-109">Each Linux distribution running on the Windows Subsystem for Linux has its own Linux user accounts and passwords.</span></span>  <span data-ttu-id="bb7ef-110">Sie müssen ein Linux-Benutzerkonto jederzeit konfigurieren, Sie fügen eine Verteilung, neu installieren oder zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-110">You will have to configure a Linux user account any time you add a distribution, reinstall, or reset.</span></span>  <span data-ttu-id="bb7ef-111">Linux-Benutzerkonten sind nicht nur pro Verteilung voneinander unabhängig, sie sind auch unabhängig von Ihrem Windows-Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-111">Linux user accounts are not only independent per distribution, they are also independent from your Windows user account.</span></span>

## <a name="resetting-your-linux-password"></a><span data-ttu-id="bb7ef-112">Zurücksetzen Ihres Kennworts Linux</span><span class="sxs-lookup"><span data-stu-id="bb7ef-112">Resetting your Linux password</span></span>

<span data-ttu-id="bb7ef-113">Wenn Sie Zugriff auf Ihre Linux-Benutzerkonto haben und wissen Ihr aktuelle Kennwort ein, ändern Sie es unter Verwendung von Linux kennwortzurücksetzung Tools dieser Distribution – wahrscheinlich `passwd`.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-113">If you have access to your Linux user account and know your current password, change it using Linux password reset tools of that distribution -- most likely `passwd`.</span></span>

<span data-ttu-id="bb7ef-114">Wenn dies nicht möglich, je nach der Verteilung ist können Sie zum Zurücksetzen Ihres Kennworts durch Standardbenutzer zurücksetzen können.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-114">If that's not an option, depending on the distribution, you may be able to reset your password by resetting the default user.</span></span>

<span data-ttu-id="bb7ef-115">WSL bietet, dass ein Standard-Benutzer-Tag, welches Benutzerkonto automatisch zu identifizieren anmeldet, wenn Sie eine WSL starten.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-115">WSL offers a default user tag to identify which user account automatically logs in when you start a WSL.</span></span>  <span data-ttu-id="bb7ef-116">Da viele Verteilungen Befehle zum Festlegen von Standardbenutzer-Stamm und auch als Root-Benutzer mit kein Kennwort festgelegt sind, ist das Ändern der Stamm des Standardbenutzers ein nützliches Tool für Aufgaben wie das Zurücksetzen des Kennworts aus.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-116">Since many distributions include commands to set the default user to root and also a root user with no password set, changing the default user to root is a handy tool for things like password reset.</span></span>

### <a name="for-creators-update-and-earlier"></a><span data-ttu-id="bb7ef-117">Für Creators Update und frühere Versionen</span><span class="sxs-lookup"><span data-stu-id="bb7ef-117">For Creators Update and earlier</span></span>
<span data-ttu-id="bb7ef-118">Wenn Sie ausführen, wird Windows 10 Creators update oder haben, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-118">If you're running Windows 10 Creators update or earlier, you can change the default Bash user by running the following commands:</span></span>

1. <span data-ttu-id="bb7ef-119">Ändern den standardmäßigen Benutzer `root`:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-119">Change the default user to `root`:</span></span>

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. <span data-ttu-id="bb7ef-120">Führen Sie `bash.exe` , melden Sie sich jetzt als `root`:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-120">Run `bash.exe` to now login as `root`:</span></span>

    ```console
    C:\> bash.exe
    ```

1. <span data-ttu-id="bb7ef-121">Zurücksetzen Sie des Kennworts, mit der Distribution-Kennwort-Befehl aus, und schließen Sie die Linux-Konsole:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-121">Reset your password using the distribution's password command, and close the Linux Console:</span></span>

    ```BASH
    $ passwd username
    $ exit
    ```

1. <span data-ttu-id="bb7ef-122">Über Windows-CMD den Standardbenutzer auf Ihre normalen Linux-Benutzerkonto zurückgesetzt werden:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-122">From Windows CMD, reset your default user back to your normal Linux user account:</span></span>

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a><span data-ttu-id="bb7ef-123">Für den Fall Creators Update und höher</span><span class="sxs-lookup"><span data-stu-id="bb7ef-123">For Fall Creators Update and later</span></span>
<span data-ttu-id="bb7ef-124">Um festzustellen, welche Befehle für eine bestimmte Verteilung verfügbar sind, führen `[distro.exe] /?`.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-124">To see what commands are available for a particular distribution, run `[distro.exe] /?`.</span></span>
    
<span data-ttu-id="bb7ef-125">Z. B. mit Ubuntu installiert:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-125">For example, with Ubuntu installed:</span></span>

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

<span data-ttu-id="bb7ef-126">Schritt-für-Schritt-Anweisungen, die mit Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-126">Step by step instructions using Ubuntu:</span></span>

1. <span data-ttu-id="bb7ef-127">Open CMD</span><span class="sxs-lookup"><span data-stu-id="bb7ef-127">Open CMD</span></span>
1. <span data-ttu-id="bb7ef-128">Legen Sie den Standard-Linux-Benutzer auf `root`:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-128">Set the default Linux user to `root`:</span></span>

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. <span data-ttu-id="bb7ef-129">Starten Sie Ihre Linux-Distribution (`ubuntu`).</span><span class="sxs-lookup"><span data-stu-id="bb7ef-129">Launch your Linux distribution (`ubuntu`).</span></span>  <span data-ttu-id="bb7ef-130">Sie werden automatisch melden Sie sich als `root`:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-130">You will automatically login as `root`:</span></span>

1. <span data-ttu-id="bb7ef-131">Zurücksetzen, Ihr Kennwort mithilfe der `passwd` Befehl:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-131">Reset your password using the `passwd` command:</span></span>

    ```BASH
    $ passwd username
    ```

1. <span data-ttu-id="bb7ef-132">Über Windows-CMD wird zurücksetzen Sie den Standardbenutzer auf Ihre normalen Linux-Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-132">From Windows CMD, reset your default user back to your normal Linux user account.</span></span>

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a><span data-ttu-id="bb7ef-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb7ef-133">Permissions</span></span>

<span data-ttu-id="bb7ef-134">Es gibt zwei wichtige Konzepte zu bedenken, wenn es um die Berechtigungen in WSL geht:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-134">There are two important concepts to keep in mind when it comes to permissions in WSL:</span></span>

1. <span data-ttu-id="bb7ef-135">Das Windows-Berechtigungsmodell regelt eines Prozesses Rechte für die Windows-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="bb7ef-135">The Windows permission model governs a process' rights to Windows resources</span></span>
2. <span data-ttu-id="bb7ef-136">Das Linux-Berechtigungsmodell steuert eines Prozesses Rechte für die Linux-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="bb7ef-136">The Linux permission model controls a process' rights to Linux resources</span></span>

<span data-ttu-id="bb7ef-137">Wenn Linux auf WSL ausführen zu können, müssen Linux die gleichen Windows-Berechtigungen wie der Prozess, das es startet.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-137">When running Linux on WSL, Linux will have the same Windows permissions as the process that launches it.</span></span> <span data-ttu-id="bb7ef-138">Linux kann in einem der beiden Berechtigungsstufen gestartet werden:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-138">Linux can be launched in one of two permission levels:</span></span>

* <span data-ttu-id="bb7ef-139">Normal (ohne erhöhte Rechte): Linux, die mit den Berechtigungen des angemeldeten Benutzers ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="bb7ef-139">Normal (non-elevated): Linux runs with the permissions of the logged-in user</span></span>
* <span data-ttu-id="bb7ef-140">Mit erhöhten Rechten/Admin: Linux, die mit erhöhten Windows/Administratorberechtigungen ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="bb7ef-140">Elevated/admin: Linux runs with elevated/admin Windows permissions</span></span>

> <span data-ttu-id="bb7ef-141">Da, die erweiterte Prozesse können Änderung/Beschädigung systemweiten Einstellungen und Daten und können geschützten Zugriff/ändern, Dateien und Ordnern, **vermeiden** Prozesse starten erhöht werden, es sei denn, Sie absolut müssen – gibt an, ob sie Windows sind oder Linux-Anwendungen/Tools/Shells!</span><span class="sxs-lookup"><span data-stu-id="bb7ef-141">Because that elevated processes can change/damage system-wide settings and data, and can access/modify protected files and folders, **AVOID** launching elevated processes unless you absolutely have to - whether they're Windows or Linux applications/tools/shells!</span></span>

<span data-ttu-id="bb7ef-142">Die oben aufgeführten Windows-Berechtigungen werden unabhängig von Ihren Berechtigungen innerhalb einer Linux-Instanz: Linux "Stammberechtigungen" wirken sich nur auf die Rechte des Benutzers innerhalb des Linux-Umgebung & Filesystem; Sie haben keine Auswirkung auf die Windows-Berechtigungen erteilt.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-142">The above Windows permissions are independent of the permissions within a Linux instance: Linux "Root privileges" only impact the user’s rights within the Linux environment & filesystem; they have no impact on the Windows privileges granted.</span></span> <span data-ttu-id="bb7ef-143">Daher einen Linux-Prozess ausgeführt, als Root-Benutzer (z.B. über die `sudo`) nur gewährt, die über Administratorrechte in der Linux-Umgebung zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-143">Thus, running a Linux process as root (e.g. via `sudo`) only grants that process admin rights within the Linux environment.</span></span>

**<span data-ttu-id="bb7ef-144">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-144">Example:</span></span>**    
<span data-ttu-id="bb7ef-145">Eine Bash-Sitzung mit Administratorrechten für Windows möglicherweise Zugriff auf `cd /mnt/c/Users/Administrator` zwar eine Bash-Sitzung, ohne über Administratorrechte für einen Fehler "Zugriff verweigert" finden Sie unter würde.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-145">A Bash session with Windows admin privileges may access `cd /mnt/c/Users/Administrator` while a Bash session without admin privileges would see a "Permission Denied" error.</span></span>

<span data-ttu-id="bb7ef-146">Unter Linux eingeben `sudo cd /mnt/c/Users/Administrator` Zugriff auf das Administratorkennwort Verzeichnis wird nicht gewährt werden, da Berechtigungen in Windows, die von Windows verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-146">In Linux, typing `sudo cd /mnt/c/Users/Administrator` will not grant access to the Administrator’s directory since permissions within Windows are managed by Windows.</span></span>

<span data-ttu-id="bb7ef-147">Das Linux-Berechtigungsmodell ist wichtig, in die Linux-Umgebung, in denen der Benutzer die Berechtigungen, die basierend auf dem aktuellen Linux-Benutzer verfügt.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-147">The Linux permission model is important when inside the Linux environment where the user has permissions based on the current Linux user.</span></span>

**<span data-ttu-id="bb7ef-148">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="bb7ef-148">Example:</span></span>**  
<span data-ttu-id="bb7ef-149">Ein Benutzer in der Gruppe "sudo" ausgeführt `sudo apt update`.</span><span class="sxs-lookup"><span data-stu-id="bb7ef-149">A user in the sudo group may run `sudo apt update`.</span></span>
