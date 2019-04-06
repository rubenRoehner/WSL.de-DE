---
title: Installieren Sie Windows-Subsystem für Linux (WSL) auf unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: Installieren Sie BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 40bbe73acbfd0483e18ab6ff1696fdb44eaff2e4
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063288"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a><span data-ttu-id="d7e9b-104">Windows-Subsystem für Linux – Installationsleitfaden für Windows 10</span><span class="sxs-lookup"><span data-stu-id="d7e9b-104">Windows Subsystem for Linux Installation Guide for Windows 10</span></span>

## <a name="install-the-windows-subsystem-for-linux"></a><span data-ttu-id="d7e9b-105">Installieren Sie das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="d7e9b-105">Install the Windows Subsystem for Linux</span></span>

<span data-ttu-id="d7e9b-106">Vor der Installation alle Linux-Distributionen für WSL, müssen Sie sicherstellen, dass die "Windows-Subsystem für Linux" optionales Feature aktiviert ist:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-106">Before installing any Linux distros for WSL, you must ensure that the "Windows Subsystem for Linux" optional feature is enabled:</span></span>

1. <span data-ttu-id="d7e9b-107">Öffnen Sie PowerShell als Administrator, und führen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-107">Open PowerShell as Administrator and run:</span></span>
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. <span data-ttu-id="d7e9b-108">Starten Sie Ihre Computer bei entsprechender Aufforderung neu.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-108">Restart your computer when prompted.</span></span>

## <a name="install-your-linux-distribution-of-choice"></a><span data-ttu-id="d7e9b-109">Ihre Linux-Distribution Ihrer Wahl installieren</span><span class="sxs-lookup"><span data-stu-id="d7e9b-109">Install your Linux Distribution of Choice</span></span>
<span data-ttu-id="d7e9b-110">Zum Herunterladen und installieren Ihre bevorzugte Distro(s), haben Sie drei Optionen:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-110">To download and install your preferred distro(s), you have three choices:</span></span>
1. <span data-ttu-id="d7e9b-111">Herunterladen und Installieren von den Windows Store (siehe unten)</span><span class="sxs-lookup"><span data-stu-id="d7e9b-111">Download and install from the Windows Store (see below)</span></span>
1. <span data-ttu-id="d7e9b-112">Herunterladen und installieren Sie die Befehlszeilenversion-Befehlszeile/Skripts ([lesen Sie die Anweisungen für die manuelle Installation](install-manual.md))</span><span class="sxs-lookup"><span data-stu-id="d7e9b-112">Download and install from the Command-Line/Script ([read the manual installation instructions](install-manual.md))</span></span>
1. <span data-ttu-id="d7e9b-113">Herunterladen und manuell zu entpacken und installieren (für Windows Server - [Anleitung](install-on-server.md))</span><span class="sxs-lookup"><span data-stu-id="d7e9b-113">Download and manually unpack and install (for Windows Server - [instructions here](install-on-server.md))</span></span>

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a><span data-ttu-id="d7e9b-114">Windows 10 Fall Creators Update und höher: Installieren Sie von den Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="d7e9b-114">Windows 10 Fall Creators Update and later: Install from the Microsoft Store</span></span>

> <span data-ttu-id="d7e9b-115">Dieser Abschnitt ist für Windows-Build 16215 oder höher.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-115">This section is for Windows build 16215 or later.</span></span>  <span data-ttu-id="d7e9b-116">Führen Sie diese Schritte zum [überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="d7e9b-116">Follow these steps to [check your build](troubleshooting.md#check-your-build-number).</span></span> 

1. <span data-ttu-id="d7e9b-117">Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugten Linux-Distribution.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-117">Open the Microsoft Store and choose your favorite Linux distribution.</span></span>

    ![Anzeigen der Linux-Distributionen im Windows store](media/store.png)

    <span data-ttu-id="d7e9b-119">Die folgenden Links wird für jede Verteilung der Windows Store-Seite geöffnet:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-119">The following links will open the Windows store page for each distribution:</span></span>

    * [<span data-ttu-id="d7e9b-120">Ubuntu</span><span class="sxs-lookup"><span data-stu-id="d7e9b-120">Ubuntu</span></span>](https://www.microsoft.com/store/p/ubuntu/9nblggh4msv6)
    * [<span data-ttu-id="d7e9b-121">OpenSUSE</span><span class="sxs-lookup"><span data-stu-id="d7e9b-121">OpenSUSE</span></span>](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [<span data-ttu-id="d7e9b-122">SLES</span><span class="sxs-lookup"><span data-stu-id="d7e9b-122">SLES</span></span>](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [<span data-ttu-id="d7e9b-123">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="d7e9b-123">Kali Linux</span></span>](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [<span data-ttu-id="d7e9b-124">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="d7e9b-124">Debian GNU/Linux</span></span>](https://www.microsoft.com/store/apps/9MSVKQC78PK6)

1. <span data-ttu-id="d7e9b-125">Die Distribution, die auf der Seite Wählen Sie "Get"</span><span class="sxs-lookup"><span data-stu-id="d7e9b-125">From the distro's page, select "Get"</span></span>

    ![Anzeigen der Linux-Distributionen im Windows store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a><span data-ttu-id="d7e9b-127">Initialisierung von Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="d7e9b-127">Complete initialization of your distro</span></span>
<span data-ttu-id="d7e9b-128">Nun, da Ihre Linux-Distribution installiert ist, müssen Sie [initialisieren Sie die neue Instanz der Distribution](initialize-distro.md) einmal, bevor sie verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-128">Now that your Linux distro is installed, you must [initialize your new distro instance](initialize-distro.md) once, before it can be used.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d7e9b-129">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-129">Troubleshooting:</span></span> 

<span data-ttu-id="d7e9b-130">Im folgenden finden Sie zugehörige Fehler und Vorschläge zur Behebung.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-130">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="d7e9b-131">Finden Sie in der [WSL Problembehandlungsseite](troubleshooting.md) andere häufig auftretende Fehler und ihre Lösungen.</span><span class="sxs-lookup"><span data-stu-id="d7e9b-131">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

* **<span data-ttu-id="d7e9b-132">Fehler 0 x 80070003 bei der Installation</span><span class="sxs-lookup"><span data-stu-id="d7e9b-132">Installation failed with error 0x80070003</span></span>**
    * <span data-ttu-id="d7e9b-133">Der Windows-Subsystem für Linux nur ausgeführt wird, auf dem Systemlaufwerk (Dies ist normalerweise Ihr `C:` Laufwerk).</span><span class="sxs-lookup"><span data-stu-id="d7e9b-133">The Windows Subsystem for Linux only runs on your system drive (usually this is your `C:` drive).</span></span> <span data-ttu-id="d7e9b-134">Stellen Sie sicher, dass Distributionen, die auf dem Systemlaufwerk gespeichert werden:</span><span class="sxs-lookup"><span data-stu-id="d7e9b-134">Make sure that distros are stored on your system drive:</span></span>  
    * <span data-ttu-id="d7e9b-135">Open **Einstellungen** -> **Storage** -> **Weitere Einstellungen: Ändern, in dem neuer Inhalt gespeichert wird**
    ![Bild der Systemeinstellungen von apps auf Laufwerk "c:" installieren](media/AppStorage.png)</span><span class="sxs-lookup"><span data-stu-id="d7e9b-135">Open **Settings** -> **Storage** -> **More Storage Settings: Change where new content is saved**
![Picture of system settings to install apps on C: drive](media/AppStorage.png)</span></span>
