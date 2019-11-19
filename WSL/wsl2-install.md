---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 91994f3a075436c022acb9dadeea072142687b72
ms.sourcegitcommit: cf6d8e277ed3102f8f879b9f39ba0966d4ea6135
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/18/2019
ms.locfileid: "74164343"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="6bc78-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="6bc78-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="6bc78-105">Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:</span><span class="sxs-lookup"><span data-stu-id="6bc78-105">To install and start using WSL 2 complete the following steps:</span></span>

> <span data-ttu-id="6bc78-106">WSL 2 ist nur in Windows 10-Builds 18917 oder höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6bc78-106">WSL 2 is only available in Windows 10 builds 18917 or higher</span></span>

- <span data-ttu-id="6bc78-107">Stellen Sie sicher, dass WSL installiert ist ( [hier](./install-win10.md)finden Sie entsprechende Anweisungen) und dass Windows 10 **Build 18917** oder höher ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="6bc78-107">Ensure that you have WSL installed (you can find instructions to do so [here](./install-win10.md)) and that you are running Windows 10 **build 18917** or higher</span></span>
   - <span data-ttu-id="6bc78-108">Um sicherzustellen, dass Sie Build 18917 oder höher verwenden, fügen Sie [das Windows Insider-Programm](https://insider.windows.com/en-us/) an, und wählen Sie den Ring "fast" aus.</span><span class="sxs-lookup"><span data-stu-id="6bc78-108">To make sure you are using build 18917 or higher please join [the Windows Insider Program](https://insider.windows.com/en-us/) and select the 'Fast' ring.</span></span> 
   - <span data-ttu-id="6bc78-109">Sie können Ihre Windows-Version überprüfen, indem Sie die Eingabeaufforderung öffnen und den Befehl `ver` ausführen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-109">You can check your Windows version by opening Command Prompt and running the `ver` command.</span></span>
- <span data-ttu-id="6bc78-110">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="6bc78-110">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="6bc78-111">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="6bc78-111">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="6bc78-112">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="6bc78-112">Verify what versions of WSL your distros are using</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a><span data-ttu-id="6bc78-113">Aktivieren Sie die optionale Komponente "Virtual Machine Platform", und stellen Sie sicher, dass WSL aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6bc78-113">Enable the 'Virtual Machine Platform' optional component and make sure WSL is enabled</span></span>

<span data-ttu-id="6bc78-114">Öffnen Sie PowerShell als Administrator, und führen Sie den folgenden Befehl aus, um die Komponente "Virtual Machine Platform" zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6bc78-114">To enable the 'Virtual Machine Platform' component open PowerShell as an administrator and run the command below.</span></span> <span data-ttu-id="6bc78-115">Wenn Sie WSL zum ersten Mal installieren, wählen Sie "Nein" aus, wenn Sie zur Eingabe eines Neustarts aufgefordert werden, da Sie den Computer nach der Installation der optionalen Komponente "Windows-Subsystem für Linux" trotzdem neu starten müssen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-115">If you are installing WSL for the first time then select 'No' when prompted for a restart, as you will need to restart your machine anyway after installing the 'Windows Subsystem for Linux' optional component.</span></span>

```powershell
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
```

<span data-ttu-id="6bc78-116">Außerdem müssen Sie sicherstellen, dass die optionale Komponente des Windows-Subsystems für Linux aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6bc78-116">You will also need to make sure that the Windows Subsystem for Linux optional component is enabled.</span></span> <span data-ttu-id="6bc78-117">Hierzu können Sie den folgenden Befehl in einem PowerShell-Fenster mit Administratorrechten ausführen:</span><span class="sxs-lookup"><span data-stu-id="6bc78-117">You can do this by running the following command from a PowerShell window with administrator privileges:</span></span> 

```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

<span data-ttu-id="6bc78-118">Starten Sie den Computer neu, um die Installation beider Komponenten abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-118">Please restart your machine to finish installing both components.</span></span>


## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="6bc78-119">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="6bc78-119">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="6bc78-120">Wenn Sie nicht über eine installierte Linux-Distribution verfügen, finden Sie unter [Installieren auf der Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs-Seite Anweisungen zur Installation.</span><span class="sxs-lookup"><span data-stu-id="6bc78-120">If you do not have a Linux distro installed, please refer to the [Install on Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs page for instructions on installing one.</span></span> 

<span data-ttu-id="6bc78-121">Führen Sie in PowerShell diesen Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="6bc78-121">In PowerShell run:</span></span>

`wsl --set-version <Distro> 2`

<span data-ttu-id="6bc78-122">Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="6bc78-122">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="6bc78-123">(Eine Suche danach ist über diesen Befehl möglich `wsl -l`.)</span><span class="sxs-lookup"><span data-stu-id="6bc78-123">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="6bc78-124">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-124">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="6bc78-125">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="6bc78-125">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

`wsl --set-default-version 2`

<span data-ttu-id="6bc78-126">Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.</span><span class="sxs-lookup"><span data-stu-id="6bc78-126">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="6bc78-127">Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="6bc78-127">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="6bc78-128">Verwenden Sie den folgenden Befehl, um zu überprüfen, welche Versionen von WSL für jede Distribution verwendet werden (nur verfügbar in Windows Build 18917 oder höher):</span><span class="sxs-lookup"><span data-stu-id="6bc78-128">To verify what versions of WSL each distro is using use the following command (only available in Windows Build 18917 or higher):</span></span>

<span data-ttu-id="6bc78-129">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="6bc78-129">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="6bc78-130">Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-130">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="6bc78-131">Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden!</span><span class="sxs-lookup"><span data-stu-id="6bc78-131">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="6bc78-132">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="6bc78-132">Troubleshooting:</span></span> 

<span data-ttu-id="6bc78-133">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben.</span><span class="sxs-lookup"><span data-stu-id="6bc78-133">Below are related errors and suggested fixes when installing WSL 2.</span></span> <span data-ttu-id="6bc78-134">Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="6bc78-134">Please refer to the [WSL troubleshooting page](troubleshooting.md) for other general WSL errors and their solutions.</span></span>

* <span data-ttu-id="6bc78-135">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="6bc78-135">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
    * <span data-ttu-id="6bc78-136">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6bc78-136">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="6bc78-137">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="6bc78-137">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>
   
* <span data-ttu-id="6bc78-138">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="6bc78-138">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
    * <span data-ttu-id="6bc78-139">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="6bc78-139">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 18917 or higher.</span></span> <span data-ttu-id="6bc78-140">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="6bc78-140">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="6bc78-141">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="6bc78-141">You can find the full WSL install instructions [here](./install-win10.md).</span></span>

* <span data-ttu-id="6bc78-142">**Der angeforderte Vorgang konnte aufgrund einer Einschränkung des virtuellen Festplattensystems nicht abgeschlossen werden. Dateien für virtuelle Festplatten müssen unkomprimiert und unverschlüsselt sein und dürfen nicht mit geringer Dichte sein.**</span><span class="sxs-lookup"><span data-stu-id="6bc78-142">**The requested operation could not be completed due to a virtual disk system limitation. Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.**</span></span>
    * <span data-ttu-id="6bc78-143">Überprüfen Sie den [WSL-GitHub-Thread #4103](https://github.com/microsoft/WSL/issues/4103) , in dem dieses Problem nach aktualisierten Informationen nachverfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="6bc78-143">Please check [WSL Github thread #4103](https://github.com/microsoft/WSL/issues/4103) where this issue is being tracked for updated information.</span></span>