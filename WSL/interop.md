---
title: Windows-Interoperabilität mit Linux
description: Beschreibt die Windows-Interoperabilität mit Linux-Distributionen, die im Windows-Subsystem für Linux ausgeführt werden.
author: scooley
ms.author: scooley
ms.date: 12/20/2017
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.custom: seodec18
ms.openlocfilehash: e4608c25c6bcc63413d53b2c808c16fe2a62dd5c
ms.sourcegitcommit: cd239efc5c7c25ffbe5de25b2438d44181a838a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/14/2019
ms.locfileid: "67040816"
---
# <a name="windows-subsystem-for-linux-interoperability-with-windows"></a>Windows-Subsystem für Linux-Interoperabilität mit Windows

> **Das Thema wurde für das Fall Creators Update aktualisiert.**  
Wenn Sie Creators Update oder Anniversary Update ausführen, springen Sie zum [Abschnitt Creators/Anniversary Update](interop.md#creators-update-and-anniversary-update).

Das Windows-Subsystem für Linux (WSL) verbessert die Integration zwischen Windows und Linux kontinuierlich.  Sie haben folgende Möglichkeiten:

1. Aufrufen von Windows-Binärdateien über die Linux-Konsole.
1. Aufrufen von Linux-Binärdateien von einer Windows-Konsole aus.
1. **Windows Insider erstellt 17063 +** Freigeben von Umgebungsvariablen zwischen Linux und Windows.

Dies bietet eine nahtlose Darstellung zwischen Windows und WSL.  Technische Details finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).

## <a name="run-linux-tools-from-a-windows-command-line"></a>Ausführen von Linux-Tools über eine Windows-Befehlszeile

Ausführen von Linux-Binärdateien an der Windows-Eingabeaufforderung (cmd oder PowerShell) mithilfe `wsl.exe <command>`von.

Auf diese Weise aufgerufene Binärdateien:

1. Verwenden Sie das gleiche Arbeitsverzeichnis wie bei der aktuellen cmd-oder PowerShell-Eingabeaufforderung.
1. Führen Sie als WSL-Standardbenutzer aus.
1. Sie haben dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.

Zum Beispiel:

```console
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

Der folgende `wsl.exe` Linux-Befehl wird wie ein beliebiger Befehl verarbeitet, der in WSL ausgeführt wird.  Dinge wie "sudo", "Piping" und "Datei Umleitung" funktionieren.

Beispiel für die Verwendung von sudo:

```console
C:\temp> wsl sudo apt-get update
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

Beispiele zum Mischen von WSL-und Windows-Befehlen:

```console
C:\temp> wsl ls -la | findstr "foo"
-rwxrwxrwx 1 root root     14 Sep 27 14:26 foo.bat

C:\temp> dir | wsl grep foo
09/27/2016  02:26 PM                14 foo.bat

C:\temp> wsl ls -la > out.txt
```

Die an weiter `wsl.exe` gegebenen Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.  Dateipfade müssen im WSL-Format angegeben werden.

Beispiel mit Pfaden:

```console
C:\temp> wsl ls -la /proc/cpuinfo
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> wsl ls -la "/mnt/c/Program Files"
<- contents of C:\Program Files ->
```

## <a name="run-windows-tools-from-wsl"></a>Ausführen von Windows-Tools aus WSL

WSL kann Windows-Binärdateien direkt über die WSL-Befehlszeile `[binary name].exe`mithilfe von aufrufen.  Beispiel: `notepad.exe`Hyper-V-Hosts oder Hyper-V-Hostcluster in einem separaten Namespace als verwaltete Hyper-V-Hosts hinzuzufügen.  Damit ausführbare Windows-Dateien einfacher ausgeführt werden können, ist Windows Path im Fall Creators `$PATH` Update in Linux enthalten.

Anwendungen, die auf diese Weise ausgeführt werden, haben die folgenden Eigenschaften:

1. Behalten Sie das Arbeitsverzeichnis als WSL-Eingabeaufforderung bei (in den meisten Fällen werden die Ausnahmen unten erläutert).
1. Sie müssen über die gleichen Berechtigungs Rechte wie der WSL-Prozess verfügen.
1. Führen Sie als aktiver Windows-Benutzer aus.
1. Wird im Windows Task-Manager so angezeigt, als ob er direkt von der cmd-Eingabeaufforderung ausgeführt wird.

Beispiel:

``` BASH
$ notepad.exe
```

Ausführbare Windows-Dateien, die in WSL ausgeführt werden, werden ähnlich wie Native ausführbare Linux-Dateien verarbeitet

Beispiele für die Verwendung von Pipes:

``` BASH
$ ipconfig.exe | grep IPv4 | cut -d: -f2
172.21.240.1
10.159.21.24
```

Beispiel für die Verwendung gemischter Windows-und WSL-Befehle:

``` BASH
$ ls -la | findstr.exe foo.txt

$ cmd.exe /c dir
<- contents of C:\ ->
```

Windows-Binärdateien müssen die Dateierweiterung enthalten, dem Datei Fall entsprechen und ausführbare Dateien sein.  Nicht ausführbare Dateien, einschließlich Batch Skripts.  Native cmd-Befehle `dir` wie können mit `cmd.exe /C` einem Befehl ausgeführt werden.

Beispiele:

``` BASH
$ cmd.exe /C dir
<- contents of C:\ ->

$ PING.EXE www.microsoft.com
Pinging e1863.dspb.akamaiedge.net [2600:1409:a:5a2::747] with 32 bytes of data:
Reply from 2600:1409:a:5a2::747: time=2ms
```

Parameter werden unverändert an die Windows-Binärdatei (Binary) übermittelt.

Beispielsweise werden die folgenden Befehle in `C:\temp\foo.txt` `notepad.exe`geöffnet:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Das Ändern von Dateien, die sich auf volfs `/mnt/<x>`(Dateien nicht unter) mit einer Windows-Anwendung in WSL befinden, wird nicht unterstützt.

Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als Aktuelles WSL-Verzeichnis beizubehalten. wenn sich das Arbeitsverzeichnis auf "volfs" befindet, wird das Verzeichnis für die Instanzerstellung zurückgegriffen.

Beispiel: wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in die Startseite des Benutzers geändert. `wsl.exe`  Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, wird WSL automatisch `C:\temp` als "Notepad. exe"-Arbeitsverzeichnis wieder hergestellt:

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

## <a name="share-environment-variables-between-windows-and-wsl"></a>Freigeben von Umgebungsvariablen zwischen Windows und WSL

> Verfügbar in Windows Insider-Builds 17063 und höher.

Vor 17063 war `PATH` nur die Windows-Umgebungsvariable, auf die WSL zugreifen konnte (sodass Sie ausführbare Win32-Dateien unter WSL starten konnten).

Ab 17063, WSL und Windows Share `WSLENV`, eine spezielle Umgebungsvariable, die zum Überbrücken von Windows-und Linux-Distributionen erstellt wird, die auf WSL ausgeführt werden.

Eigenschaften von `WSLENV`:

* Es ist freigegeben. Es ist sowohl in Windows-als auch in WSL-Umgebungen vorhanden.
* Es handelt sich um eine Liste von Umgebungsvariablen, die zwischen Windows und WSL gemeinsam genutzt werden können.
* Sie können Umgebungsvariablen so formatieren, dass Sie in Windows und WSL gut funktionieren.

In `WSLENV` sind vier Flags verfügbar, die beeinflussen, wie die Umgebungsvariable übersetzt wird.

`WSLENV`fahren

* `/p`: übersetzt den Pfad zwischen WSL-/Linux-stylepfaden und Win32-Pfaden.
* `/l`-Gibt an, dass die Umgebungsvariable eine Liste von Pfaden ist.
* `/u`: gibt an, dass diese Umgebungsvariable nur beim Ausführen von WSL von Win32 eingeschlossen werden soll.
* `/w`Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden soll, wenn Win32 von WSL aus ausgeführt wird.

Flags können nach Bedarf kombiniert werden.

## <a name="disable-interop"></a>Interop deaktivieren

Benutzer können die Möglichkeit zum Ausführen von Windows-Binärdateien für eine einzelne WSL-Sitzung deaktivieren, indem Sie den folgenden Befehl als Root-Befehl ausführen:

``` BASH
$ echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Zum erneuten Aktivieren von Windows-Binärdateien beenden Sie entweder alle WSL-Sitzungen, führen Sie bash. exe erneut aus, oder führen Sie den folgenden Befehl als root aus:

``` BASH
$ echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Das Deaktivieren von Interop wird nicht zwischen WSL-Sitzungen beibehalten--Interop wird erneut aktiviert, wenn eine neue Sitzung gestartet wird.

## <a name="creators-update-and-anniversary-update"></a>Creators Update und Anniversary Update

Während das Interop-erstellerupdate vor Fall der aktuellen Interop-Erfahrung ähnelt, gibt es einige wichtige Unterschiede.

Zusammenfassung:

* `bash.exe`wurde als veraltet markiert und durch ersetzt `wsl.exe`.
* `-c`die Option zum Ausführen eines einzelnen Befehls ist mit `wsl.exe`nicht erforderlich.
* Der Windows-Pfad ist im WSL enthalten.`$PATH`

Der Prozess zum Deaktivieren der Interop ist unverändert.

### <a name="invoking-wsl-from-the-windows-command-line"></a>Aufrufen von WSL von der Windows-Befehlszeile aus

Linux-Binärdateien können von der Windows-Eingabeaufforderung oder von PowerShell aufgerufen werden.  Auf diese Weise aufgerufene Binärdateien verfügen über die folgenden Eigenschaften:

1. Verwenden Sie das gleiche Arbeitsverzeichnis wie die CMD-oder PowerShell-Eingabeaufforderung.
1. Führen Sie als WSL-Standardbenutzer aus.
1. Sie haben dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.

Beispiel:

```console
C:\temp> bash -c "ls -la"
```

Linux-Befehle, die auf diese Weise aufgerufen werden, werden wie jede andere Windows-Anwendung behandelt.  Dinge wie Eingabe, Piping und Datei Umleitung funktionieren erwartungsgemäß.

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

Die an weiter `bash -c` gegebenen WSL-Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.  Dateipfade müssen im WSL-Format angegeben werden, und es muss darauf geachtet werden, dass relevante Zeichen mit Escapezeichen versehen werden. Beispiel:

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
<- contents of C:\Program Files ->
```

### <a name="invoking-windows-binaries-from-wsl"></a>Aufrufen von Windows-Binärdateien aus WSL

Das Windows-Subsystem für Linux kann Windows-Binärdateien direkt über die WSL-Befehlszeile aufrufen.  Anwendungen, die auf diese Weise ausgeführt werden, haben die folgenden Eigenschaften:

1. Behalten Sie das Arbeitsverzeichnis als WSL-Eingabeaufforderung mit Ausnahme des unten beschriebenen Szenarios bei.
1. Sie müssen über die gleichen Berechtigungs `bash.exe` Rechte wie der Prozess verfügen. 
1. Führen Sie als aktiver Windows-Benutzer aus.
1. Wird im Windows Task-Manager so angezeigt, als ob er direkt von der cmd-Eingabeaufforderung ausgeführt wird.

Beispiel:

``` BASH
$ /mnt/c/Windows/System32/notepad.exe
```

In WSL werden diese ausführbaren Dateien ähnlich wie Native ausführbare Linux-Dateien behandelt.  Dies bedeutet, dass das Hinzufügen von Verzeichnissen zum Linux-Pfad und die Weiterleitung zwischen Befehlen erwartungsgemäß funktioniert.  Beispiele:

``` BASH
$ export PATH=$PATH:/mnt/c/Windows/System32
$ notepad.exe
$ ipconfig.exe | grep IPv4 | cut -d: -f2
$ ls -la | findstr.exe foo.txt
$ cmd.exe /c dir
```

Die Windows-Binärdatei muss die Dateierweiterung enthalten, dem Datei Fall entsprechen und ausführbare Dateien sein.  Nicht ausführbare Dateien einschließlich Batch Skripts und Befehls like `dir` können mit `/mnt/c/Windows/System32/cmd.exe /C` einem Befehl ausgeführt werden.

Beispiele:

``` BASH
$ /mnt/c/Windows/System32/cmd.exe /C dir
$ /mnt/c/Windows/System32/PING.EXE www.microsoft.com
```

Parameter werden unverändert an die Windows-Binärdatei (Binary) übermittelt.  

Beispielsweise werden die folgenden Befehle in `C:\temp\foo.txt` `notepad.exe`geöffnet:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Das Ändern von Dateien in volfs (Dateien nicht `/mnt/<x>`unter) mit einer Windows-Anwendung wird nicht unterstützt.  Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als Aktuelles WSL-Verzeichnis beizubehalten. wenn sich das Arbeitsverzeichnis auf "volfs" befindet, wird das Verzeichnis für die Instanzerstellung zurückgegriffen.

Beispiel: wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in die Startseite des Benutzers geändert. `bash.exe`  Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, wird WSL automatisch `C:\temp` als "Notepad. exe"-Arbeitsverzeichnis wieder hergestellt:

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
