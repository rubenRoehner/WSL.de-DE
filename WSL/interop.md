---
title: Windows-Interoperabilität mit Linux
description: Beschreibt die Windows-Interoperabilität mit Linux-Distributionen, die im Windows-Subsystem für Linux ausgeführt werden.
author: scooley
ms.author: scooley
ms.date: 12/20/2017
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 3f3df3337ece75d7af77313f5fc55eb4e18e31cb
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122733"
---
# <a name="windows-subsystem-for-linux-interoperability-with-windows"></a><span data-ttu-id="d355d-103">Windows-Subsystem für Linux-Interoperabilität mit Windows</span><span class="sxs-lookup"><span data-stu-id="d355d-103">Windows Subsystem for Linux interoperability with Windows</span></span>

> <span data-ttu-id="d355d-104">**Das Thema wurde für das Fall Creators Update aktualisiert.**</span><span class="sxs-lookup"><span data-stu-id="d355d-104">**Updated for Fall Creators Update.**</span></span>  
<span data-ttu-id="d355d-105">Wenn Sie Creators Update oder Anniversary Update ausführen, springen Sie zum [Abschnitt Creators/Anniversary Update](interop.md#creators-update-and-anniversary-update).</span><span class="sxs-lookup"><span data-stu-id="d355d-105">If you're running Creators Update or Anniversary Update, jump to the [Creators/Anniversary Update section](interop.md#creators-update-and-anniversary-update).</span></span>

<span data-ttu-id="d355d-106">Das Windows-Subsystem für Linux (WSL) verbessert die Integration zwischen Windows und Linux kontinuierlich.</span><span class="sxs-lookup"><span data-stu-id="d355d-106">The Windows Subsystem for Linux (WSL) is continuously improving integration between Windows and Linux.</span></span>  <span data-ttu-id="d355d-107">Sie haben folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="d355d-107">You can:</span></span>

1. <span data-ttu-id="d355d-108">Aufrufen von Windows-Binärdateien über die Linux-Konsole.</span><span class="sxs-lookup"><span data-stu-id="d355d-108">Invoke Windows binaries from the Linux console.</span></span>
1. <span data-ttu-id="d355d-109">Aufrufen von Linux-Binärdateien von einer Windows-Konsole aus.</span><span class="sxs-lookup"><span data-stu-id="d355d-109">Invoke Linux binaries from a Windows console.</span></span>
1. <span data-ttu-id="d355d-110">**Windows Insider erstellt 17063 +** Freigeben von Umgebungsvariablen zwischen Linux und Windows.</span><span class="sxs-lookup"><span data-stu-id="d355d-110">**Windows Insiders Builds 17063+** Share environment variables between Linux and Windows.</span></span>

<span data-ttu-id="d355d-111">Dies bietet eine nahtlose Darstellung zwischen Windows und WSL.</span><span class="sxs-lookup"><span data-stu-id="d355d-111">This delivers a seamless experience between Windows and WSL.</span></span>  <span data-ttu-id="d355d-112">Technische Details finden Sie im [WSL-Blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).</span><span class="sxs-lookup"><span data-stu-id="d355d-112">Technical details are on the [WSL blog](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/).</span></span>

## <a name="run-linux-tools-from-a-windows-command-line"></a><span data-ttu-id="d355d-113">Ausführen von Linux-Tools über eine Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="d355d-113">Run Linux tools from a Windows command line</span></span>

<span data-ttu-id="d355d-114">Ausführen von Linux-Binärdateien an der Windows-Eingabeaufforderung (cmd oder PowerShell) mithilfe `wsl.exe <command>`von.</span><span class="sxs-lookup"><span data-stu-id="d355d-114">Run Linux binaries from the Windows Command Prompt (CMD or PowerShell) using `wsl.exe <command>`.</span></span>

<span data-ttu-id="d355d-115">Auf diese Weise aufgerufene Binärdateien:</span><span class="sxs-lookup"><span data-stu-id="d355d-115">Binaries invoked in this way:</span></span>

1. <span data-ttu-id="d355d-116">Verwenden Sie das gleiche Arbeitsverzeichnis wie bei der aktuellen cmd-oder PowerShell-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="d355d-116">Use the same working directory as the current CMD or PowerShell prompt.</span></span>
1. <span data-ttu-id="d355d-117">Führen Sie als WSL-Standardbenutzer aus.</span><span class="sxs-lookup"><span data-stu-id="d355d-117">Run as the WSL default user.</span></span>
1. <span data-ttu-id="d355d-118">Sie haben dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.</span><span class="sxs-lookup"><span data-stu-id="d355d-118">Have the same Windows administrative rights as the calling process and terminal.</span></span>

<span data-ttu-id="d355d-119">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d355d-119">For example:</span></span>

```console
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

<span data-ttu-id="d355d-120">Der folgende `wsl.exe` Linux-Befehl wird wie ein beliebiger Befehl verarbeitet, der in WSL ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-120">The Linux command following `wsl.exe` is handled like any command run in WSL.</span></span>  <span data-ttu-id="d355d-121">Dinge wie "sudo", "Piping" und "Datei Umleitung" funktionieren.</span><span class="sxs-lookup"><span data-stu-id="d355d-121">Things such as sudo, piping, and file redirection work.</span></span>

<span data-ttu-id="d355d-122">Beispiel für die Verwendung von sudo:</span><span class="sxs-lookup"><span data-stu-id="d355d-122">Example using sudo:</span></span>

```console
C:\temp> wsl sudo apt-get update
[sudo] password for username:
Hit:1 https://archive.ubuntu.com/ubuntu xenial InRelease
Get:2 https://security.ubuntu.com/ubuntu xenial-security InRelease [94.5 kB]
```

<span data-ttu-id="d355d-123">Beispiele zum Mischen von WSL-und Windows-Befehlen:</span><span class="sxs-lookup"><span data-stu-id="d355d-123">Examples mixing WSL and Windows commands:</span></span>

```console
C:\temp> wsl ls -la | findstr "foo"
-rwxrwxrwx 1 root root     14 Sep 27 14:26 foo.bat

C:\temp> dir | wsl grep foo
09/27/2016  02:26 PM                14 foo.bat

C:\temp> wsl ls -la > out.txt
```

<span data-ttu-id="d355d-124">Die an weiter `wsl.exe` gegebenen Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="d355d-124">The commands passed into `wsl.exe` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="d355d-125">Dateipfade müssen im WSL-Format angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-125">File paths must be specified in the WSL format.</span></span>

<span data-ttu-id="d355d-126">Beispiel mit Pfaden:</span><span class="sxs-lookup"><span data-stu-id="d355d-126">Example with paths:</span></span>

```console
C:\temp> wsl ls -la /proc/cpuinfo
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> wsl ls -la "/mnt/c/Program Files"
<- contents of C:\Program Files ->
```

## <a name="run-windows-tools-from-wsl"></a><span data-ttu-id="d355d-127">Ausführen von Windows-Tools aus WSL</span><span class="sxs-lookup"><span data-stu-id="d355d-127">Run Windows tools from WSL</span></span>

<span data-ttu-id="d355d-128">WSL kann Windows-Binärdateien direkt über die WSL-Befehlszeile `[binary name].exe`mithilfe von aufrufen.</span><span class="sxs-lookup"><span data-stu-id="d355d-128">WSL can invoke Windows binaries directly from the WSL command line using `[binary name].exe`.</span></span>  <span data-ttu-id="d355d-129">Beispiel: `notepad.exe`Hyper-V-Hosts oder Hyper-V-Hostcluster in einem separaten Namespace als verwaltete Hyper-V-Hosts hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="d355d-129">For example, `notepad.exe`.</span></span>  <span data-ttu-id="d355d-130">Damit ausführbare Windows-Dateien einfacher ausgeführt werden können, ist Windows Path im Fall Creators `$PATH` Update in Linux enthalten.</span><span class="sxs-lookup"><span data-stu-id="d355d-130">To make Windows executables easier to run, Windows path is included in the Linux `$PATH` in Fall Creators Update.</span></span>

<span data-ttu-id="d355d-131">Anwendungen, die auf diese Weise ausgeführt werden, haben die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="d355d-131">Applications run this way have the following properties:</span></span>

1. <span data-ttu-id="d355d-132">Behalten Sie das Arbeitsverzeichnis als WSL-Eingabeaufforderung bei (in den meisten Fällen werden die Ausnahmen unten erläutert).</span><span class="sxs-lookup"><span data-stu-id="d355d-132">Retain the working directory as the WSL command prompt (for the most part -- exceptions are explained below).</span></span>
1. <span data-ttu-id="d355d-133">Sie müssen über die gleichen Berechtigungs Rechte wie der WSL-Prozess verfügen.</span><span class="sxs-lookup"><span data-stu-id="d355d-133">Have the same permission rights as the WSL process.</span></span>
1. <span data-ttu-id="d355d-134">Führen Sie als aktiver Windows-Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="d355d-134">Run as the active Windows user.</span></span>
1. <span data-ttu-id="d355d-135">Wird im Windows Task-Manager so angezeigt, als ob er direkt von der cmd-Eingabeaufforderung ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-135">Appear in the Windows Task Manager as if directly executed from the CMD prompt.</span></span>

<span data-ttu-id="d355d-136">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d355d-136">Example:</span></span>

``` BASH
$ notepad.exe
```

<span data-ttu-id="d355d-137">Ausführbare Windows-Dateien, die in WSL ausgeführt werden, werden ähnlich wie Native ausführbare Linux-Dateien verarbeitet</span><span class="sxs-lookup"><span data-stu-id="d355d-137">Windows executables run in WSL are handled similarly to native Linux executables -- piping, redirects, and even backgrounding work as expected.</span></span>

<span data-ttu-id="d355d-138">Beispiele für die Verwendung von Pipes:</span><span class="sxs-lookup"><span data-stu-id="d355d-138">Examples using pipes:</span></span>

``` BASH
$ ipconfig.exe | grep IPv4 | cut -d: -f2
172.21.240.1
10.159.21.24
```

<span data-ttu-id="d355d-139">Beispiel für die Verwendung gemischter Windows-und WSL-Befehle:</span><span class="sxs-lookup"><span data-stu-id="d355d-139">Example using mixed Windows and WSL commands:</span></span>

``` BASH
$ ls -la | findstr.exe foo.txt

$ cmd.exe /c dir
<- contents of C:\ ->
```

<span data-ttu-id="d355d-140">Windows-Binärdateien müssen die Dateierweiterung enthalten, dem Datei Fall entsprechen und ausführbare Dateien sein.</span><span class="sxs-lookup"><span data-stu-id="d355d-140">Windows binaries must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="d355d-141">Nicht ausführbare Dateien, einschließlich Batch Skripts.</span><span class="sxs-lookup"><span data-stu-id="d355d-141">Non-executables including batch scripts.</span></span>  <span data-ttu-id="d355d-142">Native cmd-Befehle `dir` wie können mit `cmd.exe /C` einem Befehl ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-142">CMD native commands like `dir` can be run with `cmd.exe /C` command.</span></span>

<span data-ttu-id="d355d-143">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="d355d-143">Examples:</span></span>

``` BASH
$ cmd.exe /C dir
<- contents of C:\ ->

$ PING.EXE www.microsoft.com
Pinging e1863.dspb.akamaiedge.net [2600:1409:a:5a2::747] with 32 bytes of data:
Reply from 2600:1409:a:5a2::747: time=2ms
```

<span data-ttu-id="d355d-144">Parameter werden unverändert an die Windows-Binärdatei (Binary) übermittelt.</span><span class="sxs-lookup"><span data-stu-id="d355d-144">Parameters are passed to the Windows binary unmodified.</span></span>

<span data-ttu-id="d355d-145">Beispielsweise werden die folgenden Befehle in `C:\temp\foo.txt` `notepad.exe`geöffnet:</span><span class="sxs-lookup"><span data-stu-id="d355d-145">As an example, the following commands will open `C:\temp\foo.txt` in `notepad.exe`:</span></span>

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

<span data-ttu-id="d355d-146">Das Ändern von Dateien, die sich auf volfs `/mnt/<x>`(Dateien nicht unter) mit einer Windows-Anwendung in WSL befinden, wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d355d-146">Modifying files located on VolFs (files not under `/mnt/<x>`) with a Windows application in WSL is not supported.</span></span>

<span data-ttu-id="d355d-147">Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als Aktuelles WSL-Verzeichnis beizubehalten. wenn sich das Arbeitsverzeichnis auf "volfs" befindet, wird das Verzeichnis für die Instanzerstellung zurückgegriffen.</span><span class="sxs-lookup"><span data-stu-id="d355d-147">By default, WSL tries to keep the working directory of the Windows binary as the current WSL directory, but will fall back on the instance creation directory if the working directory is on VolFs.</span></span>

<span data-ttu-id="d355d-148">Beispiel: wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in die Startseite des Benutzers geändert. `wsl.exe`</span><span class="sxs-lookup"><span data-stu-id="d355d-148">As an example; `wsl.exe` is initially launched from `C:\temp` and the current WSL directory is changed to the user’s home.</span></span>  <span data-ttu-id="d355d-149">Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, wird WSL automatisch `C:\temp` als "Notepad. exe"-Arbeitsverzeichnis wieder hergestellt:</span><span class="sxs-lookup"><span data-stu-id="d355d-149">When `notepad.exe` is called from the user’s home directory, WSL automatically reverts to `C:\temp` as the notepad.exe working directory:</span></span>

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

## <a name="share-environment-variables-between-windows-and-wsl"></a><span data-ttu-id="d355d-150">Freigeben von Umgebungsvariablen zwischen Windows und WSL</span><span class="sxs-lookup"><span data-stu-id="d355d-150">Share environment variables between Windows and WSL</span></span>

> <span data-ttu-id="d355d-151">Verfügbar in Windows Insider-Builds 17063 und höher.</span><span class="sxs-lookup"><span data-stu-id="d355d-151">Available in Windows Insider builds 17063 and later.</span></span>

<span data-ttu-id="d355d-152">Vor 17063 war `PATH` nur die Windows-Umgebungsvariable, auf die WSL zugreifen konnte (sodass Sie ausführbare Win32-Dateien unter WSL starten konnten).</span><span class="sxs-lookup"><span data-stu-id="d355d-152">Prior to 17063, only Windows environment variable that WSL could access was `PATH` (so you could launch Win32 executables from under WSL).</span></span>

<span data-ttu-id="d355d-153">Ab 17063, WSL und Windows Share `WSLENV`, eine spezielle Umgebungsvariable, die zum Überbrücken von Windows-und Linux-Distributionen erstellt wird, die auf WSL ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-153">Starting in 17063, WSL and Windows share `WSLENV`, a special environment variable created to bridge Windows and Linux distros running on WSL.</span></span>

<span data-ttu-id="d355d-154">Eigenschaften von `WSLENV`:</span><span class="sxs-lookup"><span data-stu-id="d355d-154">Properties of `WSLENV`:</span></span>

* <span data-ttu-id="d355d-155">Es ist freigegeben. Es ist sowohl in Windows-als auch in WSL-Umgebungen vorhanden.</span><span class="sxs-lookup"><span data-stu-id="d355d-155">It is shared; it exists in both Windows and WSL environments.</span></span>
* <span data-ttu-id="d355d-156">Es handelt sich um eine Liste von Umgebungsvariablen, die zwischen Windows und WSL gemeinsam genutzt werden können.</span><span class="sxs-lookup"><span data-stu-id="d355d-156">It is a list of environment variables to share between Windows and WSL.</span></span>
* <span data-ttu-id="d355d-157">Sie können Umgebungsvariablen so formatieren, dass Sie in Windows und WSL gut funktionieren.</span><span class="sxs-lookup"><span data-stu-id="d355d-157">It can format environment variables to work well in Windows and WSL.</span></span>

<span data-ttu-id="d355d-158">In `WSLENV` sind vier Flags verfügbar, die beeinflussen, wie die Umgebungsvariable übersetzt wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-158">There are four flags available in `WSLENV` to influence how that environment variable is translated.</span></span>

<span data-ttu-id="d355d-159">`WSLENV`fahren</span><span class="sxs-lookup"><span data-stu-id="d355d-159">`WSLENV` flags:</span></span>

* <span data-ttu-id="d355d-160">`/p`: übersetzt den Pfad zwischen WSL-/Linux-stylepfaden und Win32-Pfaden.</span><span class="sxs-lookup"><span data-stu-id="d355d-160">`/p` - translates the path between WSL/Linux style paths and Win32 paths.</span></span>
* <span data-ttu-id="d355d-161">`/l`-Gibt an, dass die Umgebungsvariable eine Liste von Pfaden ist.</span><span class="sxs-lookup"><span data-stu-id="d355d-161">`/l` - indicates the environment variable is a list of paths.</span></span>
* <span data-ttu-id="d355d-162">`/u`: gibt an, dass diese Umgebungsvariable nur beim Ausführen von WSL von Win32 eingeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="d355d-162">`/u` - indicates that this environment variable should only be included when running WSL from Win32.</span></span>
* <span data-ttu-id="d355d-163">`/w`Gibt an, dass diese Umgebungsvariable nur eingeschlossen werden soll, wenn Win32 von WSL aus ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-163">`/w` - indicates that this environment variable should only be included when running Win32 from WSL.</span></span>

<span data-ttu-id="d355d-164">Flags können nach Bedarf kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-164">Flags can be combined as needed.</span></span>

## <a name="disable-interop"></a><span data-ttu-id="d355d-165">Interop deaktivieren</span><span class="sxs-lookup"><span data-stu-id="d355d-165">Disable Interop</span></span>

<span data-ttu-id="d355d-166">Benutzer können die Möglichkeit zum Ausführen von Windows-Binärdateien für eine einzelne WSL-Sitzung deaktivieren, indem Sie den folgenden Befehl als Root-Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="d355d-166">Users may disable the ability to run Windows binaries for a single WSL session by running the following command as root:</span></span>

``` BASH
$ echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="d355d-167">Zum erneuten Aktivieren von Windows-Binärdateien beenden Sie entweder alle WSL-Sitzungen, führen Sie bash. exe erneut aus, oder führen Sie den folgenden Befehl als root aus:</span><span class="sxs-lookup"><span data-stu-id="d355d-167">To reenable Windows binaries either exit all WSL sessions and re-run bash.exe or run the following command as root:</span></span>

``` BASH
$ echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="d355d-168">Das Deaktivieren von Interop wird nicht zwischen WSL-Sitzungen beibehalten--Interop wird erneut aktiviert, wenn eine neue Sitzung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-168">Disabling interop will not persist between WSL sessions -- interop will be enabled again when a new session is launched.</span></span>

## <a name="creators-update-and-anniversary-update"></a><span data-ttu-id="d355d-169">Creators Update und Anniversary Update</span><span class="sxs-lookup"><span data-stu-id="d355d-169">Creators Update and Anniversary Update</span></span>

<span data-ttu-id="d355d-170">Während das Interop-erstellerupdate vor Fall der aktuellen Interop-Erfahrung ähnelt, gibt es einige wichtige Unterschiede.</span><span class="sxs-lookup"><span data-stu-id="d355d-170">While the interop experience pre-Fall Creators Update is similar to more recent interop experiences, there are a handful of major differences.</span></span>

<span data-ttu-id="d355d-171">Zusammenfassung:</span><span class="sxs-lookup"><span data-stu-id="d355d-171">To summarize:</span></span>

* <span data-ttu-id="d355d-172">`bash.exe`wurde als veraltet markiert und durch ersetzt `wsl.exe`.</span><span class="sxs-lookup"><span data-stu-id="d355d-172">`bash.exe` has been deprecated and replaced with `wsl.exe`.</span></span>
* <span data-ttu-id="d355d-173">`-c`die Option zum Ausführen eines einzelnen Befehls ist mit `wsl.exe`nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d355d-173">`-c` option for running a single command isn't needed with `wsl.exe`.</span></span>
* <span data-ttu-id="d355d-174">Der Windows-Pfad ist im WSL enthalten.`$PATH`</span><span class="sxs-lookup"><span data-stu-id="d355d-174">Windows path is included in the WSL `$PATH`</span></span>

<span data-ttu-id="d355d-175">Der Prozess zum Deaktivieren der Interop ist unverändert.</span><span class="sxs-lookup"><span data-stu-id="d355d-175">The process for disabling interop is unchanged.</span></span>

### <a name="invoking-wsl-from-the-windows-command-line"></a><span data-ttu-id="d355d-176">Aufrufen von WSL von der Windows-Befehlszeile aus</span><span class="sxs-lookup"><span data-stu-id="d355d-176">Invoking WSL from the Windows Command Line</span></span>

<span data-ttu-id="d355d-177">Linux-Binärdateien können von der Windows-Eingabeaufforderung oder von PowerShell aufgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-177">Linux binaries can be invoked from the Windows Command Prompt or from PowerShell.</span></span>  <span data-ttu-id="d355d-178">Auf diese Weise aufgerufene Binärdateien verfügen über die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="d355d-178">Binaries invoked in this way have the following properties:</span></span>

1. <span data-ttu-id="d355d-179">Verwenden Sie das gleiche Arbeitsverzeichnis wie die CMD-oder PowerShell-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="d355d-179">Use the same working directory as the CMD or PowerShell prompt.</span></span>
1. <span data-ttu-id="d355d-180">Führen Sie als WSL-Standardbenutzer aus.</span><span class="sxs-lookup"><span data-stu-id="d355d-180">Run as the WSL default user.</span></span>
1. <span data-ttu-id="d355d-181">Sie haben dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.</span><span class="sxs-lookup"><span data-stu-id="d355d-181">Have the same Windows administrative rights as the calling process and terminal.</span></span>

<span data-ttu-id="d355d-182">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d355d-182">Example:</span></span>

```console
C:\temp> bash -c "ls -la"
```

<span data-ttu-id="d355d-183">Linux-Befehle, die auf diese Weise aufgerufen werden, werden wie jede andere Windows-Anwendung behandelt.</span><span class="sxs-lookup"><span data-stu-id="d355d-183">Linux commands called in this way are handled like any other Windows application.</span></span>  <span data-ttu-id="d355d-184">Dinge wie Eingabe, Piping und Datei Umleitung funktionieren erwartungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="d355d-184">Things such as input, piping, and file redirection work as expected.</span></span>

<span data-ttu-id="d355d-185">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="d355d-185">Examples:</span></span>

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

<span data-ttu-id="d355d-186">Die an weiter `bash -c` gegebenen WSL-Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="d355d-186">The WSL commands passed into `bash -c` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="d355d-187">Dateipfade müssen im WSL-Format angegeben werden, und es muss darauf geachtet werden, dass relevante Zeichen mit Escapezeichen versehen werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-187">File paths must be specified in the WSL format and care must be taken to escape relevant characters.</span></span> <span data-ttu-id="d355d-188">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d355d-188">Example:</span></span>

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
-r--r--r-- 1 root root 0 Sep 28 11:28 /proc/cpuinfo

C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
<- contents of C:\Program Files ->
```

### <a name="invoking-windows-binaries-from-wsl"></a><span data-ttu-id="d355d-189">Aufrufen von Windows-Binärdateien aus WSL</span><span class="sxs-lookup"><span data-stu-id="d355d-189">Invoking Windows binaries from WSL</span></span>

<span data-ttu-id="d355d-190">Das Windows-Subsystem für Linux kann Windows-Binärdateien direkt über die WSL-Befehlszeile aufrufen.</span><span class="sxs-lookup"><span data-stu-id="d355d-190">The Windows Subsystem for Linux can invoke Windows binaries directly from the WSL command line.</span></span>  <span data-ttu-id="d355d-191">Anwendungen, die auf diese Weise ausgeführt werden, haben die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="d355d-191">Applications run this way have the following properties:</span></span>

1. <span data-ttu-id="d355d-192">Behalten Sie das Arbeitsverzeichnis als WSL-Eingabeaufforderung mit Ausnahme des unten beschriebenen Szenarios bei.</span><span class="sxs-lookup"><span data-stu-id="d355d-192">Retain the working directory as the WSL command prompt except in the scenario explained below.</span></span>
1. <span data-ttu-id="d355d-193">Sie müssen über die gleichen Berechtigungs `bash.exe` Rechte wie der Prozess verfügen.</span><span class="sxs-lookup"><span data-stu-id="d355d-193">Have the same permission rights as the `bash.exe` process.</span></span> 
1. <span data-ttu-id="d355d-194">Führen Sie als aktiver Windows-Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="d355d-194">Run as the active Windows user.</span></span>
1. <span data-ttu-id="d355d-195">Wird im Windows Task-Manager so angezeigt, als ob er direkt von der cmd-Eingabeaufforderung ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d355d-195">Appear in the Windows Task Manager as if directly executed from the CMD prompt.</span></span>

<span data-ttu-id="d355d-196">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="d355d-196">Example:</span></span>

``` BASH
$ /mnt/c/Windows/System32/notepad.exe
```

<span data-ttu-id="d355d-197">In WSL werden diese ausführbaren Dateien ähnlich wie Native ausführbare Linux-Dateien behandelt.</span><span class="sxs-lookup"><span data-stu-id="d355d-197">In WSL, these executables are handled similar to native Linux executables.</span></span>  <span data-ttu-id="d355d-198">Dies bedeutet, dass das Hinzufügen von Verzeichnissen zum Linux-Pfad und die Weiterleitung zwischen Befehlen erwartungsgemäß funktioniert.</span><span class="sxs-lookup"><span data-stu-id="d355d-198">This means adding directories to the Linux path and piping between commands works as expected.</span></span>  <span data-ttu-id="d355d-199">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="d355d-199">Examples:</span></span>

``` BASH
$ export PATH=$PATH:/mnt/c/Windows/System32
$ notepad.exe
$ ipconfig.exe | grep IPv4 | cut -d: -f2
$ ls -la | findstr.exe foo.txt
$ cmd.exe /c dir
```

<span data-ttu-id="d355d-200">Die Windows-Binärdatei muss die Dateierweiterung enthalten, dem Datei Fall entsprechen und ausführbare Dateien sein.</span><span class="sxs-lookup"><span data-stu-id="d355d-200">The Windows binary must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="d355d-201">Nicht ausführbare Dateien einschließlich Batch Skripts und Befehls like `dir` können mit `/mnt/c/Windows/System32/cmd.exe /C` einem Befehl ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="d355d-201">Non-executables including batch scripts and command like `dir` can be run with `/mnt/c/Windows/System32/cmd.exe /C` command.</span></span>

<span data-ttu-id="d355d-202">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="d355d-202">Examples:</span></span>

``` BASH
$ /mnt/c/Windows/System32/cmd.exe /C dir
$ /mnt/c/Windows/System32/PING.EXE www.microsoft.com
```

<span data-ttu-id="d355d-203">Parameter werden unverändert an die Windows-Binärdatei (Binary) übermittelt.</span><span class="sxs-lookup"><span data-stu-id="d355d-203">Parameters are passed to the Windows binary unmodified.</span></span>  

<span data-ttu-id="d355d-204">Beispielsweise werden die folgenden Befehle in `C:\temp\foo.txt` `notepad.exe`geöffnet:</span><span class="sxs-lookup"><span data-stu-id="d355d-204">As an example, the following commands will open `C:\temp\foo.txt` in `notepad.exe`:</span></span>

``` BASH
$ notepad.exe "C:\temp\foo.txt"
$ notepad.exe C:\\temp\\foo.txt
```

<span data-ttu-id="d355d-205">Das Ändern von Dateien in volfs (Dateien nicht `/mnt/<x>`unter) mit einer Windows-Anwendung wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d355d-205">Modifying files located on VolFs (files not under `/mnt/<x>`) with a Windows application is not supported.</span></span>  <span data-ttu-id="d355d-206">Standardmäßig versucht WSL, das Arbeitsverzeichnis der Windows-Binärdatei als Aktuelles WSL-Verzeichnis beizubehalten. wenn sich das Arbeitsverzeichnis auf "volfs" befindet, wird das Verzeichnis für die Instanzerstellung zurückgegriffen.</span><span class="sxs-lookup"><span data-stu-id="d355d-206">By default, WSL attempts to keep the working directory of the Windows binary as the current WSL directory, but will fall back on the instance creation directory if the working directory is on VolFs.</span></span>

<span data-ttu-id="d355d-207">Beispiel: wird anfänglich von `C:\temp` gestartet, und das aktuelle WSL-Verzeichnis wird in die Startseite des Benutzers geändert. `bash.exe`</span><span class="sxs-lookup"><span data-stu-id="d355d-207">As an example; `bash.exe` is initially launched from `C:\temp` and the current WSL directory is changed to the user’s home.</span></span>  <span data-ttu-id="d355d-208">Wenn `notepad.exe` aus dem Basisverzeichnis des Benutzers aufgerufen wird, wird WSL automatisch `C:\temp` als "Notepad. exe"-Arbeitsverzeichnis wieder hergestellt:</span><span class="sxs-lookup"><span data-stu-id="d355d-208">When `notepad.exe` is called from the user’s home directory, WSL automatically reverts to `C:\temp` as the notepad.exe working directory:</span></span>

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
