---
title: WSL-Benutzerkonto Updates in früheren Windows-Versionen
description: Referenz für frühere Windows-Versionen zum Aktualisieren von Linux-Benutzerkonten mit dem Windows-Subsystem für Linux.
ms.date: 01/20/2020
ms.topic: article
ROBOTS: NOINDEX
ms.openlocfilehash: 406158d769c4b465b6168d7cca45b48ff1f201fe
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520839"
---
# <a name="wsl-user-account-updates-on-previous-windows-versions"></a><span data-ttu-id="12319-103">WSL-Benutzerkonto Updates in früheren Windows-Versionen</span><span class="sxs-lookup"><span data-stu-id="12319-103">WSL User Account updates on Previous Windows Versions</span></span>

<span data-ttu-id="12319-104">Dieser Inhalt ist für Benutzer früherer Versionen des Windows-Betriebssystems archiviert, die das-Subsystem für Linux unterstützen und Unterstützung beim Aktualisieren von Linux-Benutzerkonten benötigen.</span><span class="sxs-lookup"><span data-stu-id="12319-104">This content is archived for users of earlier versions of Windows operating system that support the subsystem for Linux and need support with updating Linux user accounts.</span></span>

<span data-ttu-id="12319-105">Die aktuelle Dokumentation finden Sie unter [Benutzerkonten für das Windows-Subsystem für Linux](../user-support.md).</span><span class="sxs-lookup"><span data-stu-id="12319-105">For current documentation, see [User Accounts for Windows Subsystem for Linux](../user-support.md).</span></span>

### <a name="for-creators-update-version-of-windows-and-earlier"></a><span data-ttu-id="12319-106">Für Creators Update-Version von Windows und früher</span><span class="sxs-lookup"><span data-stu-id="12319-106">For Creators Update version of Windows and earlier</span></span>

<span data-ttu-id="12319-107">Wenn Sie Windows 10 Creators Update oder eine frühere Version ausführen, können Sie den Bash-Standardbenutzer ändern, indem Sie die folgenden Befehle ausführen:</span><span class="sxs-lookup"><span data-stu-id="12319-107">If you're running Windows 10 Creators update or earlier, you can change the default Bash user by running the following commands:</span></span>

1. <span data-ttu-id="12319-108">Ändern Sie den Standardbenutzer in `root`:</span><span class="sxs-lookup"><span data-stu-id="12319-108">Change the default user to `root`:</span></span>

    ```console
    C:\> lxrun /setdefaultuser root
    ```

1. <span data-ttu-id="12319-109">Führen `bash.exe` Sie aus, um sich jetzt als `root` anzumelden:</span><span class="sxs-lookup"><span data-stu-id="12319-109">Run `bash.exe` to now login as `root`:</span></span>

    ```console
    C:\> bash.exe
    ```

1. <span data-ttu-id="12319-110">Setzen Sie Ihr Kennwort mit dem Kennwortbefehl der Distribution zurück, und schließen Sie die Linux-Konsole:</span><span class="sxs-lookup"><span data-stu-id="12319-110">Reset your password using the distribution's password command, and close the Linux Console:</span></span>

    ```BASH
    $ passwd username
    $ exit
    ```

1. <span data-ttu-id="12319-111">Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto:</span><span class="sxs-lookup"><span data-stu-id="12319-111">From Windows CMD, reset your default user back to your normal Linux user account:</span></span>

    ```console
    C:\> lxrun.exe /setdefaultuser username
    ```

### <a name="for-fall-creators-update-and-later"></a><span data-ttu-id="12319-112">Fall Creators Update und höhere Versionen</span><span class="sxs-lookup"><span data-stu-id="12319-112">For Fall Creators Update and later</span></span>

<span data-ttu-id="12319-113">Um anzuzeigen, welche Befehle für eine bestimmte Distribution verfügbar sind, führen Sie `[distro.exe] /?` aus.</span><span class="sxs-lookup"><span data-stu-id="12319-113">To see what commands are available for a particular distribution, run `[distro.exe] /?`.</span></span>
    
<span data-ttu-id="12319-114">Beispielsweise bei einer Ubuntu-Installation:</span><span class="sxs-lookup"><span data-stu-id="12319-114">For example, with Ubuntu installed:</span></span>

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

<span data-ttu-id="12319-115">Schrittweise Anleitungen für Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="12319-115">Step by step instructions using Ubuntu:</span></span>

1. <span data-ttu-id="12319-116">Öffnen Sie CMD.</span><span class="sxs-lookup"><span data-stu-id="12319-116">Open CMD</span></span>
1. <span data-ttu-id="12319-117">Legen Sie den Linux -Standardbenutzer auf `root` fest:</span><span class="sxs-lookup"><span data-stu-id="12319-117">Set the default Linux user to `root`:</span></span>

    ```console
    C:\> ubuntu config --default-user root
    ```    

1. <span data-ttu-id="12319-118">Starten Sie Ihre Linux-Distribution (`ubuntu`).</span><span class="sxs-lookup"><span data-stu-id="12319-118">Launch your Linux distribution (`ubuntu`).</span></span>  <span data-ttu-id="12319-119">Sie werden automatisch als `root` angemeldet:</span><span class="sxs-lookup"><span data-stu-id="12319-119">You will automatically login as `root`:</span></span>

1. <span data-ttu-id="12319-120">Setzen Sie Ihr Kennwort mit dem Befehl `passwd` zurück:</span><span class="sxs-lookup"><span data-stu-id="12319-120">Reset your password using the `passwd` command:</span></span>

    ```BASH
    $ passwd username
    ```

1. <span data-ttu-id="12319-121">Setzen Sie Ihren Standardbenutzer über Windows-CMD zurück auf Ihr normales Linux-Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="12319-121">From Windows CMD, reset your default user back to your normal Linux user account.</span></span>

    ```console
    C:\> ubuntu config --default-user username
    ```
