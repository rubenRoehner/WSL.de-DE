---
title: Erstellen Sie eine benutzerdefinierte Linux-Distribution für WSL
description: Erfahren Sie, wie eine benutzerdefinierte Linux-Distribution für Windows-Subsystem für Linux zu erstellen.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem, -Distribution, Benutzerdefiniert
author: taraj
ms.author: taraj
ms.date: 03/27/2018
ms.topic: article
ms.assetid: a5095219-0c82-4ce5-9a6d-5c2fc00835a3
ms.custom: seodec18
ms.openlocfilehash: b98101c19d7d450548531521c3f8ee15ce62f9f1
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59063258"
---
# <a name="creating-a-custom-linux-distro-for-wsl"></a><span data-ttu-id="2f499-104">Erstellen eine benutzerdefinierte Linux-Distribution für WSL</span><span class="sxs-lookup"><span data-stu-id="2f499-104">Creating a Custom Linux Distro for WSL</span></span>

<span data-ttu-id="2f499-105">Verwenden Sie unsere open-Source WSL-Beispiel, das Erstellen von Paketen für WSL-Distribution, die für den Microsoft Store und/oder zum Erstellen von benutzerdefinierten Linux-Distribution, die Pakete für das querladen.</span><span class="sxs-lookup"><span data-stu-id="2f499-105">Use our open source WSL sample to build WSL distro packages for the Microsoft Store and/or to create custom Linux distro packages for sideloading.</span></span> <span data-ttu-id="2f499-106">Sie finden die [Distribution Startprogramm Repository](https://github.com/Microsoft/WSL-DistroLauncher) auf GitHub.</span><span class="sxs-lookup"><span data-stu-id="2f499-106">You can find the [distro launcher repo](https://github.com/Microsoft/WSL-DistroLauncher) on GitHub.</span></span>

<span data-ttu-id="2f499-107">Dieses Projekt ermöglicht:</span><span class="sxs-lookup"><span data-stu-id="2f499-107">This project enables:</span></span>
* <span data-ttu-id="2f499-108">Linux-Verteilung Verwalter zu packen und senden eine Linux-Distribution als eine AppX-Datei, die für WSL ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2f499-108">Linux distribution maintainers to package and submit a Linux distribution as an appx that runs on WSL</span></span>
* <span data-ttu-id="2f499-109">Entwicklern das Erstellen von benutzerdefinierter Linux-Distributionen, die auf ihrem Entwicklungscomputer sein können</span><span class="sxs-lookup"><span data-stu-id="2f499-109">Developers to create custom Linux distributions that can be sideloaded onto their dev machine</span></span>

## <a name="background"></a><span data-ttu-id="2f499-110">Hintergrund</span><span class="sxs-lookup"><span data-stu-id="2f499-110">Background</span></span>
<span data-ttu-id="2f499-111">Wir verteilen als UWP-Anwendungen über den Microsoft Store-Linux-Distributionen für WSL.</span><span class="sxs-lookup"><span data-stu-id="2f499-111">We distribute Linux distros for WSL as UWP applications through the Microsoft Store.</span></span> <span data-ttu-id="2f499-112">Sie können diese Anwendungen installieren, die dann für WSL - das Subsystem ausgeführt wird, die sich im Windows-Kernel befindet.</span><span class="sxs-lookup"><span data-stu-id="2f499-112">You can install those applications that will then run on WSL - the subsystem that sits in the Windows kernel.</span></span> <span data-ttu-id="2f499-113">Dieser Mechanismus hat viele Vorteile, wie in einem früheren Blogbeitrag beschrieben.</span><span class="sxs-lookup"><span data-stu-id="2f499-113">This delivery mechanism has many benefits as discussed in an earlier blog post.</span></span>

## <a name="sideloading-a-custom-linux-distro-package"></a><span data-ttu-id="2f499-114">Querladen eines benutzerdefinierten virtuellen Linux-Distribution-Pakets</span><span class="sxs-lookup"><span data-stu-id="2f499-114">Sideloading a Custom Linux Distro Package</span></span>
<span data-ttu-id="2f499-115">Sie können ein benutzerdefiniertes Paket von Linux-Distribution, die als eine Anwendung zum Sideloaden auf Ihr persönlicher Computer erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f499-115">You can create a custom Linux distro package as an application to sideload on your personal machine.</span></span> <span data-ttu-id="2f499-116">Bitte beachten Sie, dass das benutzerdefinierte Paket nicht über den Microsoft Store verteilt werden würde, es sei denn, Sie Maintainer Verteilung übermitteln.</span><span class="sxs-lookup"><span data-stu-id="2f499-116">Please note that your custom package would not be distributed through the Microsoft Store unless you submit as a distribution maintainer.</span></span>
<span data-ttu-id="2f499-117">Zum Einrichten von Ihrem Computers, Apps querzuladen, müssen Sie dies in den Systemeinstellungen, unter "Für Entwickler" zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="2f499-117">To set up your machine to sideload apps, you will need to enable this in the system settings under “For Developers”.</span></span>  <span data-ttu-id="2f499-118">Achten Sie darauf, dass Sie entweder den Entwicklermodus oder querladen von apps ausgewählt haben</span><span class="sxs-lookup"><span data-stu-id="2f499-118">Be sure to either have developer mode, or sideload apps selected</span></span>

## <a name="for-linux-distro-maintainers"></a><span data-ttu-id="2f499-119">Für die Verwalter von Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="2f499-119">For Linux Distro Maintainers</span></span>
<span data-ttu-id="2f499-120">Um an den Store übermitteln, müssen Sie die Arbeit mit uns auf die Genehmigung zur Veröffentlichung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="2f499-120">To submit to the Store, you will need to work with us to receive publishing approval.</span></span> <span data-ttu-id="2f499-121">Wenn Sie interessiert, Hinzufügen von Ihrer Distribution zu den Microsoft Store-Besitzer einer Linux-Verteilung sind, wenden Sie sich an wslpartners@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="2f499-121">If you are a Linux distribution owner interested in adding your distribution to the Microsoft Store, please contact wslpartners@microsoft.com.</span></span>

## <a name="getting-started"></a><span data-ttu-id="2f499-122">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="2f499-122">Getting Started</span></span>
<span data-ttu-id="2f499-123">Befolgen Sie die Anweisungen auf der [Distribution Startprogramm-GitHub-Repository](https://github.com/Microsoft/WSL-DistroLauncher) zum Erstellen eines benutzerdefinierten Linux-Distribution-Pakets.</span><span class="sxs-lookup"><span data-stu-id="2f499-123">Follow the instructions on the [Distro Launcher GitHub repo](https://github.com/Microsoft/WSL-DistroLauncher) to create a custom Linux distro package.</span></span>

 
## <a name="team-blogs"></a><span data-ttu-id="2f499-124">Team-Blogs</span><span class="sxs-lookup"><span data-stu-id="2f499-124">Team Blogs</span></span>
*  [<span data-ttu-id="2f499-125">Öffnen Sie ein Beispiel für WSL-Sourcing für die Verwalter von Linux-Verteilung und Querladen benutzerdefinierte Linux-Distributionen</span><span class="sxs-lookup"><span data-stu-id="2f499-125">Open Sourcing a WSL Sample for Linux Distribution Maintainers and Sideloading Custom Linux Distributions</span></span>](https://blogs.msdn.microsoft.com/commandline/2018/03/26/wsl-distro-launcher/)
* [<span data-ttu-id="2f499-126">Befehlszeilen-blog</span><span class="sxs-lookup"><span data-stu-id="2f499-126">Command-Line blog</span></span>](https://blogs.msdn.microsoft.com/commandline/)

## <a name="provide-feedback"></a><span data-ttu-id="2f499-127">Senden von Feedback</span><span class="sxs-lookup"><span data-stu-id="2f499-127">Provide Feedback</span></span>
* [<span data-ttu-id="2f499-128">Repository der Distribution-Startprogramm Gitub</span><span class="sxs-lookup"><span data-stu-id="2f499-128">Distro Launcher Gitub repo</span></span>](https://github.com/Microsoft/WSL-DistroLauncher)
* [<span data-ttu-id="2f499-129">GitHub-problemverfolgung für WSL</span><span class="sxs-lookup"><span data-stu-id="2f499-129">GitHub issue tracker for WSL</span></span>](https://github.com/Microsoft/BashOnWindows/issues)
* [<span data-ttu-id="2f499-130">Befehlszeile UserVoice-portal</span><span class="sxs-lookup"><span data-stu-id="2f499-130">Command-line UserVoice portal</span></span>](https://wpdev.uservoice.com/forums/266908-command-prompt-console-bash-on-ubuntu-on-windo/category/161892-bash)
