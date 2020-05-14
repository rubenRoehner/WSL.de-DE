---
title: Übersicht über das Windows-Subsystem für Linux
description: Informieren Sie sich über das Windows-Subsystem für Linux, die verschiedenen Versionen und die Art und Weise, wie Sie sie verwenden können.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, gnu, linux
ms.date: 05/12/2020
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.localizationpriority: high
ms.openlocfilehash: 90a661c408cacbef95a869ac896a40381120d52e
ms.sourcegitcommit: 1b6191351bbf9e95f3c28fc67abe4bf1bcfd3336
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83270794"
---
# <a name="what-is-the-windows-subsystem-for-linux"></a><span data-ttu-id="3540c-104">Was ist das Windows-Subsystem für Linux?</span><span class="sxs-lookup"><span data-stu-id="3540c-104">What is the Windows Subsystem for Linux?</span></span>

<span data-ttu-id="3540c-105">Mit dem Windows-Subsystem für Linux können Entwickler eine GNU-/Linux-Umgebung (einschließlich der meisten Befehlszeilentools, Hilfsprogramme und Anwendungen) direkt unter Windows unverändert ausführen, ohne den Mehraufwand eines virtuellen Computers betreiben zu müssen.</span><span class="sxs-lookup"><span data-stu-id="3540c-105">The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a virtual machine.</span></span>

<span data-ttu-id="3540c-106">Sie haben folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="3540c-106">You can:</span></span>

* <span data-ttu-id="3540c-107">Wählen Sie Ihre bevorzugten GNU-/Linux -Distributionen aus dem [Microsoft Store](https://aka.ms/wslstore) aus.</span><span class="sxs-lookup"><span data-stu-id="3540c-107">Choose your favorite GNU/Linux distributions [from the Microsoft Store](https://aka.ms/wslstore).</span></span>
* <span data-ttu-id="3540c-108">Führen Sie gängige Befehlszeilentools wie `grep`, `sed`, `awk` oder andere ELF-64-Binärdateien aus.</span><span class="sxs-lookup"><span data-stu-id="3540c-108">Run common command-line tools such as `grep`, `sed`, `awk`, or other ELF-64 binaries.</span></span>
* <span data-ttu-id="3540c-109">Führen Sie Skripts der Bash-Shell und GNU-/Linux-Befehlszeilenanwendungen aus, beispielsweise:</span><span class="sxs-lookup"><span data-stu-id="3540c-109">Run Bash shell scripts and GNU/Linux command-line applications including:</span></span>  
    * <span data-ttu-id="3540c-110">Tools: vim, emacs, tmux \*Sprachen: [NodeJS](https://docs.microsoft.com/windows/nodejs/setup-on-wsl2), Javascript, [Python](https://docs.microsoft.com/windows/python/web-frameworks), Ruby, C/C++, C# & F#, Rust, Go usw. \*Dienste: SSHD, MySQL, Apache, lighttpd, [MongoDB](https://docs.microsoft.com/windows/nodejs/databases), [PostgreSQL](https://docs.microsoft.com/windows/python/databases).</span><span class="sxs-lookup"><span data-stu-id="3540c-110">Tools: vim, emacs, tmux \*Languages: [NodeJS](https://docs.microsoft.com/windows/nodejs/setup-on-wsl2), Javascript, [Python](https://docs.microsoft.com/windows/python/web-frameworks), Ruby, C/C++, C# & F#, Rust, Go, etc. \*Services: SSHD, MySQL, Apache, lighttpd, [MongoDB](https://docs.microsoft.com/windows/nodejs/databases), [PostgreSQL](https://docs.microsoft.com/windows/python/databases).</span></span>
* <span data-ttu-id="3540c-111">Installieren Sie zusätzliche Software mit einem eigenen Paket-Manager für die GNU-/Linux-Distribution.</span><span class="sxs-lookup"><span data-stu-id="3540c-111">Install additional software using own GNU/Linux distribution package manager.</span></span>
* <span data-ttu-id="3540c-112">Rufen Sie Windows-Anwendungen mithilfe einer Unix-ähnlichen Befehlszeilenshell auf.</span><span class="sxs-lookup"><span data-stu-id="3540c-112">Invoke Windows applications using a Unix-like command-line shell.</span></span>
* <span data-ttu-id="3540c-113">Rufen Sie GNU-/Linux-Anwendungen unter Windows auf.</span><span class="sxs-lookup"><span data-stu-id="3540c-113">Invoke GNU/Linux applications on Windows.</span></span>

## <a name="what-is-wsl-2"></a><span data-ttu-id="3540c-114">Was ist WSL 2?</span><span class="sxs-lookup"><span data-stu-id="3540c-114">What is WSL 2?</span></span>

<span data-ttu-id="3540c-115">WSL 2 ist eine neue Version der Windows-Subsystem für Linux-Architektur, die es dem Windows-Subsystem für Linux ermöglicht, ELF64-Linux-Binärdateien unter Windows auszuführen.</span><span class="sxs-lookup"><span data-stu-id="3540c-115">WSL 2 is a new version of the Windows Subsystem for Linux architecture that powers the Windows Subsystem for Linux to run ELF64 Linux binaries on Windows.</span></span> <span data-ttu-id="3540c-116">Die Hauptziele sind eine **gesteigerte Leistung des Dateisystems** sowie das Hinzufügen **vollständiger Kompatibilität von Systemaufrufen**.</span><span class="sxs-lookup"><span data-stu-id="3540c-116">Its primary goals are to **increase file system performance**, as well as adding **full system call compatibility**.</span></span>

<span data-ttu-id="3540c-117">Diese neue Architektur führt zu einer Änderung der Interaktion dieser Linux-Binärdateien mit Windows und der Hardware Ihres Computers, bietet aber die gleiche Benutzererfahrung wie WSL 1 (die aktuelle, allgemein verfügbar Version).</span><span class="sxs-lookup"><span data-stu-id="3540c-117">This new architecture changes how these Linux binaries interact with Windows and your computer's hardware, but still provides the same user experience as in WSL 1 (the current widely available version).</span></span>

<span data-ttu-id="3540c-118">Einzelne Linux-Verteilungen können mit der WSL 1- oder der WSL 2-Architektur ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="3540c-118">Individual Linux distributions can be run with either the WSL 1 or WSL 2 architecture.</span></span> <span data-ttu-id="3540c-119">Für jede Verteilung kann jederzeit ein Upgrade oder Downgrade ausgeführt werden, und Sie können WSL 1- und WSL 2-Verteilungen parallel verwenden.</span><span class="sxs-lookup"><span data-stu-id="3540c-119">Each distribution can be upgraded or downgraded at any time and you can run WSL 1 and WSL 2 distributions side by side.</span></span> <span data-ttu-id="3540c-120">WSL 2 weist eine völlig neue Architektur auf, die von der Ausführung eines echten Linux-Kernels profitiert.</span><span class="sxs-lookup"><span data-stu-id="3540c-120">WSL 2 uses an entirely new architecture that benefits from running a real Linux kernel.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3540c-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="3540c-121">Next steps</span></span>

* [<span data-ttu-id="3540c-122">Installieren von WSL 1 und Aktualisieren auf WSL 2</span><span class="sxs-lookup"><span data-stu-id="3540c-122">Install WSL 1 and update to WSL 2</span></span>](./install-win10.md)

* [<span data-ttu-id="3540c-123">Vergleich zwischen WSL 2 und WSL 1</span><span class="sxs-lookup"><span data-stu-id="3540c-123">Compare WSL 2 and WSL 1</span></span>](./compare-versions.md)

* [<span data-ttu-id="3540c-124">Erstellen eines Benutzerkontos und Kennworts für Ihre neue Linux-Verteilung</span><span class="sxs-lookup"><span data-stu-id="3540c-124">Create a user account and password for your new Linux distribution</span></span>](./user-support.md)

* [<span data-ttu-id="3540c-125">Häufig gestellte Fragen (FAQ)</span><span class="sxs-lookup"><span data-stu-id="3540c-125">Read Frequently Asked Questions</span></span>](./faq.md)

* [<span data-ttu-id="3540c-126">Häufig gestellte Fragen zu WSL 2</span><span class="sxs-lookup"><span data-stu-id="3540c-126">Read Frequently Asked Questions about WSL 2</span></span>](./wsl2-faq.md)

* [<span data-ttu-id="3540c-127">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="3540c-127">Troubleshooting</span></span>](./troubleshooting.md)

* [<span data-ttu-id="3540c-128">Ausführen von Interoperabilitätsbefehlen zwischen Windows und Linux</span><span class="sxs-lookup"><span data-stu-id="3540c-128">Run interoperability commands between Windows and Linux</span></span>](./interop.md)

* [<span data-ttu-id="3540c-129">Ausführen von Startbefehlen und Konfigurationen</span><span class="sxs-lookup"><span data-stu-id="3540c-129">Run launch commands and configurations</span></span>](./wsl-config.md)

* [<span data-ttu-id="3540c-130">Einrichten von Dateiberechtigungen</span><span class="sxs-lookup"><span data-stu-id="3540c-130">Set up file permissions</span></span>](./file-permissions.md)

* [<span data-ttu-id="3540c-131">Einrichten von WSL für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="3540c-131">Set up WSL for Enterprise</span></span>](./enterprise.md)

* [<span data-ttu-id="3540c-132">Verweisen auf WSL-Befehle</span><span class="sxs-lookup"><span data-stu-id="3540c-132">Reference WSL commands</span></span>](./reference.md)

* [<span data-ttu-id="3540c-133">Erstellen von benutzerdefinierten Verteilungen</span><span class="sxs-lookup"><span data-stu-id="3540c-133">Build a custom distributions</span></span>](./build-custom-distro.md)

* [<span data-ttu-id="3540c-134">Lesen Sie die Anmerkungen zu dieser Version von WSL.</span><span class="sxs-lookup"><span data-stu-id="3540c-134">Read the WSL Release Notes</span></span>](./release-notes.md)
