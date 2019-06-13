---
title: Installieren von Windows-Subsystem für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: Installieren Sie BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: d30a5883d648e084193659e997c55d203eb5a735
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67035049"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a>Windows-Subsystem für Linux – Installationsleitfaden für Windows 10

## <a name="install-the-windows-subsystem-for-linux"></a>Installieren Sie das Windows-Subsystem für Linux

Vor der Installation alle Linux-Distributionen für WSL, müssen Sie sicherstellen, dass die "Windows-Subsystem für Linux" optionales Feature aktiviert ist:

1. Öffnen Sie PowerShell als Administrator, und führen Sie aus:
    ```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
    ```

2. Starten Sie Ihre Computer bei entsprechender Aufforderung neu.

## <a name="install-your-linux-distribution-of-choice"></a>Ihre Linux-Distribution Ihrer Wahl installieren
Zum Herunterladen und installieren Ihre bevorzugte Distro(s), haben Sie drei Optionen:
1. Herunterladen und Installieren von den Windows Store (siehe unten)
1. Herunterladen und installieren Sie die Befehlszeilenversion-Befehlszeile/Skripts ([lesen Sie die Anweisungen für die manuelle Installation](install-manual.md))
1. Herunterladen und manuell zu entpacken und installieren (für Windows Server - [Anleitung](install-on-server.md))

### <a name="windows-10-fall-creators-update-and-later-install-from-the-microsoft-store"></a>Windows 10 Fall Creators Update und höher: Installieren Sie von den Microsoft Store

> Dieser Abschnitt ist für Windows-Build 16215 oder höher.  Führen Sie diese Schritte zum [überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number). 

1. Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugten Linux-Distribution.

    ![Anzeigen der Linux-Distributionen im Windows store](media/store.png)

    Die folgenden Links wird für jede Verteilung der Windows Store-Seite geöffnet:

    * [Ubuntu 16.04 LTS](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    * [Ubuntu 18.04 LTS](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    * [OpenSUSE Leap 15](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    * [OpenSUSE Leap 42](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [SUSE Linux Enterprise Server 12](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [SUSE Linux Enterprise Server 15](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    * [Kali Linux](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [Debian GNU/Linux](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    * [Fedora Remix für WSL](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    * [WLinux](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    * [WLinux Enterprise](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    * [Alpine WSL](https://www.microsoft.com/store/apps/9p804crf0395)

1. Die Distribution, die auf der Seite Wählen Sie "Get"

    ![Anzeigen der Linux-Distributionen im Windows store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a>Initialisierung von Ihrer Distribution
Nun, da Ihre Linux-Distribution installiert ist, müssen Sie [initialisieren Sie die neue Instanz der Distribution](initialize-distro.md) einmal, bevor sie verwendet werden kann.

## <a name="troubleshooting"></a>Problembehandlung: 

Im folgenden finden Sie zugehörige Fehler und Vorschläge zur Behebung. Finden Sie in der [WSL Problembehandlungsseite](troubleshooting.md) andere häufig auftretende Fehler und ihre Lösungen.

* **Fehler 0 x 80070003 bei der Installation**
    * Der Windows-Subsystem für Linux nur ausgeführt wird, auf dem Systemlaufwerk (Dies ist normalerweise Ihr `C:` Laufwerk). Stellen Sie sicher, dass Distributionen, die auf dem Systemlaufwerk gespeichert werden:  
    * Open **Einstellungen** -> **Storage** -> **Weitere Einstellungen: Ändern, in dem neuer Inhalt gespeichert wird**
    ![Bild der Systemeinstellungen von apps auf Laufwerk "c:" installieren](media/AppStorage.png)
    
    
 * **Fehler bei 0x8007019e WslRegisterDistribution**   
  * Das Windows-Subsystem für Linux, die optionale Komponente nicht aktiviert ist: 
   * Open **Systemsteuerung** -> **Programme und Funktionen** -> ** Windows-Features ein- oder ausschalten ** Check -> **Windows-Subsystem für Linux** oder mithilfe der PowerShell-Cmdlets, die am Anfang dieses Artikels erwähnt.
