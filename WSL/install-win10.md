---
title: Installieren von Windows-Subsystem für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: Installieren Sie BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: d30a5883d648e084193659e997c55d203eb5a735
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67035049"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a><span data-ttu-id="4488e-104">Windows-Subsystem für Linux – Installationsleitfaden für Windows 10</span><span class="sxs-lookup"><span data-stu-id="4488e-104">Windows Subsystem for Linux Installation Guide for Windows 10</span></span>

## <a name="install-the-windows-subsystem-for-linux"></a><span data-ttu-id="4488e-105">Installieren Sie das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="4488e-105">Install the Windows Subsystem for Linux</span></span>

<span data-ttu-id="4488e-106">Vor der Installation alle Linux-Distributionen für WSL, müssen Sie sicherstellen, dass die "Windows-Subsystem für Linux" optionales Feature aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="4488e-106">Before installing any Linux distros for WSL, you must ensure that the "Windows Subsystem for Linux" optional feature is enabled:</span></span>

1. <span data-ttu-id="4488e-107">Öffnen Sie PowerShell als Administrator, und führen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="4488e-107">Open PowerShell as Administrator and run:</span></span>
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. <span data-ttu-id="4488e-108">Starten Sie Ihre Computer bei entsprechender Aufforderung neu.</span><span class="sxs-lookup"><span data-stu-id="4488e-108">Restart your computer when prompted.</span></span>

## <a name="install-your-linux-distribution-of-choice"></a><span data-ttu-id="4488e-109">Ihre Linux-Distribution Ihrer Wahl installieren</span><span class="sxs-lookup"><span data-stu-id="4488e-109">Install your Linux Distribution of Choice</span></span>
<span data-ttu-id="4488e-110">Zum Herunterladen und installieren Ihre bevorzugte Distro(s), haben Sie drei Optionen:</span><span class="sxs-lookup"><span data-stu-id="4488e-110">To download and install your preferred distro(s), you have three choices:</span></span>
1. <span data-ttu-id="4488e-111">Herunterladen und Installieren von den Windows Store (siehe unten)</span><span class="sxs-lookup"><span data-stu-id="4488e-111">Download and install from the Windows Store (see below)</span></span>
1. <span data-ttu-id="4488e-112">Herunterladen und installieren Sie die Befehlszeilenversion-Befehlszeile/Skripts ([lesen Sie die Anweisungen für die manuelle Installation](install-manual.md))</span><span class="sxs-lookup"><span data-stu-id="4488e-112">Download and install from the Command-Line/Script ([read the manual installation instructions](install-manual.md))</span></span>
1. <span data-ttu-id="4488e-113">Herunterladen und manuell zu entpacken und installieren (für Windows Server - [Anleitung](install-on-server.md))</span><span class="sxs-lookup"><span data-stu-id="4488e-113">Download and manually unpack and install (for Windows Server - [instructions here](install-on-server.md))</span></span>

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a><span data-ttu-id="4488e-114">Windows 10 Fall Creators Update und höher: Installieren Sie von den Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="4488e-114">Windows 10 Fall Creators Update and later: Install from the Microsoft Store</span></span>

> <span data-ttu-id="4488e-115">Dieser Abschnitt ist für Windows-Build 16215 oder höher.</span><span class="sxs-lookup"><span data-stu-id="4488e-115">This section is for Windows build 16215 or later.</span></span>  <span data-ttu-id="4488e-116">Führen Sie diese Schritte zum [überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="4488e-116">Follow these steps to [check your build](troubleshooting.md#check-your-build-number).</span></span> 

1. <span data-ttu-id="4488e-117">Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugten Linux-Distribution.</span><span class="sxs-lookup"><span data-stu-id="4488e-117">Open the Microsoft Store and choose your favorite Linux distribution.</span></span>

    ![Anzeigen der Linux-Distributionen im Windows store](media/store.png)

    <span data-ttu-id="4488e-119">Die folgenden Links wird für jede Verteilung der Windows Store-Seite geöffnet:</span><span class="sxs-lookup"><span data-stu-id="4488e-119">The following links will open the Windows store page for each distribution:</span></span>

    * [<span data-ttu-id="4488e-120">Ubuntu 16.04 LTS</span><span class="sxs-lookup"><span data-stu-id="4488e-120">Ubuntu 16.04 LTS</span></span>](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    * [<span data-ttu-id="4488e-121">Ubuntu 18.04 LTS</span><span class="sxs-lookup"><span data-stu-id="4488e-121">Ubuntu 18.04 LTS</span></span>](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    * [<span data-ttu-id="4488e-122">OpenSUSE Leap 15</span><span class="sxs-lookup"><span data-stu-id="4488e-122">OpenSUSE Leap 15</span></span>](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    * [<span data-ttu-id="4488e-123">OpenSUSE Leap 42</span><span class="sxs-lookup"><span data-stu-id="4488e-123">OpenSUSE Leap 42</span></span>](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [<span data-ttu-id="4488e-124">SUSE Linux Enterprise Server 12</span><span class="sxs-lookup"><span data-stu-id="4488e-124">SUSE Linux Enterprise Server 12</span></span>](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [<span data-ttu-id="4488e-125">SUSE Linux Enterprise Server 15</span><span class="sxs-lookup"><span data-stu-id="4488e-125">SUSE Linux Enterprise Server 15</span></span>](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    * [<span data-ttu-id="4488e-126">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="4488e-126">Kali Linux</span></span>](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [<span data-ttu-id="4488e-127">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="4488e-127">Debian GNU/Linux</span></span>](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    * [<span data-ttu-id="4488e-128">Fedora Remix für WSL</span><span class="sxs-lookup"><span data-stu-id="4488e-128">Fedora Remix for WSL</span></span>](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    * [<span data-ttu-id="4488e-129">WLinux</span><span class="sxs-lookup"><span data-stu-id="4488e-129">WLinux</span></span>](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    * [<span data-ttu-id="4488e-130">WLinux Enterprise</span><span class="sxs-lookup"><span data-stu-id="4488e-130">WLinux Enterprise</span></span>](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    * [<span data-ttu-id="4488e-131">Alpine WSL</span><span class="sxs-lookup"><span data-stu-id="4488e-131">Alpine WSL</span></span>](https://www.microsoft.com/store/apps/9p804crf0395)

1. <span data-ttu-id="4488e-132">Die Distribution, die auf der Seite Wählen Sie "Get"</span><span class="sxs-lookup"><span data-stu-id="4488e-132">From the distro's page, select "Get"</span></span>

    ![Anzeigen der Linux-Distributionen im Windows store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a><span data-ttu-id="4488e-134">Initialisierung von Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="4488e-134">Complete initialization of your distro</span></span>
<span data-ttu-id="4488e-135">Nun, da Ihre Linux-Distribution installiert ist, müssen Sie [initialisieren Sie die neue Instanz der Distribution](initialize-distro.md) einmal, bevor sie verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="4488e-135">Now that your Linux distro is installed, you must [initialize your new distro instance](initialize-distro.md) once, before it can be used.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4488e-136">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="4488e-136">Troubleshooting:</span></span> 

<span data-ttu-id="4488e-137">Im folgenden finden Sie zugehörige Fehler und Vorschläge zur Behebung.</span><span class="sxs-lookup"><span data-stu-id="4488e-137">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="4488e-138">Finden Sie in der [WSL Problembehandlungsseite](troubleshooting.md) andere häufig auftretende Fehler und ihre Lösungen.</span><span class="sxs-lookup"><span data-stu-id="4488e-138">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

* <span data-ttu-id="4488e-139">**Fehler 0 x 80070003 bei der Installation**</span><span class="sxs-lookup"><span data-stu-id="4488e-139">**Installation failed with error 0x80070003**</span></span>
    * <span data-ttu-id="4488e-140">Der Windows-Subsystem für Linux nur ausgeführt wird, auf dem Systemlaufwerk (Dies ist normalerweise Ihr `C:` Laufwerk).</span><span class="sxs-lookup"><span data-stu-id="4488e-140">The Windows Subsystem for Linux only runs on your system drive (usually this is your `C:` drive).</span></span> <span data-ttu-id="4488e-141">Stellen Sie sicher, dass Distributionen, die auf dem Systemlaufwerk gespeichert werden:</span><span class="sxs-lookup"><span data-stu-id="4488e-141">Make sure that distros are stored on your system drive:</span></span>  
    * <span data-ttu-id="4488e-142">Open **Einstellungen** -> **Storage** -> **Weitere Einstellungen: Ändern, in dem neuer Inhalt gespeichert wird**
    ![Bild der Systemeinstellungen von apps auf Laufwerk "c:" installieren](media/AppStorage.png)</span><span class="sxs-lookup"><span data-stu-id="4488e-142">Open **Settings** -> **Storage** -> **More Storage Settings: Change where new content is saved**
![Picture of system settings to install apps on C: drive](media/AppStorage.png)</span></span>
    
    
 * <span data-ttu-id="4488e-143">**Fehler bei 0x8007019e WslRegisterDistribution**</span><span class="sxs-lookup"><span data-stu-id="4488e-143">**WslRegisterDistribution failed with error 0x8007019e**</span></span>   
  * <span data-ttu-id="4488e-144">Das Windows-Subsystem für Linux, die optionale Komponente nicht aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="4488e-144">The Windows Subsystem for Linux optional component is not enabled:</span></span> 
   * <span data-ttu-id="4488e-145">Open **Systemsteuerung** -> **Programme und Funktionen** -> \*\* Windows-Features ein- oder ausschalten \*\* Check -> **Windows-Subsystem für Linux** oder mithilfe der PowerShell-Cmdlets, die am Anfang dieses Artikels erwähnt.</span><span class="sxs-lookup"><span data-stu-id="4488e-145">Open **Control Panel** -> **Programs and Features** -> \*\*Turn Windows Feature on or off \*\* -> Check **Windows Subsystem for Linux** or using the PowerShell cmdlet mentioned at the begining of this article.</span></span>
