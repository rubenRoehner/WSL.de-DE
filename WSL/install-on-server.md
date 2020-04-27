---
title: Installieren des Linux-Subsystems unter Windows Server
description: Installationsanweisungen für das Linux-Subsystem unter Windows Server.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, windows server
ms.date: 05/22/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 8859929fe45c9989d367af5f82191162963e6b4f
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "80256393"
---
# <a name="windows-server-installation-guide"></a><span data-ttu-id="2eabf-104">Windows Server-Installationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="2eabf-104">Windows Server Installation Guide</span></span>

> <span data-ttu-id="2eabf-105">Gilt für Windows Server 2019 und höher</span><span class="sxs-lookup"><span data-stu-id="2eabf-105">Applies to Windows Server 2019 and later</span></span>

<span data-ttu-id="2eabf-106">Auf der //Build2017 kündigte Microsoft an, dass das Windows-Subsystem für Linux [für Windows Server verfügbar](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/) sein wird.</span><span class="sxs-lookup"><span data-stu-id="2eabf-106">At //Build2017, Microsoft announced that Windows Subsystem for Linux will be [available on Windows Server](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/).</span></span>  <span data-ttu-id="2eabf-107">Diese Anweisungen führen Sie durch die Ausführung des Windows-Subsystems für Linux unter Windows Server 1709 und höher.</span><span class="sxs-lookup"><span data-stu-id="2eabf-107">These instructions walk through running the Windows Subsystem for Linux on Windows Server 1709 and later.</span></span>

## <a name="enable-the-windows-subsystem-for-linux-wsl"></a><span data-ttu-id="2eabf-108">Aktivieren des Windows-Subsystems für Linux (WSL)</span><span class="sxs-lookup"><span data-stu-id="2eabf-108">Enable the Windows Subsystem for Linux (WSL)</span></span>

<span data-ttu-id="2eabf-109">Damit Sie Linux-Distributionen unter Windows ausführen können, müssen Sie das optionale Feature „Windows-Subsystem für Linux“ aktivieren und das System neu starten.</span><span class="sxs-lookup"><span data-stu-id="2eabf-109">Before you can run Linux distros on Windows, you must enable the "Windows Subsystem for Linux" optional feature and reboot.</span></span>

1. <span data-ttu-id="2eabf-110">Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="2eabf-110">Open PowerShell as Administrator and run:</span></span>
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. <span data-ttu-id="2eabf-111">Starten Sie den Computer neu, wenn Sie dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="2eabf-111">Restart your computer when prompted.</span></span> <span data-ttu-id="2eabf-112">**Dieser Neustart ist erforderlich**, um sicherzustellen, dass WSL eine vertrauenswürdige Ausführungsumgebung initiieren kann.</span><span class="sxs-lookup"><span data-stu-id="2eabf-112">**This reboot is required** in order to ensure that WSL can initiate a trusted execution environment.</span></span>

## <a name="download-a-linux-distro"></a><span data-ttu-id="2eabf-113">Herunterladen einer Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="2eabf-113">Download a Linux distro</span></span>

<span data-ttu-id="2eabf-114">Befolgen Sie [diese Anweisungen](install-manual.md), um Ihre bevorzugte Linux-Distribution herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="2eabf-114">Follow [these instructions](install-manual.md) to download your favorite Linux distribution.</span></span>

## <a name="extract-and-install-a-linux-distro"></a><span data-ttu-id="2eabf-115">Extrahieren und Installieren einer Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="2eabf-115">Extract and install a Linux distro</span></span>
<span data-ttu-id="2eabf-116">Nachdem Sie nun eine Distribution heruntergeladen haben, extrahieren Sie den Inhalt, und installieren Sie die Distribution manuell:</span><span class="sxs-lookup"><span data-stu-id="2eabf-116">Now that you've downloaded a distro, extract its contents and manually install the distro:</span></span>

1. <span data-ttu-id="2eabf-117">Extrahieren Sie den Inhalt des `<distro>.appx`-Pakets, z. B. mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2eabf-117">Extract the `<distro>.appx` package's contents, e.g. using PowerShell:</span></span>

    ```powershell
    Rename-Item .\Ubuntu.appx .\Ubuntu.zip
    Expand-Archive .\Ubuntu.zip .\Ubuntu
    ```

2. <span data-ttu-id="2eabf-118">Ausführen des Startprogramms der Distribution Um die Installation abzuschließen, führen Sie die Startanwendung mit dem Namen `<distro>.exe` im Zielordner aus.</span><span class="sxs-lookup"><span data-stu-id="2eabf-118">Run the distro launcher To complete installation, run the distro launcher application in the target folder, named `<distro>.exe`.</span></span> <span data-ttu-id="2eabf-119">Beispiel: `ubuntu.exe` usw.</span><span class="sxs-lookup"><span data-stu-id="2eabf-119">For example: `ubuntu.exe`, etc.</span></span>

    ![Aufgeklappte Ubuntu-Distribution unter Windows Server](media/server-appx-expand.png)

    > <span data-ttu-id="2eabf-121">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="2eabf-121">**Troubleshooting**</span></span>
    > * <span data-ttu-id="2eabf-122">**Installation failed with error 0x8007007e** (Installationsfehler mit Fehlercode 0x8007007e): Dieser Fehler tritt auf, wenn das System WSL nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2eabf-122">**Installation failed with error 0x8007007e**: This error occurs when your system doesn't support WSL.</span></span> <span data-ttu-id="2eabf-123">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="2eabf-123">Make sure that:</span></span>
    >   * <span data-ttu-id="2eabf-124">Sie führen Windows-Build 16215 oder höher aus.</span><span class="sxs-lookup"><span data-stu-id="2eabf-124">You're running Windows build 16215 or later.</span></span> <span data-ttu-id="2eabf-125">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="2eabf-125">[Check your build](troubleshooting.md#check-your-build-number).</span></span>
    >   * <span data-ttu-id="2eabf-126">Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.</span><span class="sxs-lookup"><span data-stu-id="2eabf-126">The Windows Subsystem for Linux optional component is enabled and the computer has restarted.</span></span>  <span data-ttu-id="2eabf-127">[Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="2eabf-127">[Make sure WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled).</span></span>
    
3. <span data-ttu-id="2eabf-128">Fügen Sie der Windows-Umgebungsvariablen PATH den Pfad der Distribution hinzu (in diesem Beispiel `C:\Users\Administrator\Ubuntu`), beispielsweise mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2eabf-128">Add your distro path to the Windows environment PATH (`C:\Users\Administrator\Ubuntu` in this example), e.g. using Powershell:</span></span>
        
    ```powershell
    $userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
    [System.Environment]::SetEnvironmentVariable("PATH", $userenv + ";C:\Users\Administrator\Ubuntu", "User")
    ```
    <span data-ttu-id="2eabf-129">Sie können Ihre Distribution nun über einen beliebigen Pfad starten, indem Sie `<distro>.exe`eingeben.</span><span class="sxs-lookup"><span data-stu-id="2eabf-129">You can now launch your distro from any path by typing `<distro>.exe`.</span></span> <span data-ttu-id="2eabf-130">Beispiel: `ubuntu.exe`</span><span class="sxs-lookup"><span data-stu-id="2eabf-130">For example: `ubuntu.exe`</span></span>

<span data-ttu-id="2eabf-131">Nachdem Sie Ihre Linux-Distribution installiert haben, müssen Sie [Ihre neue Distributionsinstanz initialisieren](initialize-distro.md), bevor Sie sie verwenden.</span><span class="sxs-lookup"><span data-stu-id="2eabf-131">Now that your Linux distro is installed, you must [initialize your new distro instance](initialize-distro.md) before using your distro.</span></span>
