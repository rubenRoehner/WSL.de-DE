---
title: Windows-Interoperabilität mit Linux
description: Beschreibt die Windows-Interoperabilität mit Linux-Distributionen, die auf dem Windows-Subsystem für Linux ausführen.
author: scooley
ms.author: scooley
ms.date: 12/20/2017
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.custom: seodec18
ms.openlocfilehash: e4608c25c6bcc63413d53b2c808c16fe2a62dd5c
ms.sourcegitcommit: db69625e26bc141ea379a830790b329e51ed466b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/13/2019
ms.locfileid: "67040816"
---
# <a name="windows-subsystem-for-linux-interoperability-with-windows"></a>Windows-Subsystem für Linux-Interoperabilität mit Windows

> **Aktualisiert für Fall Creators Update.**  
Falls Sie Creators Update oder Anniversary Update ausführen, fahren Sie mit der [Ersteller/Anniversary Update Abschnitt](interop.md#creators-update-and-anniversary-update).

Das Windows-Subsystem für Linux (WSL) wird die Integration zwischen Windows und Linux ständig verbessert.  Sie haben folgende Möglichkeiten:

1. Rufen Sie die Windows-Binärdateien von der Linux-Konsole.
1. Rufen Sie die Linux-Binärdateien von einer Windows-Konsole aus.
1. **Windows-Insider-Builds 17063 +** Umgebungsvariablen zwischen Linux und Windows freigeben.

Dies bietet ein nahtloses Erlebnis zwischen Windows und WSL.  Technische Details sind auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).

## <a name="run-linux-tools-from-a-windows-command-line"></a>Ausführen von Linux-Tools über eine Windows-Befehlszeile

Ausführen von Linux-Binärdateien aus dem Windows-Eingabeaufforderung (CMD oder PowerShell) mit `wsl.exe <command>`.

Binärdateien, die auf diese Weise aufgerufen werden:

1. Verwenden Sie im selben Arbeitsverzeichnis, als der aktuelle cmd- oder PowerShell-Eingabeaufforderung.
1. Führen Sie als Standardbenutzer WSL.
1. Haben Sie die gleichen Windows-Administratorrechte als der aufrufende Prozess und Terminaldienste.

Zum Beispiel:

```console
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

Die folgenden Linux-Befehl `wsl.exe` erfolgt wie jeder Befehl in WSL ausgeführt.  Es funktioniert alles wie "sudo", Piping und Datei-Umleitung.

Beispiel für die Verwendung von "sudo":

```console
C:\temp> wsl sudo apt-get update
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

Beispiele für das Kombinieren von WSL und Windows-Befehle:

```console
C:\temp> wsl ls -la | findstr "foo"
-rwxrwxrwx 1 root root     14 Sep 27 14:26 foo.bat

C:\temp> dir | wsl grep foo
09/27/2016  02:26 PM                14 foo.bat

C:\temp> wsl ls -la > out.txt
```

Übergeben Sie die Befehle in `wsl.exe` an den Prozess WSL ohne Änderung weitergeleitet werden.  Dateipfade müssen im Format WSL angegeben werden.

Beispiel mit Pfaden:

```console
C:\temp> wsl ls -la /proc/cpuinfo
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> wsl ls -la "/mnt/c/Program Files"
<- contents of C:\Program Files ->
```

## <a name="run-windows-tools-from-wsl"></a>Führen Sie die Windows-Tools von WSL

WSL kann Windows-Binärdateien direkt aus der Befehlszeile mit WSL Aufrufen `[binary name].exe`.  Beispiel: `notepad.exe`Hyper-V-Hosts oder Hyper-V-Hostcluster in einem separaten Namespace als verwaltete Hyper-V-Hosts hinzuzufügen.  Um Windows ausführbare Dateien ausführen vereinfachen, ist Windows-Pfad in den Linux enthalten `$PATH` im Fall Creators Update.

Anwendungen, die auf diese Weise ausführen, haben die folgenden Eigenschaften:

1. Behalten Sie als die WSL-Eingabeaufforderung im Arbeitsverzeichnis (zum größten Teil – Ausnahmen werden unten erläutert).
1. Haben Sie die gleichen Berechtigungen Rechte als die WSL-Prozess.
1. Führen Sie als den aktiven Windows-Benutzer.
1. Im Windows Task-Manager angezeigt, als ob direkt über die Eingabeaufforderung ausgeführt.

Beispiel:

``` BASH
$ notepad.exe
```

Führen in WSL ausführbare Windows-Dateien werden auf ähnliche Weise auf native Linux-Dateien –, piping umleitungen und sogar hintergrundverarbeitung arbeiten, wie erwartet verarbeitet.

Beispiele zur Verwendung von Pipes:

``` BASH
$ ipconfig.exe | grep IPv4 | cut -d: -f2
172.21.240.1
10.159.21.24
```

Beispiel für die Verwendung des gemischten Windows und WSL-Befehle:

``` BASH
$ ls -la | findstr.exe foo.txt

$ cmd.exe /c dir
<- contents of C:\ ->
```

Windows-Binärdateien müssen die Dateierweiterung einbeziehen, Groß-/Kleinschreibung der Datei und nicht mehr ausführbar sein.  Nicht-ausführbare Dateien einschließlich batch-Skripts.  Native CMD-Befehle wie `dir` kann ausgeführt werden, mit `cmd.exe /C` Befehl.

Beispiele:

``` BASH
$ cmd.exe /C dir
<- contents of C:\ ->

$ PING.EXE www.microsoft.com
Pinging e1863.dspb.akamaiedge.net [2600:1409:a:5a2::747] with 32 bytes of data:
Reply from 2600:1409:a:5a2::747: time=2ms
```

Parameter werden an die Windows-binäre unverändert übergeben.

Als Beispiel die folgenden Befehle öffnet `C:\temp\foo.txt` in `notepad.exe`:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Ändern die Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einem Windows-Anwendung in WSL wird nicht unterstützt.

In der Standardeinstellung WSL versucht, das Arbeitsverzeichnis für die Windows als aktuelles Verzeichnis WSL binäre zu halten, aber zurückgreift auf der erstellen-Instanz gespeichert, wenn das Arbeitsverzeichnis auf VolFs ist.

Als Beispiel; `wsl.exe` ursprünglich gestartet wird `C:\temp` und das aktuelle WSL-Verzeichnis in der Wohnung des Benutzers geändert wird.  Wenn `notepad.exe` wird aufgerufen, in das Basisverzeichnis des Benutzers WSL automatisch wiederhergestellt `C:\temp` als Arbeitsverzeichnis notepad.exe:

``` BASH
C:\temp> wsl
/mnt/c/temp/$ cd ~
~$ notepad.exe foo.txt
~$ ls | grep foo.txt
~$ exit

exit
C:\temp>dir | findstr foo.txt
09/27/2016  02:15 PM                14 foo.txt
```

## <a name="share-environment-variables-between-windows-and-wsl"></a>Umgebungsvariablen zwischen Windows und WSL freigeben

> In der Windows-Insider-Builds 17063 und höher verfügbar.

Vor dem 17063, nur die Windows-Umgebungsvariable, die WSL zugreifen konnten wurde `PATH` (sodass Sie Win32-ausführbaren Dateien unter WSL starten konnte).

17063 ab, das Freigeben WSL und Windows `WSLENV`, eine spezielle Umgebungsvariable erstellt, um Windows und Linux-Distributionen, die unter WSL zu überbrücken.

Eigenschaften des `WSLENV`:

* Er wird gemeinsam genutzt; Es ist in Windows und WSL vorhanden.
* Es ist eine Liste von Umgebungsvariablen, die von Windows und WSL gemeinsam genutzt.
* Sie können Umgebungsvariablen funktionieren ordnungsgemäß in Windows und WSL formatieren.

Es gibt vier Flags in `WSLENV` beeinflussen, wie diese Umgebungsvariable übersetzt wird.

`WSLENV` Flaggen:

* `/p` -Pfads zwischen WSL/Linux-Style-Pfade und Pfade der Win32-übersetzt.
* `/l` -Gibt an, die Umgebungsvariable ist eine Liste von Pfaden.
* `/u` -Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden sollen, wenn WSL von Win32 ausgeführt wird.
* `/w` -Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden sollen, wenn Win32 von WSL ausgeführt wird.

Flags können kombiniert werden, je nach Bedarf.

## <a name="disable-interop"></a>Deaktivieren von Interop

Benutzer können die Möglichkeit, Windows-Binärdateien für eine einzelne WSL-Sitzung ausgeführt werden, durch den folgenden Befehl als Root ausführen:

``` BASH
$ echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Um Windows erneut aktivieren Binärdateien entweder alle WSL-Sitzungen zu beenden und bash.exe erneut ausführen oder führen den folgenden Befehl als Root-Benutzer:

``` BASH
$ echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Deaktivieren von Interop zwischen den WSL-Sitzungen nicht beibehalten: Interop wird erneut aktiviert werden, wenn eine neue Sitzung gestartet wird.

## <a name="creators-update-and-anniversary-update"></a>Creators Update und Anniversary-Update

Während der Interop-Umgebung vor Herbst Creators Update neuere Interop-Funktionen ähnelt, gibt es jedoch einige wichtige Unterschiede.

Zusammenfassung:

* `bash.exe` ist veraltet und durch ersetzt `wsl.exe`.
* `-c` Option für das Ausführen eines einzelnen Befehls mit nicht benötigt `wsl.exe`.
* Windows-Pfad ist in der WSL enthalten. `$PATH`

Der Prozess zum Deaktivieren von Interop ist unverändert.

### <a name="invoking-wsl-from-the-windows-command-line"></a>Aufrufen von WSL über die Windows-Befehlszeile

Linux-Binärdateien können über die Windows-Eingabeaufforderung oder über PowerShell aufgerufen werden.  Binärdateien, die auf diese Weise aufgerufen haben die folgenden Eigenschaften:

1. Verwenden Sie im selben Arbeitsverzeichnis, als die cmd- oder PowerShell-Eingabeaufforderung.
1. Führen Sie als Standardbenutzer WSL.
1. Haben Sie die gleichen Windows-Administratorrechte als der aufrufende Prozess und Terminaldienste.

Beispiel:

```console
C:\temp> bash -c "ls -la"
```

Linux-Befehle, die auf diese Weise aufgerufen werden wie jede andere Windows-Anwendung verarbeitet.  Z. B. Eingabe, Piping und Datei-Umleitung funktioniert wie erwartet.

Beispiele:

```console
C:\temp>bash -c "sudo apt-get update"
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

```console
C:\temp> bash -c "ls -la" | findstr foo
C:\temp> dir | bash -c "grep foo"
C:\temp> bash -c "ls -la" > out.txt
```

Übergeben Sie die WSL-Befehle in `bash -c` an den Prozess WSL ohne Änderung weitergeleitet werden.  Dateipfade in die WSL-Format angegeben werden müssen und Vorsicht relevanten Zeichen mit Escapezeichen versehen. Beispiel:

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
<- contents of C:\Program Files ->
```

### <a name="invoking-windows-binaries-from-wsl"></a>Aufrufen von Windows-Binärdateien von WSL

Die Windows-Subsystem für Linux können Sie Windows-Binärdateien direkt aus der Befehlszeile WSL aufrufen.  Anwendungen, die auf diese Weise ausführen, haben die folgenden Eigenschaften:

1. Behalten Sie das Arbeitsverzeichnis, als die WSL-Eingabeaufforderung außer in dem Szenario, das die unten beschrieben.
1. Haben Sie die gleichen Berechtigungen Rechte wie die `bash.exe` Prozess. 
1. Führen Sie als den aktiven Windows-Benutzer.
1. Im Windows Task-Manager angezeigt, als ob direkt über die Eingabeaufforderung ausgeführt.

Beispiel:

``` BASH
$ /mnt/c/Windows/System32/notepad.exe
```

In WSL werden diese ausführbaren Dateien wie native Linux ausführbaren Dateien behandelt.  Dies bedeutet, Hinzufügen von Verzeichnissen auf den Linux-Pfad, und zwischen Befehlen ordnungsgemäß weitergeleitet werden, wie erwartet.  Beispiele:

``` BASH
$ export PATH=$PATH:/mnt/c/Windows/System32
$ notepad.exe
$ ipconfig.exe | grep IPv4 | cut -d: -f2
$ ls -la | findstr.exe foo.txt
$ cmd.exe /c dir
```

Die Windows-Binärdatei muss die Dateierweiterung einbeziehen, Groß-/Kleinschreibung der Datei und nicht mehr ausführbar sein.  Nicht-ausführbare Dateien einschließlich batch-Skripts und Befehl wie `dir` kann ausgeführt werden, mit `/mnt/c/Windows/System32/cmd.exe /C` Befehl.

Beispiele:

``` BASH
$ /mnt/c/Windows/System32/cmd.exe /C dir
$ /mnt/c/Windows/System32/PING.EXE www.microsoft.com
```

Parameter werden an die Windows-binäre unverändert übergeben.  

Als Beispiel die folgenden Befehle öffnet `C:\temp\foo.txt` in `notepad.exe`:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Ändern die Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einem Windows Anwendung wird nicht unterstützt.  In der Standardeinstellung WSL versucht, das Arbeitsverzeichnis für die Windows als aktuelles Verzeichnis WSL binäre zu halten, aber zurückgreift auf der erstellen-Instanz gespeichert, wenn das Arbeitsverzeichnis auf VolFs ist.

Als Beispiel; `bash.exe` ursprünglich gestartet wird `C:\temp` und das aktuelle WSL-Verzeichnis in der Wohnung des Benutzers geändert wird.  Wenn `notepad.exe` wird aufgerufen, in das Basisverzeichnis des Benutzers WSL automatisch wiederhergestellt `C:\temp` als Arbeitsverzeichnis notepad.exe:

``` BASH
C:\temp> bash
/mnt/c/temp/$ cd ~
~$ notepad.exe foo.txt
~$ ls | grep foo.txt
~$ exit
exit

C:\temp> dir | findstr foo.txt
09/27/2016  02:15 PM                14 foo.txt
```
