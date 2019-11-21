---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 8af5ffeffdeedc5298af8125cea5c7428c8f29f8
ms.sourcegitcommit: 3c9ebe5f9ef5fb64070e21b479c2f2d31243f310
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/20/2019
ms.locfileid: "74248766"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="49ec0-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="49ec0-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="49ec0-105">Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:</span><span class="sxs-lookup"><span data-stu-id="49ec0-105">To install and start using WSL 2 complete the following steps:</span></span>

> <span data-ttu-id="49ec0-106">WSL 2 is only available in Windows 10 builds 18917 or higher</span><span class="sxs-lookup"><span data-stu-id="49ec0-106">WSL 2 is only available in Windows 10 builds 18917 or higher</span></span>

- <span data-ttu-id="49ec0-107">Ensure that you have WSL installed (you can find instructions to do so [here](./install-win10.md)) and that you are running Windows 10 **build 18917** or higher</span><span class="sxs-lookup"><span data-stu-id="49ec0-107">Ensure that you have WSL installed (you can find instructions to do so [here](./install-win10.md)) and that you are running Windows 10 **build 18917** or higher</span></span>
   - <span data-ttu-id="49ec0-108">To make sure you are using build 18917 or higher please join [the Windows Insider Program](https://insider.windows.com/en-us/) and select the 'Fast' ring.</span><span class="sxs-lookup"><span data-stu-id="49ec0-108">To make sure you are using build 18917 or higher please join [the Windows Insider Program](https://insider.windows.com/en-us/) and select the 'Fast' ring.</span></span> 
   - <span data-ttu-id="49ec0-109">You can check your Windows version by opening Command Prompt and running the `ver` command.</span><span class="sxs-lookup"><span data-stu-id="49ec0-109">You can check your Windows version by opening Command Prompt and running the `ver` command.</span></span>
- <span data-ttu-id="49ec0-110">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="49ec0-110">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="49ec0-111">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="49ec0-111">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="49ec0-112">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="49ec0-112">Verify what versions of WSL your distros are using</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a><span data-ttu-id="49ec0-113">Enable the 'Virtual Machine Platform' optional component and make sure WSL is enabled</span><span class="sxs-lookup"><span data-stu-id="49ec0-113">Enable the 'Virtual Machine Platform' optional component and make sure WSL is enabled</span></span>

<span data-ttu-id="49ec0-114">You will need to make sure that you have both the Windows Subsystem for Linux and the Virtual Machine Platform optional components installed.</span><span class="sxs-lookup"><span data-stu-id="49ec0-114">You will need to make sure that you have both the Windows Subsystem for Linux and the Virtual Machine Platform optional components installed.</span></span> <span data-ttu-id="49ec0-115">You can do that by running the following command in PowerShell:</span><span class="sxs-lookup"><span data-stu-id="49ec0-115">You can do that by running the following command in PowerShell:</span></span> 

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

<span data-ttu-id="49ec0-116">Please restart your machine to finish installing both components.</span><span class="sxs-lookup"><span data-stu-id="49ec0-116">Please restart your machine to finish installing both components.</span></span>


## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="49ec0-117">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="49ec0-117">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="49ec0-118">If you do not have a Linux distro installed, please refer to the [Install on Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs page for instructions on installing one.</span><span class="sxs-lookup"><span data-stu-id="49ec0-118">If you do not have a Linux distro installed, please refer to the [Install on Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs page for instructions on installing one.</span></span> 

<span data-ttu-id="49ec0-119">To set a distro please run:</span><span class="sxs-lookup"><span data-stu-id="49ec0-119">To set a distro please run:</span></span> 

```
wsl --set-version <Distro> 2
```

<span data-ttu-id="49ec0-120">Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="49ec0-120">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="49ec0-121">(Eine Suche danach ist über diesen Befehl möglich `wsl -l`.)</span><span class="sxs-lookup"><span data-stu-id="49ec0-121">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="49ec0-122">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="49ec0-122">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="49ec0-123">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="49ec0-123">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

```
wsl --set-default-version 2`
```

<span data-ttu-id="49ec0-124">Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.</span><span class="sxs-lookup"><span data-stu-id="49ec0-124">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="49ec0-125">Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="49ec0-125">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="49ec0-126">To verify what versions of WSL each distro is using use the following command (only available in Windows Build 18917 or higher):</span><span class="sxs-lookup"><span data-stu-id="49ec0-126">To verify what versions of WSL each distro is using use the following command (only available in Windows Build 18917 or higher):</span></span>

<span data-ttu-id="49ec0-127">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="49ec0-127">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="49ec0-128">Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen.</span><span class="sxs-lookup"><span data-stu-id="49ec0-128">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="49ec0-129">Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden!</span><span class="sxs-lookup"><span data-stu-id="49ec0-129">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="49ec0-130">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="49ec0-130">Troubleshooting:</span></span> 

<span data-ttu-id="49ec0-131">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben.</span><span class="sxs-lookup"><span data-stu-id="49ec0-131">Below are related errors and suggested fixes when installing WSL 2.</span></span> <span data-ttu-id="49ec0-132">Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="49ec0-132">Please refer to the [WSL troubleshooting page](troubleshooting.md) for other general WSL errors and their solutions.</span></span>

* <span data-ttu-id="49ec0-133">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="49ec0-133">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
    * <span data-ttu-id="49ec0-134">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="49ec0-134">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="49ec0-135">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="49ec0-135">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>
   
* <span data-ttu-id="49ec0-136">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="49ec0-136">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
    * <span data-ttu-id="49ec0-137">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="49ec0-137">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 18917 or higher.</span></span> <span data-ttu-id="49ec0-138">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="49ec0-138">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="49ec0-139">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="49ec0-139">You can find the full WSL install instructions [here](./install-win10.md).</span></span>

* <span data-ttu-id="49ec0-140">**The requested operation could not be completed due to a virtual disk system limitation. Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.**</span><span class="sxs-lookup"><span data-stu-id="49ec0-140">**The requested operation could not be completed due to a virtual disk system limitation. Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.**</span></span>
    * <span data-ttu-id="49ec0-141">Please check [WSL Github thread #4103](https://github.com/microsoft/WSL/issues/4103) where this issue is being tracked for updated information.</span><span class="sxs-lookup"><span data-stu-id="49ec0-141">Please check [WSL Github thread #4103](https://github.com/microsoft/WSL/issues/4103) where this issue is being tracked for updated information.</span></span>

* <span data-ttu-id="49ec0-142">**The term 'wsl' is not recognized as the name of a cmdlet, function, script file, or operable program.**</span><span class="sxs-lookup"><span data-stu-id="49ec0-142">**The term 'wsl' is not recognized as the name of a cmdlet, function, script file, or operable program.**</span></span> 
    * <span data-ttu-id="49ec0-143">Ensure that the [Windows Subsystem for Linux Optional Component is installed](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="49ec0-143">Ensure that the [Windows Subsystem for Linux Optional Component is installed](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).</span></span><br> <span data-ttu-id="49ec0-144">Additionally, if you are using an Arm64 device and running this command from PowerShell, you will receive this error.</span><span class="sxs-lookup"><span data-stu-id="49ec0-144">Additionally, if you are using an Arm64 device and running this command from PowerShell, you will receive this error.</span></span> <span data-ttu-id="49ec0-145">Instead run `wsl.exe` from [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6), or Command Prompt.</span><span class="sxs-lookup"><span data-stu-id="49ec0-145">Instead run `wsl.exe` from [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6), or Command Prompt.</span></span> 