---
title: Installieren oder Entfernen von auf Windows 10 Anniversary Update oder Creators Update
description: Anweisungen zur der Vorgängerversion, die Beta-Distribution, die auf Windows 10 Anniversary Update oder Creators Update-Installation und Deinstallation
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10, legacy, beta, install, remove, uninstall, un-install, delete, deprecated
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: b31bb3a542b8481c723df42292e20e364680722d
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063588"
---
# <a name="guide-to-install-or-uninstall-windows-subsystem-for-linux-on-windows-10-anniversary-update-and-creators-update"></a><span data-ttu-id="ae3b1-104">Anleitung zum Installieren oder Deinstallieren von Windows-Subsystem für Linux auf Windows 10 Anniversary Update und Creators Update</span><span class="sxs-lookup"><span data-stu-id="ae3b1-104">Guide to install or uninstall Windows Subsystem for Linux on Windows 10 Anniversary Update and Creators Update</span></span> 

<span data-ttu-id="ae3b1-105">Wenn Sie Windows 10 Creators Update ausführen, oder höher, bitte [führen Sie die installationsanweisungen für Windows 10](install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="ae3b1-105">If you're running Windows 10 Creators Update or later, please [follow the Windows 10 installation instructions](install-win10.md).</span></span>

<strong><em><span style="color: #f28014"><span data-ttu-id="ae3b1-106">Die folgenden Anweisungen gelten für Benutzer, die Windows 10 Anniversary Update oder Windows 10 Creators Update</span><span class="sxs-lookup"><span data-stu-id="ae3b1-106">The following instructions are for users running Windows 10 Anniversary Update or Windows 10 Creators Update</span></span></span></em></strong>

<span data-ttu-id="ae3b1-107">Vor Windows 10 Fall Creators Update (Version 1709) WSL als Betafunktion veröffentlicht wurde und eine einzelne Instanz von Ubuntu bei "Bash auf Ubuntu unter Windows" (oder Bash.exe) zuerst ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-107">Prior to Windows 10 Fall Creators Update (version 1709), WSL was released as a beta feature and installed a single Ubuntu instance when "Bash on Ubuntu on Windows" (or Bash.exe) was first run.</span></span>

> <span data-ttu-id="ae3b1-108">Während Sie die WSL unter früheren Versionen von Windows 10 verwenden können, ist diese Betaversion "legacy-Distribution, die" als veraltet eingestuft.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-108">While you CAN use WSL on earlier Windows 10 releases, this beta "legacy distro" is now considered obsolete.</span></span> <span data-ttu-id="ae3b1-109">Wir empfehlen Ihnen, führen Sie die neueste Version von Windows 10 verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-109">We strongly encourage you to run the most recent version of Windows 10 available.</span></span> <span data-ttu-id="ae3b1-110">Jeder neuen Windows 10-Version enthält viele Hunderte von Fehlerbehebungen und Verbesserungen in WSL eigenständig verwendet, sodass immer Linux-Tools und apps für WSL ordnungsgemäß ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-110">Each new Windows 10 release includes many hundreds of fixes and improvements in WSL alone, allowing ever more Linux tools and apps to run correctly on WSL.</span></span>

<span data-ttu-id="ae3b1-111">Wenn Sie nicht auf Fall Creators Update oder höher aktualisieren können, führen Sie die folgenden Schritte zum Aktivieren und Verwenden von WSL:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-111">If you cannot upgrade to Fall Creators Update or later, follow the steps below to enable and use WSL:</span></span>

1. <span data-ttu-id="ae3b1-112">Entwickler-Modus für die Ausführung WSL auf Windows 10 Anniversary Update oder Creators Update aktivieren, müssen Sie den Entwicklermodus aktivieren:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-112">Turn on Developer Mode  To run WSL on Windows 10 Anniversary Update or Creators Update, you must enable Developer Mode:</span></span>

    <span data-ttu-id="ae3b1-113">Open **Einstellungen** -> **Update und Sicherheit** -> **für Entwickler**</span><span class="sxs-lookup"><span data-stu-id="ae3b1-113">Open **Settings** -> **Update and Security** -> **For developers**</span></span>

    <span data-ttu-id="ae3b1-114">Wählen Sie das Optionsfeld Entwicklermodus</span><span class="sxs-lookup"><span data-stu-id="ae3b1-114">Select the Developer Mode radio button</span></span>  
    ![Aktivieren des Entwicklermodus](media/updateAndSecurity.png)

    > <span data-ttu-id="ae3b1-116">Die Anforderung zum Aktivieren der Entwicklermodus wurde [in Windows 10 Fall Creators Update entfernt](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/)</span><span class="sxs-lookup"><span data-stu-id="ae3b1-116">The requirement to enable Developer Mode was [removed in Windows 10 Fall Creators Update](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/)</span></span>

1. <span data-ttu-id="ae3b1-117">Öffnen Sie eine Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-117">Open a command prompt.</span></span>  <span data-ttu-id="ae3b1-118">Typ `bash` und die EINGABETASTE drücken</span><span class="sxs-lookup"><span data-stu-id="ae3b1-118">Type `bash` and hit enter</span></span>

    <span data-ttu-id="ae3b1-119">Beim ersten Ausführen von Bash auf Ubuntu unter Windows, werden Sie aufgefordert, Canonical Lizenz zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-119">The first time you run Bash on Ubuntu on Windows, you'll be prompted to accept Canonical's license.</span></span> <span data-ttu-id="ae3b1-120">Sobald Accpted, WSL heruntergeladen und installiert die Ubuntu-Instanz auf dem Computer, und eine "Bash auf Ubuntu unter Windows"-Verknüpfung Ihrem Startmenü hinzugefügt werden wird.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-120">Once accpted, WSL will download and install the Ubuntu instance onto your machine, and a "Bash on Ubuntu on Windows" shortcut will be added to your start menu.</span></span>

    ![Aufforderung zur Installation von Ubuntu](media/bashShellInstall.png)

    <span data-ttu-id="ae3b1-122">Beim ersten Ausführen von Bash auf Ubuntu unter Windows, werden Sie aufgefordert werden UNIX-Benutzername und Kennwort zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-122">The first time you run Bash on Ubuntu on Windows, you will be prompted to create a UNIX username and password.</span></span> <span data-ttu-id="ae3b1-123">Führen Sie die [Anweisungen für die neue Distribution Instanz](initialize-distro.md) zum Abschließen der Installations</span><span class="sxs-lookup"><span data-stu-id="ae3b1-123">Follow the [new distro instance instructions](initialize-distro.md) to complete your installation</span></span>

1. <span data-ttu-id="ae3b1-124">Starten Sie eine neue Ubuntu-Shell, indem entweder:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-124">Launch a new Ubuntu shell by either:</span></span>
    * <span data-ttu-id="ae3b1-125">Ausführung `bash` an einer Eingabeaufforderung</span><span class="sxs-lookup"><span data-stu-id="ae3b1-125">Running `bash` from a command-prompt</span></span>
    * <span data-ttu-id="ae3b1-126">Klicken Sie auf die Verknüpfung im Startmenü "Bash auf Ubuntu unter Windows"</span><span class="sxs-lookup"><span data-stu-id="ae3b1-126">Clicking the start menu "Bash on Ubuntu on Windows" shortcut</span></span>

    
## <a name="uninstallingremoving-the-legacy-distro"></a><span data-ttu-id="ae3b1-127">Die legacy-Distribution Deinstallieren/Entfernen</span><span class="sxs-lookup"><span data-stu-id="ae3b1-127">Uninstalling/Removing the legacy distro</span></span>
<span data-ttu-id="ae3b1-128">Wenn Sie von einer früheren Version von Windows 10, Windows 10 Fall Creators Update auf denen WSL installiert aktualisieren, sind Ihre vorhandenen Distribution bleibt unverändert.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-128">If you upgrade to Windows 10 Fall Creators Update from an earlier Windows 10 release upon which you installed WSL, your existing distro will remain intact.</span></span> <span data-ttu-id="ae3b1-129">Allerdings wir dringend empfohlen, eine neue Store bereitgestellte Distribution ASAP installieren und migrieren alle erforderlichen Dateien, Daten usw. aus Ihrem legacy-Distribution, die zu Ihrer neuen Distribution.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-129">However, we STRONGLY encourage you to install a new Store-delivered distro ASAP, and migrate any necessary files, data, etc. from your legacy distro to your new distro.</span></span>

<span data-ttu-id="ae3b1-130">Um die legacy-Distribution, die von Ihrem Computer zu entfernen, führen Sie Folgendes von einer Befehlszeile oder PowerShell ein:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-130">To remove the legacy distro from your machine, run the following from a Command Line or PowerShell instance:</span></span>

```console
lxrun /uninstall /full
```

### <a name="manually-deleting-the-legacy-distro"></a><span data-ttu-id="ae3b1-131">Die legacy-Distribution, die manuell zu löschen</span><span class="sxs-lookup"><span data-stu-id="ae3b1-131">Manually deleting the legacy distro</span></span>
<span data-ttu-id="ae3b1-132">Wenn Sie möchten, können Sie Ihre legacy-Instanz manuell löschen.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-132">If you wish, you can manually delete your legacy instance.</span></span> <span data-ttu-id="ae3b1-133">Dies kann erforderlich sein, wenn deinstallieren, die mithilfe des legacy-Distribution, die Probleme auftreten `lxrun.exe`, oder Windows 10 Frühjahr 2018 Update ausgeführt werden (oder höher) der werden nicht im Lieferumfang `lxrun.exe`.</span><span class="sxs-lookup"><span data-stu-id="ae3b1-133">This may be required if you encounter issues uninstalling the legacy distro using `lxrun.exe`, or are running Windows 10 Spring 2018 Update (or later) which do not ship with `lxrun.exe`.</span></span>

<span data-ttu-id="ae3b1-134">Um Ihre älteren WSL Distribution erzwungen zu löschen, löschen die `%localappdata%\lxss\` Ordner (und alle es handelt sich um untergeordneten Inhalt) mithilfe von Windows Datei-Explorer oder die Befehlszeile:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-134">To forcefully delete your legacy WSL distro, delete the `%localappdata%\lxss\` folder (and all it's sub-contents) using Windows' File Explorer, or the command-line:</span></span>

<span data-ttu-id="ae3b1-135">Mithilfe der PowerShell</span><span class="sxs-lookup"><span data-stu-id="ae3b1-135">Using PowerShell</span></span>
```powershell
rm -Recurse $env:localappdata/lxss/
```

<span data-ttu-id="ae3b1-136">Verwenden Cmd ein:</span><span class="sxs-lookup"><span data-stu-id="ae3b1-136">Using Cmd:</span></span>
```console
DEL /S %localappdata%\lxss\
```
