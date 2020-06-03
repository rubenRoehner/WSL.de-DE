---
title: Manuelles Herunterladen von WSL-Distributionen (Windows-Subsystem für Linux)
description: Anweisungen zum manuellen Herunterladen von Distributionen des Windows-Subsystems für Linux.
keywords: WSL, Windows-Subsystem für Linux, manuelle Installation, manuell installieren, Microsoft Store, Windows 10s, curl, Add-AppxPackage, Langzeitwartung, LTSC
ms.date: 05/28/2020
ms.topic: article
ms.localizationpriority: medium
ms.openlocfilehash: 621b2619d6c62e0b6c4e53f7791fc587c1c8f878
ms.sourcegitcommit: 09f5eb0f6062642e5c86deb1f34307ce3429163a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/29/2020
ms.locfileid: "84211716"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a><span data-ttu-id="da1a2-104">Manuelles Herunterladen von Distributionspaketen des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="da1a2-104">Manually download Windows Subsystem for Linux distro packages</span></span>

<span data-ttu-id="da1a2-105">Es gibt eine Reihe von Szenarien, in denen Sie möglicherweise nicht in der Lage sind, Distributionen von WSL Linux über den Microsoft Store zu installieren, oder dies nicht wünschen.</span><span class="sxs-lookup"><span data-stu-id="da1a2-105">There are several scenarios in which you may not be able (or want) to, install WSL Linux distros via the Microsoft Store.</span></span> <span data-ttu-id="da1a2-106">Insbesondere kann dies eintreten, wenn Sie eine SKU von Windows Server oder eines LTSC-Desktopbetriebssystems (Long-Term Servicing) ausführen, die den Microsoft Store nicht unterstützt, oder die Netzwerkrichtlinien Ihres Unternehmens und/oder die Administratoren die Nutzung des Microsoft Stores in Ihrer Umgebung nicht erlauben.</span><span class="sxs-lookup"><span data-stu-id="da1a2-106">Specifically, you may be running a Windows Server or Long-Term Servicing (LTSC) desktop OS SKU that doesn't support Microsoft Store, or your corporate network policies and/or admins to not permit Microsoft Store usage in your environment.</span></span>

<span data-ttu-id="da1a2-107">Wie können Sie in diesen Fällen, wenn das eigentliche WSL verfügbar ist, Linux-Distributionen herunterladen und in WSL installieren, wenn Sie nicht auf den Store zugreifen können?</span><span class="sxs-lookup"><span data-stu-id="da1a2-107">In these cases, while WSL itself is available, how do you download and install Linux distros in WSL if you can't access the store?</span></span>

> <span data-ttu-id="da1a2-108">Hinweis: **Befehlszeilenshellumgebungen, einschließlich Cmd, PowerShell und Linux/WSL-Distributionen, dürfen im Windows 10 S-Modus nicht ausgeführt werden**.</span><span class="sxs-lookup"><span data-stu-id="da1a2-108">Note: **Command-line shell environments including Cmd, PowerShell, and Linux/WSL distros are not permitted to run on Windows 10 S Mode**.</span></span> <span data-ttu-id="da1a2-109">Diese Einschränkung wurde implementiert, um die Integritäts- und Sicherheitsziele des S-Modus sicherzustellen: Weitere Informationen finden Sie in [diesem Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/).</span><span class="sxs-lookup"><span data-stu-id="da1a2-109">This restriction exists in order to ensure the integrity and safety goals that S Mode delivers: Read [this post](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) for more information.</span></span>

## <a name="downloading-distros"></a><span data-ttu-id="da1a2-110">Herunterladen von Distributionen</span><span class="sxs-lookup"><span data-stu-id="da1a2-110">Downloading distros</span></span>

<span data-ttu-id="da1a2-111">Wenn die Microsoft Store-App nicht verfügbar ist, können Sie Linux-Distributionen manuell herunterladen und installieren, indem Sie auf die folgenden Links klicken:</span><span class="sxs-lookup"><span data-stu-id="da1a2-111">If the Microsoft Store app is not available, you can download and manually install Linux distros by clicking these links:</span></span>
* [<span data-ttu-id="da1a2-112">Ubuntu 18.04</span><span class="sxs-lookup"><span data-stu-id="da1a2-112">Ubuntu 18.04</span></span>](https://aka.ms/wsl-ubuntu-1804)
* [<span data-ttu-id="da1a2-113">Ubuntu 18.04 ARM</span><span class="sxs-lookup"><span data-stu-id="da1a2-113">Ubuntu 18.04 ARM</span></span>](https://aka.ms/wsl-ubuntu-1804-arm)
* [<span data-ttu-id="da1a2-114">Ubuntu 16.04</span><span class="sxs-lookup"><span data-stu-id="da1a2-114">Ubuntu 16.04</span></span>](https://aka.ms/wsl-ubuntu-1604)
* [<span data-ttu-id="da1a2-115">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="da1a2-115">Debian GNU/Linux</span></span>](https://aka.ms/wsl-debian-gnulinux)
* [<span data-ttu-id="da1a2-116">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="da1a2-116">Kali Linux</span></span>](https://aka.ms/wsl-kali-linux-new)
* [<span data-ttu-id="da1a2-117">OpenSUSE Leap 42</span><span class="sxs-lookup"><span data-stu-id="da1a2-117">OpenSUSE Leap 42</span></span>](https://aka.ms/wsl-opensuse-42)
* [<span data-ttu-id="da1a2-118">SUSE Linux Enterprise Server 12</span><span class="sxs-lookup"><span data-stu-id="da1a2-118">SUSE Linux Enterprise Server 12</span></span>](https://aka.ms/wsl-sles-12)
* [<span data-ttu-id="da1a2-119">Fedora Remix for WSL</span><span class="sxs-lookup"><span data-stu-id="da1a2-119">Fedora Remix for WSL</span></span>](https://github.com/WhitewaterFoundry/WSLFedoraRemix/releases/)

<span data-ttu-id="da1a2-120">Dies bewirkt den Download der `<distro>.appx`-Pakete in einen Ordner Ihrer Wahl.</span><span class="sxs-lookup"><span data-stu-id="da1a2-120">This will cause the `<distro>.appx` packages to download to a folder of your choosing.</span></span> <span data-ttu-id="da1a2-121">Befolgen Sie die [Installationsanweisungen](#installing-your-distro), um die heruntergeladenen Distributionen zu installieren.</span><span class="sxs-lookup"><span data-stu-id="da1a2-121">Follow the [installation instructions](#installing-your-distro) to install your downloaded distro(s).</span></span>

## <a name="downloading-distros-via-the-command-line"></a><span data-ttu-id="da1a2-122">Herunterladen von Distributionen über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="da1a2-122">Downloading distros via the command line</span></span>
<span data-ttu-id="da1a2-123">Wenn Sie möchten, können Sie Ihre bevorzugten Distributionen auch über die Befehlszeile herunterladen:</span><span class="sxs-lookup"><span data-stu-id="da1a2-123">If you prefer, you can also download your preferred distro(s) via the command line:</span></span>

 ### <a name="download-using-powershell"></a><span data-ttu-id="da1a2-124">Herunterladen mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="da1a2-124">Download using PowerShell</span></span>
 <span data-ttu-id="da1a2-125">Zum Herunterladen von Distributionen mithilfe von PowerShell verwenden Sie das [Invoke-WebRequest](https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-5.1)-Cmdlet.</span><span class="sxs-lookup"><span data-stu-id="da1a2-125">To download distros using PowerShell, use the [Invoke-WebRequest](https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-5.1) cmdlet.</span></span> <span data-ttu-id="da1a2-126">Hier sehen Sie eine Beispielanweisung zum Herunterladen von Ubuntu 16.04.</span><span class="sxs-lookup"><span data-stu-id="da1a2-126">Here's a sample instruction to download Ubuntu 16.04.</span></span>

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> <span data-ttu-id="da1a2-127">Wenn der Download sehr lange dauert, deaktivieren Sie die Statusanzeige, indem Sie `$ProgressPreference = 'SilentlyContinue'` festlegen.</span><span class="sxs-lookup"><span data-stu-id="da1a2-127">If the download is taking a long time, turn off the progress bar by setting `$ProgressPreference = 'SilentlyContinue'`</span></span>

### <a name="download-using-curl"></a><span data-ttu-id="da1a2-128">Herunterladen mit curl</span><span class="sxs-lookup"><span data-stu-id="da1a2-128">Download using curl</span></span>
<span data-ttu-id="da1a2-129">Das Windows 10-Update aus Frühjahr 2018 (oder höher) umfasst das beliebte [curl-Befehlszeilenhilfsprogramm](https://curl.haxx.se/), mit dem Sie Webanforderungen (d. h. Befehle der Art HTTP GET, POST, PUT usw.) von der Befehlszeile aus aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="da1a2-129">Windows 10 Spring 2018 Update (or later) includes the popular [curl command-line utility](https://curl.haxx.se/) with which you can invoke web requests (i.e. HTTP GET, POST, PUT, etc. commands) from the command line.</span></span> <span data-ttu-id="da1a2-130">Mit `curl.exe` können Sie die oben genannten Distributionen herunterladen:</span><span class="sxs-lookup"><span data-stu-id="da1a2-130">You can use `curl.exe` to download the above distros:</span></span>

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

<span data-ttu-id="da1a2-131">Im Beispiel oben wird `curl.exe` ausgeführt (nicht einfach `curl`), um sicherzustellen, dass in PowerShell die echte curl-Programmdatei aufgerufen wird, nicht der curl-Alias von PowerShell für [Invoke-WebRequest](https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="da1a2-131">In the above example, `curl.exe` is executed (not just `curl`) to ensure that, in PowerShell, the real curl executable is invoked, not the PowerShell curl alias for [Invoke-WebRequest](https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)</span></span>

> <span data-ttu-id="da1a2-132">Hinweis: Die Verwendung von `curl` kann Vorteile bieten, wenn Sie mithilfe der Cmd-Shell und/oder `.bat` / `.cmd` Schritte zum Herunterladen aufrufen/skripten müssen.</span><span class="sxs-lookup"><span data-stu-id="da1a2-132">Note: Using `curl` might be preferable if you have to invoke/script download steps using Cmd shell and/or `.bat` / `.cmd` scripts.</span></span>

## <a name="installing-your-distro"></a><span data-ttu-id="da1a2-133">Installieren der Distribution</span><span class="sxs-lookup"><span data-stu-id="da1a2-133">Installing your distro</span></span>
<span data-ttu-id="da1a2-134">Wenn Sie Windows 10 verwenden, können Sie Ihre Distribution mit PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="da1a2-134">If you're using Windows 10 you can install your distro with PowerShell.</span></span> <span data-ttu-id="da1a2-135">Navigieren Sie einfach zu dem Ordner, der die oben heruntergeladene Distribution enthält, und führen Sie in diesem Verzeichnis den folgenden Befehl aus, wobei `app_name` für den Namen der APPX-Datei Ihrer Distribution steht.</span><span class="sxs-lookup"><span data-stu-id="da1a2-135">Simply navigate to folder containing the distro downloaded from above, and in that directory run the following command where `app_name` is the name of your distro .appx file.</span></span>  
```Powershell
Add-AppxPackage .\app_name.appx
```

<span data-ttu-id="da1a2-136">Wenn Sie Windows Server verwenden, finden Sie die Installationsanweisungen auf der [Windows Server](install-on-server.md)-Dokumentationsseite.</span><span class="sxs-lookup"><span data-stu-id="da1a2-136">If you are using Windows server you can find the install instructions on the [Windows Server](install-on-server.md) documentation page.</span></span>

<span data-ttu-id="da1a2-137">Sobald Ihre Verteilung installiert wurde, folgen Sie den normalen Anweisungen, um [auf WSL 2 zu aktualisieren](./install-win10.md#update-to-wsl-2) oder [ein neues Benutzerkonto und Kennwort zu erstellen](./user-support.md).</span><span class="sxs-lookup"><span data-stu-id="da1a2-137">Once your distribution is installed, follow the normal instructions to [update to WSL 2](./install-win10.md#update-to-wsl-2) or [create a new user account and password](./user-support.md).</span></span>
