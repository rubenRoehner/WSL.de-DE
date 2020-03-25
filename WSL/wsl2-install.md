---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 91bd479e922fc29bf11b89dcfe06fa381632c4fa
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520549"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="0e930-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="0e930-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="0e930-105">Sie können sich das Video unten ansehen oder in diesem Artikel weiterlesen, um zu erfahren, wie Sie WSL2 installieren.</span><span class="sxs-lookup"><span data-stu-id="0e930-105">You can watch the video below, or read on in this article to learn how to install WSL2.</span></span> 

> [!VIDEO https://channel9.msdn.com/Blogs/One-Dev-Minute/Learn-how-to-install-WSL-2/player]

<span data-ttu-id="0e930-106">Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:</span><span class="sxs-lookup"><span data-stu-id="0e930-106">To install and start using WSL 2 complete the following steps:</span></span>

> <span data-ttu-id="0e930-107">WSL 2 ist nur in Windows 10-Builds 18917 oder höher verfügbar</span><span class="sxs-lookup"><span data-stu-id="0e930-107">WSL 2 is only available in Windows 10 builds 18917 or higher</span></span>

- <span data-ttu-id="0e930-108">Vergewissern Sie sich, dass Sie WSL installiert haben (Anweisungen dazu finden Sie [hier](./install-win10.md)) und dass Sie Windows 10 **Build 18917** oder höher ausführen</span><span class="sxs-lookup"><span data-stu-id="0e930-108">Ensure that you have WSL installed (you can find instructions to do so [here](./install-win10.md)) and that you are running Windows 10 **build 18917** or higher</span></span>
   - <span data-ttu-id="0e930-109">Um sicherzustellen, dass Sie Build 18917 oder höher verwenden, treten Sie dem [Windows Insider-Programm](https://insider.windows.com/en-us/) bei, und wählen Sie den „Fast Ring“ oder den „Slow Ring“ aus.</span><span class="sxs-lookup"><span data-stu-id="0e930-109">To make sure you are using build 18917 or higher please join [the Windows Insider Program](https://insider.windows.com/en-us/) and select the 'Fast' ring or the 'Slow' ring.</span></span> 
   - <span data-ttu-id="0e930-110">Sie können Ihre Windows-Version überprüfen, indem Sie die Eingabeaufforderung öffnen und den Befehl `ver` ausführen.</span><span class="sxs-lookup"><span data-stu-id="0e930-110">You can check your Windows version by opening Command Prompt and running the `ver` command.</span></span>
- <span data-ttu-id="0e930-111">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="0e930-111">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="0e930-112">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="0e930-112">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="0e930-113">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e930-113">Verify what versions of WSL your distros are using</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a><span data-ttu-id="0e930-114">Aktivieren der optionalen Komponente „Virtual Machine Platform“ und sicherstellen, dass WSL aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="0e930-114">Enable the 'Virtual Machine Platform' optional component and make sure WSL is enabled</span></span>

<span data-ttu-id="0e930-115">Sie müssen sich vergewissern, dass auf Ihrem System die optionalen Komponenten Windows-Subsystem für Linux und Virtual Machine Platform installiert sind.</span><span class="sxs-lookup"><span data-stu-id="0e930-115">You will need to make sure that you have both the Windows Subsystem for Linux and the Virtual Machine Platform optional components installed.</span></span> <span data-ttu-id="0e930-116">Zu diesem Zweck können Sie den folgenden Befehl in PowerShell ausführen:</span><span class="sxs-lookup"><span data-stu-id="0e930-116">You can do that by running the following command in PowerShell:</span></span> 

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

<span data-ttu-id="0e930-117">Starten Sie den Computer neu, um die Installation beider Komponenten abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="0e930-117">Please restart your machine to finish installing both components.</span></span>


## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="0e930-118">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="0e930-118">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="0e930-119">Wenn Sie nicht über eine installierte Linux-Distribution verfügen, finden Sie Anweisungen zum Installieren auf der Seite [Installieren unter Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) der Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="0e930-119">If you do not have a Linux distro installed, please refer to the [Install on Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs page for instructions on installing one.</span></span> 

<span data-ttu-id="0e930-120">Führen Sie Folgendes aus, um eine Distribution festzulegen:</span><span class="sxs-lookup"><span data-stu-id="0e930-120">To set a distro please run:</span></span> 

```
wsl --set-version <Distro> 2
```

<span data-ttu-id="0e930-121">Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="0e930-121">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="0e930-122">(Eine Suche danach ist über diesen Befehl möglich `wsl -l`.)</span><span class="sxs-lookup"><span data-stu-id="0e930-122">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="0e930-123">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="0e930-123">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="0e930-124">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="0e930-124">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

```
wsl --set-default-version 2
```

<span data-ttu-id="0e930-125">Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.</span><span class="sxs-lookup"><span data-stu-id="0e930-125">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="0e930-126">Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e930-126">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="0e930-127">Verwenden Sie den folgenden Befehl, um für jede Distribution die verwendete WSL-Version zu überprüfen (nur in Windows Build 18917 oder höher verfügbar):</span><span class="sxs-lookup"><span data-stu-id="0e930-127">To verify what versions of WSL each distro is using use the following command (only available in Windows Build 18917 or higher):</span></span>

<span data-ttu-id="0e930-128">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="0e930-128">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="0e930-129">Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen.</span><span class="sxs-lookup"><span data-stu-id="0e930-129">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="0e930-130">Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden!</span><span class="sxs-lookup"><span data-stu-id="0e930-130">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="0e930-131">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="0e930-131">Troubleshooting:</span></span> 

<span data-ttu-id="0e930-132">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben.</span><span class="sxs-lookup"><span data-stu-id="0e930-132">Below are related errors and suggested fixes when installing WSL 2.</span></span> <span data-ttu-id="0e930-133">Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="0e930-133">Please refer to the [WSL troubleshooting page](troubleshooting.md) for other general WSL errors and their solutions.</span></span>

* <span data-ttu-id="0e930-134">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="0e930-134">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
    * <span data-ttu-id="0e930-135">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0e930-135">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="0e930-136">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="0e930-136">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>
   
* <span data-ttu-id="0e930-137">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="0e930-137">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
    * <span data-ttu-id="0e930-138">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e930-138">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 18917 or higher.</span></span> <span data-ttu-id="0e930-139">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="0e930-139">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="0e930-140">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="0e930-140">You can find the full WSL install instructions [here](./install-win10.md).</span></span>

* <span data-ttu-id="0e930-141">**Der angeforderte Vorgang konnte aufgrund einer Einschränkung des virtuellen Dateisystems nicht abgeschlossen werden. Dateien für virtuelle Festplatten müssen unkomprimiert und unverschlüsselt sein und dürfen keine geringe Dichte aufweisen.**</span><span class="sxs-lookup"><span data-stu-id="0e930-141">**The requested operation could not be completed due to a virtual disk system limitation. Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.**</span></span>
    * <span data-ttu-id="0e930-142">Bitte prüfen Sie den [WSL Github-Thread #4103](https://github.com/microsoft/WSL/issues/4103), der diesem Thema gewidmet ist, auf aktualisierte Informationen.</span><span class="sxs-lookup"><span data-stu-id="0e930-142">Please check [WSL Github thread #4103](https://github.com/microsoft/WSL/issues/4103) where this issue is being tracked for updated information.</span></span>

* <span data-ttu-id="0e930-143">**Der Ausdruck 'wsl' wurde nicht als Name eines Cmdlets, einer Funktion, einer Skriptdatei oder eines ausführbaren Programms erkannt.**</span><span class="sxs-lookup"><span data-stu-id="0e930-143">**The term 'wsl' is not recognized as the name of a cmdlet, function, script file, or operable program.**</span></span> 
    * <span data-ttu-id="0e930-144">Vergewissern Sie sich, dass die [optionale Komponente Windows-Subsystem für Linux installiert ist](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="0e930-144">Ensure that the [Windows Subsystem for Linux Optional Component is installed](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).</span></span><br> <span data-ttu-id="0e930-145">Außerdem wird dieser Fehler angezeigt, wenn Sie ein Arm64-Gerät verwenden und diesen Befehl aus PowerShell ausführen.</span><span class="sxs-lookup"><span data-stu-id="0e930-145">Additionally, if you are using an Arm64 device and running this command from PowerShell, you will receive this error.</span></span> <span data-ttu-id="0e930-146">Führen Sie stattdessen `wsl.exe` in [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6) oder einer Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="0e930-146">Instead run `wsl.exe` from [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6), or Command Prompt.</span></span> 
