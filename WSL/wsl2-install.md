---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 3ad180ecc9deaa1566e9870700b26f82f631c7f1
ms.sourcegitcommit: 9ad7a54668f39677e9660186e4f5172ea2597e2b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2019
ms.locfileid: "68246868"
---
# <a name="installation-instructions-for-wsl-2"></a>Installationsanweisungen für WSL 2

Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:

- Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.
- Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.
- Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.

Beachten Sie, dass zur Verwendung von WSL 2 Windows 10, Build 18917 oder höher benötigt wird. Außerdem muss WSL bereits installiert sein (Anweisungen für die Installation finden Sie [hier](./install-win10.md)). 

## <a name="enable-the-virtual-machine-platform-optional-component"></a>Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.

Öffnen Sie PowerShell als Administrator, und führen Sie diesen Befehl aus:

`Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform`

Nach der Aktivierung dieser Änderungen müssen Sie Ihren Computer neu starten.

## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a>Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.

Führen Sie in PowerShell diesen Befehl aus:

`wsl --set-version <Distro> 2`

Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution. (Eine Suche danach ist über diesen Befehl möglich `wsl -l`.) Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.

Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:

`wsl --set-default-version 2`

Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a>Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.

Verwenden Sie den folgenden Befehl, um für jede Distribution die verwendete WSL-Version zu überprüfen:

`wsl --list --verbose` oder `wsl -l -v`

Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen. Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden! 

## <a name="troubleshooting"></a>Problembehandlung: 

Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben. Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).

* **Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**
    * Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist. Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.
   
* **Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**
    * Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden. Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`. Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).