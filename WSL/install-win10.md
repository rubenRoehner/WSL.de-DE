---
title: Installieren des Windows-Subsystems für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10, install
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 17ca32db23b426ef1367ff9444b5924d9d7e1716
ms.sourcegitcommit: 3be576f946611cf36e27745bdb7c4c52af1b9928
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74200233"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a><span data-ttu-id="7a1e3-104">Windows-Subsystem für Linux: Installationsleitfaden für Windows 10</span><span class="sxs-lookup"><span data-stu-id="7a1e3-104">Windows Subsystem for Linux Installation Guide for Windows 10</span></span>

## <a name="install-the-windows-subsystem-for-linux"></a><span data-ttu-id="7a1e3-105">Installieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="7a1e3-105">Install the Windows Subsystem for Linux</span></span>

<span data-ttu-id="7a1e3-106">Bevor Sie Linux-Distributionen für WSL installieren, müssen Sie sicherstellen, dass das optionale Feature „Windows-Subsystem für Linux“ aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-106">Before installing any Linux distros for WSL, you must ensure that the "Windows Subsystem for Linux" optional feature is enabled:</span></span>

1. <span data-ttu-id="7a1e3-107">Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-107">Open PowerShell as Administrator and run:</span></span>
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. <span data-ttu-id="7a1e3-108">Starten Sie den Computer neu, wenn Sie dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-108">Restart your computer when prompted.</span></span>

## <a name="install-your-linux-distribution-of-choice"></a><span data-ttu-id="7a1e3-109">Installieren der Linux-Distribution Ihrer Wahl</span><span class="sxs-lookup"><span data-stu-id="7a1e3-109">Install your Linux Distribution of Choice</span></span>
<span data-ttu-id="7a1e3-110">Zum Herunterladen und Installieren Ihrer bevorzugten Distribution(en) haben Sie drei Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-110">To download and install your preferred distro(s), you have three choices:</span></span>
* <span data-ttu-id="7a1e3-111">Herunterladen und Installieren aus dem Microsoft Store (siehe unten)</span><span class="sxs-lookup"><span data-stu-id="7a1e3-111">Download and install from the Microsoft Store (see below)</span></span>
* <span data-ttu-id="7a1e3-112">Herunterladen und Installieren über die Befehlszeile bzw. ein Skript ([lesen Sie die Anweisungen für eine manuelle Installation](install-manual.md))</span><span class="sxs-lookup"><span data-stu-id="7a1e3-112">Download and install from the Command-Line/Script ([read the manual installation instructions](install-manual.md))</span></span>
* <span data-ttu-id="7a1e3-113">Herunterladen und manuelles Entpacken und Installieren (für Windows Server, [Anleitungen finden Sie hier](install-on-server.md))</span><span class="sxs-lookup"><span data-stu-id="7a1e3-113">Download and manually unpack and install (for Windows Server - [instructions here](install-on-server.md))</span></span>

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a><span data-ttu-id="7a1e3-114">Windows 10 Fall Creators Update oder höher: Herunterladen aus dem Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="7a1e3-114">Windows 10 Fall Creators Update and later: Install from the Microsoft Store</span></span>

> <span data-ttu-id="7a1e3-115">Dieser Abschnitt gilt für Windows Build 16215 oder höher.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-115">This section is for Windows build 16215 or later.</span></span>  <span data-ttu-id="7a1e3-116">Führen Sie diese Schritte aus, um [Ihren Build zu überprüfen](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="7a1e3-116">Follow these steps to [check your build](troubleshooting.md#check-your-build-number).</span></span> 

1. <span data-ttu-id="7a1e3-117">Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugte Linux-Distribution aus.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-117">Open the Microsoft Store and choose your favorite Linux distribution.</span></span>

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/store.png)

    <span data-ttu-id="7a1e3-119">Über die folgenden Links wird die Seite des Microsoft Store für jede Distribution geöffnet:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-119">The following links will open the Microsoft store page for each distribution:</span></span>

    * [<span data-ttu-id="7a1e3-120">Ubuntu 16.04 LTS</span><span class="sxs-lookup"><span data-stu-id="7a1e3-120">Ubuntu 16.04 LTS</span></span>](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    * [<span data-ttu-id="7a1e3-121">Ubuntu 18.04 LTS</span><span class="sxs-lookup"><span data-stu-id="7a1e3-121">Ubuntu 18.04 LTS</span></span>](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    * [<span data-ttu-id="7a1e3-122">OpenSUSE Leap 15</span><span class="sxs-lookup"><span data-stu-id="7a1e3-122">OpenSUSE Leap 15</span></span>](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    * [<span data-ttu-id="7a1e3-123">OpenSUSE Leap 42</span><span class="sxs-lookup"><span data-stu-id="7a1e3-123">OpenSUSE Leap 42</span></span>](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [<span data-ttu-id="7a1e3-124">SUSE Linux Enterprise Server 12</span><span class="sxs-lookup"><span data-stu-id="7a1e3-124">SUSE Linux Enterprise Server 12</span></span>](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [<span data-ttu-id="7a1e3-125">SUSE Linux Enterprise Server 15</span><span class="sxs-lookup"><span data-stu-id="7a1e3-125">SUSE Linux Enterprise Server 15</span></span>](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    * [<span data-ttu-id="7a1e3-126">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="7a1e3-126">Kali Linux</span></span>](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [<span data-ttu-id="7a1e3-127">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="7a1e3-127">Debian GNU/Linux</span></span>](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    * [<span data-ttu-id="7a1e3-128">Fedora Remix for WSL</span><span class="sxs-lookup"><span data-stu-id="7a1e3-128">Fedora Remix for WSL</span></span>](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    * [<span data-ttu-id="7a1e3-129">Pengwin</span><span class="sxs-lookup"><span data-stu-id="7a1e3-129">Pengwin</span></span>](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    * [<span data-ttu-id="7a1e3-130">Pengwin Enterprise</span><span class="sxs-lookup"><span data-stu-id="7a1e3-130">Pengwin Enterprise</span></span>](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    * [<span data-ttu-id="7a1e3-131">Alpine WSL</span><span class="sxs-lookup"><span data-stu-id="7a1e3-131">Alpine WSL</span></span>](https://www.microsoft.com/store/apps/9p804crf0395)

1. <span data-ttu-id="7a1e3-132">Wählen Sie auf der Seite der Distribution die Option „Get“ (Abrufen) aus.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-132">From the distro's page, select "Get"</span></span>

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a><span data-ttu-id="7a1e3-134">Vervollständigen der Initialisierung Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="7a1e3-134">Complete initialization of your distro</span></span>
<span data-ttu-id="7a1e3-135">Nachdem Sie Ihre Linux-Distribution installiert haben, müssen Sie Ihre [neue Distributionsinstanz ein Mal initialisieren](initialize-distro.md), bevor sie verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-135">Now that your Linux distro is installed, you must [initialize your new distro instance](initialize-distro.md) once, before it can be used.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="7a1e3-136">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-136">Troubleshooting:</span></span> 

<span data-ttu-id="7a1e3-137">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-137">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="7a1e3-138">Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="7a1e3-138">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

* <span data-ttu-id="7a1e3-139">**Installation failed with error 0x80070003 (Installationsfehler mit Fehlercode 0x80070003)**</span><span class="sxs-lookup"><span data-stu-id="7a1e3-139">**Installation failed with error 0x80070003**</span></span>
    * <span data-ttu-id="7a1e3-140">Das Windows-Subsystem für Linux wird nur auf dem Systemlaufwerk ausgeführt (in der Regel ist dies Ihr Laufwerk `C:`).</span><span class="sxs-lookup"><span data-stu-id="7a1e3-140">The Windows Subsystem for Linux only runs on your system drive (usually this is your `C:` drive).</span></span> <span data-ttu-id="7a1e3-141">Stellen Sie sicher, dass die Distributionen auf dem Systemlaufwerk gespeichert sind:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-141">Make sure that distros are stored on your system drive:</span></span>  
    * <span data-ttu-id="7a1e3-142">Öffnen Sie **Einstellungen** -> **Speicher** -> **Weitere Speichereinstellungen: Ändern Sie den Speicherort für neue Inhalte**
    ![Abbildung der Systemeinstellungen für die Installation von Apps auf dem Laufwerk C:](media/AppStorage.png)</span><span class="sxs-lookup"><span data-stu-id="7a1e3-142">Open **Settings** -> **Storage** -> **More Storage Settings: Change where new content is saved**
![Picture of system settings to install apps on C: drive](media/AppStorage.png)</span></span>
    
    
 * <span data-ttu-id="7a1e3-143">**WslRegisterDistribution failed with error 0x8007019e (WslRegisterDistribution-Fehler mit Fehlercode 0x8007019e)**</span><span class="sxs-lookup"><span data-stu-id="7a1e3-143">**WslRegisterDistribution failed with error 0x8007019e**</span></span>   
  * <span data-ttu-id="7a1e3-144">Die optionale Komponente des Windows-Subsystems für Linux ist nicht aktiviert:</span><span class="sxs-lookup"><span data-stu-id="7a1e3-144">The Windows Subsystem for Linux optional component is not enabled:</span></span> 
   * <span data-ttu-id="7a1e3-145">Öffnen Sie **Systemsteuerung** -> **Programme und Funktionen** -> **Windows-Funktion aktivieren oder deaktivieren**. Aktivieren Sie die Option **Windows-Subsystem für Linux**, oder verwenden Sie das PowerShell-Cmdlet, das am Anfang dieses Artikels erwähnt wurde.</span><span class="sxs-lookup"><span data-stu-id="7a1e3-145">Open **Control Panel** -> **Programs and Features** -> **Turn Windows Feature on or off** -> Check **Windows Subsystem for Linux** or using the PowerShell cmdlet mentioned at the begining of this article.</span></span>
