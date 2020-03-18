---
title: Aktualisieren des WSL2-Linux-Kernels
description: Anweisungen zum manuellen Aktualisieren Ihres WSL2-Linux-Kernels
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
ms.date: 03/12/2020
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.localizationpriority: high
ms.custom: seodec18
ms.openlocfilehash: f7fce13c2acc65e3afa2cc56873e40bc55a460bc
ms.sourcegitcommit: 506272bd7fc1cbda7e32146d54a8bdd02af3e0c4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/13/2020
ms.locfileid: "79319710"
---
# <a name="updating-the-wsl-2-linux-kernel"></a>Aktualisieren des WSL2-Linux-Kernels

Um den Linux-Kernel innerhalb von WSL2 manuell zu aktualisieren, führen Sie die folgenden Schritte aus. 

## <a name="download-the-linux-kernel-update-package"></a>Herunterladen des Updatepakets für den Linux-Kernel

Klicken Sie auf [diesen Link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi), um das neueste Updatepaket für den WSL2-Linux-Kernel für AMD64-Computer herunterzuladen.

> [!NOTE] 
> Wenn Sie einen ARM64-Computer verwenden, laden Sie stattdessen [dieses Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) herunter.

## <a name="install-the-linux-kernel-update-package"></a>Installieren des Updatepakets für den Linux-Kernel

So installieren Sie das Updatepaket für den Linux-Kernel

    1. Führen Sie das im vorherigen Schritt heruntergeladene Updatepaket aus.
    2. Sie werden zur Eingabe erhöhter Berechtigungen aufgefordert. Wählen Sie „Ja“, um diese Installation zu genehmigen.
    3. Sobald die Installation abgeschlossen ist, können Sie mit der Nutzung von WSL2 beginnen!

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a>Zukünftige Pläne zur Aktualisierung des WSL2-Linux-Kernels

Weitere Informationen über diese Änderungen finden Sie in [diesem Blogbeitrag](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im [Blog zur Windows-Befehlszeile](https://aka.ms/cliblog).
