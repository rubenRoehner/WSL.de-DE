---
title: Windows-Interoperabilität mit Linux
description: Beschreibt die Windows-Interoperabilität mit Linux-Distributionen, die im Windows-Subsystem für Linux ausgeführt werden.
ms.date: 12/20/2017
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: f8b0150c044f5011b84e80cac4befd752c4dc552
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269802"
---
# <a name="windows-subsystem-for-linux-interoperability-with-windows"></a>Windows-Subsystem für Linux: Interoperabilität mit Windows

> **Aktualisiert für Fall Creators Update.**  
Wenn Sie Creators Update oder Anniversary Update ausführen, fahren Sie mit dem Abschnitt [Creators/Anniversary Update](interop.md#creators-update-and-anniversary-update) fort.

Das Windows-Subsystem für Linux (WSL) verbessert die Integration zwischen Windows und Linux kontinuierlich.  Sie haben folgende Möglichkeiten:

1. Aufrufen von Windows-Binärdateien über die Linux-Konsole.
1. Aufrufen von Linux-Binärdateien über eine Windows-Konsole.
1. **Windows Insider Build 17063 und höher**: Freigeben von Umgebungsvariablen zwischen Linux und Windows.

Dies bietet eine nahtlose Benutzererfahrung zwischen Windows und WSL.  Technische Details finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).

## <a name="run-linux-tools-from-a-windows-command-line"></a>Ausführen von Linux-Tools über eine Windows-Befehlszeile

Führen Sie Linux-Binärdateien über die Windows-Eingabeaufforderung (CMD oder PowerShell) mithilfe von `wsl.exe <command>` aus.

Auf diese Weise aufgerufene Binärdateien:

1. Verwenden das gleiche Arbeitsverzeichnis wie die aktuelle CMD- oder PowerShell-Eingabeaufforderung.
1. Werden als WSL-Standardbenutzer aus geführt.
1. Verfügen über dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.

Beispiel:

```console
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

Der auf `wsl.exe` folgende Linux-Befehl wird wie ein beliebiger Befehl verarbeitet, der in WSL ausgeführt wird.  Dinge wie sudo, Piping und Dateiumleitung funktionieren.

Beispiel für die Verwendung von sudo:

```console
C:\temp> wsl sudo apt-get update
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

Beispiele für das Mischen von WSL- und Windows-Befehlen:

```console
C:\temp> wsl ls -la | findstr "foo"
-rwxrwxrwx 1 root root     14 Sep 27 14:26 foo.bat

C:\temp> dir | wsl grep foo
09/27/2016  02:26 PM                14 foo.bat

C:\temp> wsl ls -la > out.txt
```

Die an `wsl.exe` übergebenen Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.  Dateipfade müssen im WSL-Format angegeben werden.

Beispiel mit Pfaden:

```console
C:\temp> wsl ls -la /proc/cpuinfo
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> wsl ls -la "/mnt/c/Program Files"
<- contents of C:\Program Files ->
```

## <a name="run-windows-tools-from-wsl"></a>Ausführen von Windows-Tools aus WSL

WSL kann Windows-Binärdateien direkt über die WSL-Befehlszeile mithilfe von `[binary name].exe` aufrufen.  Beispiel: `notepad.exe`.  Damit ausführbare Windows-Dateien einfacher ausgeführt werden können, ist der Windows-Pfad im Fall Creators Update in `$PATH` von Linux enthalten.

Anwendungen, die auf diese Weise ausgeführt werden, besitzen die folgenden Eigenschaften:

1. Sie behalten das Arbeitsverzeichnis als das Verzeichnis der WSL-Eingabeaufforderung bei (in den meisten Fällen, Ausnahmen werden unten erläutert).
1. Sie verfügen über die gleichen Berechtigungen wie der WSL-Prozess.
1. Sie werden als aktiver Windows-Benutzer ausgeführt.
1. Sie werden im Task-Manager von Windows so angezeigt, als würden die direkt über die CMD-Eingabeaufforderung ausgeführt.

Beispiel:

``` BASH
$ notepad.exe
```

Ausführbare Windows-Dateien, die in WSL ausgeführt werden, werden ähnlich wie native ausführbare Linux-Dateien verarbeitet. Piping, Umleitungen und sogar Hintergrundverarbeitung funktionieren wie erwartet.

Beispiele für die Verwendung von Pipes:

``` BASH
$ ipconfig.exe | grep IPv4 | cut -d: -f2
172.21.240.1
10.159.21.24
```

Beispiel für die Verwendung gemischter Windows- und WSL-Befehle:

``` BASH
$ ls -la | findstr.exe foo.txt

$ cmd.exe /c dir
<- contents of C:\ ->
```

Windows-Binärdateien müssen die Dateierweiterung enthalten, der Groß-/Kleinschreibung der Datei Rechnung tragen und ausführbare Dateien sein.  Nicht ausführbare Dateien, einschließlich Batchskripts.  Native CMD-Befehle wie `dir` können mit einem Befehl `cmd.exe /C` ausgeführt werden.

Beispiele:

``` BASH
$ cmd.exe /C dir
<- contents of C:\ ->

$ PING.EXE www.microsoft.com
Pinging e1863.dspb.akamaiedge.net [2600:1409:a:5a2::747] with 32 bytes of data:
Reply from 2600:1409:a:5a2::747: time=2ms
```

Parameter werden unverändert an die Windows-Binärdatei übergeben.

Beispielsweise öffnen die folgenden Befehle `C:\temp\foo.txt` in `notepad.exe`:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Das Ändern von Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einer Windows-Anwendung in WSL wird nicht unterstützt.

Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als aktuelles WSL-Verzeichnis beizubehalten, greift aber auf das Instanzerstellungsverzeichnis zurück, wenn sich das Arbeitsverzeichnis in VolFs befindet.

Beispiel: `wsl.exe` wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in das Basisverzeichnis des Benutzers geändert.  Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, setzt WSL automatisch auf `C:\temp` als das Arbeitsverzeichnis von „notepad.exe“ zurück:

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

> Verfügbar in Windows Insider Build 17063 und höher.

Vor 17063 war `PATH` die einzige Windows-Umgebungsvariable, auf die WSL zugreifen konnte (sodass Sie ausführbare Win32-Dateien unter WSL starten konnten).

Ab 17063 verwenden WSL und Windows `WSLENV`, eine spezielle Umgebungsvariable, die entwickelt wurde, um Windows und Linux-Distributionen, die unter WSL ausgeführt werden, zu verbinden.

Eigenschaften von `WSLENV`:

* Die Variable ist freigegeben, und sie ist sowohl in Windows- als auch in WSL-Umgebungen vorhanden.
* Es handelt sich um eine Liste von Umgebungsvariablen, die von Windows und WSL gemeinsam genutzt werden können.
* Sie kann Umgebungsvariablen so formatieren, dass sie in Windows und WSL gut funktionieren.

In `WSLENV` sind vier Flags verfügbar, die beeinflussen, wie diese Umgebungsvariable übersetzt wird.

`WSLENV`-Flags:

* `/p`: Übersetzt den Pfad zwischen Pfaden im WSL-/Linux-Stil und Win32-Pfaden.
* `/l`: Gibt an, dass die Umgebungsvariable eine Liste von Pfaden ist.
* `/u`: Gibt an, dass diese Umgebungsvariable nur beim Ausführen von WSL aus Win32 einbezogen werden soll.
* `/w`: Gibt an, dass diese Umgebungsvariable nur beim Ausführen von Win32 aus WSL einbezogen werden soll.

Diese Flags können nach Bedarf kombiniert werden.

## <a name="disable-interop"></a>Deaktivieren von Interop

Benutzer können die Möglichkeit zum Ausführen von Windows-Binärdateien für eine einzelne WSL-Sitzung deaktivieren, indem Sie den folgenden Befehl als root ausführen:

``` BASH
$ echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Zum erneuten Aktivieren von Windows-Binärdateien beenden Sie entweder alle WSL-Sitzungen und führen „bash.exe“ erneut aus, oder führen Sie den folgenden Befehl als root aus:

``` BASH
$ echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

Die Deaktivierung von Interop wird nicht zwischen WSL-Sitzungen beibehalten. Interop wird erneut aktiviert, wenn eine neue Sitzung gestartet wird.

## <a name="creators-update-and-anniversary-update"></a>Creators Update und Anniversary Update

Während das Interopverhalten vor dem Fall Creators Update aktuellem Interopverhalten ähnelt, gibt es einige wichtige Unterschiede.

Zusammenfassung:

* `bash.exe` wurde als veraltet erklärt und durch `wsl.exe` ersetzt.
* Die `-c`-Option zum Ausführen eines einzelnen Befehls ist mit `wsl.exe` nicht erforderlich.
* Der Windows-Pfad ist in `$PATH` von WSL enthalten.

Der Prozess zum Deaktivieren von Interop ist unverändert.

### <a name="invoking-wsl-from-the-windows-command-line"></a>Aufrufen von WSL über die Windows-Befehlszeile

Linux-Binärdateien können über die Windows-Eingabeaufforderung oder aus PowerShell aufgerufen werden.  Binärdateien, die auf diese Weise aufgerufen werden, besitzen die folgenden Eigenschaften:

1. Sie verwenden das gleiche Arbeitsverzeichnis wie die CMD- oder PowerShell-Eingabeaufforderung.
1. Sie werden als WSL-Standardbenutzer ausgeführt.
1. Sie verfügen über dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.

Beispiel:

```console
C:\temp> bash -c "ls -la"
```

Linux-Befehle, die auf diese Weise aufgerufen werden, werden wie jede andere Windows-Anwendung behandelt.  Dinge wie Eingabe, Piping und Dateiumleitung funktionieren erwartungsgemäß.

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

Die an `bash -c` übergebenen WSL-Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.  Dateipfade müssen im WSL-Format angegeben werden, und es muss darauf geachtet werden, dass relevante Zeichen mit Escapezeichen versehen werden. Beispiel:

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
<- contents of C:\Program Files ->
```

### <a name="invoking-windows-binaries-from-wsl"></a>Aufrufen von Windows-Binärdateien aus WSL

Das Windows-Subsystem für Linux kann Windows-Binärdateien direkt über die WSL-Befehlszeile aufrufen.  Anwendungen, die auf diese Weise ausgeführt werden, besitzen die folgenden Eigenschaften:

1. Sie behalten das Arbeitsverzeichnis als das Verzeichnis der WSL-Eingabeaufforderung bei. Eine Ausnahme bildet das unten erläuterte Szenario.
1. Sie verfügen über die gleichen Berechtigungen wie der `bash.exe`-Prozess. 
1. Sie werden als aktiver Windows-Benutzer ausgeführt.
1. Sie werden im Task-Manager von Windows so angezeigt, als würden die direkt über die CMD-Eingabeaufforderung ausgeführt.

Beispiel:

``` BASH
$ /mnt/c/Windows/System32/notepad.exe
```

In WSL werden diese ausführbaren Dateien ähnlich wie native ausführbare Linux-Dateien behandelt.  Dies bedeutet, dass das Hinzufügen von Verzeichnissen zum Linux-Pfad und das Piping zwischen Befehlen erwartungsgemäß funktioniert.  Beispiele:

``` BASH
$ export PATH=$PATH:/mnt/c/Windows/System32
$ notepad.exe
$ ipconfig.exe | grep IPv4 | cut -d: -f2
$ ls -la | findstr.exe foo.txt
$ cmd.exe /c dir
```

Die Windows-Binärdatei muss die Dateierweiterung enthalten, der Groß-/Kleinschreibung der Datei Rechnung tragen und eine ausführbare Dateien sein.  Nicht ausführbare Dateien einschließlich Batchskripts und Befehle wie `dir` können mit dem Befehl `/mnt/c/Windows/System32/cmd.exe /C` ausgeführt werden.

Beispiele:

``` BASH
$ /mnt/c/Windows/System32/cmd.exe /C dir
$ /mnt/c/Windows/System32/PING.EXE www.microsoft.com
```

Parameter werden unverändert an die Windows-Binärdatei übergeben.  

Beispielsweise öffnen die folgenden Befehle `C:\temp\foo.txt` in `notepad.exe`:

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

Das Ändern von Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einer Windows-Anwendung wird nicht unterstützt.  Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als aktuelles WSL-Verzeichnis beizubehalten, greift aber auf das Instanzerstellungsverzeichnis zurück, wenn sich das Arbeitsverzeichnis in VolFs befindet.

Beispiel: `bash.exe` wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in das Basisverzeichnis des Benutzers geändert.  Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, setzt WSL automatisch auf `C:\temp` als das Arbeitsverzeichnis von „notepad.exe“ zurück:

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
