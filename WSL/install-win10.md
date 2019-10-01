---
title: Installieren des Windows-Subsystems für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10, install
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: c53c4507fb56f8e4a3456963b1d6f50ceac8ef37
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269815"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a>Windows-Subsystem für Linux: Installationsleitfaden für Windows 10

## <a name="install-the-windows-subsystem-for-linux"></a>Installieren des Windows-Subsystems für Linux

Bevor Sie Linux-Distributionen für WSL installieren, müssen Sie sicherstellen, dass das optionale Feature „Windows-Subsystem für Linux“ aktiviert ist:

1. Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. Starten Sie den Computer neu, wenn Sie dazu aufgefordert werden.

## <a name="install-your-linux-distribution-of-choice"></a>Installieren der Linux-Distribution Ihrer Wahl
Zum Herunterladen und Installieren Ihrer bevorzugten Distribution(en) haben Sie drei Möglichkeiten:
1. Herunterladen und Installieren aus dem Microsoft Store (siehe unten)
1. Herunterladen und Installieren über die Befehlszeile bzw. ein Skript ([lesen Sie die Anweisungen für eine manuelle Installation](install-manual.md))
1. Herunterladen und manuelles Entpacken und Installieren (für Windows Server, [Anleitungen finden Sie hier](install-on-server.md))

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a>Windows 10 Fall Creators Update oder höher: Herunterladen aus dem Microsoft Store

> Dieser Abschnitt gilt für Windows Build 16215 oder höher.  Führen Sie diese Schritte aus, um [Ihren Build zu überprüfen](troubleshooting.md#check-your-build-number). 

1. Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugte Linux-Distribution aus.

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/store.png)

    Über die folgenden Links wird die Seite des Microsoft Store für jede Distribution geöffnet:

    * [Ubuntu 16.04 LTS](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    * [Ubuntu 18.04 LTS](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    * [OpenSUSE Leap 15](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    * [OpenSUSE Leap 42](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [SUSE Linux Enterprise Server 12](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [SUSE Linux Enterprise Server 15](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    * [Kali Linux](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [Debian GNU/Linux](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    * [Fedora Remix for WSL](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    * [Pengwin](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    * [Pengwin Enterprise](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    * [Alpine WSL](https://www.microsoft.com/store/apps/9p804crf0395)

1. Wählen Sie auf der Seite der Distribution die Option „Get“ (Abrufen) aus.

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a>Vervollständigen der Initialisierung Ihrer Distribution
Nachdem Sie Ihre Linux-Distribution installiert haben, müssen Sie Ihre [neue Distributionsinstanz ein Mal initialisieren](initialize-distro.md), bevor sie verwendet werden kann.

## <a name="troubleshooting"></a>Problembehandlung: 

Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen beschrieben. Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).

* **Installation failed with error 0x80070003 (Installationsfehler mit Fehlercode 0x80070003)**
    * Das Windows-Subsystem für Linux wird nur auf dem Systemlaufwerk ausgeführt (in der Regel ist dies Ihr Laufwerk `C:`). Stellen Sie sicher, dass die Distributionen auf dem Systemlaufwerk gespeichert sind:  
    * Öffnen Sie **Einstellungen** -> **Speicher** -> **Weitere Speichereinstellungen: Ändern Sie den Speicherort für neue Inhalte**
    ![Abbildung der Systemeinstellungen für die Installation von Apps auf dem Laufwerk C:](media/AppStorage.png)
    
    
 * **WslRegisterDistribution failed with error 0x8007019e (WslRegisterDistribution-Fehler mit Fehlercode 0x8007019e)**   
  * Die optionale Komponente des Windows-Subsystems für Linux ist nicht aktiviert: 
   * Öffnen Sie **Systemsteuerung** -> **Programme und Funktionen** -> **Windows-Funktion aktivieren oder deaktivieren**. Aktivieren Sie die Option **Windows-Subsystem für Linux**, oder verwenden Sie das PowerShell-Cmdlet, das am Anfang dieses Artikels erwähnt wurde.
