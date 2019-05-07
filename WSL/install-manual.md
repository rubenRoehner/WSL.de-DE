---
title: Manuelles Herunterladen von Windows-Subsystem für Linux (WSL)-Distributionen
description: Anweisungen zum Manuelles Herunterladen von Windows-Subsystem für Linux-Distributionen.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, WSL, Windows-Subsystem, -Distribution, Ubuntu, OpenSUSE, SLES, debian, Kali
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: be1c1331183317d4f970696464110b9968208d21
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59063568"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a><span data-ttu-id="34513-104">Manuelles Herunterladen von Windows-Subsystem für Linux-Distribution-Pakete</span><span class="sxs-lookup"><span data-stu-id="34513-104">Manually download Windows Subsystem for Linux distro packages</span></span>

<span data-ttu-id="34513-105">Es gibt mehrere Szenarios, in dem darf nicht in der Lage (oder möchten), WSL-Linux-Distributionen, über den Microsoft Store zu installieren.</span><span class="sxs-lookup"><span data-stu-id="34513-105">There are several scenarios in which you may not be able (or want) to, install WSL Linux distros via the Microsoft Store.</span></span> <span data-ttu-id="34513-106">Insbesondere können Sie ausgeführt werden, einem Windows Server- oder Long-term Servicing (LTSB/LTSC) Desktop-Betriebssystem-SKU, die Microsoft Store, oder Ihre zum Zulassen von Microsoft Store-Verwendung in Ihrer Umgebung nicht Unternehmensnetzwerk Richtlinien und/oder Administratoren nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34513-106">Specifically, you may be running a Windows Server or Long-Term Servicing (LTSB/LTSC) desktop OS SKU that doesn't support Microsoft Store, or your corporate network policies and/or admins to not permit Microsoft Store usage in your environment.</span></span>

<span data-ttu-id="34513-107">In diesen Fällen WSL selbst zur Verfügung steht, wie Sie herunterladen und installieren Linux-Distributionen in WSL, wenn Sie nicht den Speicher zugreifen können?</span><span class="sxs-lookup"><span data-stu-id="34513-107">In these cases, while WSL itself is available, how do you download and install Linux distros in WSL if you can't access the store?</span></span>

> <span data-ttu-id="34513-108">Hinweis: **Befehlszeilenshell Umgebungen Cmd, PowerShell und Linux/WSL Distributionen einschließlich dürfen nicht auf Windows 10 S-Modus ausführen**.</span><span class="sxs-lookup"><span data-stu-id="34513-108">Note: **Command-line shell environments including Cmd, PowerShell, and Linux/WSL distros are not permitted to run on Windows 10 S Mode**.</span></span> <span data-ttu-id="34513-109">Diese Einschränkung gilt, um sicherzustellen, dass die Integrität und Sicherheit Ziele, die S-Modus bietet: Lesen [diesen Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) für Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="34513-109">This restriction exists in order to ensure the integrity and safety goals that S Mode delivers: Read [this post](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) for more information.</span></span>

## <a name="downloading-distros"></a><span data-ttu-id="34513-110">Herunterladen von Distributionen</span><span class="sxs-lookup"><span data-stu-id="34513-110">Downloading distros</span></span>

<span data-ttu-id="34513-111">Wenn die Microsoft Store-app nicht verfügbar ist, können Sie herunterladen und installieren Linux-Distributionen manuell durch Klicken auf diese Links:</span><span class="sxs-lookup"><span data-stu-id="34513-111">If the Microsoft Store app is not available, you can download and manually install Linux distros by clicking these links:</span></span>
* [<span data-ttu-id="34513-112">Ubuntu 18.04</span><span class="sxs-lookup"><span data-stu-id="34513-112">Ubuntu 18.04</span></span>](https://aka.ms/wsl-ubuntu-1804)
* [<span data-ttu-id="34513-113">Ubuntu 18.04 ARM</span><span class="sxs-lookup"><span data-stu-id="34513-113">Ubuntu 18.04 ARM</span></span>](https://aka.ms/wsl-ubuntu-1804-arm)
* [<span data-ttu-id="34513-114">Ubuntu 16.04</span><span class="sxs-lookup"><span data-stu-id="34513-114">Ubuntu 16.04</span></span>](https://aka.ms/wsl-ubuntu-1604)
* [<span data-ttu-id="34513-115">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="34513-115">Debian GNU/Linux</span></span>](https://aka.ms/wsl-debian-gnulinux)
* [<span data-ttu-id="34513-116">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="34513-116">Kali Linux</span></span>](https://aka.ms/wsl-kali-linux)
* [<span data-ttu-id="34513-117">OpenSUSE</span><span class="sxs-lookup"><span data-stu-id="34513-117">OpenSUSE</span></span>](https://aka.ms/wsl-opensuse-42)
* [<span data-ttu-id="34513-118">SLES</span><span class="sxs-lookup"><span data-stu-id="34513-118">SLES</span></span>](https://aka.ms/wsl-sles-12)

<span data-ttu-id="34513-119">Dies bewirkt, dass die `<distro>.appx` Pakete in einen Ordner Ihrer Wahl herunterladen.</span><span class="sxs-lookup"><span data-stu-id="34513-119">This will cause the `<distro>.appx` packages to download to a folder of your choosing.</span></span> <span data-ttu-id="34513-120">Führen Sie die [installationsanweisungen](#installing-your-distro) um Ihre heruntergeladene Distro(s) zu installieren.</span><span class="sxs-lookup"><span data-stu-id="34513-120">Follow the [installation instructions](#installing-your-distro) to install your downloaded distro(s).</span></span>

## <a name="downloading-distros-via-the-command-line"></a><span data-ttu-id="34513-121">Herunterladen von Distributionen über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="34513-121">Downloading distros via the command line</span></span>
<span data-ttu-id="34513-122">Falls gewünscht, können Sie auch Ihre bevorzugte Distro(s) über die Befehlszeile herunterladen:</span><span class="sxs-lookup"><span data-stu-id="34513-122">If you prefer, you can also download your preferred distro(s) via the command line:</span></span>

 ### <a name="download-using-powershell"></a><span data-ttu-id="34513-123">Laden Sie mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="34513-123">Download using PowerShell</span></span>
 <span data-ttu-id="34513-124">Verwenden Sie zum Herunterladen mithilfe von PowerShell Distributionen die [Invoke-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) Cmdlet.</span><span class="sxs-lookup"><span data-stu-id="34513-124">To download distros using PowerShell, use the [Invoke-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) cmdlet.</span></span> <span data-ttu-id="34513-125">Hier ist eine Beispiel-Anleitung zum Herunterladen von Ubuntu 16.04.</span><span class="sxs-lookup"><span data-stu-id="34513-125">Here's a sample instruction to download Ubuntu 16.04.</span></span>

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> <span data-ttu-id="34513-126">Wenn der Download sehr lange dauert, deaktivieren Sie die Statusanzeige festlegen `$ProgressPreference = 'SilentlyContinue'`</span><span class="sxs-lookup"><span data-stu-id="34513-126">If the download is taking a long time, turn off the progress bar by setting `$ProgressPreference = 'SilentlyContinue'`</span></span>

### <a name="download-using-curl"></a><span data-ttu-id="34513-127">Laden Sie mithilfe von curl</span><span class="sxs-lookup"><span data-stu-id="34513-127">Download using curl</span></span>
<span data-ttu-id="34513-128">Windows 10 Frühjahr 2018 Update (oder höher) enthält das beliebte [curl-Befehlszeilen-Hilfsprogramm](https://curl.haxx.se/) mit dem Sie webanforderungen (d. h. HTTP-GET, POST, PUT, Befehle von usw.) über die Befehlszeile aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="34513-128">Windows 10 Spring 2018 Update (or later) includes the popular [curl command-line utility](https://curl.haxx.se/) with which you can invoke web requests (i.e. HTTP GET, POST, PUT, etc. commands) from the command line.</span></span> <span data-ttu-id="34513-129">Sie können `curl.exe` zum Herunterladen von der oben aufgeführten Distributionen:</span><span class="sxs-lookup"><span data-stu-id="34513-129">You can use `curl.exe` to download the above distros:</span></span>

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

<span data-ttu-id="34513-130">Im obigen Beispiel `curl.exe` ausgeführt wird (nicht nur `curl`) sicherstellen, dass in PowerShell ist die echten Curl ausführbare Datei aufgerufen wird, nicht PowerShell Curl alias für [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="34513-130">In the above example, `curl.exe` is executed (not just `curl`) to ensure that, in PowerShell, the real curl executable is invoked, not the PowerShell curl alias for [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)</span></span>

> <span data-ttu-id="34513-131">Hinweis: Mithilfe von `curl` kann vorteilhafter sein, wenn man Download-Schritte, die mithilfe des Cmd-Shell aufrufen bzw. das Skript bzw. `.bat`  /  `.cmd` Skripts.</span><span class="sxs-lookup"><span data-stu-id="34513-131">Note: Using `curl` might be preferable if you have to invoke/script download steps using Cmd shell and/or `.bat` / `.cmd` scripts.</span></span>

## <a name="installing-your-distro"></a><span data-ttu-id="34513-132">Installieren von Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="34513-132">Installing your distro</span></span>
<span data-ttu-id="34513-133">Anweisungen dazu, wie Sie Ihre heruntergeladene Distro(s) installieren, finden Sie in der [Windows Desktop](install-win10.md) oder [WindowsServer](install-on-server.md) installationsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="34513-133">For instructions on how to install your downloaded distro(s), please refer to the [Windows Desktop](install-win10.md) or [Windows Server](install-on-server.md) installation instructions.</span></span>
