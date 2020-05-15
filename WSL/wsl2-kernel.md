---
title: Aktualisieren des WSL2-Linux-Kernels
description: Anweisungen zum manuellen Aktualisieren Ihres WSL2-Linux-Kernels
keywords: WSL, Windows, Linux-Kernel, Windows-Subsystem für Linux, Kernel
ms.date: 03/12/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: 89e5755699938b7797aa65a5f3131f93e3e31796
ms.sourcegitcommit: e6e888f2b88a2d9c105cee46e5ab5b70aa43dd80
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83343832"
---
# <a name="updating-the-wsl-2-linux-kernel"></a><span data-ttu-id="b0db0-104">Aktualisieren des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="b0db0-104">Updating the WSL 2 Linux kernel</span></span>

<span data-ttu-id="b0db0-105">Um den Linux-Kernel innerhalb von WSL2 manuell zu aktualisieren, führen Sie die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="b0db0-105">To manually update the Linux kernel inside of WSL 2 please follow these steps.</span></span>

> [!NOTE] 
> <span data-ttu-id="b0db0-106">Wenn das Installationsprogramm WSL 1 nicht finden kann, klicken Sie mit der rechten Maustaste auf das Installationsprogramm für das Linux-Kernel-Update, Wählen Sie „Deinstallieren“ aus, und starten Sie das Installationsprogramm erneut.</span><span class="sxs-lookup"><span data-stu-id="b0db0-106">If the installer cant find WSL 1 right click the Linux kernel update installer, then press uninstall then rerun the installer</span></span>

## <a name="download-the-linux-kernel-update-package"></a><span data-ttu-id="b0db0-107">Herunterladen des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="b0db0-107">Download the Linux kernel update package</span></span>

<span data-ttu-id="b0db0-108">[Laden Sie das neueste Updatepaket für den WSL2-Linux-Kernel für x64-Computer herunter](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).</span><span class="sxs-lookup"><span data-stu-id="b0db0-108">Please [download the latest WSL2 Linux kernel](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) update package for x64 machines.</span></span>

> [!NOTE]
> <span data-ttu-id="b0db0-109">Wenn Sie einen ARM64-Computer verwenden, laden Sie stattdessen [das ARM64-Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) herunter.</span><span class="sxs-lookup"><span data-stu-id="b0db0-109">If you're using an ARM64 machine, please download the [ARM64 package](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) instead.</span></span>

## <a name="install-the-linux-kernel-update-package"></a><span data-ttu-id="b0db0-110">Installieren des Updatepakets für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="b0db0-110">Install the Linux kernel update package</span></span>

<span data-ttu-id="b0db0-111">So installieren Sie das Updatepaket für den Linux-Kernel</span><span class="sxs-lookup"><span data-stu-id="b0db0-111">To install the Linux kernel update package:</span></span>

  1. <span data-ttu-id="b0db0-112">Führen Sie das im vorherigen Schritt heruntergeladene Updatepaket aus.</span><span class="sxs-lookup"><span data-stu-id="b0db0-112">Run the update package downloaded in the previous step.</span></span>

  2. <span data-ttu-id="b0db0-113">Sie werden zur Eingabe erhöhter Berechtigungen aufgefordert. Wählen Sie „Ja“, um diese Installation zu genehmigen.</span><span class="sxs-lookup"><span data-stu-id="b0db0-113">You will be prompted for elevated permissions, select ‘yes’ to approve this installation.</span></span>

  3. <span data-ttu-id="b0db0-114">Sobald die Installation abgeschlossen ist, können Sie mit der Nutzung von WSL2 beginnen!</span><span class="sxs-lookup"><span data-stu-id="b0db0-114">Once the installation is complete, you are ready to begin using WSL2!</span></span>

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a><span data-ttu-id="b0db0-115">Zukünftige Pläne zur Aktualisierung des WSL2-Linux-Kernels</span><span class="sxs-lookup"><span data-stu-id="b0db0-115">Future plans for updating the WSL2 Linux kernel</span></span>

<span data-ttu-id="b0db0-116">Weitere Informationen finden Sie im Artikel über die [Änderungen an der Aktualisierung des WSL2 Linux-Kernels](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im [Blog zur Windows-Befehlszeile](https://aka.ms/cliblog).</span><span class="sxs-lookup"><span data-stu-id="b0db0-116">For more information, read the article [changes to updating the WSL2 Linux kernel](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004), available on the [Windows Command Line Blog](https://aka.ms/cliblog).</span></span>
