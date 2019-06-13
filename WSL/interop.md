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
# <a name="windows-subsystem-for-linux-interoperability-with-windows"></a><span data-ttu-id="5b349-103">Windows-Subsystem für Linux-Interoperabilität mit Windows</span><span class="sxs-lookup"><span data-stu-id="5b349-103">Windows Subsystem for Linux interoperability with Windows</span></span>

> <span data-ttu-id="5b349-104">**Aktualisiert für Fall Creators Update.**</span><span class="sxs-lookup"><span data-stu-id="5b349-104">**Updated for Fall Creators Update.**</span></span>  
<span data-ttu-id="5b349-105">Falls Sie Creators Update oder Anniversary Update ausführen, fahren Sie mit der [Ersteller/Anniversary Update Abschnitt](interop.md#creators-update-and-anniversary-update).</span><span class="sxs-lookup"><span data-stu-id="5b349-105">If you're running Creators Update or Anniversary Update, jump to the [Creators/Anniversary Update section](interop.md#creators-update-and-anniversary-update).</span></span>

<span data-ttu-id="5b349-106">Das Windows-Subsystem für Linux (WSL) wird die Integration zwischen Windows und Linux ständig verbessert.</span><span class="sxs-lookup"><span data-stu-id="5b349-106">The Windows Subsystem for Linux (WSL) is continuously improving integration between Windows and Linux.</span></span>  <span data-ttu-id="5b349-107">Sie haben folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="5b349-107">You can:</span></span>

1. <span data-ttu-id="5b349-108">Rufen Sie die Windows-Binärdateien von der Linux-Konsole.</span><span class="sxs-lookup"><span data-stu-id="5b349-108">Invoke Windows binaries from the Linux console.</span></span>
1. <span data-ttu-id="5b349-109">Rufen Sie die Linux-Binärdateien von einer Windows-Konsole aus.</span><span class="sxs-lookup"><span data-stu-id="5b349-109">Invoke Linux binaries from a Windows console.</span></span>
1. <span data-ttu-id="5b349-110">**Windows-Insider-Builds 17063 +** Umgebungsvariablen zwischen Linux und Windows freigeben.</span><span class="sxs-lookup"><span data-stu-id="5b349-110">**Windows Insiders Builds 17063+** Share environment variables between Linux and Windows.</span></span>

<span data-ttu-id="5b349-111">Dies bietet ein nahtloses Erlebnis zwischen Windows und WSL.</span><span class="sxs-lookup"><span data-stu-id="5b349-111">This delivers a seamless experience between Windows and WSL.</span></span>  <span data-ttu-id="5b349-112">Technische Details sind auf die [WSL Blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).</span><span class="sxs-lookup"><span data-stu-id="5b349-112">Technical details are on the [WSL blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).</span></span>

## <a name="run-linux-tools-from-a-windows-command-line"></a><span data-ttu-id="5b349-113">Ausführen von Linux-Tools über eine Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="5b349-113">Run Linux tools from a Windows command line</span></span>

<span data-ttu-id="5b349-114">Ausführen von Linux-Binärdateien aus dem Windows-Eingabeaufforderung (CMD oder PowerShell) mit `wsl.exe <command>`.</span><span class="sxs-lookup"><span data-stu-id="5b349-114">Run Linux binaries from the Windows Command Prompt (CMD or PowerShell) using `wsl.exe <command>`.</span></span>

<span data-ttu-id="5b349-115">Binärdateien, die auf diese Weise aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="5b349-115">Binaries invoked in this way:</span></span>

1. <span data-ttu-id="5b349-116">Verwenden Sie im selben Arbeitsverzeichnis, als der aktuelle cmd- oder PowerShell-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="5b349-116">Use the same working directory as the current CMD or PowerShell prompt.</span></span>
1. <span data-ttu-id="5b349-117">Führen Sie als Standardbenutzer WSL.</span><span class="sxs-lookup"><span data-stu-id="5b349-117">Run as the WSL default user.</span></span>
1. <span data-ttu-id="5b349-118">Haben Sie die gleichen Windows-Administratorrechte als der aufrufende Prozess und Terminaldienste.</span><span class="sxs-lookup"><span data-stu-id="5b349-118">Have the same Windows administrative rights as the calling process and terminal.</span></span>

<span data-ttu-id="5b349-119">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5b349-119">For example:</span></span>

```console
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

<span data-ttu-id="5b349-120">Die folgenden Linux-Befehl `wsl.exe` erfolgt wie jeder Befehl in WSL ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5b349-120">The Linux command following `wsl.exe` is handled like any command run in WSL.</span></span>  <span data-ttu-id="5b349-121">Es funktioniert alles wie "sudo", Piping und Datei-Umleitung.</span><span class="sxs-lookup"><span data-stu-id="5b349-121">Things such as sudo, piping, and file redirection work.</span></span>

<span data-ttu-id="5b349-122">Beispiel für die Verwendung von "sudo":</span><span class="sxs-lookup"><span data-stu-id="5b349-122">Example using sudo:</span></span>

```console
C:\temp> wsl sudo apt-get update
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

<span data-ttu-id="5b349-123">Beispiele für das Kombinieren von WSL und Windows-Befehle:</span><span class="sxs-lookup"><span data-stu-id="5b349-123">Examples mixing WSL and Windows commands:</span></span>

```console
C:\temp> wsl ls -la | findstr "foo"
-rwxrwxrwx 1 root root     14 Sep 27 14:26 foo.bat

C:\temp> dir | wsl grep foo
09/27/2016  02:26 PM                14 foo.bat

C:\temp> wsl ls -la > out.txt
```

<span data-ttu-id="5b349-124">Übergeben Sie die Befehle in `wsl.exe` an den Prozess WSL ohne Änderung weitergeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="5b349-124">The commands passed into `wsl.exe` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="5b349-125">Dateipfade müssen im Format WSL angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="5b349-125">File paths must be specified in the WSL format.</span></span>

<span data-ttu-id="5b349-126">Beispiel mit Pfaden:</span><span class="sxs-lookup"><span data-stu-id="5b349-126">Example with paths:</span></span>

```console
C:\temp> wsl ls -la /proc/cpuinfo
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> wsl ls -la "/mnt/c/Program Files"
<- contents of C:\Program Files ->
```

## <a name="run-windows-tools-from-wsl"></a><span data-ttu-id="5b349-127">Führen Sie die Windows-Tools von WSL</span><span class="sxs-lookup"><span data-stu-id="5b349-127">Run Windows tools from WSL</span></span>

<span data-ttu-id="5b349-128">WSL kann Windows-Binärdateien direkt aus der Befehlszeile mit WSL Aufrufen `[binary name].exe`.</span><span class="sxs-lookup"><span data-stu-id="5b349-128">WSL can invoke Windows binaries directly from the WSL command line using `[binary name].exe`.</span></span>  <span data-ttu-id="5b349-129">Beispiel: `notepad.exe`Hyper-V-Hosts oder Hyper-V-Hostcluster in einem separaten Namespace als verwaltete Hyper-V-Hosts hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="5b349-129">For example, `notepad.exe`.</span></span>  <span data-ttu-id="5b349-130">Um Windows ausführbare Dateien ausführen vereinfachen, ist Windows-Pfad in den Linux enthalten `$PATH` im Fall Creators Update.</span><span class="sxs-lookup"><span data-stu-id="5b349-130">To make Windows executables easier to run, Windows path is included in the Linux `$PATH` in Fall Creators Update.</span></span>

<span data-ttu-id="5b349-131">Anwendungen, die auf diese Weise ausführen, haben die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="5b349-131">Applications run this way have the following properties:</span></span>

1. <span data-ttu-id="5b349-132">Behalten Sie als die WSL-Eingabeaufforderung im Arbeitsverzeichnis (zum größten Teil – Ausnahmen werden unten erläutert).</span><span class="sxs-lookup"><span data-stu-id="5b349-132">Retain the working directory as the WSL command prompt (for the most part -- exceptions are explained below).</span></span>
1. <span data-ttu-id="5b349-133">Haben Sie die gleichen Berechtigungen Rechte als die WSL-Prozess.</span><span class="sxs-lookup"><span data-stu-id="5b349-133">Have the same permission rights as the WSL process.</span></span>
1. <span data-ttu-id="5b349-134">Führen Sie als den aktiven Windows-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5b349-134">Run as the active Windows user.</span></span>
1. <span data-ttu-id="5b349-135">Im Windows Task-Manager angezeigt, als ob direkt über die Eingabeaufforderung ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5b349-135">Appear in the Windows Task Manager as if directly executed from the CMD prompt.</span></span>

<span data-ttu-id="5b349-136">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5b349-136">Example:</span></span>

``` BASH
$ notepad.exe
```

<span data-ttu-id="5b349-137">Führen in WSL ausführbare Windows-Dateien werden auf ähnliche Weise auf native Linux-Dateien –, piping umleitungen und sogar hintergrundverarbeitung arbeiten, wie erwartet verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="5b349-137">Windows executables run in WSL are handled similarly to native Linux executables -- piping, redirects, and even backgrounding work as expected.</span></span>

<span data-ttu-id="5b349-138">Beispiele zur Verwendung von Pipes:</span><span class="sxs-lookup"><span data-stu-id="5b349-138">Examples using pipes:</span></span>

``` BASH
$ ipconfig.exe | grep IPv4 | cut -d: -f2
172.21.240.1
10.159.21.24
```

<span data-ttu-id="5b349-139">Beispiel für die Verwendung des gemischten Windows und WSL-Befehle:</span><span class="sxs-lookup"><span data-stu-id="5b349-139">Example using mixed Windows and WSL commands:</span></span>

``` BASH
$ ls -la | findstr.exe foo.txt

$ cmd.exe /c dir
<- contents of C:\ ->
```

<span data-ttu-id="5b349-140">Windows-Binärdateien müssen die Dateierweiterung einbeziehen, Groß-/Kleinschreibung der Datei und nicht mehr ausführbar sein.</span><span class="sxs-lookup"><span data-stu-id="5b349-140">Windows binaries must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="5b349-141">Nicht-ausführbare Dateien einschließlich batch-Skripts.</span><span class="sxs-lookup"><span data-stu-id="5b349-141">Non-executables including batch scripts.</span></span>  <span data-ttu-id="5b349-142">Native CMD-Befehle wie `dir` kann ausgeführt werden, mit `cmd.exe /C` Befehl.</span><span class="sxs-lookup"><span data-stu-id="5b349-142">CMD native commands like `dir` can be run with `cmd.exe /C` command.</span></span>

<span data-ttu-id="5b349-143">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="5b349-143">Examples:</span></span>

``` BASH
$ cmd.exe /C dir
<- contents of C:\ ->

$ PING.EXE www.microsoft.com
Pinging e1863.dspb.akamaiedge.net [2600:1409:a:5a2::747] with 32 bytes of data:
Reply from 2600:1409:a:5a2::747: time=2ms
```

<span data-ttu-id="5b349-144">Parameter werden an die Windows-binäre unverändert übergeben.</span><span class="sxs-lookup"><span data-stu-id="5b349-144">Parameters are passed to the Windows binary unmodified.</span></span>

<span data-ttu-id="5b349-145">Als Beispiel die folgenden Befehle öffnet `C:\temp\foo.txt` in `notepad.exe`:</span><span class="sxs-lookup"><span data-stu-id="5b349-145">As an example, the following commands will open `C:\temp\foo.txt` in `notepad.exe`:</span></span>

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

<span data-ttu-id="5b349-146">Ändern die Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einem Windows-Anwendung in WSL wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b349-146">Modifying files located on VolFs (files not under `/mnt/<x>`) with a Windows application in WSL is not supported.</span></span>

<span data-ttu-id="5b349-147">In der Standardeinstellung WSL versucht, das Arbeitsverzeichnis für die Windows als aktuelles Verzeichnis WSL binäre zu halten, aber zurückgreift auf der erstellen-Instanz gespeichert, wenn das Arbeitsverzeichnis auf VolFs ist.</span><span class="sxs-lookup"><span data-stu-id="5b349-147">By default, WSL tries to keep the working directory of the Windows binary as the current WSL directory, but will fall back on the instance creation directory if the working directory is on VolFs.</span></span>

<span data-ttu-id="5b349-148">Als Beispiel; `wsl.exe` ursprünglich gestartet wird `C:\temp` und das aktuelle WSL-Verzeichnis in der Wohnung des Benutzers geändert wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-148">As an example; `wsl.exe` is initially launched from `C:\temp` and the current WSL directory is changed to the user’s home.</span></span>  <span data-ttu-id="5b349-149">Wenn `notepad.exe` wird aufgerufen, in das Basisverzeichnis des Benutzers WSL automatisch wiederhergestellt `C:\temp` als Arbeitsverzeichnis notepad.exe:</span><span class="sxs-lookup"><span data-stu-id="5b349-149">When `notepad.exe` is called from the user’s home directory, WSL automatically reverts to `C:\temp` as the notepad.exe working directory:</span></span>

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

## <a name="share-environment-variables-between-windows-and-wsl"></a><span data-ttu-id="5b349-150">Umgebungsvariablen zwischen Windows und WSL freigeben</span><span class="sxs-lookup"><span data-stu-id="5b349-150">Share environment variables between Windows and WSL</span></span>

> <span data-ttu-id="5b349-151">In der Windows-Insider-Builds 17063 und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5b349-151">Available in Windows Insider builds 17063 and later.</span></span>

<span data-ttu-id="5b349-152">Vor dem 17063, nur die Windows-Umgebungsvariable, die WSL zugreifen konnten wurde `PATH` (sodass Sie Win32-ausführbaren Dateien unter WSL starten konnte).</span><span class="sxs-lookup"><span data-stu-id="5b349-152">Prior to 17063, only Windows environment variable that WSL could access was `PATH` (so you could launch Win32 executables from under WSL).</span></span>

<span data-ttu-id="5b349-153">17063 ab, das Freigeben WSL und Windows `WSLENV`, eine spezielle Umgebungsvariable erstellt, um Windows und Linux-Distributionen, die unter WSL zu überbrücken.</span><span class="sxs-lookup"><span data-stu-id="5b349-153">Starting in 17063, WSL and Windows share `WSLENV`, a special environment variable created to bridge Windows and Linux distros running on WSL.</span></span>

<span data-ttu-id="5b349-154">Eigenschaften des `WSLENV`:</span><span class="sxs-lookup"><span data-stu-id="5b349-154">Properties of `WSLENV`:</span></span>

* <span data-ttu-id="5b349-155">Er wird gemeinsam genutzt; Es ist in Windows und WSL vorhanden.</span><span class="sxs-lookup"><span data-stu-id="5b349-155">It is shared; it exists in both Windows and WSL environments.</span></span>
* <span data-ttu-id="5b349-156">Es ist eine Liste von Umgebungsvariablen, die von Windows und WSL gemeinsam genutzt.</span><span class="sxs-lookup"><span data-stu-id="5b349-156">It is a list of environment variables to share between Windows and WSL.</span></span>
* <span data-ttu-id="5b349-157">Sie können Umgebungsvariablen funktionieren ordnungsgemäß in Windows und WSL formatieren.</span><span class="sxs-lookup"><span data-stu-id="5b349-157">It can format environment variables to work well in Windows and WSL.</span></span>

<span data-ttu-id="5b349-158">Es gibt vier Flags in `WSLENV` beeinflussen, wie diese Umgebungsvariable übersetzt wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-158">There are four flags available in `WSLENV` to influence how that environment variable is translated.</span></span>

<span data-ttu-id="5b349-159">`WSLENV` Flaggen:</span><span class="sxs-lookup"><span data-stu-id="5b349-159">`WSLENV` flags:</span></span>

* <span data-ttu-id="5b349-160">`/p` -Pfads zwischen WSL/Linux-Style-Pfade und Pfade der Win32-übersetzt.</span><span class="sxs-lookup"><span data-stu-id="5b349-160">`/p` - translates the path between WSL/Linux style paths and Win32 paths.</span></span>
* <span data-ttu-id="5b349-161">`/l` -Gibt an, die Umgebungsvariable ist eine Liste von Pfaden.</span><span class="sxs-lookup"><span data-stu-id="5b349-161">`/l` - indicates the environment variable is a list of paths.</span></span>
* <span data-ttu-id="5b349-162">`/u` -Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden sollen, wenn WSL von Win32 ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-162">`/u` - indicates that this environment variable should only be included when running WSL from Win32.</span></span>
* <span data-ttu-id="5b349-163">`/w` -Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden sollen, wenn Win32 von WSL ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-163">`/w` - indicates that this environment variable should only be included when running Win32 from WSL.</span></span>

<span data-ttu-id="5b349-164">Flags können kombiniert werden, je nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="5b349-164">Flags can be combined as needed.</span></span>

## <a name="disable-interop"></a><span data-ttu-id="5b349-165">Deaktivieren von Interop</span><span class="sxs-lookup"><span data-stu-id="5b349-165">Disable Interop</span></span>

<span data-ttu-id="5b349-166">Benutzer können die Möglichkeit, Windows-Binärdateien für eine einzelne WSL-Sitzung ausgeführt werden, durch den folgenden Befehl als Root ausführen:</span><span class="sxs-lookup"><span data-stu-id="5b349-166">Users may disable the ability to run Windows binaries for a single WSL session by running the following command as root:</span></span>

``` BASH
$ echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="5b349-167">Um Windows erneut aktivieren Binärdateien entweder alle WSL-Sitzungen zu beenden und bash.exe erneut ausführen oder führen den folgenden Befehl als Root-Benutzer:</span><span class="sxs-lookup"><span data-stu-id="5b349-167">To reenable Windows binaries either exit all WSL sessions and re-run bash.exe or run the following command as root:</span></span>

``` BASH
$ echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="5b349-168">Deaktivieren von Interop zwischen den WSL-Sitzungen nicht beibehalten: Interop wird erneut aktiviert werden, wenn eine neue Sitzung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-168">Disabling interop will not persist between WSL sessions -- interop will be enabled again when a new session is launched.</span></span>

## <a name="creators-update-and-anniversary-update"></a><span data-ttu-id="5b349-169">Creators Update und Anniversary-Update</span><span class="sxs-lookup"><span data-stu-id="5b349-169">Creators Update and Anniversary Update</span></span>

<span data-ttu-id="5b349-170">Während der Interop-Umgebung vor Herbst Creators Update neuere Interop-Funktionen ähnelt, gibt es jedoch einige wichtige Unterschiede.</span><span class="sxs-lookup"><span data-stu-id="5b349-170">While the interop experience pre-Fall Creators Update is similar to more recent interop experiences, there are a handful of major differences.</span></span>

<span data-ttu-id="5b349-171">Zusammenfassung:</span><span class="sxs-lookup"><span data-stu-id="5b349-171">To summarize:</span></span>

* <span data-ttu-id="5b349-172">`bash.exe` ist veraltet und durch ersetzt `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="5b349-172">`bash.exe` has been deprecated and replaced with `wsl.exe`.</span></span>
* <span data-ttu-id="5b349-173">`-c` Option für das Ausführen eines einzelnen Befehls mit nicht benötigt `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="5b349-173">`-c` option for running a single command isn't needed with `wsl.exe`.</span></span>
* <span data-ttu-id="5b349-174">Windows-Pfad ist in der WSL enthalten. `$PATH`</span><span class="sxs-lookup"><span data-stu-id="5b349-174">Windows path is included in the WSL `$PATH`</span></span>

<span data-ttu-id="5b349-175">Der Prozess zum Deaktivieren von Interop ist unverändert.</span><span class="sxs-lookup"><span data-stu-id="5b349-175">The process for disabling interop is unchanged.</span></span>

### <a name="invoking-wsl-from-the-windows-command-line"></a><span data-ttu-id="5b349-176">Aufrufen von WSL über die Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="5b349-176">Invoking WSL from the Windows Command Line</span></span>

<span data-ttu-id="5b349-177">Linux-Binärdateien können über die Windows-Eingabeaufforderung oder über PowerShell aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="5b349-177">Linux binaries can be invoked from the Windows Command Prompt or from PowerShell.</span></span>  <span data-ttu-id="5b349-178">Binärdateien, die auf diese Weise aufgerufen haben die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="5b349-178">Binaries invoked in this way have the following properties:</span></span>

1. <span data-ttu-id="5b349-179">Verwenden Sie im selben Arbeitsverzeichnis, als die cmd- oder PowerShell-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="5b349-179">Use the same working directory as the CMD or PowerShell prompt.</span></span>
1. <span data-ttu-id="5b349-180">Führen Sie als Standardbenutzer WSL.</span><span class="sxs-lookup"><span data-stu-id="5b349-180">Run as the WSL default user.</span></span>
1. <span data-ttu-id="5b349-181">Haben Sie die gleichen Windows-Administratorrechte als der aufrufende Prozess und Terminaldienste.</span><span class="sxs-lookup"><span data-stu-id="5b349-181">Have the same Windows administrative rights as the calling process and terminal.</span></span>

<span data-ttu-id="5b349-182">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5b349-182">Example:</span></span>

```console
C:\temp> bash -c "ls -la"
```

<span data-ttu-id="5b349-183">Linux-Befehle, die auf diese Weise aufgerufen werden wie jede andere Windows-Anwendung verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="5b349-183">Linux commands called in this way are handled like any other Windows application.</span></span>  <span data-ttu-id="5b349-184">Z. B. Eingabe, Piping und Datei-Umleitung funktioniert wie erwartet.</span><span class="sxs-lookup"><span data-stu-id="5b349-184">Things such as input, piping, and file redirection work as expected.</span></span>

<span data-ttu-id="5b349-185">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="5b349-185">Examples:</span></span>

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

<span data-ttu-id="5b349-186">Übergeben Sie die WSL-Befehle in `bash -c` an den Prozess WSL ohne Änderung weitergeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="5b349-186">The WSL commands passed into `bash -c` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="5b349-187">Dateipfade in die WSL-Format angegeben werden müssen und Vorsicht relevanten Zeichen mit Escapezeichen versehen.</span><span class="sxs-lookup"><span data-stu-id="5b349-187">File paths must be specified in the WSL format and care must be taken to escape relevant characters.</span></span> <span data-ttu-id="5b349-188">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5b349-188">Example:</span></span>

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
<- contents of C:\Program Files ->
```

### <a name="invoking-windows-binaries-from-wsl"></a><span data-ttu-id="5b349-189">Aufrufen von Windows-Binärdateien von WSL</span><span class="sxs-lookup"><span data-stu-id="5b349-189">Invoking Windows binaries from WSL</span></span>

<span data-ttu-id="5b349-190">Die Windows-Subsystem für Linux können Sie Windows-Binärdateien direkt aus der Befehlszeile WSL aufrufen.</span><span class="sxs-lookup"><span data-stu-id="5b349-190">The Windows Subsystem for Linux can invoke Windows binaries directly from the WSL command line.</span></span>  <span data-ttu-id="5b349-191">Anwendungen, die auf diese Weise ausführen, haben die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="5b349-191">Applications run this way have the following properties:</span></span>

1. <span data-ttu-id="5b349-192">Behalten Sie das Arbeitsverzeichnis, als die WSL-Eingabeaufforderung außer in dem Szenario, das die unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="5b349-192">Retain the working directory as the WSL command prompt except in the scenario explained below.</span></span>
1. <span data-ttu-id="5b349-193">Haben Sie die gleichen Berechtigungen Rechte wie die `bash.exe` Prozess.</span><span class="sxs-lookup"><span data-stu-id="5b349-193">Have the same permission rights as the `bash.exe` process.</span></span> 
1. <span data-ttu-id="5b349-194">Führen Sie als den aktiven Windows-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5b349-194">Run as the active Windows user.</span></span>
1. <span data-ttu-id="5b349-195">Im Windows Task-Manager angezeigt, als ob direkt über die Eingabeaufforderung ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="5b349-195">Appear in the Windows Task Manager as if directly executed from the CMD prompt.</span></span>

<span data-ttu-id="5b349-196">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5b349-196">Example:</span></span>

``` BASH
$ /mnt/c/Windows/System32/notepad.exe
```

<span data-ttu-id="5b349-197">In WSL werden diese ausführbaren Dateien wie native Linux ausführbaren Dateien behandelt.</span><span class="sxs-lookup"><span data-stu-id="5b349-197">In WSL, these executables are handled similar to native Linux executables.</span></span>  <span data-ttu-id="5b349-198">Dies bedeutet, Hinzufügen von Verzeichnissen auf den Linux-Pfad, und zwischen Befehlen ordnungsgemäß weitergeleitet werden, wie erwartet.</span><span class="sxs-lookup"><span data-stu-id="5b349-198">This means adding directories to the Linux path and piping between commands works as expected.</span></span>  <span data-ttu-id="5b349-199">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="5b349-199">Examples:</span></span>

``` BASH
$ export PATH=$PATH:/mnt/c/Windows/System32
$ notepad.exe
$ ipconfig.exe | grep IPv4 | cut -d: -f2
$ ls -la | findstr.exe foo.txt
$ cmd.exe /c dir
```

<span data-ttu-id="5b349-200">Die Windows-Binärdatei muss die Dateierweiterung einbeziehen, Groß-/Kleinschreibung der Datei und nicht mehr ausführbar sein.</span><span class="sxs-lookup"><span data-stu-id="5b349-200">The Windows binary must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="5b349-201">Nicht-ausführbare Dateien einschließlich batch-Skripts und Befehl wie `dir` kann ausgeführt werden, mit `/mnt/c/Windows/System32/cmd.exe /C` Befehl.</span><span class="sxs-lookup"><span data-stu-id="5b349-201">Non-executables including batch scripts and command like `dir` can be run with `/mnt/c/Windows/System32/cmd.exe /C` command.</span></span>

<span data-ttu-id="5b349-202">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="5b349-202">Examples:</span></span>

``` BASH
$ /mnt/c/Windows/System32/cmd.exe /C dir
$ /mnt/c/Windows/System32/PING.EXE www.microsoft.com
```

<span data-ttu-id="5b349-203">Parameter werden an die Windows-binäre unverändert übergeben.</span><span class="sxs-lookup"><span data-stu-id="5b349-203">Parameters are passed to the Windows binary unmodified.</span></span>  

<span data-ttu-id="5b349-204">Als Beispiel die folgenden Befehle öffnet `C:\temp\foo.txt` in `notepad.exe`:</span><span class="sxs-lookup"><span data-stu-id="5b349-204">As an example, the following commands will open `C:\temp\foo.txt` in `notepad.exe`:</span></span>

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

<span data-ttu-id="5b349-205">Ändern die Dateien in VolFs (Dateien nicht unter `/mnt/<x>`) mit einem Windows Anwendung wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b349-205">Modifying files located on VolFs (files not under `/mnt/<x>`) with a Windows application is not supported.</span></span>  <span data-ttu-id="5b349-206">In der Standardeinstellung WSL versucht, das Arbeitsverzeichnis für die Windows als aktuelles Verzeichnis WSL binäre zu halten, aber zurückgreift auf der erstellen-Instanz gespeichert, wenn das Arbeitsverzeichnis auf VolFs ist.</span><span class="sxs-lookup"><span data-stu-id="5b349-206">By default, WSL attempts to keep the working directory of the Windows binary as the current WSL directory, but will fall back on the instance creation directory if the working directory is on VolFs.</span></span>

<span data-ttu-id="5b349-207">Als Beispiel; `bash.exe` ursprünglich gestartet wird `C:\temp` und das aktuelle WSL-Verzeichnis in der Wohnung des Benutzers geändert wird.</span><span class="sxs-lookup"><span data-stu-id="5b349-207">As an example; `bash.exe` is initially launched from `C:\temp` and the current WSL directory is changed to the user’s home.</span></span>  <span data-ttu-id="5b349-208">Wenn `notepad.exe` wird aufgerufen, in das Basisverzeichnis des Benutzers WSL automatisch wiederhergestellt `C:\temp` als Arbeitsverzeichnis notepad.exe:</span><span class="sxs-lookup"><span data-stu-id="5b349-208">When `notepad.exe` is called from the user’s home directory, WSL automatically reverts to `C:\temp` as the notepad.exe working directory:</span></span>

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
