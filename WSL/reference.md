---
title: Windows-Subsystem für Linux-Befehlsreferenz
description: Liste der Befehle, die das Windows-Subsystem für Linux verwalten
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, ubuntu
author: scooley
ms.author: scooley
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.openlocfilehash: 978a35d593e37877949c24cbd833a519888d54bf
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063578"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a>Befehlsreferenz für Windows-Subsystem für Linux

> `lxrun.exe` ist als veraltet markierte seit Windows 10-Version 1803 und höher.

Der Befehl `lxrun.exe` kann verwendet werden, für die Interaktion mit der [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) direkt.  Diese Befehle werden installiert, in der `\Windows\System32` Verzeichnis und ggf. einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.

* `lxrun.exe` Dient zum Verwalten von WSL.  Dieser Befehl kann zum Installieren oder deinstallieren das Ubuntu-Image verwendet werden.


| Befehl                     | Beschreibung                     |
|:----------------------------|:---------------------------|
| `bash`                      | Startet die Bash-Shell im aktuellen Verzeichnis.  Wenn die Bash-Shell nicht automatisch installiert wird ausgeführt `lxrun /install` |
| `bash ~`                    | Startet die Bash-Shell in Ubuntu-Basisverzeichnis des Benutzers an.  Ähnlich wie beim Ausführen von cd ~            |
| `bash -c "<command>"`       | Führt den Befehl und druckt die Ausgabe an der Eingabeaufforderung von Windows beendet wird. <br/> <br/> Beispiel: **bash -c "ls"** |

<p>

| Befehl                     | Beschreibung                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | Der Befehl Lxrun wird verwendet, zum Verwalten der WSL-Instanz. |
| `lxrun /install`            | Der Download gestartet und die Installation. <br/> **/ y** können hinzugefügt werden, um alle eingabeaufforderungen zu umgehen.  Die bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer als Stamm festgelegt ist.          |
| `lxrun /uninstall`          | Deinstalliert, und löscht das Ubuntu-Image.  Standardmäßig wird dadurch nicht die Ubuntu-Basisverzeichnis des Benutzers entfernt. <br/> **/ y** können hinzugefügt werden, um automatisch die bestätigungsaufforderung akzeptieren <br/>**/ vollständiges** deinstalliert, und löscht die Ubuntu-Basisverzeichnis des Benutzers         |
| `lxrun /setdefaultuser <userName>`     | Die Standardeinstellung Bash festgelegt auf Ubuntu-Benutzer. Wird für ein Kennwort angefordert werden, wenn der angegebene Benutzer nicht vorhanden ist.  Weitere Informationen finden Sie unter: https://aka.ms/wslusers. <br/> **/ y** umgehungen Promping für das Kennwort.  Ohne Angabe eines Kennworts wird der Benutzer erstellt werden.|
| `lxrun /update`            | Aktualisiert das Subsystem des Paket-index          |
