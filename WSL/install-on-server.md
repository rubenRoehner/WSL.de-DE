---
title: Installieren des Linux-Subsystems unter Windows Server
description: Installationsanweisungen für das Linux-Subsystem unter Windows Server.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Windows Server
ms.date: 05/22/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: 51a2e3f3443ed9b1ba3d8ab79977f22839ee0283
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269783"
---
# <a name="windows-server-installation-guide"></a>Windows Server-Installationshandbuch

> Gilt für Windows Server 2019 und höher

In//Build2017 kündigte Microsoft an, dass das Windows-Subsystem für Linux [unter Windows Server verfügbar](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/)sein wird.  Diese Anleitung führt Sie durch die Ausführung des Windows-Subsystems für Linux unter Windows Server 1709 und höher.

## <a name="enable-the-windows-subsystem-for-linux-wsl"></a>Aktivieren des Windows-Subsystems für Linux (WSL)

Bevor Sie Linux-Distributionen unter Windows ausführen können, müssen Sie das optionale Feature "Windows-Subsystem für Linux" aktivieren und neu starten.

1. Öffnen Sie PowerShell als Administrator, und führen Sie aus:
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. Starten Sie den Computer bei entsprechender Aufforderung neu. **Dieser Neustart ist erforderlich** , um sicherzustellen, dass WSL eine vertrauenswürdige Ausführungsumgebung initiieren kann.

## <a name="download-a-linux-distro"></a>Herunterladen einer Linux-Distribution

Befolgen Sie [diese Anweisungen](install-manual.md) , um Ihre bevorzugte Linux-Distribution herunterzuladen.

## <a name="extract-and-install-a-linux-distro"></a>Extrahieren und Installieren einer Linux-Distribution
Nachdem Sie nun eine Distribution heruntergeladen haben, extrahieren Sie den Inhalt, und installieren Sie die Distribution manuell:

1. Extrahieren Sie `<distro>.appx` den Inhalt des Pakets, z. b. mithilfe von PowerShell:

    ```powershell
    Rename-Item ./Ubuntu.appx ./Ubuntu.zip
    Expand-Archive ./Ubuntu.zip ./Ubuntu
    ```

2. Führen Sie das Distribution-Start Programm aus, um die Installation abzuschließen, und führen Sie die Distribution-Start `<distro>.exe`Programm Anwendung im Zielordner namens aus. Beispiel: `ubuntu.exe`, usw.

    ![Erweiterte Ubuntu-Distribution unter Windows Server](media/server-appx-expand.png)

    > **Problembehandlung**
    > * **Fehler bei der Installation: 0x8007007e**: Dieser Fehler tritt auf, wenn das System WSL nicht unterstützt. Stellen Sie Folgendes sicher:
    >   * Sie führen Windows Build 16215 oder höher aus. [Überprüfen Sie den Build](troubleshooting.md#check-your-build-number).
    >   * Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.  [Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).
    
3. Fügen Sie den Pfad Ihrer Distribution zum Windows-Umgebungs Pfad`C:\Users\Administrator\Ubuntu` (in diesem Beispiel) hinzu, z. b. mithilfe von PowerShell:
        
    ```powershell
    $userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
    [System.Environment]::SetEnvironmentVariable("PATH", $userenv + ";C:\Users\Administrator\Ubuntu", "User")
    ```
    Sie können Ihre Distribution nun über einen beliebigen Pfad starten, indem `<distro>.exe`Sie eingeben. Beispiel: `ubuntu.exe`

Nachdem Sie Ihre Linux-Distribution installiert haben, müssen Sie [Ihre neue Distribution-Instanz](initialize-distro.md) vor der Verwendung Ihrer Distribution initialisieren.
