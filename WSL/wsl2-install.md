---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 7c031b1348a77e1dac967fae5e4df772e10a9084
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "80256343"
---
# <a name="installation-instructions-for-wsl-2"></a>Installationsanweisungen für WSL 2

Sie können sich das Video unten ansehen oder in diesem Artikel weiterlesen, um zu erfahren, wie Sie WSL2 installieren. 

> [!VIDEO https://channel9.msdn.com/Blogs/One-Dev-Minute/Learn-how-to-install-WSL-2/player]

Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:

> WSL 2 ist nur in Windows 10-Builds 18917 oder höher verfügbar

- Vergewissern Sie sich, dass Sie WSL installiert haben (Anweisungen dazu finden Sie [hier](./install-win10.md)) und dass Sie Windows 10 **Build 18917** oder höher ausführen
   - Um sicherzustellen, dass Sie Build 18917 oder höher verwenden, treten Sie dem [Windows Insider-Programm](https://insider.windows.com/en-us/) bei, und wählen Sie den „Fast Ring“ oder den „Slow Ring“ aus. 
   - Sie können Ihre Windows-Version überprüfen, indem Sie die Eingabeaufforderung öffnen und den Befehl `ver` ausführen.
- Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.
- Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.
- Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a>Aktivieren der optionalen Komponente „Virtual Machine Platform“ und sicherstellen, dass WSL aktiviert ist

Sie müssen sich vergewissern, dass auf Ihrem System die optionalen Komponenten Windows-Subsystem für Linux und Virtual Machine Platform installiert sind. Zu diesem Zweck können Sie den folgenden Befehl in PowerShell ausführen: 

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

Starten Sie den Computer neu, um die Installation beider Komponenten abzuschließen.


## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a>Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.

Wenn Sie nicht über eine installierte Linux-Distribution verfügen, finden Sie Anweisungen zum Installieren auf der Seite [Installieren unter Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) der Dokumentation. 

Führen Sie Folgendes aus, um eine Distribution festzulegen: 

```
wsl --set-version <Distro> 2
```

Ersetzen Sie hierbei `<Distro>` durch den tatsächlichen Namen Ihrer Distribution. (Eine Suche danach ist über diesen Befehl möglich `wsl -l`.) Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.

Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:

```
wsl --set-default-version 2
```

Hierdurch wird jede neue Distribution, die Sie installieren, als WSL 2-Distribution initialisiert.

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a>Überprüfen Sie abschließend, welche Versionen von WSL Ihre Distributionen verwenden.

Verwenden Sie den folgenden Befehl, um für jede Distribution die verwendete WSL-Version zu überprüfen (nur in Windows Build 18917 oder höher verfügbar):

`wsl --list --verbose` oder `wsl -l -v`

Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen. Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden! 

## <a name="troubleshooting"></a>Problembehandlung: 

Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben. Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).

* **Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**
    * Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist. Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.
   
* **Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**
    * Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden. Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`. Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).

* **Der angeforderte Vorgang konnte aufgrund einer Einschränkung des virtuellen Dateisystems nicht abgeschlossen werden. Dateien für virtuelle Festplatten müssen unkomprimiert und unverschlüsselt sein und dürfen keine geringe Dichte aufweisen.**
    * Bitte prüfen Sie den [WSL Github-Thread #4103](https://github.com/microsoft/WSL/issues/4103), der diesem Thema gewidmet ist, auf aktualisierte Informationen.

* **Der Ausdruck 'wsl' wurde nicht als Name eines Cmdlets, einer Funktion, einer Skriptdatei oder eines ausführbaren Programms erkannt.** 
    * Vergewissern Sie sich, dass die [optionale Komponente Windows-Subsystem für Linux installiert ist](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).<br> Außerdem wird dieser Fehler angezeigt, wenn Sie ein Arm64-Gerät verwenden und diesen Befehl aus PowerShell ausführen. Führen Sie stattdessen `wsl.exe` in [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6) oder einer Eingabeaufforderung aus. 
