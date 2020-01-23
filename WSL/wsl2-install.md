---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 91bd479e922fc29bf11b89dcfe06fa381632c4fa
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520549"
---
# <a name="installation-instructions-for-wsl-2"></a>Installationsanweisungen für WSL 2

Sie können sich das folgende Video ansehen oder in diesem Artikel weiterlesen, um zu erfahren, wie Sie WSL2 installieren. 

> [!VIDEO https://channel9.msdn.com/Blogs/One-Dev-Minute/Learn-how-to-install-WSL-2/player]

Führen Sie die folgenden Schritte aus, um WSL 2 zu installieren und mit dessen Verwendung zu beginnen:

> WSL 2 ist nur in Windows 10-Builds 18917 oder höher verfügbar.

- Stellen Sie sicher, dass WSL installiert ist ( [hier](./install-win10.md)finden Sie entsprechende Anweisungen) und dass Windows 10 **Build 18917** oder höher ausgeführt wird.
   - Um sicherzustellen, dass Sie Build 18917 oder höher verwenden, fügen Sie [das Windows Insider-Programm](https://insider.windows.com/en-us/) an, und wählen Sie den "schnellen" Ring oder den "langsamen" Ring aus. 
   - Sie können Ihre Windows-Version überprüfen, indem Sie die Eingabeaufforderung öffnen und den Befehl `ver` ausführen.
- Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.
- Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.
- Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden.

## <a name="enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled"></a>Aktivieren Sie die optionale Komponente "Virtual Machine Platform", und stellen Sie sicher, dass WSL aktiviert ist.

Sie müssen sicherstellen, dass das Windows-Subsystem für Linux und die optionalen Komponenten der virtuellen Computerplattform installiert sind. Hierzu können Sie den folgenden Befehl in PowerShell ausführen: 

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

Starten Sie den Computer neu, um die Installation beider Komponenten abzuschließen.


## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a>Legen Sie über die Befehlszeile eine Distribution fest, die sich auf WSL 2 stützen soll.

Wenn Sie nicht über eine installierte Linux-Distribution verfügen, finden Sie unter [Installieren auf der Windows 10](./install-win10.md#install-your-linux-distribution-of-choice) docs-Seite Anweisungen zur Installation. 

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

Verwenden Sie den folgenden Befehl, um zu überprüfen, welche Versionen von WSL für jede Distribution verwendet werden (nur verfügbar in Windows Build 18917 oder höher):

`wsl --list --verbose` oder `wsl -l -v`

Die oben ausgewählte Distribution sollte jetzt unterhalb der Spalte für die Version eine 2 anzeigen. Damit ist die Einrichtung abgeschlossen, und Sie können Ihre WSL 2-Distribution verwenden! 

## <a name="troubleshooting"></a>Problembehandlung: 

Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen für die Installation von WSL 2 beschrieben. Weitere allgemeine WSL-Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).

* **Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**
    * Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist. Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.
   
* **Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**
    * Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 18917 oder höher verwenden. Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`. Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).

* **Der angeforderte Vorgang konnte aufgrund einer Einschränkung des virtuellen Festplattensystems nicht abgeschlossen werden. Dateien für virtuelle Festplatten müssen unkomprimiert und unverschlüsselt sein und dürfen nicht mit geringer Dichte sein.**
    * Überprüfen Sie den [WSL-GitHub-Thread #4103](https://github.com/microsoft/WSL/issues/4103) , in dem dieses Problem nach aktualisierten Informationen nachverfolgt wird.

* **Der Begriff "WSL" wird nicht als Name eines Cmdlets, einer Funktion, einer Skriptdatei oder eines ausführbaren Programms erkannt.** 
    * Stellen Sie sicher, dass die [optionale Komponente "Windows-Subsystem für Linux" installiert ist](./wsl2-install.md#enable-the-virtual-machine-platform-optional-component-and-make-sure-wsl-is-enabled).<br> Wenn Sie ein Arm64-Gerät verwenden und diesen Befehl in PowerShell ausführen, wird dieser Fehler angezeigt. Führen Sie stattdessen `wsl.exe` über [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6)oder die Eingabeaufforderung aus. 
