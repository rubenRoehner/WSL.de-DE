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
# <a name="updating-the-wsl-2-linux-kernel"></a>Aktualisieren des WSL2-Linux-Kernels

Um den Linux-Kernel innerhalb von WSL2 manuell zu aktualisieren, führen Sie die folgenden Schritte aus.

> [!NOTE] 
> Wenn das Installationsprogramm WSL 1 nicht finden kann, klicken Sie mit der rechten Maustaste auf das Installationsprogramm für das Linux-Kernel-Update, wählen Sie „Deinstallieren“ aus, und starten Sie das Installationsprogramm erneut.

## <a name="download-the-linux-kernel-update-package"></a>Herunterladen des Updatepakets für den Linux-Kernel

[Laden Sie das neueste Updatepaket für den WSL2-Linux-Kernel für x64-Computer herunter](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).

> [!NOTE]
> Wenn Sie einen ARM64-Computer verwenden, laden Sie stattdessen [das ARM64-Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) herunter.

## <a name="install-the-linux-kernel-update-package"></a>Installieren des Updatepakets für den Linux-Kernel

So installieren Sie das Updatepaket für den Linux-Kernel

  1. Führen Sie das im vorherigen Schritt heruntergeladene Updatepaket aus.

  2. Sie werden zur Eingabe erhöhter Berechtigungen aufgefordert. Wählen Sie „Ja“, um diese Installation zu genehmigen.

  3. Sobald die Installation abgeschlossen ist, können Sie mit der Nutzung von WSL2 beginnen!

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a>Zukünftige Pläne zur Aktualisierung des WSL2-Linux-Kernels

Weitere Informationen finden Sie im Artikel über die [Änderungen an der Aktualisierung des WSL2 Linux-Kernels](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im [Blog zur Windows-Befehlszeile](https://aka.ms/cliblog).
