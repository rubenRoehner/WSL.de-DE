---
title: Aktualisieren des WSL 2-Linux-Kernels
description: Anweisungen zum manuellen Aktualisieren Ihres WSL 2 Linux-Kernels
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
ms.date: 03/12/2020
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: edc7ea35d8ebe0c71488763017cde2bb45c53b6d
ms.sourcegitcommit: 8795e1c4c5d2efdc8a9c78af05fb7be3ac1eef3d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/12/2020
ms.locfileid: "79138189"
---
# <a name="updating-the-wsl-2-linux-kernel"></a><span data-ttu-id="06266-104">Aktualisieren des WSL 2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="06266-104">Updating the WSL 2 Linux kernel</span></span>

<span data-ttu-id="06266-105">Führen Sie die folgenden Schritte aus, um den Linux-Kernel innerhalb von WSL 2 manuell zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="06266-105">To manually update the Linux kernel inside of WSL 2 please follow these steps.</span></span> 

## <a name="download-the-linux-kernel-update-package"></a><span data-ttu-id="06266-106">Herunterladen des Linux-Kernel Update Pakets</span><span class="sxs-lookup"><span data-stu-id="06266-106">Download the Linux kernel update package</span></span>

<span data-ttu-id="06266-107">Klicken Sie auf [diesen Link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) , um das neueste WSL2 Linux Kernel Update Package for amd64 Machines herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="06266-107">Please click on [this link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) to download the latest WSL2 Linux kernel update package for AMD64 machines.</span></span>

> [!NOTE] <span data-ttu-id="06266-108">Wenn Sie einen ARM64-Computer verwenden, müssen Sie [Dieses Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) stattdessen herunterladen.</span><span class="sxs-lookup"><span data-stu-id="06266-108">if you're using an ARM64 machine, please download [this package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) instead.</span></span>

## <a name="install-the-linux-kernel-update-package"></a><span data-ttu-id="06266-109">Installieren des Linux-Kernel Update Pakets</span><span class="sxs-lookup"><span data-stu-id="06266-109">Install the Linux kernel update package</span></span>

<span data-ttu-id="06266-110">So installieren Sie das Linux-Kernel Update Paket:</span><span class="sxs-lookup"><span data-stu-id="06266-110">To install the Linux kernel update package:</span></span>
    1. <span data-ttu-id="06266-111">Führen Sie das im vorherigen Schritt heruntergeladene Update Paket aus.</span><span class="sxs-lookup"><span data-stu-id="06266-111">Run the update package downloaded in the previous step.</span></span>
    2. <span data-ttu-id="06266-112">Wenn Sie aufgefordert werden, erweiterte Berechtigungen zu erhalten, wählen Sie "Ja", um diese Installation zu genehmigen.</span><span class="sxs-lookup"><span data-stu-id="06266-112">You will be prompted for elevated permissions, select ‘yes’ to approve this installation.</span></span>
    3. <span data-ttu-id="06266-113">Nachdem die Installation abgeschlossen ist, können Sie mit der Verwendung von WSL2 beginnen!</span><span class="sxs-lookup"><span data-stu-id="06266-113">Once the installation is complete, you are ready to begin using WSL2!</span></span>

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a><span data-ttu-id="06266-114">Zukünftige Pläne zum Aktualisieren des WSL2 Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="06266-114">Future plans for updating the WSL2 Linux kernel</span></span>

<span data-ttu-id="06266-115">Weitere Informationen zu diesen Änderungen finden Sie in [diesem Blogbeitrag](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im Windows- [befehlszeilenblog](https://aka.ms/cliblog).</span><span class="sxs-lookup"><span data-stu-id="06266-115">For more info on these changes, please read [this blog post](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) on the [Windows Command Line Blog](https://aka.ms/cliblog).</span></span>