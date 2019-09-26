---
title: Installieren oder Entfernen von Windows 10 Anniversary Update oder Creators Update
description: Installations-und Deinstallations Anweisungen für die Legacy-, Beta-Distribution von Windows 10 Anniversary Update oder Creators Update
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10, Legacy, Beta, installieren, entfernen, deinstallieren, Deinstallation, löschen, veraltet
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 416bed3ed3a0470da2eb5e6beb75e73eb6836200
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269772"
---
# <a name="guide-to-install-or-uninstall-windows-subsystem-for-linux-on-windows-10-anniversary-update-and-creators-update"></a><span data-ttu-id="47a20-104">Leitfaden zum Installieren oder Deinstallieren des Windows-Subsystems für Linux unter Windows 10 Anniversary Update und Creators Update</span><span class="sxs-lookup"><span data-stu-id="47a20-104">Guide to install or uninstall Windows Subsystem for Linux on Windows 10 Anniversary Update and Creators Update</span></span> 

<span data-ttu-id="47a20-105">Wenn Sie Windows 10 Creators Update oder höher ausführen, befolgen Sie [die Installationsanweisungen für Windows 10](install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="47a20-105">If you're running Windows 10 Creators Update or later, please [follow the Windows 10 installation instructions](install-win10.md).</span></span>

<span data-ttu-id="47a20-106"><strong><em><span style="color: #f28014">Die folgenden Anweisungen gelten für Benutzer, die Windows 10 Anniversary Update oder Windows 10 Creators Update ausführen.</span></em></strong></span><span class="sxs-lookup"><span data-stu-id="47a20-106"><strong><em><span style="color: #f28014">The following instructions are for users running Windows 10 Anniversary Update or Windows 10 Creators Update</span></em></strong></span></span>

<span data-ttu-id="47a20-107">Vor Windows 10 Fall Creators Update (Version 1709) wurde WSL als Beta Funktion veröffentlicht und eine einzelne Ubuntu-Instanz installiert, als "bash on Ubuntu on Windows" (oder bash. exe) zum ersten Mal ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="47a20-107">Prior to Windows 10 Fall Creators Update (version 1709), WSL was released as a beta feature and installed a single Ubuntu instance when "Bash on Ubuntu on Windows" (or Bash.exe) was first run.</span></span>

> <span data-ttu-id="47a20-108">Obwohl Sie WSL unter früheren Versionen von Windows 10 verwenden können, ist diese Beta Version "Legacy Distribution" mittlerweile als veraltet eingestuft.</span><span class="sxs-lookup"><span data-stu-id="47a20-108">While you CAN use WSL on earlier Windows 10 releases, this beta "legacy distro" is now considered obsolete.</span></span> <span data-ttu-id="47a20-109">Wir empfehlen Ihnen dringend, die neueste verfügbare Version von Windows 10 auszuführen.</span><span class="sxs-lookup"><span data-stu-id="47a20-109">We strongly encourage you to run the most recent version of Windows 10 available.</span></span> <span data-ttu-id="47a20-110">Jede neue Version von Windows 10 enthält viele hundert Korrekturen und Verbesserungen in WSL, sodass immer mehr Linux-Tools und-Apps auf WSL ordnungsgemäß ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="47a20-110">Each new Windows 10 release includes many hundreds of fixes and improvements in WSL alone, allowing ever more Linux tools and apps to run correctly on WSL.</span></span>

<span data-ttu-id="47a20-111">Wenn Sie kein Upgrade auf Fall Creators Update oder höher ausführen können, führen Sie die folgenden Schritte aus, um WSL zu aktivieren und zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="47a20-111">If you cannot upgrade to Fall Creators Update or later, follow the steps below to enable and use WSL:</span></span>

1. <span data-ttu-id="47a20-112">Aktivieren Sie den Entwicklermodus, um WSL auf Windows 10 Anniversary Update oder Creators Update auszuführen. Sie müssen den Entwicklermodus aktivieren:</span><span class="sxs-lookup"><span data-stu-id="47a20-112">Turn on Developer Mode  To run WSL on Windows 10 Anniversary Update or Creators Update, you must enable Developer Mode:</span></span>

    <span data-ttu-id="47a20-113">Öffnen von **Einstellungen** -> **aktualisieren und Sicherheit** -> **für Entwickler**</span><span class="sxs-lookup"><span data-stu-id="47a20-113">Open **Settings** -> **Update and Security** -> **For developers**</span></span>

    <span data-ttu-id="47a20-114">Wählen Sie das Optionsfeld Entwicklermodus aus.</span><span class="sxs-lookup"><span data-stu-id="47a20-114">Select the Developer Mode radio button</span></span>  
    ![Aktivieren des Entwicklermodus](media/updateAndSecurity.png)

    > <span data-ttu-id="47a20-116">Die Anforderung zum Aktivieren des Entwicklermodus wurde [in Windows 10 Fall Creators Update entfernt](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/) .</span><span class="sxs-lookup"><span data-stu-id="47a20-116">The requirement to enable Developer Mode was [removed in Windows 10 Fall Creators Update](https://blogs.msdn.microsoft.com/commandline/2017/06/08/developer-mode-no-longer-required-for-windows-subsystem-for-linux/)</span></span>

1. <span data-ttu-id="47a20-117">Öffnen Sie eine Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="47a20-117">Open a command prompt.</span></span>  <span data-ttu-id="47a20-118">Eingeben `bash` und drücken der EINGABETASTE</span><span class="sxs-lookup"><span data-stu-id="47a20-118">Type `bash` and hit enter</span></span>

    <span data-ttu-id="47a20-119">Wenn Sie bash auf Ubuntu unter Windows zum ersten Mal ausführen, werden Sie aufgefordert, die kanonische Lizenz zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="47a20-119">The first time you run Bash on Ubuntu on Windows, you'll be prompted to accept Canonical's license.</span></span> <span data-ttu-id="47a20-120">Nach der Annahme wird die Ubuntu-Instanz von WSL auf Ihren Computer heruntergeladen und installiert, und dem Startmenü wird eine "bash on Ubuntu on Windows"-Verknüpfung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="47a20-120">Once accepted, WSL will download and install the Ubuntu instance onto your machine, and a "Bash on Ubuntu on Windows" shortcut will be added to your start menu.</span></span>

    ![Eingabeaufforderung zur Installation von Ubuntu](media/bashShellInstall.png)

    <span data-ttu-id="47a20-122">Wenn Sie bash unter Windows zum ersten Mal ausführen, werden Sie aufgefordert, einen UNIX-Benutzernamen und ein Kennwort zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="47a20-122">The first time you run Bash on Ubuntu on Windows, you will be prompted to create a UNIX username and password.</span></span> <span data-ttu-id="47a20-123">Befolgen Sie die [Anweisungen der neuen Distribution-Instanz](initialize-distro.md) , um die Installation abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="47a20-123">Follow the [new distro instance instructions](initialize-distro.md) to complete your installation</span></span>

1. <span data-ttu-id="47a20-124">Starten Sie eine neue Ubuntu-Shell mit folgenden Optionen:</span><span class="sxs-lookup"><span data-stu-id="47a20-124">Launch a new Ubuntu shell by either:</span></span>
    * <span data-ttu-id="47a20-125">Ausführen `bash` über eine Eingabeaufforderung</span><span class="sxs-lookup"><span data-stu-id="47a20-125">Running `bash` from a command-prompt</span></span>
    * <span data-ttu-id="47a20-126">Klicken auf das Startmenü "bash on Ubuntu on Windows"-Verknüpfung</span><span class="sxs-lookup"><span data-stu-id="47a20-126">Clicking the start menu "Bash on Ubuntu on Windows" shortcut</span></span>

    
## <a name="uninstallingremoving-the-legacy-distro"></a><span data-ttu-id="47a20-127">Deinstallieren/Entfernen der Legacy Distribution</span><span class="sxs-lookup"><span data-stu-id="47a20-127">Uninstalling/Removing the legacy distro</span></span>
<span data-ttu-id="47a20-128">Wenn Sie von einer früheren Windows 10-Version, auf der Sie WSL installiert haben, ein Upgrade auf Windows 10 Fall Creators Update durchführen, bleibt Ihre vorhandene Distribution unverändert.</span><span class="sxs-lookup"><span data-stu-id="47a20-128">If you upgrade to Windows 10 Fall Creators Update from an earlier Windows 10 release upon which you installed WSL, your existing distro will remain intact.</span></span> <span data-ttu-id="47a20-129">Es wird jedoch dringend empfohlen, dass Sie eine neue, vom Speicher bereitgestellte Distribution-ASaP installieren und alle notwendigen Dateien, Daten usw. aus Ihrer Legacy-Distribution zu ihrer neuen Distribution migrieren.</span><span class="sxs-lookup"><span data-stu-id="47a20-129">However, we STRONGLY encourage you to install a new Store-delivered distro ASAP, and migrate any necessary files, data, etc. from your legacy distro to your new distro.</span></span>

<span data-ttu-id="47a20-130">Um die Legacy-Distribution von Ihrem Computer zu entfernen, führen Sie Folgendes über eine Befehlszeile oder eine PowerShell-Instanz aus:</span><span class="sxs-lookup"><span data-stu-id="47a20-130">To remove the legacy distro from your machine, run the following from a Command Line or PowerShell instance:</span></span>

```console
wsl --unregister Legacy
```

<span data-ttu-id="47a20-131">Wenn Sie nicht Windows-Version 1903 oder höher verwenden, müssen Sie möglicherweise oder `wslconfig /u Legacy` `lxrun /uninstall /full` stattdessen ausführen.</span><span class="sxs-lookup"><span data-stu-id="47a20-131">If you are not using Windows Version 1903 or higher, you may need to run `wslconfig /u Legacy` or `lxrun /uninstall /full` instead.</span></span> 

### <a name="manually-deleting-the-legacy-distro"></a><span data-ttu-id="47a20-132">Manuelles Löschen der Legacy-Distribution</span><span class="sxs-lookup"><span data-stu-id="47a20-132">Manually deleting the legacy distro</span></span>
<span data-ttu-id="47a20-133">Wenn Sie möchten, können Sie die Legacy Instanz manuell löschen.</span><span class="sxs-lookup"><span data-stu-id="47a20-133">If you wish, you can manually delete your legacy instance.</span></span> <span data-ttu-id="47a20-134">Dies ist möglicherweise erforderlich, wenn Probleme beim Deinstallieren der Legacy-Distribution `lxrun.exe`mithilfe von auftreten oder wenn Windows 10 Spring 2018 Update (oder höher) ausgeführt wird, das `lxrun.exe`nicht mit ausgeliefert wird.</span><span class="sxs-lookup"><span data-stu-id="47a20-134">This may be required if you encounter issues uninstalling the legacy distro using `lxrun.exe`, or are running Windows 10 Spring 2018 Update (or later) which do not ship with `lxrun.exe`.</span></span>

<span data-ttu-id="47a20-135">Löschen Sie den Ordner (und dessen unter Inhalt) mit dem `%localappdata%\lxss\` Windows-Datei-Explorer oder der Befehlszeile, um das Löschen der alten WSL-Distribution zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="47a20-135">To forcefully delete your legacy WSL distro, delete the `%localappdata%\lxss\` folder (and all it's sub-contents) using Windows' File Explorer, or the command-line:</span></span>

<span data-ttu-id="47a20-136">Mithilfe der PowerShell</span><span class="sxs-lookup"><span data-stu-id="47a20-136">Using PowerShell</span></span>
```powershell
rm -Recurse $env:localappdata/lxss/
```

<span data-ttu-id="47a20-137">Mithilfe von cmd:</span><span class="sxs-lookup"><span data-stu-id="47a20-137">Using Cmd:</span></span>
```console
DEL /S %localappdata%\lxss\
```
