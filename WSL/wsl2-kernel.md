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
# <a name="updating-the-wsl-2-linux-kernel"></a>Aktualisieren des WSL 2-Linux-Kernels

Führen Sie die folgenden Schritte aus, um den Linux-Kernel innerhalb von WSL 2 manuell zu aktualisieren. 

## <a name="download-the-linux-kernel-update-package"></a>Herunterladen des Linux-Kernel Update Pakets

Klicken Sie auf [diesen Link](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) , um das neueste WSL2 Linux Kernel Update Package for amd64 Machines herunterzuladen.

> [!NOTE] Wenn Sie einen ARM64-Computer verwenden, müssen Sie [Dieses Paket](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi) stattdessen herunterladen.

## <a name="install-the-linux-kernel-update-package"></a>Installieren des Linux-Kernel Update Pakets

So installieren Sie das Linux-Kernel Update Paket:
    1. Führen Sie das im vorherigen Schritt heruntergeladene Update Paket aus.
    2. Wenn Sie aufgefordert werden, erweiterte Berechtigungen zu erhalten, wählen Sie "Ja", um diese Installation zu genehmigen.
    3. Nachdem die Installation abgeschlossen ist, können Sie mit der Verwendung von WSL2 beginnen!

## <a name="future-plans-for-updating-the-wsl2-linux-kernel"></a>Zukünftige Pläne zum Aktualisieren des WSL2 Linux-Kernels

Weitere Informationen zu diesen Änderungen finden Sie in [diesem Blogbeitrag](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004) im Windows- [befehlszeilenblog](https://aka.ms/cliblog).