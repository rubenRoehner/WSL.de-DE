---
title: Installieren Sie Windows-Subsystem für Linux (WSL) auf unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: Installieren Sie BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 40bbe73acbfd0483e18ab6ff1696fdb44eaff2e4
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063288"
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

    * [Ubuntu](https://www.microsoft.com/store/p/ubuntu/9nblggh4msv6)
    * [OpenSUSE](https://www.microsoft.com/store/apps/9njvjts82tjx)
    * [SLES](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    * [Kali Linux](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    * [Debian GNU/Linux](https://www.microsoft.com/store/apps/9MSVKQC78PK6)

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
