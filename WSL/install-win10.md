---
title: Installieren des Windows-Subsystems für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10, Installation
author: taraj
ms.author: taraj
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 82b5c0ccba7a444f13f186a2e33f210ac2cf48da
ms.sourcegitcommit: 5844c6dbf692780b86b30bd65e11820fff43b3bd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2019
ms.locfileid: "67499284"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a>Windows-Subsystem für Linux-Installationshandbuch für Windows 10

## <a name="install-the-windows-subsystem-for-linux"></a>Installieren des Windows-Subsystems für Linux

Bevor Sie Linux-Distributionen für WSL installieren, müssen Sie sicherstellen, dass das optionale Feature "Windows-Subsystem für Linux" aktiviert ist:

1. Öffnen Sie PowerShell als Administrator, und führen Sie aus:
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. Starten Sie den Computer bei entsprechender Aufforderung neu.

## <a name="install-your-linux-distribution-of-choice"></a>Installieren der Linux-Distribution Ihrer Wahl
Zum herunterladen und Installieren Ihrer bevorzugten Distribution haben Sie drei Möglichkeiten:
1. Herunterladen und installieren aus dem Microsoft Store (siehe unten)
1. Herunterladen und installieren über die Befehlszeile bzw. das Skript ([Lesen Sie die Anweisungen zur manuellen Installation](install-manual.md))
1. Herunterladen und manuelles entpacken und installieren (für Windows Server- [Anleitungen hier](install-on-server.md))

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a>Windows 10 Fall Creators Update und höher: Installieren von Microsoft Store

> Dieser Abschnitt ist für Windows Build 16215 oder höher.  Führen Sie diese Schritte aus, um [den Build zu überprüfen](troubleshooting.md#check-your-build-number) 

1. Öffnen Sie die Microsoft Store, und wählen Sie Ihre bevorzugte Linux-Distribution aus.

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/store.png)

    Über die folgenden Links wird die Seite Microsoft Store für jede Distribution geöffnet:

    * [Ubuntu 16,04 LTS](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    * [Ubuntu 18,04 LTS](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    * [OpenSUSE, Schritt 15](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    * [OpenSUSE-Schritt 42](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [SUSE Linux Enterprise Server 12](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [SUSE Linux Enterprise Server 15](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    * [Kali Linux](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [Debian GNU/Linux](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    * [Fedora Remix für WSL](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    * [Pengwin](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    * [Pengwin Enterprise](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    * [Alpine WSL](https://www.microsoft.com/store/apps/9p804crf0395)

1. Wählen Sie auf der Seite der Distribution die Option "Get" aus.

    ![Anzeigen von Linux-Distributionen im Microsoft Store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a>Vervollständigen der Initialisierung Ihrer Distribution
Nachdem Sie Ihre Linux-Distribution installiert haben, müssen Sie [Ihre neue Distribution-Instanz einmal initialisieren](initialize-distro.md) , bevor Sie verwendet werden kann.

## <a name="troubleshooting"></a>Problembehandlung: 

Im folgenden finden Sie verwandte Fehler und empfohlene Korrekturen. Weitere häufige Fehler und deren Lösungen finden Sie auf der [WSL-Seite zur Problem](troubleshooting.md) Behandlung.

* **Fehler bei der Installation (Fehler 0x80070003).**
    * Das Windows-Subsystem für Linux wird nur auf dem Systemlaufwerk ausgeführt (in der `C:` Regel ist dies Ihr Laufwerk). Stellen Sie sicher, dass die Distributionen auf dem Systemlaufwerk gespeichert sind:  
    * Öffnen Sie **Settings** -> **Storage** -> more**Storage Settings: Ändern Sie den Speicherort**
    ![der neuen Inhalte der Systemeinstellungen für die Installation von apps auf Laufwerk C:.](media/AppStorage.png)
    
    
 * **Wslregisterdistribution ist mit Fehler 0x8007019e fehlgeschlagen.**   
  * Die optionale Komponente des Windows-Subsystems für Linux ist nicht aktiviert: 
   * Öffnen Sie **Systemsteuerung** -> **Programme und Features** -> * * Windows-Funktion ein-oder ausschalten * *-> Überprüfen Sie das **Windows-Subsystem für Linux** , oder verwenden Sie das PowerShell-Cmdlet, das am Anfang dieses Artikels erwähnt wurde.
