---
title: Installieren Sie das Subsystem für Linux unter WindowsServer
description: Installationsanweisungen für das Linux-Subsystem unter Windows Server.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu und WindowsServer
author: scooley
ms.author: scooley
ms.date: 05/22/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: 25723395212575f8fe2dcbfbd30b59de9431816a
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67035073"
---
# <a name="windows-server-installation-guide"></a>Windows Server-Installationshandbuch

> Gilt für Windows Server-2019 und höher

Auf / / Build2017, Microsoft hat angekündigt, dass Windows-Subsystem für Linux ist [unter Windows Server verfügbaren](https://blogs.technet.microsoft.com/hybridcloud/2017/05/10/windows-server-for-developers-news-from-microsoft-build-2017/).  Diese Anweisungen erläutert, die das Windows-Subsystem für Linux unter Windows Server 1709 und höher ausgeführt.

## <a name="enable-the-windows-subsystem-for-linux-wsl"></a>Aktivieren Sie das Windows-Subsystem für Linux (WSL)

Vor dem Ausführen von Linux-Distributionen für Windows müssen Sie die optionale Funktion von "Windows-Subsystem für Linux" aktivieren und neu starten.

1. Öffnen Sie PowerShell als Administrator, und führen Sie aus:
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. Starten Sie Ihre Computer bei entsprechender Aufforderung neu. **Dieser Neustart ist erforderlich,** um sicherzustellen, dass es sich bei eine vertrauenswürdigen ausführungsumgebung WSL initiiert werden kann.

## <a name="download-a-linux-distro"></a>Laden Sie eine Linux-Distribution

Führen Sie [diese Anweisungen](install-manual.md) , Ihre bevorzugten Linux-Distribution herunterzuladen.

## <a name="extract-and-install-a-linux-distro"></a>Extrahieren Sie und installieren Sie eine Linux-Distribution
Nun, da Sie eine Distribution heruntergeladen haben, extrahieren Sie den Inhalt, und installieren Sie manuell die Distribution:

1. Extrahieren Sie die `<distro>.appx` Inhalt des Pakets, z. B. mithilfe von PowerShell:

    ```powershell
    Rename-Item ~/Ubuntu.appx ~/Ubuntu.zip
    Expand-Archive ~/Ubuntu.zip ~/Ubuntu
    ```

2. Führen Sie das Startprogramm-Distribution, die Installation abzuschließen, führen Sie die Distribution-Startprogramm-Anwendung im Zielordner, mit dem Namen `<distro>.exe`. Zum Beispiel: `ubuntu.exe`usw.

    ![Erweiterte Distribution von Ubuntu unter Windows Server](media/server-appx-expand.png)

    > **Problembehandlung**
    > * **Fehler bei der Installation Fehler 0x8007007e**: Dieser Fehler tritt auf, wenn Ihr System WSL nicht unterstützt. Stellen Sie Folgendes sicher:
    >   * Sie können Windows Build 16215 oder höher ausführen. [Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).
    >   * Das Windows-Subsystem für Linux optionale Komponente aktiviert ist, und der Computer neu gestartet wurde.  [WSL aktiviert](troubleshooting.md#confirm-wsl-is-enabled).
    
3. Hinzufügen von Ihrem Pfad-Distribution, die in der Windows-Umgebung Pfad (`C:\Users\Administrator\Ubuntu` in diesem Beispiel), z. B. mithilfe von Powershell:
        
    ```powershell
    $userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
    [System.Environment]::SetEnvironmentVariable("PATH", $userenv + ";C:\Users\Administrator\Ubuntu", "User")
    ```
    Sie können jetzt Ihre Distribution von jedem beliebigen Pfad starten, indem Sie eingeben `<distro>.exe`. Beispiel: `ubuntu.exe`

Nun, da Ihre Linux-Distribution installiert ist, müssen Sie [initialisieren Sie die neue Instanz der Distribution](initialize-distro.md) vor der Verwendung von Ihrer Distribution.
