---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: Installieren Sie BashOnWindows, Bash, Wsl, wsl2, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 2af43a046333fc8c7b4142cdc5077cdfbf29fea7
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67038080"
---
# <a name="installation-instructions-for-wsl-2"></a><span data-ttu-id="28b06-104">Installationsanweisungen für WSL 2</span><span class="sxs-lookup"><span data-stu-id="28b06-104">Installation Instructions for WSL 2</span></span>

<span data-ttu-id="28b06-105">Führen Sie zum Installieren und nutzen Sie WSL 2 die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="28b06-105">To install and start using WSL 2 complete the following steps:</span></span>

- <span data-ttu-id="28b06-106">Aktivieren Sie die "VM-Plattform" optionale Komponente</span><span class="sxs-lookup"><span data-stu-id="28b06-106">Enable the 'Virtual Machine Platform' optional component</span></span>
- <span data-ttu-id="28b06-107">Legen Sie eine Distribution, die durch die WSL-2, die über die Befehlszeile unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="28b06-107">Set a distro to be backed by WSL 2 using the command line</span></span>
- <span data-ttu-id="28b06-108">Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden</span><span class="sxs-lookup"><span data-stu-id="28b06-108">Verify what versions of WSL your distros are using</span></span>

## <a name="enable-the-virtual-machine-platform-optional-component"></a><span data-ttu-id="28b06-109">Aktivieren Sie die "VM-Plattform" optionale Komponente</span><span class="sxs-lookup"><span data-stu-id="28b06-109">Enable the 'Virtual Machine Platform' optional component</span></span>

<span data-ttu-id="28b06-110">Öffnen Sie PowerShell als Administrator, und führen Sie aus:</span><span class="sxs-lookup"><span data-stu-id="28b06-110">Open PowerShell as an Administrator and run:</span></span>

`Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform`

<span data-ttu-id="28b06-111">Nachdem diese Änderungen aktiviert sind, müssen Sie den Computer neu starten.</span><span class="sxs-lookup"><span data-stu-id="28b06-111">After these changes are enabled you will need to restart your computer.</span></span>

## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a><span data-ttu-id="28b06-112">Legen Sie eine Distribution, die durch die WSL-2, die über die Befehlszeile unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="28b06-112">Set a distro to be backed by WSL 2 using the command line</span></span>

<span data-ttu-id="28b06-113">In PowerShell ausführen:</span><span class="sxs-lookup"><span data-stu-id="28b06-113">In PowerShell run:</span></span>

`wsl --set-version <Distro> 2`

<span data-ttu-id="28b06-114">und achten Sie darauf, ersetzen Sie dies `<Distro>` durch den tatsächlichen Namen von Ihrer Distribution.</span><span class="sxs-lookup"><span data-stu-id="28b06-114">and make sure to replace `<Distro>` with the actual name of your distro.</span></span> <span data-ttu-id="28b06-115">(Sie finden diese mit dem Befehl: `wsl -l`).</span><span class="sxs-lookup"><span data-stu-id="28b06-115">(You can find these with the command: `wsl -l`).</span></span> <span data-ttu-id="28b06-116">Sie können an WSL 1 auf jederzeit ändern, indem den gleichen Befehl wie oben ausführen, aber ersetzen die "2" mit "1".</span><span class="sxs-lookup"><span data-stu-id="28b06-116">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="28b06-117">Darüber hinaus sollten Sie WSL 2 Stellen Sie die Standardarchitektur können Sie mit diesem Befehl dafür:</span><span class="sxs-lookup"><span data-stu-id="28b06-117">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

`wsl --set-default-version 2`

<span data-ttu-id="28b06-118">Dies veranlasst alle neuen-Distribution, die Sie installieren, als eine Distribution WSL 2 initialisiert.</span><span class="sxs-lookup"><span data-stu-id="28b06-118">This will make any new distro that you install be initialized as a WSL 2 distro.</span></span>

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a><span data-ttu-id="28b06-119">Beim Überprüfen, welche Versionen von WSL Ihre Distribution verwenden, sind abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="28b06-119">Finish with verifying what versions of WSL your distro are using</span></span>

<span data-ttu-id="28b06-120">So überprüfen, welche Versionen von WSL jede Distribution verwendet den folgenden Befehl verwenden:</span><span class="sxs-lookup"><span data-stu-id="28b06-120">To verify what versions of WSL each distro is using use the following command:</span></span>

<span data-ttu-id="28b06-121">`wsl --list --verbose` oder `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="28b06-121">`wsl --list --verbose` or `wsl -l -v`</span></span>

<span data-ttu-id="28b06-122">Die Distribution, der Sie oben ausgewählt haben, sollte nun eine "2" in der Spalte "Version" anzeigen.</span><span class="sxs-lookup"><span data-stu-id="28b06-122">The distro that you've chosen above should now display a '2' under the 'version' column.</span></span> <span data-ttu-id="28b06-123">Nun, da Sie danach können Sie beim Einstieg in Ihre WSL-2-Distribution!</span><span class="sxs-lookup"><span data-stu-id="28b06-123">Now that you're finished feel free to start using your WSL 2 distro!</span></span> 