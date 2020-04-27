---
title: 'Windows-Subsystem für Linux: Befehlsreferenz'
description: Liste der Befehle, mit denen das Windows-Subsystem für Linux verwaltet wird
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: d74a6926fd797f2e1ede0fd5d8d080d0f1ce3f6b
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "71269840"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a>Befehlsreferenz für das Windows-Subsystem für Linux

Die beste Möglichkeit, mit dem Windows-Subsystem für Linux zu interagieren, ist die Verwendung des Befehls `wsl.exe`. 


## `wsl.exe`

Unten finden Sie eine Liste mit allen Optionen, wenn Sie `wsl.exe` ab Windows Version 1903 verwenden.

Syntax: `wsl [Argument] [Options...] [CommandLine]`

### <a name="arguments-for-running-linux-binaries"></a>Argumente für das Ausführen von Linux-Binärdateien

* **Ohne Argumente**

  Wenn keine Befehlszeile angegeben wird, startet „wsl.exe“ die Standardshell.

* **--exec, -e \<BefehlsZeile>**
  
  Führt den angegebenen Befehl ohne Verwendung der Linux-Standardshell aus.

* **--**
  
  Übergibt die verbleibende Befehlszeile unverändert.

Die oben genannten Befehle akzeptieren außerdem die folgenden Optionen:

* **--distribution, -d \<Distribution>**

  Führt die angegebene Distribution aus.

* **--user, -u \<BenutzerName>**

  Ausführung als der angegebene Benutzer.

### <a name="arguments-for-managing-windows-subsystem-for-linux"></a>Argumente für die Verwaltung des Windows-Subsystems für Linux

* **--export \<Distribution> \<DateiName>**
  
  Exportiert die Distribution in eine TAR-Datei. Der Dateiname kann „-“ für Standardausgabe sein.

* **--import \<Distribution> \<InstallationsOrt> \<DateiName>**
  
  Importiert die angegebene TAR-Datei als neue Distribution. Der Dateiname kann „-“ für Standardeingabe sein.

* **--list, -l [Optionen]**
  
  Listet Distributionen auf.

  Optionen:
  * **--all**
      
    Listet alle Distributionen auf, einschließlich Distributionen, die zurzeit installiert oder deinstalliert werden.

  * **--running**
      
    Listet nur Distributionen auf, die zurzeit ausgeführt werden.

* **--set-default, -s \<Distribution>**
  
  Legt die Distribution als Standard fest.

* **--terminate, -t \<Distribution>**
  
  Beendet die angegebene Distribution.

* **--unregister \<Distribution>**
  
  Hebt die Registrierung der Distribution auf.
   
* **--help**: Zeigt Syntaxinformationen an.

## <a name="additional-commands"></a>Weitere Befehle

Es gibt auch historische Befehle für die Interaktion mit dem Windows-Subsystem für Linux. Ihre Funktionalität ist in `wsl.exe` enthalten, sie sind jedoch weiterhin zur Verwendung verfügbar. 

### `wslconfig.exe`

Mit diesem Befehl können Sie Ihre WSL-Distribution konfigurieren. Es folgt eine Liste der zugehörigen Optionen.

Syntax: `wslconfig [Argument] [Options...]`

#### <a name="arguments"></a>Argumente
* **/l, /list [Optionen]**
  
  Listet registrierte Distributionen auf.
  
  Optionen:
    * **/all**
    
      Listet optional alle Distributionen auf, einschließlich Distributionen, die zurzeit installiert oder deinstalliert werden.

    * **/running**
      
      Listet nur Distributionen auf, die zurzeit ausgeführt werden.

* **/s, /setdefault \<Distribution>**
  
  Legt die Distribution als Standard fest.

* **/t, /terminate \<Distribution>**
  
  Beendet die Distribution.

* **/u, /unregister \<Distribution>**
  
  Hebt die Registrierung der Distribution auf.
   
* **/upgrade \<Distribution>**
  
  Führt ein Upgrade der Distribution auf das WslFs-Dateisystemformat durch.

### `bash.exe`

Dieser Befehl wird verwendet, um eine Bash-Shell zu starten. Unten finden Sie die Optionen, die Sie mit diesem Befehl verwenden können.

Syntax: `bash [Options...]`

* **Keine Option angegeben**
  
  Startet die Bash-Shell im aktuellen Verzeichnis. Wenn die Bash-Shell nicht installiert ist, wird automatisch `lxrun /install` ausgeführt.

* **~**
  
  `bash ~` startet die Bash-Shell im Basisverzeichnis des Benutzers.  Vergleichbar mit der Ausführung von `cd ~`.

* **-c "\<Befehl>"**
  
  Führt den Befehl aus, gibt die Ausgabe aus, und kehrt zur Windows-Eingabeaufforderung zurück.
    
  Beispiel: `bash -c "ls"`.

## <a name="deprecated-commands"></a>Veraltete Befehle

`lxrun.exe` war der erste Befehl, der zum Installieren und Verwalten des Windows-Subsystems für Linux verwendet wurde. Er gilt ab Windows 10 Version 1803 und höher als veraltet.

Der Befehl `lxrun.exe` kann verwendet werden, um direkt mit dem [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) zu interagieren.  Diese Befehle werden im Verzeichnis `\Windows\System32` installiert und können in einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.

| Befehl                     | Beschreibung                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | Der lxrun-Befehl wird verwendet, um die WSL-Instanz zu verwalten. |
| `lxrun /install`            | Startet den Download- und Installationsvorgang. <br/> **/y** kann hinzugefügt werden, um alle Eingabeaufforderungen zu umgehen.  Die Bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer wird auf „root“ festgelegt.          |
| `lxrun /uninstall`          | Deinstalliert und löscht das Ubuntu-Image.  Standardmäßig wird hierdurch nicht das Ubuntu-Basisverzeichnis des Benutzers entfernt. <br/> **/y** kann hinzugefügt werden, um die Bestätigungsaufforderung automatisch zu akzeptieren. <br/>**/full** deinstalliert und löscht das Ubuntu-Basisverzeichnis des Benutzers.         |
| `lxrun /setdefaultuser <userName>`     | Legt die Standard-Bash für den Ubuntu-Benutzer fest. Fordert zur Eingabe eines Kennworts auf, wenn der angegebene Benutzer nicht vorhanden ist.  Weitere Informationen finden Sie unter https://aka.ms/wslusers. <br/> **/y** umgeht die Eingabeaufforderung für das Kennwort.  Der Benutzer wird ohne Kennwort erstellt.|
| `lxrun /update`            | Aktualisiert den Paketindex des Subsystems.          |
