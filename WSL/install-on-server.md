---
title: Installieren Sie das Subsystem für Linux unter WindowsServer
description: Installationsanweisungen für das Linux-Subsystem unter Windows Server.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu und WindowsServer
author: scooley
ms.author: scooley
ms.date: 05/22/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: c0b8af08a06428ebd292b8c6b9b275726988bdbe
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59063618"
---
# <a name="windows-server-installation-guide"></a><span data-ttu-id="1cae8-104">Windows Server-Installationshandbuch</span><span class="sxs-lookup"><span data-stu-id="1cae8-104">Windows Server Installation Guide</span></span>

> <span data-ttu-id="1cae8-105">Gilt für Windows Server-2019 und höher</span><span class="sxs-lookup"><span data-stu-id="1cae8-105">Applies to Windows Server 2019 and later</span></span>

<span data-ttu-id="1cae8-106">Auf / / Build2017, Microsoft hat angekündigt, dass Windows-Subsystem für Linux ist [unter Windows Server verfügbaren](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/).</span><span class="sxs-lookup"><span data-stu-id="1cae8-106">At //Build2017, Microsoft announced that Windows Subsystem for Linux will be [available on Windows Server](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/).</span></span>  <span data-ttu-id="1cae8-107">Diese Anweisungen erläutert, die das Windows-Subsystem für Linux unter Windows Server 1709 und höher ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="1cae8-107">These instructions walk through running the Windows Subsystem for Linux on Windows Server 1709 and later.</span></span>

## <a name="enable-the-windows-subsystem-for-linux-wsl"></a><span data-ttu-id="1cae8-108">Aktivieren Sie das Windows-Subsystem für Linux (WSL)</span><span class="sxs-lookup"><span data-stu-id="1cae8-108">Enable the Windows Subsystem for Linux (WSL)</span></span>

<span data-ttu-id="1cae8-109">Vor dem Ausführen von Linux-Distributionen für Windows müssen Sie die optionale Funktion von "Windows-Subsystem für Linux" aktivieren und neu starten.</span><span class="sxs-lookup"><span data-stu-id="1cae8-109">Before you can run Linux distros on Windows, you must enable the "Windows Subsystem for Linux" optional feature and reboot.</span></span>

1. <span data-ttu-id="1cae8-110">Öffnen Sie PowerShell als Administrator, und führen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="1cae8-110">Open PowerShell as Administrator and run:</span></span>
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. <span data-ttu-id="1cae8-111">Starten Sie Ihre Computer bei entsprechender Aufforderung neu.</span><span class="sxs-lookup"><span data-stu-id="1cae8-111">Restart your computer when prompted.</span></span> <span data-ttu-id="1cae8-112">**Dieser Neustart ist erforderlich,** um sicherzustellen, dass es sich bei eine vertrauenswürdigen ausführungsumgebung WSL initiiert werden kann.</span><span class="sxs-lookup"><span data-stu-id="1cae8-112">**This reboot is required** in order to ensure that WSL can initiate a trusted execution environment.</span></span>

## <a name="download-a-linux-distro"></a><span data-ttu-id="1cae8-113">Laden Sie eine Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="1cae8-113">Download a Linux distro</span></span>

<span data-ttu-id="1cae8-114">Führen Sie [diese Anweisungen](install-manual.md) , Ihre bevorzugten Linux-Distribution herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="1cae8-114">Follow [these instructions](install-manual.md) to download your favorite Linux distribution.</span></span>

## <a name="extract-and-install-a-linux-distro"></a><span data-ttu-id="1cae8-115">Extrahieren Sie und installieren Sie eine Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="1cae8-115">Extract and install a Linux distro</span></span>
<span data-ttu-id="1cae8-116">Nun, da Sie eine Distribution heruntergeladen haben, extrahieren Sie den Inhalt, und installieren Sie manuell die Distribution:</span><span class="sxs-lookup"><span data-stu-id="1cae8-116">Now that you've downloaded a distro, extract its contents and manually install the distro:</span></span>

1. <span data-ttu-id="1cae8-117">Extrahieren Sie die `<distro>.appx` Inhalt des Pakets, z. B. mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1cae8-117">Extract the `<distro>.appx` package's contents, e.g. using PowerShell:</span></span>

    ```powershell
    Rename-Item ~/Ubuntu.appx ~/Ubuntu.zip
    Expand-Archive ~/Ubuntu.zip ~/Ubuntu
    ```

2. <span data-ttu-id="1cae8-118">Führen Sie das Startprogramm-Distribution, die Installation abzuschließen, führen Sie die Distribution-Startprogramm-Anwendung im Zielordner, mit dem Namen `<distro>.exe`.</span><span class="sxs-lookup"><span data-stu-id="1cae8-118">Run the distro launcher To complete installation, run the distro launcher application in the target folder, named `<distro>.exe`.</span></span> <span data-ttu-id="1cae8-119">Zum Beispiel: `ubuntu.exe`usw.</span><span class="sxs-lookup"><span data-stu-id="1cae8-119">For example: `ubuntu.exe`, etc.</span></span>

    ![Erweiterte Distribution von Ubuntu unter Windows Server](media/server-appx-expand.png)

    > <span data-ttu-id="1cae8-121">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="1cae8-121">**Troubleshooting**</span></span>
    > * <span data-ttu-id="1cae8-122">**Fehler bei der Installation Fehler 0x8007007e**: Dieser Fehler tritt auf, wenn Ihr System WSL nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1cae8-122">**Installation failed with error 0x8007007e**: This error occurs when your system doesn't support WSL.</span></span> <span data-ttu-id="1cae8-123">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="1cae8-123">Make sure that:</span></span>
    >   * <span data-ttu-id="1cae8-124">Sie können Windows Build 16215 oder höher ausführen.</span><span class="sxs-lookup"><span data-stu-id="1cae8-124">You're running Windows build 16215 or later.</span></span> <span data-ttu-id="1cae8-125">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="1cae8-125">[Check your build](troubleshooting.md#check-your-build-number).</span></span>
    >   * <span data-ttu-id="1cae8-126">Das Windows-Subsystem für Linux optionale Komponente aktiviert ist, und der Computer neu gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="1cae8-126">The Windows Subsystem for Linux optional component is enabled and the computer has restarted.</span></span>  <span data-ttu-id="1cae8-127">[WSL aktiviert](troubleshooting.md#confirm-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="1cae8-127">[Make sure WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled).</span></span>
    
3. <span data-ttu-id="1cae8-128">Hinzufügen von Ihrem Pfad-Distribution, die in der Windows-Umgebung Pfad (`C:\Users\Administrator\Ubuntu` in diesem Beispiel), z. B. mithilfe von Powershell:</span><span class="sxs-lookup"><span data-stu-id="1cae8-128">Add your distro path to the Windows environment PATH (`C:\Users\Administrator\Ubuntu` in this example), e.g. using Powershell:</span></span>
        
    ```powershell
    $userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
    [System.Environment]::SetEnvironmentVariable("PATH", $userenv + "C:\Users\Administrator\Ubuntu", "User")
    ```
    <span data-ttu-id="1cae8-129">Sie können jetzt Ihre Distribution von jedem beliebigen Pfad starten, indem Sie eingeben `<distro>.exe`.</span><span class="sxs-lookup"><span data-stu-id="1cae8-129">You can now launch your distro from any path by typing `<distro>.exe`.</span></span> <span data-ttu-id="1cae8-130">Beispiel: `ubuntu.exe`</span><span class="sxs-lookup"><span data-stu-id="1cae8-130">For example: `ubuntu.exe`</span></span>

<span data-ttu-id="1cae8-131">Nun, da Ihre Linux-Distribution installiert ist, müssen Sie [initialisieren Sie die neue Instanz der Distribution](initialize-distro.md) vor der Verwendung von Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="1cae8-131">Now that your Linux distro is installed, you must [initialize your new distro instance](initialize-distro.md) before using your distro.</span></span>
