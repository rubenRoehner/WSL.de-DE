---
title: Aktualisieren des WSL2-Linux-Kernels
description: Anweisungen zum manuellen Aktualisieren Ihres WSL2-Linux-Kernels
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
ms.date: 03/12/2020
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.localizationpriority: high
ms.custom: seodec18
ms.openlocfilehash: a1a2f23fb05c426f80878e12e82026a96c71354e
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "79447743"
---
# <a name="updating-the-wsl-2-linux-kernel"></a><span data-ttu-id="14956-104">Aktualisieren des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="14956-104">Updating the WSL 2 Linux kernel</span></span>

<span data-ttu-id="14956-105">Um den Linux-Kernel innerhalb von WSL2 manuell zu aktualisieren, führen Sie die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="14956-105">To manually update the Linux kernel inside of WSL 2 please follow these steps.</span></span> 

## <a name="download-the-linux-kernel-update-package"></a><span data-ttu-id="14956-106">Herunterladen des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="14956-106">Download the Linux kernel update package</span></span>

<span data-ttu-id="14956-107">Klicken Sie auf [diesen Link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi), um das neueste Updatepaket für den WSL2-Linux-Kernel für x64-Computer herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="14956-107">Please click on [this link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) to download the latest WSL2 Linux kernel update package for x64 machines.</span></span>

> [!NOTE] 
> <span data-ttu-id="14956-108">Wenn Sie einen ARM64-Computer verwenden, laden Sie stattdessen [dieses Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) herunter.</span><span class="sxs-lookup"><span data-stu-id="14956-108">If you're using an ARM64 machine, please download [this package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) instead.</span></span>

## <a name="install-the-linux-kernel-update-package"></a><span data-ttu-id="14956-109">Installieren des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="14956-109">Install the Linux kernel update package</span></span>

<span data-ttu-id="14956-110">So installieren Sie das Updatepaket für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="14956-110">To install the Linux kernel update package:</span></span>

    1. <span data-ttu-id="14956-111">Führen Sie das im vorherigen Schritt heruntergeladene Updatepaket aus.</span><span class="sxs-lookup"><span data-stu-id="14956-111">Run the update package downloaded in the previous step.</span></span>
    2. <span data-ttu-id="14956-112">Sie werden zur Eingabe erhöhter Berechtigungen aufgefordert. Wählen Sie „Ja“, um diese Installation zu genehmigen.</span><span class="sxs-lookup"><span data-stu-id="14956-112">You will be prompted for elevated permissions, select ‘yes’ to approve this installation.</span></span>
    3. <span data-ttu-id="14956-113">Sobald die Installation abgeschlossen ist, können Sie mit der Nutzung von WSL2 beginnen!</span><span class="sxs-lookup"><span data-stu-id="14956-113">Once the installation is complete, you are ready to begin using WSL2!</span></span>

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a><span data-ttu-id="14956-114">Zukünftige Pläne zur Aktualisierung des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="14956-114">Future plans for updating the WSL2 Linux kernel</span></span>

<span data-ttu-id="14956-115">Weitere Informationen über diese Änderungen finden Sie in [diesem Blogbeitrag](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im [Blog zur Windows-Befehlszeile](https://aka.ms/cliblog).</span><span class="sxs-lookup"><span data-stu-id="14956-115">For more info on these changes, please read [this blog post](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) on the [Windows Command Line Blog](https://aka.ms/cliblog).</span></span>
