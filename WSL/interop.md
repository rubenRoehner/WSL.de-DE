---
title: Windows-Interoperabilität mit Linux
description: Beschreibt die Windows-Interoperabilität mit Linux-Distributionen, die im Windows-Subsystem für Linux ausgeführt werden.
ms.date: 05/12/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: b1c7a64a86cf088159d1abee3b341328151428f6
ms.sourcegitcommit: 1b6191351bbf9e95f3c28fc67abe4bf1bcfd3336
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83270844"
---
# <a name="windows-interoperability-with-linux"></a><span data-ttu-id="ea678-103">Windows-Interoperabilität mit Linux</span><span class="sxs-lookup"><span data-stu-id="ea678-103">Windows interoperability with Linux</span></span>

<span data-ttu-id="ea678-104">Das Windows-Subsystem für Linux (WSL) verbessert die Integration zwischen Windows und Linux kontinuierlich.</span><span class="sxs-lookup"><span data-stu-id="ea678-104">The Windows Subsystem for Linux (WSL) is continuously improving integration between Windows and Linux.</span></span>  <span data-ttu-id="ea678-105">Sie haben folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="ea678-105">You can:</span></span>

* <span data-ttu-id="ea678-106">Ausführen von Windows-Tools (z. B. „notepad.exe“) über eine Linux-Befehlszeile aus (d. h. Ubuntu).</span><span class="sxs-lookup"><span data-stu-id="ea678-106">Run Windows tools (ie. notepad.exe) from a Linux command line (ie. Ubuntu).</span></span>
* <span data-ttu-id="ea678-107">Ausführen von Linux-Tools (z. B. „grep“) über eine Windows-Befehlszeile (d. h. PowerShell).</span><span class="sxs-lookup"><span data-stu-id="ea678-107">Run Linux tools (ie. grep) from a Windows command line (ie. PowerShell).</span></span>
* <span data-ttu-id="ea678-108">Freigeben von Umgebungsvariablen zwischen Linux und Windows.</span><span class="sxs-lookup"><span data-stu-id="ea678-108">Share environment variables between Linux and Windows.</span></span> <span data-ttu-id="ea678-109">(Build 17063+)</span><span class="sxs-lookup"><span data-stu-id="ea678-109">(Build 17063+)</span></span>

> [!NOTE]
> <span data-ttu-id="ea678-110">Wenn Sie das Creators Update (Okt. 2017, Build 16299) oder das Anniversary Update (Aug. 2016, Build 14393) ausführen, fahren Sie mit [Frühere Versionen von Windows 10](#earlier-versions-of-windows-10) fort.</span><span class="sxs-lookup"><span data-stu-id="ea678-110">If you're running Creators Update (Oct 2017, Build 16299) or Anniversary Update (Aug 2016, Build 14393), jump to the [Earlier versions of Windows 10](#earlier-versions-of-windows-10).</span></span>

## <a name="run-linux-tools-from-a-windows-command-line"></a><span data-ttu-id="ea678-111">Ausführen von Linux-Tools über eine Windows-Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="ea678-111">Run Linux tools from a Windows command line</span></span>

<span data-ttu-id="ea678-112">Führen Sie Linux-Binärdateien über die Windows-Eingabeaufforderung (CMD oder PowerShell) mithilfe von `wsl <command>` (oder `wsl.exe <command>`) aus.</span><span class="sxs-lookup"><span data-stu-id="ea678-112">Run Linux binaries from the Windows Command Prompt (CMD) or PowerShell using `wsl <command>` (or `wsl.exe <command>`).</span></span>

<span data-ttu-id="ea678-113">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ea678-113">For example:</span></span>

```powershell
C:\temp> wsl ls -la
<- contents of C:\temp ->
```

<span data-ttu-id="ea678-114">Auf diese Weise aufgerufene Binärdateien:</span><span class="sxs-lookup"><span data-stu-id="ea678-114">Binaries invoked in this way:</span></span>

* <span data-ttu-id="ea678-115">Verwenden das gleiche Arbeitsverzeichnis wie die aktuelle CMD- oder PowerShell-Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="ea678-115">Use the same working directory as the current CMD or PowerShell prompt.</span></span>
* <span data-ttu-id="ea678-116">Werden als WSL-Standardbenutzer aus geführt.</span><span class="sxs-lookup"><span data-stu-id="ea678-116">Run as the WSL default user.</span></span>
* <span data-ttu-id="ea678-117">Sie verfügen über dieselben Windows-Administratorrechte wie der aufrufende Prozess und das Terminal.</span><span class="sxs-lookup"><span data-stu-id="ea678-117">Have the same Windows administrative rights as the calling process and terminal.</span></span>

<span data-ttu-id="ea678-118">Der auf `wsl` (oder `wsl.exe`) folgende Linux-Befehl wird wie ein beliebiger Befehl verarbeitet, der in WSL ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="ea678-118">The Linux command following `wsl` (or `wsl.exe`) is handled like any command run in WSL.</span></span>  <span data-ttu-id="ea678-119">Dinge wie sudo, Piping und Dateiumleitung funktionieren.</span><span class="sxs-lookup"><span data-stu-id="ea678-119">Things such as sudo, piping, and file redirection work.</span></span>

<span data-ttu-id="ea678-120">Beispiel für die Verwendung von sudo zum Aktualisieren Ihrer Linux-Standardverteilung:</span><span class="sxs-lookup"><span data-stu-id="ea678-120">Example using sudo to update your default Linux distribution:</span></span>

```powershell
C:\temp> wsl sudo apt-get update
```

<span data-ttu-id="ea678-121">Nachdem Sie diesen Befehl ausgeführt haben, wird der Benutzername Ihrer Linux-Standardverteilung angezeigt, und Sie werden zur Eingabe Ihres Kennworts aufgefordert.</span><span class="sxs-lookup"><span data-stu-id="ea678-121">Your default Linux distribution user name will be listed after running this command and you will be asked for your password.</span></span> <span data-ttu-id="ea678-122">Nachdem Sie Ihr Kennwort ordnungsgemäß eingegeben haben, werden von Ihrer Verteilung die Updates heruntergeladen.</span><span class="sxs-lookup"><span data-stu-id="ea678-122">After entering your password correctly, your distribution will download updates.</span></span>

## <a name="mixing-linux-and-windows-commands"></a><span data-ttu-id="ea678-123">Kombinieren von Linux- und Windows-Befehlen</span><span class="sxs-lookup"><span data-stu-id="ea678-123">Mixing Linux and Windows commands</span></span>

<span data-ttu-id="ea678-124">Hier finden Sie einige Beispiele für das Kombinieren von Linux- und Windows-Befehlen unter Verwendung von PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ea678-124">Here are a few examples of mixing Linux and Windows commands using PowerShell.</span></span>

<span data-ttu-id="ea678-125">Um den Linux-Befehl `ls -la` zum Auflisten von Dateien und den PowerShell-Befehl `findstr` zum Filtern der Ergebnisse nach Wörtern zu verwenden, die die Zeichenfolge „git“ enthalten, kombinieren Sie die Befehle:</span><span class="sxs-lookup"><span data-stu-id="ea678-125">To use the Linux command `ls -la` to list files and the PowerShell command `findstr` to filter the results for words containing "git", combine the commands:</span></span>

```powershell
wsl ls -la | findstr "git"
```

<span data-ttu-id="ea678-126">Um den PowerShell-Befehl `dir` zum Auflisten von Dateien und den Linux-Befehl `grep` zum Filtern der Ergebnisse nach Wörtern zu verwenden, die die Zeichenfolge „git“ enthalten, kombinieren Sie die Befehle:</span><span class="sxs-lookup"><span data-stu-id="ea678-126">To use the PowerShell command `dir` to list files and the Linux command `grep` to filter the results for words containing "git", combine the commands:</span></span>

```powershell
C:\temp> dir | wsl grep git
```

<span data-ttu-id="ea678-127">Um den Linux-Befehl `ls -la` zum Auflisten von Dateien und den PowerShell-Befehl `> out.txt` zum Drucken dieser Liste in eine Textdatei mit dem Namen „out.txt“ zu verwenden, kombinieren Sie die Befehle:</span><span class="sxs-lookup"><span data-stu-id="ea678-127">To use the Linux command `ls -la` to list files and the PowerShell command `> out.txt` to print that list to a text file named "out.txt", combine the commands:</span></span>

```powershell
C:\temp> wsl ls -la > out.txt
```

<span data-ttu-id="ea678-128">Die an `wsl.exe` übergebenen Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="ea678-128">The commands passed into `wsl.exe` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="ea678-129">Dateipfade müssen im WSL-Format angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ea678-129">File paths must be specified in the WSL format.</span></span>

<span data-ttu-id="ea678-130">So verwenden Sie den Linux-Befehl `ls -la` zum Auflisten von Dateien im `/proc/cpuinfo`-Linux-Dateisystempfad mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ea678-130">To use the Linux command `ls -la` to list files in the `/proc/cpuinfo` Linux file system path, using PowerShell:</span></span>

```powershell
C:\temp> wsl ls -la /proc/cpuinfo
```

<span data-ttu-id="ea678-131">So verwenden Sie den Linux-Befehl `ls -la` zum Auflisten von Dateien im `C:\Program Files`-Windows-Dateisystempfad mithilfe von PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ea678-131">To use the Linux command `ls -la` to list files in the `C:\Program Files` Windows file system path, using PowerShell:</span></span>

```powershell
C:\temp> wsl ls -la "/mnt/c/Program Files"
```

## <a name="run-windows-tools-from-linux"></a><span data-ttu-id="ea678-132">Ausführen von Windows-Tools aus Linux</span><span class="sxs-lookup"><span data-stu-id="ea678-132">Run Windows tools from Linux</span></span>

<span data-ttu-id="ea678-133">WSL kann Windows-Tools direkt über die WSL-Befehlszeile mithilfe von `[tool-name].exe` ausführen.</span><span class="sxs-lookup"><span data-stu-id="ea678-133">WSL can run Windows tools directly from the WSL command line using `[tool-name].exe`.</span></span>  <span data-ttu-id="ea678-134">Beispiel: `notepad.exe`.</span><span class="sxs-lookup"><span data-stu-id="ea678-134">For example, `notepad.exe`.</span></span>

<!-- Craig - could you help add a section with an example here to explain this scenario: "To access your Linux files using a Windows tool, use `\\wsl$\<distroName>\'` as the file path." Currently it I can just enter `notepad.exe foo.txt` and it seems to work fine, so explaining a situation where the file path is needed would be helpful. -->

<span data-ttu-id="ea678-135">Anwendungen, die auf diese Weise ausgeführt werden, besitzen die folgenden Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="ea678-135">Applications run this way have the following properties:</span></span>

* <span data-ttu-id="ea678-136">Sie behalten das Arbeitsverzeichnis als das Verzeichnis der WSL-Eingabeaufforderung bei (in den meisten Fällen, Ausnahmen werden unten erläutert).</span><span class="sxs-lookup"><span data-stu-id="ea678-136">Retain the working directory as the WSL command prompt (for the most part -- exceptions are explained below).</span></span>
* <span data-ttu-id="ea678-137">Sie verfügen über die gleichen Berechtigungen wie der WSL-Prozess.</span><span class="sxs-lookup"><span data-stu-id="ea678-137">Have the same permission rights as the WSL process.</span></span>
* <span data-ttu-id="ea678-138">Sie werden als aktiver Windows-Benutzer ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ea678-138">Run as the active Windows user.</span></span>
* <span data-ttu-id="ea678-139">Sie werden im Task-Manager von Windows so angezeigt, als würden die direkt über die CMD-Eingabeaufforderung ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ea678-139">Appear in the Windows Task Manager as if directly executed from the CMD prompt.</span></span>

<span data-ttu-id="ea678-140">Ausführbare Windows-Dateien, die in WSL ausgeführt werden, werden ähnlich wie native ausführbare Linux-Dateien verarbeitet. Piping, Umleitungen und sogar Hintergrundverarbeitung funktionieren wie erwartet.</span><span class="sxs-lookup"><span data-stu-id="ea678-140">Windows executables run in WSL are handled similarly to native Linux executables -- piping, redirects, and even backgrounding work as expected.</span></span>

<span data-ttu-id="ea678-141">Um das Windows-Tool `ipconfig.exe` auszuführen, das Linux-Tool `grep` zum Filtern der „IPv4“-Ergebnisse und das Linux-Tool `cut` zum Entfernen der Spaltenfelder zu verwenden,geben Sie aus einer Linux-Verteilung (z. B. Ubuntu) Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="ea678-141">To run the Windows tool `ipconfig.exe`, use the Linux tool `grep` to filter the "IPv4" results, and use the Linux tool `cut` to remove the column fields, from a Linux distribution (for example, Ubuntu) enter:</span></span>

```bash
ipconfig.exe | grep IPv4 | cut -d: -f2
```

<span data-ttu-id="ea678-142">Sehen wir uns ein Beispiel für das Kombinieren von Windows- und Linux-Befehlen an.</span><span class="sxs-lookup"><span data-stu-id="ea678-142">Let's try an example mixing Windows and Linux commands.</span></span> <span data-ttu-id="ea678-143">Öffnen Sie Ihre Linux-Verteilung (d. h. Ubuntu) und erstellen Sie eine Textdatei: `touch foo.txt`.</span><span class="sxs-lookup"><span data-stu-id="ea678-143">Open your Linux distribution (ie. Ubuntu) and create a text file: `touch foo.txt`.</span></span> <span data-ttu-id="ea678-144">Verwenden Sie nun den Linux-Befehl `ls -la`, um die direkten Dateien und deren Erstellungsdetails aufzulisten, sowie das Windows PowerShell-Tool `findstr.exe`, um die Ergebnisse zu filtern, sodass nur Ihre `foo.txt`-Datei in den Ergebnissen angezeigt wird:</span><span class="sxs-lookup"><span data-stu-id="ea678-144">Now use the Linux command `ls -la` to list the direct files and their creation details, plus the Windows PowerShell tool `findstr.exe` to filter the results so only your `foo.txt` file shows in the results:</span></span>

```bash
ls -la | findstr.exe foo.txt
```

<span data-ttu-id="ea678-145">Windows-Tools müssen die Dateierweiterung enthalten, der Groß-/Kleinschreibung der Datei Rechnung tragen und ausführbare Dateien sein.</span><span class="sxs-lookup"><span data-stu-id="ea678-145">Windows tools must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="ea678-146">Nicht ausführbare Dateien, einschließlich Batchskripts.</span><span class="sxs-lookup"><span data-stu-id="ea678-146">Non-executables including batch scripts.</span></span>  <span data-ttu-id="ea678-147">Native CMD-Befehle wie `dir` können mit einem Befehl `cmd.exe /C` ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ea678-147">CMD native commands like `dir` can be run with `cmd.exe /C` command.</span></span>

<span data-ttu-id="ea678-148">Listen Sie z. B. den Inhalt Ihres Windows-Dateisystemverzeichnisses „C:\“ auf, indem Sie Folgendes eingeben:</span><span class="sxs-lookup"><span data-stu-id="ea678-148">For example, list the contents of your Windows files system C:\ directory, by entering:</span></span>

```bash
cmd.exe /C dir
```

<span data-ttu-id="ea678-149">Oder verwenden Sie den Befehl `ping`, um eine Echoanforderung an die Website „microsoft.com“ zu senden:</span><span class="sxs-lookup"><span data-stu-id="ea678-149">Or use the `ping` command to send an echo request to the microsoft.com website:</span></span>

```bash
ping.exe www.microsoft.com
```

<span data-ttu-id="ea678-150">Parameter werden unverändert an die Windows-Binärdatei übergeben.</span><span class="sxs-lookup"><span data-stu-id="ea678-150">Parameters are passed to the Windows binary unmodified.</span></span> <span data-ttu-id="ea678-151">Beispielsweise öffnet der folgende Befehl `C:\temp\foo.txt` in `notepad.exe`:</span><span class="sxs-lookup"><span data-stu-id="ea678-151">As an example, the following command will open `C:\temp\foo.txt` in `notepad.exe`:</span></span>

```bash
notepad.exe "C:\temp\foo.txt"
```

<span data-ttu-id="ea678-152">Dies funktioniert auch:</span><span class="sxs-lookup"><span data-stu-id="ea678-152">This will also work:</span></span>

```bash
notepad.exe C:\\temp\\foo.txt
```

## <a name="share-environment-variables-between-windows-and-wsl"></a><span data-ttu-id="ea678-153">Freigeben von Umgebungsvariablen zwischen Windows und WSL</span><span class="sxs-lookup"><span data-stu-id="ea678-153">Share environment variables between Windows and WSL</span></span>

<span data-ttu-id="ea678-154">WSL und Windows verwenden `WSLENV`, eine spezielle Umgebungsvariable, die entwickelt wurde, um Windows- und Linux-Verteilungen, die unter WSL ausgeführt werden, zu verbinden.</span><span class="sxs-lookup"><span data-stu-id="ea678-154">WSL and Windows share a special environment variable, `WSLENV`, created to bridge Windows and Linux distributions running on WSL.</span></span>

<span data-ttu-id="ea678-155">Eigenschaften einer `WSLENV`-Variablen:</span><span class="sxs-lookup"><span data-stu-id="ea678-155">Properties of `WSLENV` variable:</span></span>

* <span data-ttu-id="ea678-156">Die Variable ist freigegeben, und sie ist sowohl in Windows- als auch in WSL-Umgebungen vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ea678-156">It is shared; it exists in both Windows and WSL environments.</span></span>
* <span data-ttu-id="ea678-157">Es handelt sich um eine Liste von Umgebungsvariablen, die von Windows und WSL gemeinsam genutzt werden können.</span><span class="sxs-lookup"><span data-stu-id="ea678-157">It is a list of environment variables to share between Windows and WSL.</span></span>
* <span data-ttu-id="ea678-158">Sie kann Umgebungsvariablen so formatieren, dass sie in Windows und WSL gut funktionieren.</span><span class="sxs-lookup"><span data-stu-id="ea678-158">It can format environment variables to work well in Windows and WSL.</span></span>

> [!NOTE]
> <span data-ttu-id="ea678-159">Vor 17063 war `PATH` die einzige Windows-Umgebungsvariable, auf die WSL zugreifen konnte (sodass Sie ausführbare Win32-Dateien unter WSL starten konnten).</span><span class="sxs-lookup"><span data-stu-id="ea678-159">Prior to 17063, only Windows environment variable that WSL could access was `PATH` (so you could launch Win32 executables from under WSL).</span></span> <span data-ttu-id="ea678-160">Ab 17063 wird `WSLENV` unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea678-160">Starting in 17063, `WSLENV` begins being supported.</span></span>

## <a name="wslenv-flags"></a><span data-ttu-id="ea678-161">WSLENV-Flags</span><span class="sxs-lookup"><span data-stu-id="ea678-161">WSLENV flags</span></span>

<span data-ttu-id="ea678-162">In `WSLENV` sind vier Flags verfügbar, die beeinflussen, wie die Umgebungsvariable übersetzt wird.</span><span class="sxs-lookup"><span data-stu-id="ea678-162">There are four flags available in `WSLENV` to influence how the environment variable is translated.</span></span>

<span data-ttu-id="ea678-163">`WSLENV`-Flags:</span><span class="sxs-lookup"><span data-stu-id="ea678-163">`WSLENV` flags:</span></span>

* <span data-ttu-id="ea678-164">`/p`: Übersetzt den Pfad zwischen Pfaden im WSL-/Linux-Stil und Win32-Pfaden.</span><span class="sxs-lookup"><span data-stu-id="ea678-164">`/p` - translates the path between WSL/Linux style paths and Win32 paths.</span></span>
* <span data-ttu-id="ea678-165">`/l`: Gibt an, dass die Umgebungsvariable eine Liste von Pfaden ist.</span><span class="sxs-lookup"><span data-stu-id="ea678-165">`/l` - indicates the environment variable is a list of paths.</span></span>
* <span data-ttu-id="ea678-166">`/u`: Gibt an, dass diese Umgebungsvariable nur beim Ausführen von WSL aus Win32 einbezogen werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea678-166">`/u` - indicates that this environment variable should only be included when running WSL from Win32.</span></span>
* <span data-ttu-id="ea678-167">`/w`: Gibt an, dass diese Umgebungsvariable nur beim Ausführen von Win32 aus WSL einbezogen werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea678-167">`/w` - indicates that this environment variable should only be included when running Win32 from WSL.</span></span>

<span data-ttu-id="ea678-168">Diese Flags können nach Bedarf kombiniert werden.</span><span class="sxs-lookup"><span data-stu-id="ea678-168">Flags can be combined as needed.</span></span>

## <a name="disable-interoperability"></a><span data-ttu-id="ea678-169">Deaktivieren der Interoperabilität</span><span class="sxs-lookup"><span data-stu-id="ea678-169">Disable interoperability</span></span>

<span data-ttu-id="ea678-170">Benutzer können die Möglichkeit zum Ausführen von Windows-Tools für eine einzelne WSL-Sitzung deaktivieren, indem Sie den folgenden Befehl als root ausführen:</span><span class="sxs-lookup"><span data-stu-id="ea678-170">Users may disable the ability to run Windows tools for a single WSL session by running the following command as root:</span></span>

```bash
echo 0 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="ea678-171">Zum erneuten Aktivieren von Windows-Binärdateien beenden Sie alle WSL-Sitzungen und führen „bash.exe“ erneut aus, oder führen Sie den folgenden Befehl als root aus:</span><span class="sxs-lookup"><span data-stu-id="ea678-171">To re-enable Windows binaries, exit all WSL sessions and re-run bash.exe or run the following command as root:</span></span>

```bash
echo 1 > /proc/sys/fs/binfmt_misc/WSLInterop
```

<span data-ttu-id="ea678-172">Die Deaktivierung von Interop wird nicht zwischen WSL-Sitzungen beibehalten. Interop wird erneut aktiviert, wenn eine neue Sitzung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="ea678-172">Disabling interop will not persist between WSL sessions -- interop will be enabled again when a new session is launched.</span></span>

## <a name="earlier-versions-of-windows-10"></a><span data-ttu-id="ea678-173">Frühere Windows 10-Versionen</span><span class="sxs-lookup"><span data-stu-id="ea678-173">Earlier versions of Windows 10</span></span>

<span data-ttu-id="ea678-174">Für die Interoperabilitätsbefehle in früheren Windows 10-Versionen bestehen mehrere Unterschiede.</span><span class="sxs-lookup"><span data-stu-id="ea678-174">There are several differences for the interoperability commands on earlier Windows 10 versions.</span></span> <span data-ttu-id="ea678-175">Wenn Sie ein Creators Update (Okt. 2017, Build 16299) oder ein Anniversary Update (Aug. 2016, Build 14393) von Windows 10 ausführen, empfehlen wir, dass Sie [auf die neueste Windows-Version aktualisieren](ms-settings:windowsupdate). Wenn dies jedoch nicht möglich ist, werden nachfolgend einige der Unterschiede in der Interoperabilität erläutert.</span><span class="sxs-lookup"><span data-stu-id="ea678-175">If you're running a Creators Update (Oct 2017, Build 16299), or Anniversary Update (Aug 2016, Build 14393) version of Windows 10, we recommend you [update to the latest Windows version](ms-settings:windowsupdate), but if that's not possible, we have outlined some of the interop differences below.</span></span>

<span data-ttu-id="ea678-176">Zusammenfassung:</span><span class="sxs-lookup"><span data-stu-id="ea678-176">Summary:</span></span>

* <span data-ttu-id="ea678-177">`bash.exe` wurde durch `wsl.exe` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="ea678-177">`bash.exe` has been replaced with `wsl.exe`.</span></span>
* <span data-ttu-id="ea678-178">Die `-c`-Option zum Ausführen eines einzelnen Befehls ist mit `wsl.exe` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ea678-178">`-c` option for running a single command isn't needed with `wsl.exe`.</span></span>
* <span data-ttu-id="ea678-179">Der Windows-Pfad ist in `$PATH` von WSL enthalten.</span><span class="sxs-lookup"><span data-stu-id="ea678-179">Windows path is included in the WSL `$PATH`.</span></span>
* <span data-ttu-id="ea678-180">Der Prozess zum Deaktivieren von Interop ist unverändert.</span><span class="sxs-lookup"><span data-stu-id="ea678-180">The process for disabling interop is unchanged.</span></span>

<span data-ttu-id="ea678-181">Linux-Befehle können an der Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden. Für frühe Windows-Versionen müssen Sie jedoch möglicherweise den Befehl `bash` verwenden.</span><span class="sxs-lookup"><span data-stu-id="ea678-181">Linux commands can be run from the Windows Command Prompt or from PowerShell, but for early Windows versions, you man need to use the `bash` command.</span></span> <span data-ttu-id="ea678-182">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ea678-182">For example:</span></span>

```powershell
C:\temp> bash -c "ls -la"
```

<span data-ttu-id="ea678-183">Dinge wie Eingabe, Piping und Dateiumleitung funktionieren erwartungsgemäß.</span><span class="sxs-lookup"><span data-stu-id="ea678-183">Things such as input, piping, and file redirection work as expected.</span></span>

<span data-ttu-id="ea678-184">Die an `bash -c` übergebenen WSL-Befehle werden ohne Änderung an den WSL-Prozess weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="ea678-184">The WSL commands passed into `bash -c` are forwarded to the WSL process without modification.</span></span>  <span data-ttu-id="ea678-185">Dateipfade müssen im WSL-Format angegeben werden, und es muss darauf geachtet werden, dass relevante Zeichen mit Escapezeichen versehen werden.</span><span class="sxs-lookup"><span data-stu-id="ea678-185">File paths must be specified in the WSL format and care must be taken to escape relevant characters.</span></span> <span data-ttu-id="ea678-186">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ea678-186">Example:</span></span>

```console
C:\temp> bash -c "ls -la /proc/cpuinfo"
```

<span data-ttu-id="ea678-187">Oder:</span><span class="sxs-lookup"><span data-stu-id="ea678-187">Or...</span></span>

```powershell
C:\temp> bash -c "ls -la \"/mnt/c/Program Files\""
```

<span data-ttu-id="ea678-188">Wenn Sie ein Windows-Tool aus einer WSL-Verteilung in einer früheren Version von Windows 10 aufrufen, müssen Sie den Verzeichnispfad angeben.</span><span class="sxs-lookup"><span data-stu-id="ea678-188">When calling a Windows tool from a WSL distribution in an earlier version of Windows 10, you will need to specify the directory path.</span></span> <span data-ttu-id="ea678-189">Geben Sie z. B. in der WSL-Befehlszeile Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="ea678-189">For example, from your WSL command line, enter:</span></span>

```bash
/mnt/c/Windows/System32/notepad.exe
```

<span data-ttu-id="ea678-190">In WSL werden diese ausführbaren Dateien ähnlich wie native ausführbare Linux-Dateien behandelt.</span><span class="sxs-lookup"><span data-stu-id="ea678-190">In WSL, these executables are handled similar to native Linux executables.</span></span>  <span data-ttu-id="ea678-191">Dies bedeutet, dass das Hinzufügen von Verzeichnissen zum Linux-Pfad und das Piping zwischen Befehlen erwartungsgemäß funktioniert.</span><span class="sxs-lookup"><span data-stu-id="ea678-191">This means adding directories to the Linux path and piping between commands works as expected.</span></span>  <span data-ttu-id="ea678-192">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ea678-192">For example:</span></span>

```bash
export PATH=$PATH:/mnt/c/Windows/System32
```
<span data-ttu-id="ea678-193">Oder</span><span class="sxs-lookup"><span data-stu-id="ea678-193">Or</span></span>

```bash
ipconfig.exe | grep IPv4 | cut -d: -f2
```

<span data-ttu-id="ea678-194">Die Windows-Binärdatei muss die Dateierweiterung enthalten, der Groß-/Kleinschreibung der Datei Rechnung tragen und eine ausführbare Dateien sein.</span><span class="sxs-lookup"><span data-stu-id="ea678-194">The Windows binary must include the file extension, match the file case, and be executable.</span></span>  <span data-ttu-id="ea678-195">Nicht ausführbare Dateien einschließlich Batchskripts und Befehle wie `dir` können mit dem Befehl `/mnt/c/Windows/System32/cmd.exe /C` ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ea678-195">Non-executables including batch scripts and command like `dir` can be run with `/mnt/c/Windows/System32/cmd.exe /C` command.</span></span> <span data-ttu-id="ea678-196">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="ea678-196">For example:</span></span>

```bash
/mnt/c/Windows/System32/cmd.exe /C dir
```

## <a name="additional-resources"></a><span data-ttu-id="ea678-197">Zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ea678-197">Additional resources</span></span>

* [<span data-ttu-id="ea678-198">WSL-Blogbeitrag zur Interoperabilität von 2016</span><span class="sxs-lookup"><span data-stu-id="ea678-198">WSL blog post on interoperability from 2016</span></span>](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/)
