---
title: Häufig gestellte Fragen
description: Häufig gestellte Fragen zum Windows-Subsystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, faq
ms.date: 9/4/2018
ms.topic: article
ms.assetid: 129101ed-b88a-43c2-b6a2-cd2c4ff6fee1
ms.localizationpriority: high
ms.openlocfilehash: 3c3681b0e0e8317917b4ec7c37c9bb2f0bbe9c95
ms.sourcegitcommit: e6e888f2b88a2d9c105cee46e5ab5b70aa43dd80
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83343900"
---
# <a name="frequently-asked-questions-about-windows-subsystem-for-linux"></a><span data-ttu-id="c8225-104">Häufig gestellte Fragen zum Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="c8225-104">Frequently Asked Questions about Windows Subsystem for Linux</span></span>

## <a name="what-is-windows-subsystem-for-linux-wsl"></a><span data-ttu-id="c8225-105">Was ist das Windows-Subsystem für Linux (WSL)?</span><span class="sxs-lookup"><span data-stu-id="c8225-105">What is Windows Subsystem for Linux (WSL)?</span></span>

<span data-ttu-id="c8225-106">Das Windows-Subsystem für Linux (WSL) ist ein neues Windows 10-Feature, das es ermöglicht, native Befehlszeilentools für Linux direkt unter Windows zusammen mit Ihren traditionellen Desktop- und modernen Store-Apps auszuführen.</span><span class="sxs-lookup"><span data-stu-id="c8225-106">The Windows Subsystem for Linux (WSL) is a new Windows 10 feature that enables you to run native Linux command-line tools directly on Windows, alongside your traditional Windows desktop and modern store apps.</span></span>

<span data-ttu-id="c8225-107">Ausführlichere Informationen finden Sie auf der Seite [Informationen](./about.md).</span><span class="sxs-lookup"><span data-stu-id="c8225-107">See the [about page](./about.md) for more details.</span></span>

## <a name="who-is-wsl-for"></a><span data-ttu-id="c8225-108">Für wen ist WSL geeignet?</span><span class="sxs-lookup"><span data-stu-id="c8225-108">Who is WSL for?</span></span>

<span data-ttu-id="c8225-109">Dies ist in erster Linie ein Tool für Entwickler, insbesondere Webentwickler und Benutzer, die an oder mit Open-Source-Projekten arbeiten.</span><span class="sxs-lookup"><span data-stu-id="c8225-109">This is primarily a tool for developers -- especially web developers and those who work on or with open source projects.</span></span> <span data-ttu-id="c8225-110">Dies ermöglicht es Benutzern, die Bash, gängige Linux-Tools (`sed`, `awk` usw.) und viele Linux-First-Tools (Ruby, Python usw.) verwenden möchten/müssen, Ihre Toolkette unter Windows zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="c8225-110">This allows those who want/need to use Bash, common Linux tools (`sed`, `awk`, etc.) and many Linux-first tools (Ruby, Python, etc.) to use their toolchain on Windows.</span></span>

## <a name="what-can-i-do-with-wsl"></a><span data-ttu-id="c8225-111">Welche Aufgaben kann ich mit WSL erledigen?</span><span class="sxs-lookup"><span data-stu-id="c8225-111">What can I do with WSL?</span></span>

<span data-ttu-id="c8225-112">WSL bietet eine Anwendung namens „Bash. exe“, die eine Windows-Konsole mit der Bash-Shell öffnet, wenn sie gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="c8225-112">WSL provides an application called Bash.exe that, when started, opens a Windows console running the Bash shell.</span></span> <span data-ttu-id="c8225-113">Mithilfe von Bash können Sie Linux-Befehlszeilentools und -Apps ausführen.</span><span class="sxs-lookup"><span data-stu-id="c8225-113">Using Bash, you can run command-line Linux tools and apps.</span></span> <span data-ttu-id="c8225-114">Geben Sie z.B. `lsb_release -a` ein, und drücken Sie die EINGABETASTE. Es werden Details zu der derzeit ausgeführten Linux-Distribution angezeigt:</span><span class="sxs-lookup"><span data-stu-id="c8225-114">For example, type `lsb_release -a` and hit enter; you’ll see details of the Linux distro currently running:</span></span>

![Screenshot der Details der Distribution](media/distro.png)

<span data-ttu-id="c8225-116">Sie können über die Linux Bash-Shell auch auf das Dateisystem des lokalen Computers zugreifen. Ihre lokalen Laufwerke werden unter dem Ordner `/mnt` eingebunden.</span><span class="sxs-lookup"><span data-stu-id="c8225-116">You can also access your local machine’s filesystem from within the Linux Bash shell – you’ll find your local drives mounted under the `/mnt` folder.</span></span> <span data-ttu-id="c8225-117">Das Laufwerk `C:` wird beispielsweise unter `/mnt/c` eingebunden:</span><span class="sxs-lookup"><span data-stu-id="c8225-117">For example, your `C:` drive is mounted under `/mnt/c`:</span></span>  

![Screenshot des eingebundenen Laufwerks „C:“](media/ls.png)

## <a name="what-is-bash"></a><span data-ttu-id="c8225-119">Was ist Bash?</span><span class="sxs-lookup"><span data-stu-id="c8225-119">What is Bash?</span></span>

<span data-ttu-id="c8225-120">[Bash](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) ist eine beliebte, textbasierte Shell und Befehlssprache.</span><span class="sxs-lookup"><span data-stu-id="c8225-120">[Bash](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) is a popular text-based shell and command-language.</span></span> <span data-ttu-id="c8225-121">Dabei handelt es sich um die Standardshell, die in Ubuntu und anderen Linux-Distributionen sowie in macOS enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="c8225-121">It is the default shell included within Ubuntu and other Linux distros, and in macOS.</span></span> <span data-ttu-id="c8225-122">Benutzer geben Befehle in eine Shell ein, um Skripts und/oder Befehle und Tools auszuführen, um zahlreiche Aufgaben zu erledigen.</span><span class="sxs-lookup"><span data-stu-id="c8225-122">Users type commands into a shell to execute scripts and/or run commands and tools to accomplish many tasks.</span></span>

## <a name="how-does-this-work"></a><span data-ttu-id="c8225-123">Wie funktioniert das?</span><span class="sxs-lookup"><span data-stu-id="c8225-123">How does this work?</span></span>

<span data-ttu-id="c8225-124">Sehen Sie sich unseren [Blog](https://blogs.msdn.microsoft.com/wsl/) an, in dem wir ausführlich über die zugrunde liegende Technologie informieren.</span><span class="sxs-lookup"><span data-stu-id="c8225-124">Check out our [blog](https://blogs.msdn.microsoft.com/wsl/) where we go into detail about the underlying technology.</span></span>

## <a name="why-would-i-use-wsl-rather-than-linux-in-a-vm"></a><span data-ttu-id="c8225-125">Warum sollte ich WSL anstelle von Linux auf einem virtuellen Computer verwenden?</span><span class="sxs-lookup"><span data-stu-id="c8225-125">Why would I use WSL rather than Linux in a VM?</span></span>

<span data-ttu-id="c8225-126">WSL erfordert weniger Ressourcen (CPU, Arbeitsspeicher und Speicher) als ein vollständiger virtueller Computer.</span><span class="sxs-lookup"><span data-stu-id="c8225-126">WSL requires fewer resources (CPU, memory, and storage) than a full virtual machine.</span></span> <span data-ttu-id="c8225-127">WSL ermöglicht es Ihnen auch, Linux-Befehlszeilentools und -Apps neben Ihren Windows Befehlszeilen-, Desktop- und Store-Apps auszuführen und von Linux aus auf Ihre Windows-Dateien zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="c8225-127">WSL also allows you to run Linux command-line tools and apps alongside your Windows command-line, desktop and store apps, and to access your Windows files from within Linux.</span></span> <span data-ttu-id="c8225-128">Auf diese Weise können Sie Windows-Apps und Linux-Befehlszeilentools für denselben Satz von Dateien verwenden, wenn Sie möchten.</span><span class="sxs-lookup"><span data-stu-id="c8225-128">This enables you to use Windows apps and Linux command-line tools on the same set of files if you wish.</span></span>

## <a name="why-would-i-use-for-example-ruby-on-linux-instead-of-on-windows"></a><span data-ttu-id="c8225-129">Warum sollte ich beispielsweise Ruby unter Linux anstatt unter Windows verwenden?</span><span class="sxs-lookup"><span data-stu-id="c8225-129">Why would I use, for example, Ruby on Linux instead of on Windows?</span></span>

<span data-ttu-id="c8225-130">Einige plattformübergreifende Tools wurden unter der Annahme erstellt, dass sich die Umgebung, in der sie ausgeführt werden, wie Linux verhält.</span><span class="sxs-lookup"><span data-stu-id="c8225-130">Some cross-platform tools were built assuming that the environment in which they run behaves like Linux.</span></span> <span data-ttu-id="c8225-131">Einige Tools gehen beispielsweise davon aus, dass auf sehr lange Dateipfade zugegriffen werden kann oder dass bestimmte Dateien/Ordner vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="c8225-131">For example, some tools assume that they are able to access very long file paths or that specific files/folders exist.</span></span> <span data-ttu-id="c8225-132">Dies verursacht unter Windows häufig Probleme, da sich dieses Betriebssystem meistens anders als Linux verhält.</span><span class="sxs-lookup"><span data-stu-id="c8225-132">This often causes problems on Windows which often behaves differently from Linux.</span></span>

<span data-ttu-id="c8225-133">Viele Sprachen wie Ruby und node werden häufig in Windows portiert und lassen sich dort hervorragend ausführen.</span><span class="sxs-lookup"><span data-stu-id="c8225-133">Many languages like Ruby and node are often ported to, and run great, on Windows.</span></span> <span data-ttu-id="c8225-134">Allerdings portieren nicht alle Besitzer von Ruby Gem- oder node/NPM-Bibliotheken ihre Bibliotheken, um Windows zu unterstützen, und viele von ihnen verfügen über Linux-spezifische Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="c8225-134">However, not all of the Ruby Gem or node/NPM library owners port their libraries to support Windows, and many have Linux-specific dependencies.</span></span> <span data-ttu-id="c8225-135">Dies kann häufig dazu führen, dass Systeme, die mit solchen Tools und Bibliotheken erstellt wurden, unter Windows unter Build- und manchmal unter Laufzeitfehlern leiden oder unerwünschtes Verhalten aufweisen.</span><span class="sxs-lookup"><span data-stu-id="c8225-135">This can often result in systems built using such tools and libraries suffering from build and sometimes runtime errors or unwanted behaviors on Windows.</span></span>

<span data-ttu-id="c8225-136">Dies sind nur einige der Probleme, die viele Benutzer veranlasst haben, Microsoft zu bitten, die Befehlszeilentools von Windows zu verbessern. Dies hat uns auch dazu veranlasst, eine Partnerschaft mit Canonical einzugehen, damit native Bash- und Linux-Befehlszeilentools unter Windows ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="c8225-136">These are just some of issues that caused many people to ask Microsoft to improve Windows’ command-line tools and what drove us to partner with Canonical to enable native Bash and Linux command-line tools to run on Windows.</span></span>

## <a name="what-does-this-mean-for-powershell"></a><span data-ttu-id="c8225-137">Was bedeutet das für PowerShell?</span><span class="sxs-lookup"><span data-stu-id="c8225-137">What does this mean for PowerShell?</span></span>

<span data-ttu-id="c8225-138">Während der Arbeit mit OSS-Projekten gibt es zahlreiche Szenarien, in denen es äußerst nützlich ist, aus einer PowerShell-Eingabeaufforderung zu Bash zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="c8225-138">While working with OSS projects, there are numerous scenarios where it’s immensely useful to drop into Bash from a PowerShell prompt.</span></span> <span data-ttu-id="c8225-139">Die Bash-Unterstützung ist ergänzend und stärkt den Wert der Befehlszeile unter Windows, sodass PowerShell und die PowerShell-Community andere gängige Technologien nutzen können.</span><span class="sxs-lookup"><span data-stu-id="c8225-139">Bash support is complementary and strengthens the value of the command-line on Windows, allowing PowerShell and the PowerShell community to leverage other popular technologies.</span></span>

<span data-ttu-id="c8225-140">Weitere Informationen finden Sie im Blog des PowerShell-Teams: [Bash for Windows: Why it’s awesome and what it means for PowerShell](https://blogs.msdn.microsoft.com/powershell/2016/04/01/bash-for-windows-why-its-awesome-and-what-it-means-for-powershell/).</span><span class="sxs-lookup"><span data-stu-id="c8225-140">Read more on the PowerShell team blog -- [Bash for Windows: Why it’s awesome and what it means for PowerShell](https://blogs.msdn.microsoft.com/powershell/2016/04/01/bash-for-windows-why-its-awesome-and-what-it-means-for-powershell/)</span></span>

## <a name="can-i-run-all-linux-apps-in-wsl"></a><span data-ttu-id="c8225-141">Kann ich ALLE Linux-Apps in WSL ausführen?</span><span class="sxs-lookup"><span data-stu-id="c8225-141">Can I run ALL Linux apps in WSL?</span></span>

<span data-ttu-id="c8225-142">Nein!</span><span class="sxs-lookup"><span data-stu-id="c8225-142">No!</span></span> <span data-ttu-id="c8225-143">WSL ist ein Tool, das es Benutzern, die diese Funktionalität benötigen, ermöglicht, Bash und wichtige Linux-Befehlszeilentools unter Windows auszuführen.</span><span class="sxs-lookup"><span data-stu-id="c8225-143">WSL is a tool aimed at enabling users who need them to run Bash and core Linux command-line tools on Windows.</span></span>

<span data-ttu-id="c8225-144">WSL zielt **nicht** darauf ab, GUI-Desktops oder -Anwendungen (z.B. Gnome, KDE usw.) zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="c8225-144">WSL does **not** aim to support GUI desktops or applications (e.g. Gnome, KDE, etc.)</span></span>  

<span data-ttu-id="c8225-145">Auch wenn Sie viele gängige Serveranwendungen (z.B. Redis) ausführen können, empfehlen wir WSL nicht für das Hosting von Produktionsdiensten. Microsoft bietet eine Vielzahl von Lösungen für die Ausführung von Linux-Produktionsworkloads in Azure, Hyper-V und Docker.</span><span class="sxs-lookup"><span data-stu-id="c8225-145">Also, even though you will be able to run many popular server applications (e.g. Redis), we do not recommend WSL for hosting production services – Microsoft offers a variety of solutions for running production Linux workloads in Azure, Hyper-V, and Docker.</span></span> 

## <a name="what-windows-skus-is-wsl-included-in"></a><span data-ttu-id="c8225-146">In welchen Windows-SKUs ist WSL enthalten?</span><span class="sxs-lookup"><span data-stu-id="c8225-146">What Windows SKUs is WSL included in?</span></span>

<span data-ttu-id="c8225-147">Das Windows-Subsystem für Linux ist in der Desktopversion von Windows für Windows 10 Anniversary und Creators Update oder höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c8225-147">Windows Subsystem for Linux is available on the desktop version of Windows for Windows 10 Anniversary and Creators update or later.</span></span>

<span data-ttu-id="c8225-148">Beginnend mit dem Fall Creators Update ist WSL für die Desktop- und Server-SKUs von Windows verfügbar.</span><span class="sxs-lookup"><span data-stu-id="c8225-148">Beginning in the Fall Creators update WSL will be available on both the desktop and server SKUs of Windows.</span></span>

## <a name="what-processors-does-wsl-support"></a><span data-ttu-id="c8225-149">Welche Prozessoren werden von WSL unterstützt?</span><span class="sxs-lookup"><span data-stu-id="c8225-149">What processors does WSL support?</span></span>

<span data-ttu-id="c8225-150">WSL unterstützt x64- und ARM-CPUs.</span><span class="sxs-lookup"><span data-stu-id="c8225-150">WSL supports x64 and ARM CPUs.</span></span>

## <a name="how-do-i-access-my-c-drive"></a><span data-ttu-id="c8225-151">Wie greife ich auf mein Laufwerk „C:“ zu?</span><span class="sxs-lookup"><span data-stu-id="c8225-151">How do I access my C: drive?</span></span>

<span data-ttu-id="c8225-152">Einbindungspunkte für Festplatten auf dem lokalen Computer werden automatisch erstellt und ermöglichen einfachen Zugriff auf das Windows-Dateisystem.</span><span class="sxs-lookup"><span data-stu-id="c8225-152">Mount points for hard drives on the local machine are automatically created and provide easy access to the Windows filesystem.</span></span>

<span data-ttu-id="c8225-153">**/mnt/\<Laufwerkbuchstabe>/**</span><span class="sxs-lookup"><span data-stu-id="c8225-153">**/mnt/\<drive letter>/**</span></span>

<span data-ttu-id="c8225-154">Beispielsyntax für den Zugriff auf „C:\“: `cd /mnt/c`</span><span class="sxs-lookup"><span data-stu-id="c8225-154">Example usage would be `cd /mnt/c` to access c:\</span></span>

## <a name="how-do-i-set-up-git-credential-manager-how-do-i-use-my-windows-git-permissions-in-wsl"></a><span data-ttu-id="c8225-155">Wie richte ich die Git-Anmeldeinformationsverwaltung ein?</span><span class="sxs-lookup"><span data-stu-id="c8225-155">How do I set up Git Credential Manager?</span></span> <span data-ttu-id="c8225-156">(Wie verwende ich meine Windows Git-Berechtigungen in WSL?)</span><span class="sxs-lookup"><span data-stu-id="c8225-156">(How do I use my Windows Git permissions in WSL?)</span></span> 

<span data-ttu-id="c8225-157">Die Git-Anmeldeinformationsverwaltung ermöglicht Ihnen das Authentifizieren eines Git-Remoteservers, auch wenn Sie über ein komplexes Authentifizierungsmuster wie Azure Active Directory oder eine zweistufige Authentifizierung verfügen.</span><span class="sxs-lookup"><span data-stu-id="c8225-157">Git Credential Manager enables you to authenticate a remote Git server, even if you have a complex authentication pattern like Azure Active Directory or two-factor authentication.</span></span> <span data-ttu-id="c8225-158">Die Git-Anmeldeinformationsverwaltung kann in den Authentifizierungsablauf für Dienste wie GitHub integriert werden, und sobald Sie bei Ihrem Hostinganbieter authentifiziert sind, fordert sie ein neues Authentifizierungstoken an.</span><span class="sxs-lookup"><span data-stu-id="c8225-158">Git Credential Manager integrates into the authentication flow for services like GitHub and, once you're authenticated to your hosting provider, requests a new authentication token.</span></span> <span data-ttu-id="c8225-159">Anschließend wird das Token sicher in der Windows-Anmeldeinformationsverwaltung gespeichert.</span><span class="sxs-lookup"><span data-stu-id="c8225-159">It then stores the token securely in the Windows Credential Manager.</span></span> <span data-ttu-id="c8225-160">Nach dem ersten Mal können Sie Git verwenden, um mit Ihrem Hostinganbieter zu kommunizieren, ohne sich erneut authentifizieren zu müssen.</span><span class="sxs-lookup"><span data-stu-id="c8225-160">After the first time, you can use git to talk to your hosting provider without needing to re-authenticate.</span></span> <span data-ttu-id="c8225-161">Er greift einfach auf das Token in Windows-Anmeldeinformationsverwaltung zu.</span><span class="sxs-lookup"><span data-stu-id="c8225-161">It will just access the token in the Windows Credential Manager.</span></span>

<span data-ttu-id="c8225-162">Zum Einrichten der Git-Anmeldeinformationsverwaltung für die Verwendung mit einer WSL-Distribution öffnen Sie die Distribution, und geben Sie den folgenden Befehl ein:</span><span class="sxs-lookup"><span data-stu-id="c8225-162">To set up Git Credential Manager for use with a WSL distribution, open your distribution and enter this command:</span></span>

```Bash
git config --global credential.helper "/mnt/c/Program\ Files/Git/mingw64/libexec/git-core/git-credential-manager.exe"
```

<span data-ttu-id="c8225-163">Nun wird für jeden Git-Vorgang, den Sie in der WSL-Distribution ausführen, die Anmeldeinformationsverwaltung verwendet.</span><span class="sxs-lookup"><span data-stu-id="c8225-163">Now any git operation you perform within your WSL distribution will use the credential manager.</span></span> <span data-ttu-id="c8225-164">Wenn Sie bereits Anmeldeinformationen für einen Host zwischengespeichert haben, greifen Sie über die Anmeldeinformationsverwaltung auf diese zu.</span><span class="sxs-lookup"><span data-stu-id="c8225-164">If you already have credentials cached for a host, it will access them from the credential manager.</span></span> <span data-ttu-id="c8225-165">Andernfalls erhalten Sie eine Dialogfeldantwort, in der Ihre Anmeldeinformationen angefordert werden, auch wenn Sie sich in einer Linux-Konsole befinden.</span><span class="sxs-lookup"><span data-stu-id="c8225-165">If not, you'll receive a dialog response requesting your credentials, even if you're in a Linux console.</span></span>

<span data-ttu-id="c8225-166">Diese Unterstützung basiert auf der [Interoperabilität zwischen dem Windows-Subsystem für Linux und Windows selbst](https://docs.microsoft.com/windows/wsl/interop).</span><span class="sxs-lookup"><span data-stu-id="c8225-166">This support relies on the [interoperability between Windows Subsystem for Linux and Windows itself](https://docs.microsoft.com/windows/wsl/interop).</span></span>

## <a name="how-do-i-use-a-windows-file-with-a-linux-app"></a><span data-ttu-id="c8225-167">Wie verwende ich eine Windows-Datei mit einer Linux-App?</span><span class="sxs-lookup"><span data-stu-id="c8225-167">How do I use a Windows file with a Linux app?</span></span>

<span data-ttu-id="c8225-168">Einer der Vorteile von WSL besteht darin, dass Sie über Windows- und Linux-Apps oder -Tools auf Ihre Dateien zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="c8225-168">One of the benefits of WSL is being able to access your files via both Windows and Linux apps or tools.</span></span> 

<span data-ttu-id="c8225-169">WSL bindet die Festplattenlaufwerke Ihres Computers unter dem Ordner `/mnt/<drive>` in Ihre Linux-Distributionen ein.</span><span class="sxs-lookup"><span data-stu-id="c8225-169">WSL mounts your machine's fixed drives under the `/mnt/<drive>` folder in your Linux distros.</span></span> <span data-ttu-id="c8225-170">Das Laufwerk `C:` wird beispielsweise unter `/mnt/c/` eingebunden.</span><span class="sxs-lookup"><span data-stu-id="c8225-170">For example, your `C:` drive is mounted under `/mnt/c/`</span></span>

<span data-ttu-id="c8225-171">Mit den eingebundenen Laufwerken können Sie beispielsweise Code in `C:\dev\myproj\` mit [Visual Studio](https://visualstudio.microsoft.com/vs/) oder [VS Code](https://code.visualstudio.com/) bearbeiten und diesen Code in Linux erstellen und testen, indem Sie über `/mnt/c/dev/myproj` auf die gleichen Dateien zugreifen.</span><span class="sxs-lookup"><span data-stu-id="c8225-171">Using your mounted drives, you can edit code in, for example, `C:\dev\myproj\` using [Visual Studio](https://visualstudio.microsoft.com/vs/) / or [VS Code](https://code.visualstudio.com/), and build/test that code in Linux by accessing the same files via `/mnt/c/dev/myproj`.</span></span>

> <span data-ttu-id="c8225-172">**WICHTIGER HINWEIS**: Eine der wichtigsten Einschränkungen bei der Verwendung von WSL besteht darin, dass der direkte Zugriff auf und die Änderung von Dateien im Dateisystem Ihrer Linux-Distribution mit Windows-Anwendungen oder -Tools nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="c8225-172">**IMPORTANT NOTE**: One of the key limitations of using WSL is that directly accessing/changing files in your Linux distros' filesystem using Windows apps or tools is not supported.</span></span> <span data-ttu-id="c8225-173">Weitere Informationen: [Ändern Sie Linux-Dateien nicht mithilfe von Windows-Apps und -Tools](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/)</span><span class="sxs-lookup"><span data-stu-id="c8225-173">See: [Do not change Linux files using Windows apps and tools](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/)</span></span>

## <a name="are-files-in-the-linux-drive-different-from-the-mounted-windows-drive"></a><span data-ttu-id="c8225-174">Unterscheiden sich die Dateien im Linux-Laufwerk vom eingebundenen Windows-Laufwerk?</span><span class="sxs-lookup"><span data-stu-id="c8225-174">Are files in the Linux drive different from the mounted Windows drive?</span></span>

1. <span data-ttu-id="c8225-175">Dateien unter dem Linuxstamm (d.h. `/`) werden von WSL gesteuert, indem Linux-spezifisches Verhalten imitiert wird, einschließlich, aber nicht beschränkt auf:</span><span class="sxs-lookup"><span data-stu-id="c8225-175">Files under the Linux root (i.e. `/`) are controlled by WSL which mimics Linux specific behavior, including but not limited to:</span></span>
   * <span data-ttu-id="c8225-176">Dateien, die ungültige Zeichen für Windows-Dateinamen enthalten</span><span class="sxs-lookup"><span data-stu-id="c8225-176">Files which contain invalid Windows filename characters</span></span>
   * <span data-ttu-id="c8225-177">Für Benutzer ohne Administratorrechte erstellte symbolische Verknüpfungen</span><span class="sxs-lookup"><span data-stu-id="c8225-177">Symlinks created for non-admin users</span></span>
   * <span data-ttu-id="c8225-178">Ändern von Dateiattributen über chmod und chown</span><span class="sxs-lookup"><span data-stu-id="c8225-178">Changing file attributes through chmod and chown</span></span>
   * <span data-ttu-id="c8225-179">Unterscheidung von Groß-/Kleinschreibung für Dateien/Ordner</span><span class="sxs-lookup"><span data-stu-id="c8225-179">File/folder case sensitivity</span></span>

2. <span data-ttu-id="c8225-180">Dateien in eingebundenen Laufwerken werden von Windows gesteuert und weisen das folgende Verhalten auf:</span><span class="sxs-lookup"><span data-stu-id="c8225-180">Files in mounted drives are controlled by Windows and have the following behaviors:</span></span>
   * <span data-ttu-id="c8225-181">Unterstützung von Unterscheidung zwischen Groß-/Kleinschreibung</span><span class="sxs-lookup"><span data-stu-id="c8225-181">Support case sensitivity</span></span>
   * <span data-ttu-id="c8225-182">Alle Berechtigungen sind so festgelegt, dass Sie die Windows-Berechtigungen bestmöglich widerspiegeln</span><span class="sxs-lookup"><span data-stu-id="c8225-182">All permissions are set to best reflect the Windows permissions</span></span>

## <a name="why-are-there-so-many-errors-when-i-run-apt-get-upgrade"></a><span data-ttu-id="c8225-183">Warum treten so viele Fehler auf, wenn ich apt-get upgrade ausführe?</span><span class="sxs-lookup"><span data-stu-id="c8225-183">Why are there so many errors when I run apt-get upgrade?</span></span>

<span data-ttu-id="c8225-184">In einigen Paketen werden Features verwendet, die noch nicht implementiert wurden.</span><span class="sxs-lookup"><span data-stu-id="c8225-184">Some packages use features that we haven't implemented yet.</span></span> <span data-ttu-id="c8225-185">`udev` wird z.B. noch nicht unterstützt und verursacht mehrere `apt-get upgrade`-Fehler.</span><span class="sxs-lookup"><span data-stu-id="c8225-185">`udev`, for example, isn't supported yet and causes several `apt-get upgrade` errors.</span></span>

<span data-ttu-id="c8225-186">Führen Sie die folgenden Schritte aus, um Probleme im Zusammenhang mit `udev` zu beheben:</span><span class="sxs-lookup"><span data-stu-id="c8225-186">To fix issues related to `udev`, follow the following steps:</span></span>

1. <span data-ttu-id="c8225-187">Schreiben Sie Folgendes in `/usr/sbin/policy-rc.d`, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="c8225-187">Write the following to `/usr/sbin/policy-rc.d` and save your changes.</span></span>

    ```bash
    #!/bin/sh
    exit 101
    ```

2. <span data-ttu-id="c8225-188">Fügen Sie `/usr/sbin/policy-rc.d` Ausführungsberechtigungen hinzu.</span><span class="sxs-lookup"><span data-stu-id="c8225-188">Add execute permissions to `/usr/sbin/policy-rc.d`</span></span>

    ```bash
    chmod +x /usr/sbin/policy-rc.d
    ```
  
3. <span data-ttu-id="c8225-189">Führen Sie die folgenden Befehle aus.</span><span class="sxs-lookup"><span data-stu-id="c8225-189">Run the following commands</span></span>

    ```bash
    dpkg-divert --local --rename --add /sbin/initctl
    ln -s /bin/true /sbin/initctl
    ```

## <a name="how-do-i-uninstall-a-wsl-distribution"></a><span data-ttu-id="c8225-190">Wie deinstalliere ich eine WSL-Distribution?</span><span class="sxs-lookup"><span data-stu-id="c8225-190">How do I uninstall a WSL Distribution?</span></span>

<span data-ttu-id="c8225-191">Öffnen Sie in Builds vor 1709 (16299) eine Eingabeaufforderung, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="c8225-191">On builds prior to 1709 (16299) open a command prompt and run:</span></span>

  ```batchfile
  lxrun /uninstall /full
  ```
  
<span data-ttu-id="c8225-192">WSL-Distributionen, die aus dem Store installiert werden, können wie jede andere Windows-App deinstalliert werden, indem Sie mit der rechten Maustaste auf die App-Kachel und dann auf „Deinstallieren“ klicken oder indem Sie PowerShell und das [`Remove-AppxPackage`-Cmdlet](https://technet.microsoft.com/library/hh856038.aspx) verwenden.</span><span class="sxs-lookup"><span data-stu-id="c8225-192">WSL distributions installed from the store can be uninstalled like any other Windows app, by right-clicking on the app tile and clicking Uninstall, or via PowerShell using the [`Remove-AppxPackage` cmdlet](https://technet.microsoft.com/library/hh856038.aspx).</span></span>

## <a name="why-does-ping-generate-permission-denied-errors"></a><span data-ttu-id="c8225-193">Warum werden bei Ping Fehler des Typs „Berechtigung verweigert“ generiert?</span><span class="sxs-lookup"><span data-stu-id="c8225-193">Why does ping generate permission denied errors?</span></span>

<span data-ttu-id="c8225-194">In WSL-Builds vor 14926 erforderte Ping, dass WSL über eine Konsole mit erhöhten Rechten ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c8225-194">In WSL builds < 14926, ping required WSL to run via an elevated Console.</span></span> <span data-ttu-id="c8225-195">Dieses Problem wurde in Build 14926 und höher behoben.</span><span class="sxs-lookup"><span data-stu-id="c8225-195">This issue was fixed in Build 14926 and later.</span></span>

## <a name="how-do-i-run-an-openssh-server"></a><span data-ttu-id="c8225-196">Wie führe ich einen OpenSSH-Server aus?</span><span class="sxs-lookup"><span data-stu-id="c8225-196">How do I run an OpenSSH server?</span></span>

<span data-ttu-id="c8225-197">Zum Ausführen von OpenSSH in WSL sind Administratorberechtigungen in Windows erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8225-197">Administrator privileges in Windows are required to run OpenSSH in WSL.</span></span> <span data-ttu-id="c8225-198">Um einen OpenSSH-Server auszuführen, führen Sie Bash unter Ubuntu unter Windows als Administrator aus, oder starten Sie „bash.exe“ über eine CMD-/PowerShell-Eingabeaufforderung mit Administratorrechten.</span><span class="sxs-lookup"><span data-stu-id="c8225-198">To run an OpenSSH server, run Bash on Ubuntu on Windows as an administrator, or run bash.exe from a CMD/PowerShell prompt with administrator privileges.</span></span>

## <a name="why-do-i-get-error-0x80040306-when-i-try-to-install"></a><span data-ttu-id="c8225-199">Warum erhalte ich „Error: 0x80040306“ beim Installationsversuch?</span><span class="sxs-lookup"><span data-stu-id="c8225-199">Why do I get "Error: 0x80040306" when I try to install?</span></span>

<span data-ttu-id="c8225-200">WSL unterstützt die Ausführung in einer Legacykonsole nicht.</span><span class="sxs-lookup"><span data-stu-id="c8225-200">WSL does not support running in a legacy console.</span></span> <span data-ttu-id="c8225-201">So deaktivieren Sie die Legacykonsole:</span><span class="sxs-lookup"><span data-stu-id="c8225-201">To turn off legacy console:</span></span>

1. <span data-ttu-id="c8225-202">Öffnen Sie WSL, PowerShell oder Cmd.</span><span class="sxs-lookup"><span data-stu-id="c8225-202">Open WSL, PowerShell, or Cmd</span></span>
1. <span data-ttu-id="c8225-203">Klicken Sie mit der rechten Maustaste auf der Titelleiste auf „Eigenschaften“. Deaktivieren Sie die Option „Legacykonsole verwenden“.</span><span class="sxs-lookup"><span data-stu-id="c8225-203">Right click title bar -> Properties -> Uncheck "Use legacy console"</span></span>
1. <span data-ttu-id="c8225-204">Auf "OK" klicken</span><span class="sxs-lookup"><span data-stu-id="c8225-204">Click OK</span></span>

## <a name="why-do-i-get-error-0x80040154-when-i-run-bashexe-after-upgrading-windows"></a><span data-ttu-id="c8225-205">Warum erhalte ich „Error: 0x80040154“ beim Ausführen von „bash.exe“ nach dem Upgrade von Windows?</span><span class="sxs-lookup"><span data-stu-id="c8225-205">Why do I get "Error: 0x80040154" when I run bash.exe after upgrading Windows?</span></span>

<span data-ttu-id="c8225-206">Das Feature „Windows-Subsystem für Linux“ ist möglicherweise während eines Windows-Updates deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c8225-206">The "Windows Subsystem for Linux" feature may be disabled during a Windows update.</span></span> <span data-ttu-id="c8225-207">Wenn dies der Fall ist, muss das Windows-Feature erneut aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="c8225-207">If this happens the Windows feature must be re-enabled.</span></span> <span data-ttu-id="c8225-208">Anweisungen zum Aktivieren des Features „Windows-Subsystem für Linux“ finden Sie im [Installationshandbuch.](https://docs.microsoft.com/windows/wsl/install-win10#install-the-windows-subsystem-for-linux)</span><span class="sxs-lookup"><span data-stu-id="c8225-208">Instructions for enabling the "Windows Subsystem for Linux" feature can be found in the [Installation Guide](https://docs.microsoft.com/windows/wsl/install-win10#install-the-windows-subsystem-for-linux).</span></span>

## <a name="how-do-i-change-the-display-language-of-wsl"></a><span data-ttu-id="c8225-209">Wie ändere ich die Anzeigesprache von WSL?</span><span class="sxs-lookup"><span data-stu-id="c8225-209">How do I change the display language of WSL?</span></span>

<span data-ttu-id="c8225-210">Die WSL-Installation versucht, das Ubuntu-Gebietsschema automatisch so zu ändern, dass es dem Gebietsschema Ihrer Windows-Installation entspricht.</span><span class="sxs-lookup"><span data-stu-id="c8225-210">WSL install will try to automatically change the Ubuntu locale to match the locale of your Windows install.</span></span> <span data-ttu-id="c8225-211">Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl ausführen, um das Ubuntu-Gebietsschema zu ändern, nachdem die Installation abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="c8225-211">If you do not want this behavior you can run this command to change the Ubuntu locale after install completes.</span></span> <span data-ttu-id="c8225-212">Sie müssen „bash.exe“ neu starten, damit diese Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="c8225-212">You will have to relaunch bash.exe for this change to take effect.</span></span>

<span data-ttu-id="c8225-213">Im folgenden Beispiel wird das Gebietsschema in „en-US“ geändert:</span><span class="sxs-lookup"><span data-stu-id="c8225-213">The below example changes to locale to en-US:</span></span>

```bash
sudo update-locale LANG=en_US.UTF8
```

## <a name="why-do-i-not-have-internet-access-from-wsl"></a><span data-ttu-id="c8225-214">Warum habe ich aus WSL keinen Internetzugriff?</span><span class="sxs-lookup"><span data-stu-id="c8225-214">Why do I not have internet access from WSL?</span></span>

<span data-ttu-id="c8225-215">Einige Benutzer haben Probleme mit bestimmten Firewallanwendungen gemeldet, die den Internetzugriff in WSL blockieren.</span><span class="sxs-lookup"><span data-stu-id="c8225-215">Some users have reported issues with specific firewall applications blocking internet access in WSL.</span></span> <span data-ttu-id="c8225-216">Die gemeldeten Firewalls sind:</span><span class="sxs-lookup"><span data-stu-id="c8225-216">The firewalls reported are:</span></span>

1. <span data-ttu-id="c8225-217">Kaspersky</span><span class="sxs-lookup"><span data-stu-id="c8225-217">Kaspersky</span></span>
1. <span data-ttu-id="c8225-218">AVG</span><span class="sxs-lookup"><span data-stu-id="c8225-218">AVG</span></span>
1. <span data-ttu-id="c8225-219">Avast</span><span class="sxs-lookup"><span data-stu-id="c8225-219">Avast</span></span>

<span data-ttu-id="c8225-220">In einigen Fällen ermöglicht das Deaktivieren der Firewall den Zugriff.</span><span class="sxs-lookup"><span data-stu-id="c8225-220">In some cases turning off the firewall allows for access.</span></span> <span data-ttu-id="c8225-221">In einigen Fällen sieht es so aus, als ob bereits die Installation der Firewall den Zugriff blockiert.</span><span class="sxs-lookup"><span data-stu-id="c8225-221">In some cases simply having the firewall installed looks to block access.</span></span>

## <a name="how-do-i-access-a-port-from-wsl-in-windows"></a><span data-ttu-id="c8225-222">Wie greife ich aus WSL unter Windows auf einen Port zu?</span><span class="sxs-lookup"><span data-stu-id="c8225-222">How do I access a port from WSL in Windows?</span></span>
<span data-ttu-id="c8225-223">WSL nutzt die IP-Adresse von Windows, da es unter Windows ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c8225-223">WSL shares the IP address of Windows, as it is running on Windows.</span></span> <span data-ttu-id="c8225-224">Daher können Sie auf alle Ports auf localhost zugreifen. Wenn Sie z.B. Webinhalte an Port 1234 verwenden, können Sie https://localhost:1234 in Ihren Windows-Browser eingeben.</span><span class="sxs-lookup"><span data-stu-id="c8225-224">As such you can access any ports on localhost e.g. if you had web content on port 1234 you could https://localhost:1234 into your Windows browser.</span></span>

## <a name="how-can-i-back-up-my-wsl-distros-or-move-them-from-one-drive-to-another"></a><span data-ttu-id="c8225-225">Wie kann ich meine WSL-Verteilungen sichern oder von einem Laufwerk auf ein anderes verschieben?</span><span class="sxs-lookup"><span data-stu-id="c8225-225">How can I back up my WSL distros, or move them from one drive to another?</span></span>

<span data-ttu-id="c8225-226">Die beste Möglichkeit zum Sichern oder Verschieben Ihrer Verteilungen sind die in Windows Version 1809 und höher verfügbaren Export/Import-Befehle.</span><span class="sxs-lookup"><span data-stu-id="c8225-226">The best way to backup or move your distros is via the export/import commands available in Windows Version 1809 and later.</span></span> <span data-ttu-id="c8225-227">Sie können die gesamte Distribution mithilfe des Befehls `wsl --export` in einen Tarball exportieren.</span><span class="sxs-lookup"><span data-stu-id="c8225-227">You can export your entire distribution to a tarball using the `wsl --export` command.</span></span> <span data-ttu-id="c8225-228">Sie können diese Verteilung dann mit dem Befehl `wsl --import`, in dem ein neuer Speicherort für den Import angegeben werden kann, wieder in WSL importieren, wodurch Sie Zustände Ihrer WSL-Verteilungen sichern und speichern (oder verschieben) können.</span><span class="sxs-lookup"><span data-stu-id="c8225-228">You can then import this distro back into WSL using the `wsl --import` command, which can name a new drive location for the import, allowing you to backup and save states of (or move) your WSL distributions.</span></span> 

<span data-ttu-id="c8225-229">Beachten Sie, dass herkömmliche Sicherungsdienste, die Dateien in ihren Appdata-Ordnern sichern (z.B. die Windows-Sicherung), Ihre Linux-Dateien nicht beschädigen.</span><span class="sxs-lookup"><span data-stu-id="c8225-229">Please note that traditional backup services that backup files in your Appdata folders (like Windows Backup) will not corrupt your Linux files.</span></span>

## <a name="where-can-i-provide-feedback"></a><span data-ttu-id="c8225-230">Wo kann ich Feedback bereitstellen?</span><span class="sxs-lookup"><span data-stu-id="c8225-230">Where can I provide feedback?</span></span>

<span data-ttu-id="c8225-231">Sie können Ihr Feedback über mehrere Kanäle übermitteln und Fragen stellen.</span><span class="sxs-lookup"><span data-stu-id="c8225-231">You can share feedback and ask questions through multiple channels.</span></span>

<span data-ttu-id="c8225-232">Wenn Sie technische Probleme haben oder neue Features anfordern möchten, besuchen Sie unsere GitHub-Problemverfolgung:</span><span class="sxs-lookup"><span data-stu-id="c8225-232">If you have technical issues, or want to request new features please go to our Github issue tracker:</span></span>

* [<span data-ttu-id="c8225-233">GitHub-Problemverfolgung</span><span class="sxs-lookup"><span data-stu-id="c8225-233">GitHub issue tracker</span></span>](https://github.com/Microsoft/BashOnWindows/issues)

<span data-ttu-id="c8225-234">Wenn Sie mit den neuesten WSL-News auf dem neuesten Stand bleiben möchten, nutzen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="c8225-234">If you'd like to stay up to date with the latest WSL news you can do so with:</span></span>

* <span data-ttu-id="c8225-235">Unseren [Befehlszeilen-Teamblog](https://blogs.msdn.microsoft.com/commandline/)</span><span class="sxs-lookup"><span data-stu-id="c8225-235">Our [command-line team blog](https://blogs.msdn.microsoft.com/commandline/)</span></span>
* <span data-ttu-id="c8225-236">Twitter.</span><span class="sxs-lookup"><span data-stu-id="c8225-236">Twitter.</span></span> <span data-ttu-id="c8225-237">Folgen Sie [@craigaloewen](https://twitter.com/craigaloewen) auf Twitter, um über Neuigkeiten, Updates usw. informiert zu werden.</span><span class="sxs-lookup"><span data-stu-id="c8225-237">Please follow [@craigaloewen](https://twitter.com/craigaloewen) on Twitter to learn of news, updates, etc.</span></span>
