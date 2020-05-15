---
title: Installieren des Linux-Subsystems unter Windows Server
description: Installationsanweisungen für das Linux-Subsystem unter Windows Server.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, windows server
ms.date: 05/12/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: 86fd7de0ef45af760f46bb2a18932f513b813609
ms.sourcegitcommit: 1b6191351bbf9e95f3c28fc67abe4bf1bcfd3336
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83270884"
---
# <a name="windows-server-installation-guide"></a><span data-ttu-id="c06c3-104">Windows Server-Installationsleitfaden</span><span class="sxs-lookup"><span data-stu-id="c06c3-104">Windows Server Installation Guide</span></span>

<span data-ttu-id="c06c3-105">Das Windows-Subsystem für Linux ist für die Installation unter Windows Server 2019 (Version 1709) und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c06c3-105">The Windows Subsystem for Linux is available for installation on Windows Server 2019 (version 1709) and later.</span></span> <span data-ttu-id="c06c3-106">Diese Anleitung führt Sie durch die Schritte zum Aktivieren von WSL auf Ihrem Computer.</span><span class="sxs-lookup"><span data-stu-id="c06c3-106">This guide will walk through the steps of enabling WSL on your machine.</span></span>

## <a name="enable-the-windows-subsystem-for-linux"></a><span data-ttu-id="c06c3-107">Aktivieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="c06c3-107">Enable the Windows Subsystem for Linux</span></span>

<span data-ttu-id="c06c3-108">Damit Sie Linux-Distributionen unter Windows ausführen können, müssen Sie das optionale Feature „Windows-Subsystem für Linux“ aktivieren und das System neu starten.</span><span class="sxs-lookup"><span data-stu-id="c06c3-108">Before you can run Linux distros on Windows, you must enable the "Windows Subsystem for Linux" optional feature and reboot.</span></span>

<span data-ttu-id="c06c3-109">Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="c06c3-109">Open PowerShell as Administrator and run:</span></span>

```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

```

<span data-ttu-id="c06c3-110">**Wenn Sie 100%ige Systemaufruf-Kompatibilität und schnellere E/A-Leistung suchen, lesen Sie die unten stehenden Informationen zur Installation von WSL 2.**</span><span class="sxs-lookup"><span data-stu-id="c06c3-110">**If you're looking for 100% system call compatibility and faster IO performance, read below to install WSL 2!**</span></span>

<span data-ttu-id="c06c3-111">WSL 2 ist nur in Windows 10, Version 2004, Build 19041 oder höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c06c3-111">WSL 2 is only available in Windows 10, Version 2004, Build 19041 or higher.</span></span> <span data-ttu-id="c06c3-112">Sie müssen [Ihre Windows-Version aktualisieren](ms-settings:windowsupdate), dem [Windows Insider-Programm beitreten](https://insider.windows.com/insidersigninboth/) und am „Release Preview“-Ring teilnehmen, bis die öffentliche Version Ende Mai verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="c06c3-112">You will need to [update your Windows version](ms-settings:windowsupdate) and [join the Windows Insider program](https://insider.windows.com/insidersigninboth/) on the "Release Preview" ring until the public release in late May.</span></span>

<span data-ttu-id="c06c3-113">**Falls Sie mit WSL 1 fortfahren, starten Sie Ihren Rechner neu, wenn Sie dazu aufgefordert werden, und setzen Sie die Installation [hier](./install-on-server.md#download-a-linux-distribution) fort.**</span><span class="sxs-lookup"><span data-stu-id="c06c3-113">**If continuing with WSL 1, restart your machine when prompted and continue with installation [here](./install-on-server.md#download-a-linux-distribution)**</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component"></a><span data-ttu-id="c06c3-114">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="c06c3-114">Enable the Virtual Machine Platform optional component</span></span>

<span data-ttu-id="c06c3-115">Stellen Sie sicher, dass die optionale Komponente „Virtual Machine Platform“ installiert ist.</span><span class="sxs-lookup"><span data-stu-id="c06c3-115">Ensure the 'Virtual Machine Platform' optional component is installed.</span></span> <span data-ttu-id="c06c3-116">Zu diesem Zweck können Sie den folgenden Befehl in PowerShell ausführen:</span><span class="sxs-lookup"><span data-stu-id="c06c3-116">You can do that by running the following command in PowerShell:</span></span>

```powershell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

## <a name="download-a-linux-distribution"></a><span data-ttu-id="c06c3-117">Herunterladen einer Linux-Verteilung</span><span class="sxs-lookup"><span data-stu-id="c06c3-117">Download a Linux distribution</span></span>

<span data-ttu-id="c06c3-118">Befolgen Sie [diese Anweisungen](install-manual.md), um Ihre bevorzugte Linux-Distribution herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="c06c3-118">Follow [these instructions](install-manual.md) to download your favorite Linux distribution.</span></span>

## <a name="extract-and-install-a-linux-distribution"></a><span data-ttu-id="c06c3-119">Extrahieren und Installieren einer Linux-Verteilung</span><span class="sxs-lookup"><span data-stu-id="c06c3-119">Extract and install a Linux distribution</span></span>

<span data-ttu-id="c06c3-120">Nachdem Sie nun eine Linux-Verteilung heruntergeladen haben, um ihren Inhalt zu extrahieren und manuell zu installieren, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="c06c3-120">Now that you've downloaded a Linux distribution, in order to extract its contents and manually install, follow these steps:</span></span>

1. <span data-ttu-id="c06c3-121">Extrahieren Sie den Inhalt des `<distro>.appx`-Pakets mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c06c3-121">Extract the `<distro>.appx` package's contents, using PowerShell:</span></span>

    ```powershell
    Rename-Item .\Ubuntu.appx .\Ubuntu.zip
    Expand-Archive .\Ubuntu.zip .\Ubuntu
    ```

2. <span data-ttu-id="c06c3-122">Führen Sie die Startanwendung der Verteilung im Zielordner aus.</span><span class="sxs-lookup"><span data-stu-id="c06c3-122">Run the distribution launcher application in the target folder.</span></span> <span data-ttu-id="c06c3-123">Die Startanwendung heißt normalerweise `<distro>.exe` (z. B. `ubuntu.exe`).</span><span class="sxs-lookup"><span data-stu-id="c06c3-123">The launcher is typically named `<distro>.exe` (for example, `ubuntu.exe`).</span></span>

    ![Aufgeklappte Ubuntu-Distribution unter Windows Server](media/server-appx-expand.png)

> [!CAUTION]
> <span data-ttu-id="c06c3-125">**Installation failed with error 0x8007007e** (Installationsfehler mit Fehlercode 0x8007007e): Sie erhalten diesen Fehler, wenn das System WSL nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c06c3-125">**Installation failed with error 0x8007007e**: If you receive this error, then your system doesn't support WSL.</span></span> <span data-ttu-id="c06c3-126">Stellen Sie sicher, dass Sie Windows-Build 16215 oder höher aus führen.</span><span class="sxs-lookup"><span data-stu-id="c06c3-126">Ensure that you're running Windows build 16215 or later.</span></span> <span data-ttu-id="c06c3-127">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="c06c3-127">[Check your build](troubleshooting.md#check-your-build-number).</span></span> <span data-ttu-id="c06c3-128">[Vergewissern Sie sich auch, dass die WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled) und Ihr Computer neu gestartet wurde, nachdem das Feature aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="c06c3-128">Also check to [confirm that WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled) and your computer was restarted after the feature was enabled.</span></span>  

<span data-ttu-id="c06c3-129">3. Fügen Sie der Windows-Umgebungsvariablen PATH den Pfad der Verteilung hinzu (in diesem Beispiel `C:\Users\Administrator\Ubuntu`), mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c06c3-129">3.Add your distro path to the Windows environment PATH (`C:\Users\Administrator\Ubuntu` in this example), using PowerShell:</span></span>

```powershell
$userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
[System.Environment]::SetEnvironmentVariable("PATH", $userenv + ";C:\Users\Administrator\Ubuntu", "User")
```

<span data-ttu-id="c06c3-130">Sie können Ihre Verteilung nun über einen beliebigen Pfad starten, indem Sie `<distro>.exe`eingeben.</span><span class="sxs-lookup"><span data-stu-id="c06c3-130">You can now launch your distribution from any path by typing `<distro>.exe`.</span></span> <span data-ttu-id="c06c3-131">Beispiel: `ubuntu.exe`.</span><span class="sxs-lookup"><span data-stu-id="c06c3-131">For example: `ubuntu.exe`.</span></span>

<span data-ttu-id="c06c3-132">Nachdem der Installation müssen Sie [Ihre neue Verteilungsinstanz initialisieren](initialize-distro.md), bevor Sie sie verwenden.</span><span class="sxs-lookup"><span data-stu-id="c06c3-132">Now that it is installed, you must [initialize your new distribution instance](initialize-distro.md) before using it.</span></span>
