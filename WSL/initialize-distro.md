---
title: Initialisieren einer neuen WSL Linux-Distribution
description: Nach dem Installieren einer Linux-Distribution für WSL führen Sie die folgenden einfachen Schritte aus, um die Initialisierung abzuschließen.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: c33d349a6d39c325b079ccbf7ed6350bed796e33
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "71269586"
---
# <a name="initializing-a-newly-installed-distro"></a><span data-ttu-id="0db24-104">Initialisieren einer neu installierten Distribution</span><span class="sxs-lookup"><span data-stu-id="0db24-104">Initializing a newly installed distro</span></span>
<span data-ttu-id="0db24-105">Nachdem Sie Ihre Distribution heruntergeladen und installiert haben, müssen Sie die Initialisierung der neuen Distribution abschließen:</span><span class="sxs-lookup"><span data-stu-id="0db24-105">Once your distro has been downloaded and installed, you'll need to complete initialization of the new distro:</span></span>

## <a name="launch-a-distro"></a><span data-ttu-id="0db24-106">Starten einer Distribution</span><span class="sxs-lookup"><span data-stu-id="0db24-106">Launch a distro</span></span>
<span data-ttu-id="0db24-107">Um die Initialisierung der neu installierten Distribution abzuschließen, starten Sie eine neue Instanz.</span><span class="sxs-lookup"><span data-stu-id="0db24-107">To complete the initialization of your newly installed distro, launch a new instance.</span></span> <span data-ttu-id="0db24-108">Klicken Sie hierzu in der Microsoft Store-App auf die Schaltfläche „Starten“, oder starten Sie die Distribution über das Startmenü:</span><span class="sxs-lookup"><span data-stu-id="0db24-108">You can do this by clicking the "launch" button in the Microsoft Store app, or launching the distro from the Start menu:</span></span>

> <span data-ttu-id="0db24-109">Tipp: Möglicherweise möchten Sie Ihre am häufigsten verwendeten Distributionen an das Startmenü und/oder an die Taskleiste anheften.</span><span class="sxs-lookup"><span data-stu-id="0db24-109">Tip: You might want to pin your most frequently used distros to your Start menu, and/or to your taskbar!</span></span>

![Starten von Distributionen über das Startmenü](media/start-menu.png)

> <span data-ttu-id="0db24-111">Unter Windows Server können Sie die ausführbare Startprogrammdatei `<distro>.exe` Ihrer Distribution über dem Distributionsinstallationsordner starten.</span><span class="sxs-lookup"><span data-stu-id="0db24-111">On Windows Server, you can launch your distro's launcher executable `<distro>.exe` from the distro installation folder.</span></span>

<span data-ttu-id="0db24-112">Wenn eine neu installierte Distribution zum ersten Mal ausgeführt wird, wird ein Konsolenfenster geöffnet, und Sie werden aufgefordert, bis zum Abschluss der Installation wenige Minuten zu warten.</span><span class="sxs-lookup"><span data-stu-id="0db24-112">The first time a newly installed distro runs, a Console window will open, and you'll be asked to wait for a minute or two for the installation to complete.</span></span>

> <span data-ttu-id="0db24-113">In dieser letzten Phase der Installation werden die Dateien der Distribution dekomprimiert und auf Ihrem PC gespeichert. Sie sind dann einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="0db24-113">During this final stage of installation, the distro's files are de-compressed and stored on your PC, ready for use.</span></span> <span data-ttu-id="0db24-114">Dies kann je nach Leistung der Speichergeräte Ihres PCs etwa eine Minute oder ggf. auch länger dauern.</span><span class="sxs-lookup"><span data-stu-id="0db24-114">This may take around a minute or more depending on the performance of your PC's storage devices.</span></span> <span data-ttu-id="0db24-115">Diese erste Installationsphase ist nur erforderlich, wenn eine „saubere“ Distribution installiert wird. Alle zukünftigen Starts sollten weniger als eine Sekunde in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="0db24-115">This initial installation phase is only required when a distro is clean-installed - all future launches should take less than a second.</span></span>

## <a name="setting-up-a-new-linux-user-account"></a><span data-ttu-id="0db24-116">Einrichten eines neuen Linux-Benutzerkontos</span><span class="sxs-lookup"><span data-stu-id="0db24-116">Setting up a new Linux user account</span></span>

<span data-ttu-id="0db24-117">Nach Abschluss der Installation werden Sie aufgefordert, ein neues Benutzerkonto (und das zugehörige Kennwort) zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="0db24-117">Once installation is complete, you will be prompted to create a new user account (and its password).</span></span> 

![Entpacken von Ubuntu in der Windows-Konsole](media/UbuntuInstall.png)

<span data-ttu-id="0db24-119">Dieses Benutzerkonto gilt für den normalen Benutzer ohne Administratorrechte, als der Sie beim Starten einer Distribution standardmäßig angemeldet werden.</span><span class="sxs-lookup"><span data-stu-id="0db24-119">This user account is for the normal non-admin user that you'll be logged-in as by default when launching a distro.</span></span>

> <span data-ttu-id="0db24-120">Sie können einen beliebigen Benutzernamen und ein gewünschtes Kennwort auswählen. Beides hat keinen Einfluss auf Ihren Windows-Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="0db24-120">You can choose any username and password you wish - they have no bearing on your Windows username.</span></span> 

<span data-ttu-id="0db24-121">Wenn Sie eine neue Distributionsinstanz öffnen, werden Sie nicht zur Eingabe Ihres Kennworts aufgefordert. Wenn Sie jedoch **einen Prozess mit `sudo` heraufstufen, müssen Sie Ihr Kennwort eingeben**. Stellen Sie also sicher, dass Sie ein Kennwort auswählen, das Sie sich leicht merken können.</span><span class="sxs-lookup"><span data-stu-id="0db24-121">When you open a new distro instance, you won't be prompted for your password, but **if you elevate a process using `sudo`, you will need to enter your password**, so make sure you choose a password you can easily remember!</span></span> <span data-ttu-id="0db24-122">Weitere Informationen finden Sie auf der Seite [Benutzersupport](user-support.md).</span><span class="sxs-lookup"><span data-stu-id="0db24-122">See the [User Support](user-support.md) page for more info.</span></span>

## <a name="update--upgrade-your-distros-packages"></a><span data-ttu-id="0db24-123">Aktualisieren und Upgraden der Pakete Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="0db24-123">Update & upgrade your distro's packages</span></span>

<span data-ttu-id="0db24-124">Die meisten Distributionen werden mit einem leeren/minimalen Paketkatalog ausgeliefert.</span><span class="sxs-lookup"><span data-stu-id="0db24-124">Most distros ship with an empty/minimal package catalog.</span></span> <span data-ttu-id="0db24-125">Es wird dringend empfohlen, den Paketkatalog regelmäßig zu aktualisieren und ein Upgrade der installierten Pakete mit dem bevorzugten Paket-Manager Ihrer Distribution auszuführen.</span><span class="sxs-lookup"><span data-stu-id="0db24-125">We strongly recommend regularly updating your package catalog, and upgrading your installed packages using your distro's preferred package manager.</span></span> <span data-ttu-id="0db24-126">Unter Debian/Ubuntu verwenden Sie apt:</span><span class="sxs-lookup"><span data-stu-id="0db24-126">On Debian/Ubuntu, you use apt:</span></span>

```bash
sudo apt update && sudo apt upgrade
```

> <span data-ttu-id="0db24-127">Windows führt für Ihre Linux-Distributionen nicht automatisch eine Aktualisierung oder ein Upgrade aus: Linux-Benutzer ziehen es vor, diese Aufgabe selbst zu steuern.</span><span class="sxs-lookup"><span data-stu-id="0db24-127">Windows does not automatically update or upgrade your Linux distro(s): This is a task that the Linux users prefer to control themselves.</span></span>

<span data-ttu-id="0db24-128">Fertig!</span><span class="sxs-lookup"><span data-stu-id="0db24-128">You're done!</span></span> <span data-ttu-id="0db24-129">Viel Spaß bei der Verwendung Ihrer neuen Linux-Distribution unter WSL!</span><span class="sxs-lookup"><span data-stu-id="0db24-129">Enjoy using your new Linux distro on WSL!</span></span> <span data-ttu-id="0db24-130">Weitere Informationen zu WSL finden Sie in der weiteren [WSL-Dokumentation](https://aka.ms/wsldocs) oder auf der [Seite mit den WSL-Lernressourcen](https://aka.ms/learnwsl).</span><span class="sxs-lookup"><span data-stu-id="0db24-130">To learn more about WSL, review the other [WSL docs](https://aka.ms/wsldocs), or the [WSL learning resources page](https://aka.ms/learnwsl).</span></span>

![Viel Spaß bei der Verwendung von Linux unter WSL!](media/linux-on-wsl.png)

## <a name="troubleshooting"></a><span data-ttu-id="0db24-132">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="0db24-132">Troubleshooting</span></span>

<span data-ttu-id="0db24-133">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="0db24-133">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="0db24-134">Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="0db24-134">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

> <span data-ttu-id="0db24-135">**Fehler bei der Installation: 0x8007007e**: Dieser Fehler tritt auf, wenn das System Linux aus dem Store nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0db24-135">**Installation failed with error 0x8007007e** This error occurs when your system doesn't support Linux from the store.</span></span>  <span data-ttu-id="0db24-136">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="0db24-136">Make sure that:</span></span>
> * <span data-ttu-id="0db24-137">Sie führen Windows-Build 16215 oder höher aus.</span><span class="sxs-lookup"><span data-stu-id="0db24-137">You're running Windows build 16215 or later.</span></span> <span data-ttu-id="0db24-138">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="0db24-138">[Check your build](troubleshooting.md#check-your-build-number).</span></span>
> * <span data-ttu-id="0db24-139">Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.</span><span class="sxs-lookup"><span data-stu-id="0db24-139">The Windows Subsystem for Linux optional component is enabled and the computer has restarted.</span></span>  <span data-ttu-id="0db24-140">[Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="0db24-140">[Make sure WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled).</span></span>
