---
title: Aktualisieren des WSL2-Linux-Kernels
description: Anweisungen zum manuellen Aktualisieren Ihres WSL2-Linux-Kernels
keywords: WSL, Windows, Linux-Kernel, Windows-Subsystem für Linux, Kernel
ms.date: 03/12/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: 1628bea2f1bae590928b055425413e5b085dffef
ms.sourcegitcommit: 90f7caeefe886bf6c0ba2b90c1b56b5f9795ad1b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/28/2020
ms.locfileid: "84153049"
---
# <a name="updating-the-wsl-2-linux-kernel"></a><span data-ttu-id="6f7d7-104">Aktualisieren des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="6f7d7-104">Updating the WSL 2 Linux kernel</span></span>

<span data-ttu-id="6f7d7-105">Um den Linux-Kernel innerhalb von WSL2 manuell zu aktualisieren, führen Sie die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="6f7d7-105">To manually update the Linux kernel inside of WSL 2 please follow these steps.</span></span>

> [!NOTE] 
> <span data-ttu-id="6f7d7-106">Wenn das Installationsprogramm WSL 1 nicht finden kann, klicken Sie mit der rechten Maustaste auf das Installationsprogramm für das Linux-Kernel-Update, wählen Sie „Deinstallieren“ aus, und starten Sie das Installationsprogramm erneut.</span><span class="sxs-lookup"><span data-stu-id="6f7d7-106">If the installer can't find WSL 1, right-click the Linux kernel update installer and press "Uninstall", then rerun the installer.</span></span>

## <a name="download-the-linux-kernel-update-package"></a><span data-ttu-id="6f7d7-107">Herunterladen des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="6f7d7-107">Download the Linux kernel update package</span></span>

<span data-ttu-id="6f7d7-108">[Laden Sie das neueste Updatepaket für den WSL2-Linux-Kernel für x64-Computer herunter](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).</span><span class="sxs-lookup"><span data-stu-id="6f7d7-108">Please [download the latest WSL2 Linux kernel](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) update package for x64 machines.</span></span>

> [!NOTE]
> <span data-ttu-id="6f7d7-109">Wenn Sie einen ARM64-Computer verwenden, laden Sie stattdessen [das ARM64-Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) herunter.</span><span class="sxs-lookup"><span data-stu-id="6f7d7-109">If you're using an ARM64 machine, please download the [ARM64 package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) instead.</span></span>

## <a name="install-the-linux-kernel-update-package"></a><span data-ttu-id="6f7d7-110">Installieren des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="6f7d7-110">Install the Linux kernel update package</span></span>

<span data-ttu-id="6f7d7-111">So installieren Sie das Updatepaket für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="6f7d7-111">To install the Linux kernel update package:</span></span>

  1. <span data-ttu-id="6f7d7-112">Führen Sie das im vorherigen Schritt heruntergeladene Updatepaket aus.</span><span class="sxs-lookup"><span data-stu-id="6f7d7-112">Run the update package downloaded in the previous step.</span></span>

  2. <span data-ttu-id="6f7d7-113">Sie werden zur Eingabe erhöhter Berechtigungen aufgefordert. Wählen Sie „Ja“, um diese Installation zu genehmigen.</span><span class="sxs-lookup"><span data-stu-id="6f7d7-113">You will be prompted for elevated permissions, select ‘yes’ to approve this installation.</span></span>

  3. <span data-ttu-id="6f7d7-114">Sobald die Installation abgeschlossen ist, können Sie mit der Nutzung von WSL2 beginnen!</span><span class="sxs-lookup"><span data-stu-id="6f7d7-114">Once the installation is complete, you are ready to begin using WSL2!</span></span>

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a><span data-ttu-id="6f7d7-115">Zukünftige Pläne zur Aktualisierung des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="6f7d7-115">Future plans for updating the WSL2 Linux kernel</span></span>

<span data-ttu-id="6f7d7-116">Weitere Informationen finden Sie im Artikel über die [Änderungen an der Aktualisierung des WSL2 Linux-Kernels](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im [Blog zur Windows-Befehlszeile](https://aka.ms/cliblog).</span><span class="sxs-lookup"><span data-stu-id="6f7d7-116">For more information, read the article [changes to updating the WSL2 Linux kernel](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004), available on the [Windows Command Line Blog](https://aka.ms/cliblog).</span></span>
