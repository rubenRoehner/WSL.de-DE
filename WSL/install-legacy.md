---
title: Installieren oder Entfernen von Windows 10 Anniversary Update oder Creators Update
description: Installations-und Deinstallations Anweisungen für die Legacy-, Beta-Distribution von Windows 10 Anniversary Update oder Creators Update
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10, Legacy, Beta, installieren, entfernen, deinstallieren, Deinstallation, löschen, veraltet
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 0d8fdabd61fadbfc58549a220ead23585a3d3656
ms.sourcegitcommit: 5844c6dbf692780b86b30bd65e11820fff43b3bd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2019
ms.locfileid: "67499264"
---
# <a name="guide-to-install-or-uninstall-windows-subsystem-for-linux-on-windows-10-anniversary-update-and-creators-update"></a>Leitfaden zum Installieren oder Deinstallieren des Windows-Subsystems für Linux unter Windows 10 Anniversary Update und Creators Update 

Wenn Sie Windows 10 Creators Update oder höher ausführen, befolgen Sie [die Installationsanweisungen für Windows 10](install-win10.md).

<strong><em><span style="color: #f28014">Die folgenden Anweisungen gelten für Benutzer, die Windows 10 Anniversary Update oder Windows 10 Creators Update ausführen.</span></em></strong>

Vor Windows 10 Fall Creators Update (Version 1709) wurde WSL als Beta Funktion veröffentlicht und eine einzelne Ubuntu-Instanz installiert, als "bash on Ubuntu on Windows" (oder bash. exe) zum ersten Mal ausgeführt wurde.

> Obwohl Sie WSL unter früheren Versionen von Windows 10 verwenden können, ist diese Beta Version "Legacy Distribution" mittlerweile als veraltet eingestuft. Wir empfehlen Ihnen dringend, die neueste verfügbare Version von Windows 10 auszuführen. Jede neue Version von Windows 10 enthält viele hundert Korrekturen und Verbesserungen in WSL, sodass immer mehr Linux-Tools und-Apps auf WSL ordnungsgemäß ausgeführt werden können.

Wenn Sie kein Upgrade auf Fall Creators Update oder höher ausführen können, führen Sie die folgenden Schritte aus, um WSL zu aktivieren und zu verwenden:

1. Aktivieren Sie den Entwicklermodus, um WSL auf Windows 10 Anniversary Update oder Creators Update auszuführen. Sie müssen den Entwicklermodus aktivieren:

    Öffnen von **Einstellungen** -> **aktualisieren und Sicherheit** -> **für Entwickler**

    Wählen Sie das Optionsfeld Entwicklermodus aus.  
    ![Aktivieren des Entwicklermodus](media/updateAndSecurity.png)

    > Die Anforderung zum Aktivieren des Entwicklermodus wurde [in Windows 10 Fall Creators Update entfernt](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/) .

1. Öffnen Sie eine Eingabeaufforderung.  Eingeben `bash` und drücken der EINGABETASTE

    Wenn Sie bash auf Ubuntu unter Windows zum ersten Mal ausführen, werden Sie aufgefordert, die kanonische Lizenz zu akzeptieren. Nach der Annahme wird die Ubuntu-Instanz von WSL auf Ihren Computer heruntergeladen und installiert, und dem Startmenü wird eine "bash on Ubuntu on Windows"-Verknüpfung hinzugefügt.

    ![Eingabeaufforderung zur Installation von Ubuntu](media/bashShellInstall.png)

    Wenn Sie bash unter Windows zum ersten Mal ausführen, werden Sie aufgefordert, einen UNIX-Benutzernamen und ein Kennwort zu erstellen. Befolgen Sie die [Anweisungen der neuen Distribution-Instanz](initialize-distro.md) , um die Installation abzuschließen.

1. Starten Sie eine neue Ubuntu-Shell mit folgenden Optionen:
    * Ausführen `bash` über eine Eingabeaufforderung
    * Klicken auf das Startmenü "bash on Ubuntu on Windows"-Verknüpfung

    
## <a name="uninstallingremoving-the-legacy-distro"></a>Deinstallieren/Entfernen der Legacy Distribution
Wenn Sie von einer früheren Windows 10-Version, auf der Sie WSL installiert haben, ein Upgrade auf Windows 10 Fall Creators Update durchführen, bleibt Ihre vorhandene Distribution unverändert. Es wird jedoch dringend empfohlen, dass Sie eine neue, vom Speicher bereitgestellte Distribution-ASaP installieren und alle notwendigen Dateien, Daten usw. aus Ihrer Legacy-Distribution zu ihrer neuen Distribution migrieren.

Um die Legacy-Distribution von Ihrem Computer zu entfernen, führen Sie Folgendes über eine Befehlszeile oder eine PowerShell-Instanz aus:

```console
wsl --unregister Legacy
```

Wenn Sie nicht Windows-Version 1903 oder höher verwenden, müssen Sie möglicherweise oder `wslconfig /u Legacy` `lxrun /uninstall /full` stattdessen ausführen. 

### <a name="manually-deleting-the-legacy-distro"></a>Manuelles Löschen der Legacy-Distribution
Wenn Sie möchten, können Sie die Legacy Instanz manuell löschen. Dies ist möglicherweise erforderlich, wenn Probleme beim Deinstallieren der Legacy-Distribution `lxrun.exe`mithilfe von auftreten oder wenn Windows 10 Spring 2018 Update (oder höher) ausgeführt wird, das `lxrun.exe`nicht mit ausgeliefert wird.

Löschen Sie den Ordner (und dessen unter Inhalt) mit dem `%localappdata%\lxss\` Windows-Datei-Explorer oder der Befehlszeile, um das Löschen der alten WSL-Distribution zu erzwingen.

Mithilfe der PowerShell
```powershell
rm -Recurse $env:localappdata/lxss/
```

Mithilfe von cmd:
```console
DEL /S %localappdata%\lxss\
```
