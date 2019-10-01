---
title: Linux-Benutzerkonto und -Berechtigungen
description: Referenz für Benutzerkonten und Berechtigungsverwaltung mit dem Windows-Subsystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, user accounts
ms.date: 09/11/2017
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: d8434283e459ae25637fac0c0b1877ca07d9a255
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269711"
---
# <a name="user-accounts-and-permissions-for-windows-subsystem-for-linux"></a><span data-ttu-id="251c8-104">Benutzerkonten und Berechtigungen für das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="251c8-104">User Accounts and Permissions for Windows Subsystem for Linux</span></span>

<span data-ttu-id="251c8-105">Das Erstellen eines Linux-Benutzers ist der erste Schritt beim Einrichten einer neuen Linux-Distribution unter WSL.</span><span class="sxs-lookup"><span data-stu-id="251c8-105">Creating your Linux user is the first step in setting up a new Linux distribution on WSL.</span></span>  <span data-ttu-id="251c8-106">Das erste Benutzerkonto, das Sie erstellen, wird automatisch mit einigen speziellen Attributen konfiguriert:</span><span class="sxs-lookup"><span data-stu-id="251c8-106">The first user account you create is automatically configured with a few special attributes:</span></span>

1. <span data-ttu-id="251c8-107">Dies ist der Standardbenutzer, der sich beim Start automatisch anmeldet.</span><span class="sxs-lookup"><span data-stu-id="251c8-107">It is your default user -- it signs-in automatically on launch.</span></span>
1. <span data-ttu-id="251c8-108">Standardmäßig ist dies der Linux-Administrator (Mitglied der Gruppe „sudo“).</span><span class="sxs-lookup"><span data-stu-id="251c8-108">It is Linux administrator (a member of the sudo group) by default.</span></span>

<span data-ttu-id="251c8-109">Jede Linux-Distribution, die unter dem Windows-Subsystem für Linux ausgeführt wird, verfügt über eigene Linux-Benutzerkonten und -Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="251c8-109">Each Linux distribution running on the Windows Subsystem for Linux has its own Linux user accounts and passwords.</span></span>  <span data-ttu-id="251c8-110">Sie müssen ein Linux-Benutzerkonto konfigurieren, wenn Sie eine Distribution hinzufügen, erneut installieren oder zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="251c8-110">You will have to configure a Linux user account any time you add a distribution, reinstall, or reset.</span></span>  <span data-ttu-id="251c8-111">Linux-Benutzerkonten sind nicht nur pro Distribution unabhängig, sondern auch von Ihrem Windows-Benutzerkonto unabhängig.</span><span class="sxs-lookup"><span data-stu-id="251c8-111">Linux user accounts are not only independent per distribution, they are also independent from your Windows user account.</span></span>

## <a name="resetting-your-linux-password"></a><span data-ttu-id="251c8-112">Zurücksetzen Ihres Linux-Kennworts</span><span class="sxs-lookup"><span data-stu-id="251c8-112">Resetting your Linux password</span></span>

<span data-ttu-id="251c8-113">Wenn Sie Zugriff auf Ihr Linux-Benutzerkonto haben und Ihr aktuelles Kennwort kennen, ändern Sie es mit den Tools für die Linux-Kennwortzurücksetzung dieser Distribution (höchstwahrscheinlich `passwd`).</span><span class="sxs-lookup"><span data-stu-id="251c8-113">If you have access to your Linux user account and know your current password, change it using Linux password reset tools of that distribution -- most likely `passwd`.</span></span>

<span data-ttu-id="251c8-114">Wenn dies nicht möglich ist, können Sie je nach Distribution Ihr Kennwort zurücksetzen, indem Sie den Standardbenutzer zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="251c8-114">If that's not an option, depending on the distribution, you may be able to reset your password by resetting the default user.</span></span>

<span data-ttu-id="251c8-115">WSL bietet ein Standardbenutzertag, um zu ermitteln, welches Benutzerkonto beim Starten einer WSL-Sitzung automatisch angemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="251c8-115">WSL offers a default user tag to identify which user account automatically logs in when you start a WSL.</span></span>  <span data-ttu-id="251c8-116">Da viele Distributionen Befehle enthalten, um den Standardbenutzer auf „root“ und auch einen root-Benutzer ohne Kennwort festzulegen, ist das Ändern des Standardbenutzers in „root“ eine praktisches Möglichkeit für die Kennwortzurücksetzung.</span><span class="sxs-lookup"><span data-stu-id="251c8-116">Since many distributions include commands to set the default user to root and also a root user with no password set, changing the default user to root is a handy tool for things like password reset.</span></span>

### <a name="for-creators-update-and-earlier"></a><span data-ttu-id="251c8-117">Creators Update und frühere Versionen</span><span class="sxs-lookup"><span data-stu-id="251c8-117">For Creators Update and earlier</span></span>
<span data-ttu-id="251c8-118">Wenn Sie Windows 10 Creators Update oder eine frühere Version ausführen, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="251c8-118">If you're running Windows 10 Creators update or earlier, you can change the default Bash user by running the following commands:</span></span>

1. <span data-ttu-id="251c8-119">Ändern Sie den Standardbenutzer in `root`:</span><span class="sxs-lookup"><span data-stu-id="251c8-119">Change the default user to `root`:</span></span>

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. <span data-ttu-id="251c8-120">Führen `bash.exe` Sie aus, um sich jetzt als `root` anzumelden:</span><span class="sxs-lookup"><span data-stu-id="251c8-120">Run `bash.exe` to now login as `root`:</span></span>

    ```console
    C:\> bash.exe
    ```

1. <span data-ttu-id="251c8-121">Setzen Sie Ihr Kennwort mit dem Kennwortbefehl der Distribution zurück, und schließen Sie die Linux-Konsole:</span><span class="sxs-lookup"><span data-stu-id="251c8-121">Reset your password using the distribution's password command, and close the Linux Console:</span></span>

    ```BASH
    $ passwd username
    $ exit
    ```

1. <span data-ttu-id="251c8-122">Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto:</span><span class="sxs-lookup"><span data-stu-id="251c8-122">From Windows CMD, reset your default user back to your normal Linux user account:</span></span>

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a><span data-ttu-id="251c8-123">Fall Creators Update und höhere Versionen</span><span class="sxs-lookup"><span data-stu-id="251c8-123">For Fall Creators Update and later</span></span>
<span data-ttu-id="251c8-124">Um anzuzeigen, welche Befehle für eine bestimmte Distribution verfügbar sind, führen Sie `[distro.exe] /?` aus.</span><span class="sxs-lookup"><span data-stu-id="251c8-124">To see what commands are available for a particular distribution, run `[distro.exe] /?`.</span></span>
    
<span data-ttu-id="251c8-125">Beispielsweise bei einer Ubuntu-Installation:</span><span class="sxs-lookup"><span data-stu-id="251c8-125">For example, with Ubuntu installed:</span></span>

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

<span data-ttu-id="251c8-126">Schrittweise Anleitungen für Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="251c8-126">Step by step instructions using Ubuntu:</span></span>

1. <span data-ttu-id="251c8-127">Öffnen Sie CMD.</span><span class="sxs-lookup"><span data-stu-id="251c8-127">Open CMD</span></span>
1. <span data-ttu-id="251c8-128">Legen Sie den Linux -Standardbenutzer auf `root` fest:</span><span class="sxs-lookup"><span data-stu-id="251c8-128">Set the default Linux user to `root`:</span></span>

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. <span data-ttu-id="251c8-129">Starten Sie Ihre Linux-Distribution (`ubuntu`).</span><span class="sxs-lookup"><span data-stu-id="251c8-129">Launch your Linux distribution (`ubuntu`).</span></span>  <span data-ttu-id="251c8-130">Sie werden automatisch als `root` angemeldet:</span><span class="sxs-lookup"><span data-stu-id="251c8-130">You will automatically login as `root`:</span></span>

1. <span data-ttu-id="251c8-131">Setzen Sie Ihr Kennwort mit dem Befehl `passwd` zurück:</span><span class="sxs-lookup"><span data-stu-id="251c8-131">Reset your password using the `passwd` command:</span></span>

    ```BASH
    $ passwd username
    ```

1. <span data-ttu-id="251c8-132">Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="251c8-132">From Windows CMD, reset your default user back to your normal Linux user account.</span></span>

    ```console
    C:\> ubuntu config --default-user username
    ```

## <a name="permissions"></a><span data-ttu-id="251c8-133">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="251c8-133">Permissions</span></span>

<span data-ttu-id="251c8-134">Es gibt zwei wichtige Konzepte, die Sie beachten sollten, wenn es um Berechtigungen in WSL geht:</span><span class="sxs-lookup"><span data-stu-id="251c8-134">There are two important concepts to keep in mind when it comes to permissions in WSL:</span></span>

1. <span data-ttu-id="251c8-135">Mit dem Windows-Berechtigungsmodell werden die Rechte eines Prozesses für Windows-Ressourcen gesteuert.</span><span class="sxs-lookup"><span data-stu-id="251c8-135">The Windows permission model governs a process' rights to Windows resources</span></span>
2. <span data-ttu-id="251c8-136">Mit dem Linux-Berechtigungsmodell werden die Rechte eines Prozesses für Linux-Ressourcen gesteuert.</span><span class="sxs-lookup"><span data-stu-id="251c8-136">The Linux permission model controls a process' rights to Linux resources</span></span>

<span data-ttu-id="251c8-137">Bei der Ausführung von Linux unter WSL verfügt Linux über dieselben Windows-Berechtigungen wie der Prozess, der die Anwendung startet.</span><span class="sxs-lookup"><span data-stu-id="251c8-137">When running Linux on WSL, Linux will have the same Windows permissions as the process that launches it.</span></span> <span data-ttu-id="251c8-138">Linux kann mit einer von zwei Berechtigungsstufen gestartet werden:</span><span class="sxs-lookup"><span data-stu-id="251c8-138">Linux can be launched in one of two permission levels:</span></span>

* <span data-ttu-id="251c8-139">Normal (ohne erhöhte Rechte): Linux wird mit den Berechtigungen des angemeldeten Benutzers ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="251c8-139">Normal (non-elevated): Linux runs with the permissions of the logged-in user</span></span>
* <span data-ttu-id="251c8-140">Erhöhte Rechte/Administrator: Linux wird mit erhöhten Rechten/Windows-Administratorberechtigungen ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="251c8-140">Elevated/admin: Linux runs with elevated/admin Windows permissions</span></span>

> <span data-ttu-id="251c8-141">Da Prozesse mit erhöhten Rechten auf systemweite Einstellungen und systemweite/geschützte Daten zugreifen bzw. diese ändern (und dadurch beschädigen) können , sollten Sie es **VERMEIDEN**, erhöhte Prozesse zu starten, es sei denn, dies ist unbedingt erforderlich. Dabei ist es gleichgültig, ob es sich um Windows- oder Linux- Anwendungen/Tools/Shells handelt!</span><span class="sxs-lookup"><span data-stu-id="251c8-141">Because elevated processes can access/modify (and therefore damage) system-wide settings and system-wide/protected data, **AVOID** launching elevated processes unless you absolutely have to - whether they're Windows or Linux applications/tools/shells!</span></span>

<span data-ttu-id="251c8-142">Die oben genannten Windows-Berechtigungen sind unabhängig von den Berechtigungen innerhalb einer Linux-Instanz: „root-Berechtigungen“ von Linux wirken sich nur auf die Rechte des Benutzers in der Linux-Umgebung und im -Dateisystem aus. Sie besitzen keine Auswirkung auf die gewährten Windows-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="251c8-142">The above Windows permissions are independent of the permissions within a Linux instance: Linux "Root privileges" only impact the user’s rights within the Linux environment & filesystem; they have no impact on the Windows privileges granted.</span></span> <span data-ttu-id="251c8-143">Folglich werden durch das Ausführen eines Linux-Prozesses als „root“ ( z.B. über `sudo`) dem Prozess nur die Administratorrechte innerhalb der Linux-Umgebung erteilt.</span><span class="sxs-lookup"><span data-stu-id="251c8-143">Thus, running a Linux process as root (e.g. via `sudo`) only grants that process admin rights within the Linux environment.</span></span>

<span data-ttu-id="251c8-144">**Beispiel:**   </span><span class="sxs-lookup"><span data-stu-id="251c8-144">**Example:**  </span></span>  
<span data-ttu-id="251c8-145">Eine Bash-Sitzung mit Windows-Administratorberechtigungen kann auf `cd /mnt/c/Users/Administrator` zugreifen, während in einer Bash-Sitzung ohne Administratorberechtigungen der Fehler „Permission Denied“ (Berechtigung verweigert) angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="251c8-145">A Bash session with Windows admin privileges may access `cd /mnt/c/Users/Administrator` while a Bash session without admin privileges would see a "Permission Denied" error.</span></span>

<span data-ttu-id="251c8-146">Unter Linux gewährt die Eingabe von `sudo cd /mnt/c/Users/Administrator` keinen Zugriff auf das Verzeichnis des Administrators, da Berechtigungen innerhalb von Windows von Windows verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="251c8-146">In Linux, typing `sudo cd /mnt/c/Users/Administrator` will not grant access to the Administrator’s directory since permissions within Windows are managed by Windows.</span></span>

<span data-ttu-id="251c8-147">Das Linux-Berechtigungsmodell ist in der Linux-Umgebung wichtig, wenn der Benutzer über Berechtigungen verfügt, die auf dem aktuellen Linux-Benutzer basieren.</span><span class="sxs-lookup"><span data-stu-id="251c8-147">The Linux permission model is important when inside the Linux environment where the user has permissions based on the current Linux user.</span></span>

<span data-ttu-id="251c8-148">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="251c8-148">**Example:**</span></span>  
<span data-ttu-id="251c8-149">Ein Benutzer in der Gruppe „sudo“ kann `sudo apt update`ausführen.</span><span class="sxs-lookup"><span data-stu-id="251c8-149">A user in the sudo group may run `sudo apt update`.</span></span>
