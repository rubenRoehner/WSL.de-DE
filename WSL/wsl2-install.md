---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 386b6793f00300bc9dabd1613cfd69b19d222f0b
ms.sourcegitcommit: eb7b572388c6bddbf6e8ad8d01927660fe66aecf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2019
ms.locfileid: "71692464"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="a5fa0-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="a5fa0-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="a5fa0-105">Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:</span><span class="sxs-lookup"><span data-stu-id="a5fa0-105">To install and start using WSL 2 complete the following steps:</span></span>

> <span data-ttu-id="a5fa0-106">WSL 2 ist nur in Windows 10-Builds 18917 oder höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-106">WSL 2 is only available in Windows 10 builds 18917 or higher</span></span>

- <span data-ttu-id="a5fa0-107">Stellen Sie sicher, dass WSL installiert ist ( [hier](./install-win10.md)finden Sie entsprechende Anweisungen) und dass Windows 10 **Build 18917** oder höher ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-107">Ensure that you have WSL installed (you can find instructions to do so [here](./install-win10.md)) and that you are running Windows 10 **build 18917** or higher</span></span>
   - <span data-ttu-id="a5fa0-108">Um sicherzustellen, dass Sie Build 18917 oder höher verwenden, fügen Sie [das Windows Insider-Programm](https://insider.windows.com/en-us/) an, und wählen Sie den Ring "fast" aus.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-108">To make sure you are using build 18917 or higher please join [the Windows Insider Program](https://insider.windows.com/en-us/) and select the 'Fast' ring.</span></span> 
   - <span data-ttu-id="a5fa0-109">Sie können Ihre Windows-Version überprüfen, indem Sie die Eingabe `ver` Aufforderung öffnen und den Befehl ausführen.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-109">You can check your Windows version by opening Command Prompt and running the `ver` command.</span></span>
- <span data-ttu-id="a5fa0-110">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-110">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="a5fa0-111">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-111">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="a5fa0-112">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-112">Verify what versions of WSL your distros are using</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a><span data-ttu-id="a5fa0-113">Aktivieren Sie die optionale Komponente "Virtual Machine Platform", und stellen Sie sicher, dass WSL aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-113">Enable the 'Virtual Machine Platform' optional component and make sure WSL is enabled</span></span>

<span data-ttu-id="a5fa0-114">Öffnen Sie PowerShell als Administrator, und führen Sie diesen Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="a5fa0-114">Open PowerShell as an Administrator and run:</span></span>

```powershell
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

<span data-ttu-id="a5fa0-115">Dadurch wird sichergestellt, dass sowohl die Plattform für virtuelle Computer als auch das Windows-Subsystem für Linux optionale Komponenten installiert sind.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-115">This will make sure that both the Virtual Machine Platform and Windows Subsystem for Linux optional components are installed.</span></span> <span data-ttu-id="a5fa0-116">Nachdem Sie diese Befehle ausgeführt haben, müssen Sie den Computer neu starten.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-116">After you've run these commands you'll need to restart your computer.</span></span> 

## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="a5fa0-117">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-117">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="a5fa0-118">Führen Sie in PowerShell diesen Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="a5fa0-118">In PowerShell run:</span></span>

`wsl --set-version <Distro> 2`

<span data-ttu-id="a5fa0-119">Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-119">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="a5fa0-120">(Eine Suche danach ist über diesen Befehl möglich `wsl -l`.)</span><span class="sxs-lookup"><span data-stu-id="a5fa0-120">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="a5fa0-121">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-121">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="a5fa0-122">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="a5fa0-122">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

`wsl --set-default-version 2`

<span data-ttu-id="a5fa0-123">Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-123">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="a5fa0-124">Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-124">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="a5fa0-125">Verwenden Sie den folgenden Befehl, um zu überprüfen, welche Versionen von WSL für jede Distribution verwendet werden (nur verfügbar in Windows Build 18917 oder höher):</span><span class="sxs-lookup"><span data-stu-id="a5fa0-125">To verify what versions of WSL each distro is using use the following command (only available in Windows Build 18917 or higher):</span></span>

<span data-ttu-id="a5fa0-126">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="a5fa0-126">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="a5fa0-127">Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-127">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="a5fa0-128">Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden!</span><span class="sxs-lookup"><span data-stu-id="a5fa0-128">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="a5fa0-129">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="a5fa0-129">Troubleshooting:</span></span> 

<span data-ttu-id="a5fa0-130">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-130">Below are related errors and suggested fixes when installing WSL 2.</span></span> <span data-ttu-id="a5fa0-131">Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="a5fa0-131">Please refer to the [WSL troubleshooting page](troubleshooting.md) for other general WSL errors and their solutions.</span></span>

* <span data-ttu-id="a5fa0-132">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="a5fa0-132">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
    * <span data-ttu-id="a5fa0-133">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-133">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="a5fa0-134">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-134">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>
   
* <span data-ttu-id="a5fa0-135">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="a5fa0-135">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
    * <span data-ttu-id="a5fa0-136">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-136">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 18917 or higher.</span></span> <span data-ttu-id="a5fa0-137">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="a5fa0-137">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="a5fa0-138">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="a5fa0-138">You can find the full WSL install instructions [here](./install-win10.md).</span></span>