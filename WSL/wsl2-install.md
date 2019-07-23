---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 3ad180ecc9deaa1566e9870700b26f82f631c7f1
ms.sourcegitcommit: 9ad7a54668f39677e9660186e4f5172ea2597e2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2019
ms.locfileid: "68246868"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="06ae2-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="06ae2-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="06ae2-105">Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:</span><span class="sxs-lookup"><span data-stu-id="06ae2-105">To install and start using WSL 2 complete the following steps:</span></span>

- <span data-ttu-id="06ae2-106">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="06ae2-106">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="06ae2-107">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="06ae2-107">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="06ae2-108">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="06ae2-108">Verify what versions of WSL your distros are using</span></span>

<span data-ttu-id="06ae2-109">Beachten Sie, dass zur Verwendung von WSL 2 Windows 10, Build 18917 oder höher benötigt wird. Außerdem muss WSL bereits installiert sein (Anweisungen für die Installation finden Sie [hier](./install-win10.md)).</span><span class="sxs-lookup"><span data-stu-id="06ae2-109">Please note that you'll need to be running Windows 10 build 18917 or higher to use WSL 2, and that you will need to have WSL already installed (you can find instructions to do so [here](./install-win10.md)).</span></span> 

## <a name="enable-the-virtual-machine-platform-optional-component"></a><span data-ttu-id="06ae2-110">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="06ae2-110">Enable the 'Virtual Machine Platform' optional component</span></span>

<span data-ttu-id="06ae2-111">Öffnen Sie PowerShell als Administrator, und führen Sie diesen Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="06ae2-111">Open PowerShell as an Administrator and run:</span></span>

`Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform`

<span data-ttu-id="06ae2-112">Nach der Aktivierung dieser Änderungen müssen Sie Ihren Computer neu starten.</span><span class="sxs-lookup"><span data-stu-id="06ae2-112">After these changes are enabled you will need to restart your computer.</span></span>

## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="06ae2-113">Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.</span><span class="sxs-lookup"><span data-stu-id="06ae2-113">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="06ae2-114">Führen Sie in PowerShell diesen Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="06ae2-114">In PowerShell run:</span></span>

`wsl --set-version <Distro> 2`

<span data-ttu-id="06ae2-115">Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="06ae2-115">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="06ae2-116">(Eine Suche danach ist über diesen Befehl möglich `wsl -l`.)</span><span class="sxs-lookup"><span data-stu-id="06ae2-116">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="06ae2-117">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="06ae2-117">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="06ae2-118">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="06ae2-118">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

`wsl --set-default-version 2`

<span data-ttu-id="06ae2-119">Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.</span><span class="sxs-lookup"><span data-stu-id="06ae2-119">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="06ae2-120">Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.</span><span class="sxs-lookup"><span data-stu-id="06ae2-120">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="06ae2-121">Verwenden Sie den folgenden Befehl, um für jede Distribution die verwendete WSL-Version zu überprüfen:</span><span class="sxs-lookup"><span data-stu-id="06ae2-121">To verify what versions of WSL each distro is using use the following command:</span></span>

<span data-ttu-id="06ae2-122">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="06ae2-122">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="06ae2-123">Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen.</span><span class="sxs-lookup"><span data-stu-id="06ae2-123">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="06ae2-124">Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden!</span><span class="sxs-lookup"><span data-stu-id="06ae2-124">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="06ae2-125">Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="06ae2-125">Troubleshooting:</span></span> 

<span data-ttu-id="06ae2-126">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben.</span><span class="sxs-lookup"><span data-stu-id="06ae2-126">Below are related errors and suggested fixes when installing WSL 2.</span></span> <span data-ttu-id="06ae2-127">Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="06ae2-127">Please refer to the [WSL troubleshooting page](troubleshooting.md) for other general WSL errors and their solutions.</span></span>

* <span data-ttu-id="06ae2-128">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="06ae2-128">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
    * <span data-ttu-id="06ae2-129">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="06ae2-129">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="06ae2-130">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="06ae2-130">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>
   
* <span data-ttu-id="06ae2-131">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="06ae2-131">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
    * <span data-ttu-id="06ae2-132">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="06ae2-132">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 18917 or higher.</span></span> <span data-ttu-id="06ae2-133">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="06ae2-133">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="06ae2-134">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="06ae2-134">You can find the full WSL install instructions [here](./install-win10.md).</span></span>