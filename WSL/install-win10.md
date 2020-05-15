---
title: Installieren des Windows-Subsystems für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: BashOnWindows, Bash, WSL, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installieren, Aktivieren, WSL2, Version 2
ms.date: 05/12/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: acb83234a90dc5e65c98518b869f29c4ecf973d8
ms.sourcegitcommit: e6e888f2b88a2d9c105cee46e5ab5b70aa43dd80
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/13/2020
ms.locfileid: "83343912"
---
# <a name="windows-subsystem-for-linux-installation-guide-for-windows-10"></a><span data-ttu-id="abe01-104">Windows-Subsystem für Linux: Installationsleitfaden für Windows 10</span><span class="sxs-lookup"><span data-stu-id="abe01-104">Windows Subsystem for Linux Installation Guide for Windows 10</span></span>

## <a name="install-the-windows-subsystem-for-linux"></a><span data-ttu-id="abe01-105">Installieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="abe01-105">Install the Windows Subsystem for Linux</span></span>

<span data-ttu-id="abe01-106">Bevor Sie eine Linux-Verteilung unter Windows installieren können, müssen Sie das optionale Feature „Windows-Subsystem für Linux“ aktivieren.</span><span class="sxs-lookup"><span data-stu-id="abe01-106">Before installing any Linux distributions on Windows, you must enable the "Windows Subsystem for Linux" optional feature.</span></span>

<span data-ttu-id="abe01-107">Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="abe01-107">Open PowerShell as Administrator and run:</span></span>

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

<span data-ttu-id="abe01-108">Um nur WSL 1 zu installieren, sollten Sie nun den Computer neu starten und mit dem [Installieren der Linux-Verteilung Ihrer Wahl](./install-win10.md#install-your-linux-distribution-of-choice) fortfahren. Andernfalls warten Sie auf den Neustart, und fahren Sie mit dem Update auf WSL 2 fort.</span><span class="sxs-lookup"><span data-stu-id="abe01-108">To only install WSL 1, you should now restart your machine and move on to [Install your Linux distribution of choice](./install-win10.md#install-your-linux-distribution-of-choice), otherwise wait to restart and move on to update to WSL 2.</span></span> <span data-ttu-id="abe01-109">Erfahren Sie mehr über den [Vergleich zwischen WSL 2 und WSL 1](./compare-versions.md).</span><span class="sxs-lookup"><span data-stu-id="abe01-109">Read more about [Comparing WSL 2 and WSL 1](./compare-versions.md).</span></span>

## <a name="update-to-wsl-2"></a><span data-ttu-id="abe01-110">Aktualisieren auf WSL 2</span><span class="sxs-lookup"><span data-stu-id="abe01-110">Update to WSL 2</span></span>

<span data-ttu-id="abe01-111">Um ein Update auf WSL 2 durchführen zu können, müssen die folgenden Kriterien erfüllt sein:</span><span class="sxs-lookup"><span data-stu-id="abe01-111">To update to WSL 2, you must meet the follow criteria:</span></span>

- <span data-ttu-id="abe01-112">Ausgeführt unter Windows 10, [aktualisiert auf Version 2004](ms-settings:windowsupdate), **Build 19041** oder höher.</span><span class="sxs-lookup"><span data-stu-id="abe01-112">Running Windows 10, [updated to version 2004](ms-settings:windowsupdate), **Build 19041** or higher.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="abe01-113">Derzeit müssen Sie zum Aktualisieren auf Windows 10, Version 2004 (Build 19041), dem [Windows Insider-Programm beitreten](https://insider.windows.com/insidersigninboth/) und den Ring „Release Preview“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="abe01-113">Currently to update to Windows 10, version 2004 (Build 19041), you will need to [join the Windows Insider program](https://insider.windows.com/insidersigninboth/) and select the "Release Preview" ring.</span></span> <span data-ttu-id="abe01-114">Das öffentliche Release sollte Ende Mai verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="abe01-114">The public release should arrive by late May.</span></span>

- <span data-ttu-id="abe01-115">Überprüfen Sie Ihre Windows-Version, indem Sie die **Windows-Logo-Taste+R** auswählen, **winver** eingeben und **OK** auswählen.</span><span class="sxs-lookup"><span data-stu-id="abe01-115">Check your Windows version by selecting the **Windows logo key + R**, type **winver**, select **OK**.</span></span> <span data-ttu-id="abe01-116">(Oder geben Sie den Befehl `ver` an der Windows-Eingabeaufforderung ein.)</span><span class="sxs-lookup"><span data-stu-id="abe01-116">(Or enter the `ver` command in Windows Command Prompt).</span></span> <span data-ttu-id="abe01-117">[Aktualisieren Sie auf die neueste Windows-Version](ms-settings:windowsupdate), wenn Ihr Build niedriger als 19041 ist.</span><span class="sxs-lookup"><span data-stu-id="abe01-117">Please [update to the latest Windows version](ms-settings:windowsupdate) if your build is lower than 19041.</span></span> <span data-ttu-id="abe01-118">[Holen Sie sich den Windows Update-Assistenten](https://www.microsoft.com/software-download/windows10).</span><span class="sxs-lookup"><span data-stu-id="abe01-118">[Get Windows Update Assistant](https://www.microsoft.com/software-download/windows10).</span></span>

### <a name="enable-the-virtual-machine-platform-optional-component"></a><span data-ttu-id="abe01-119">Aktivieren Sie die optionale Komponente „Virtual Machine Platform“.</span><span class="sxs-lookup"><span data-stu-id="abe01-119">Enable the 'Virtual Machine Platform' optional component</span></span>

<span data-ttu-id="abe01-120">Vor der Installation von WSL 2 müssen Sie das optionale Feature „Virtual Machine Platform“ aktivieren.</span><span class="sxs-lookup"><span data-stu-id="abe01-120">Before installing WSL 2, you must enable the "Virtual Machine Platform" optional feature.</span></span>

<span data-ttu-id="abe01-121">Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="abe01-121">Open PowerShell as Administrator and run:</span></span>

```powershell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

<span data-ttu-id="abe01-122">**Starten Sie Ihrem Computer neu**, um die WSL-Installation und das Update auf WSL 2 abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="abe01-122">**Restart** your machine to complete the WSL install and update to WSL 2.</span></span>

### <a name="set-wsl-2-as-your-default-version"></a><span data-ttu-id="abe01-123">Festlegen von WSL 2 als Standardversion</span><span class="sxs-lookup"><span data-stu-id="abe01-123">Set WSL 2 as your default version</span></span>

<span data-ttu-id="abe01-124">Führen Sie bei der Installation einer neuen Linux-Verteilung den folgenden Befehl in PowerShell aus, um WSL 2 als Standardversion festzulegen:</span><span class="sxs-lookup"><span data-stu-id="abe01-124">Run the following command in Powershell to set WSL 2 as the default version when installing a new Linux distribution:</span></span>

```powershell
wsl --set-default-version 2
```

## <a name="install-your-linux-distribution-of-choice"></a><span data-ttu-id="abe01-125">Installieren der Linux-Verteilung Ihrer Wahl</span><span class="sxs-lookup"><span data-stu-id="abe01-125">Install your Linux distribution of choice</span></span>

1. <span data-ttu-id="abe01-126">Öffnen Sie den [Microsoft Store](https://aka.ms/wslstore), und wählen Sie Ihre bevorzugte Linux-Verteilung aus.</span><span class="sxs-lookup"><span data-stu-id="abe01-126">Open the [Microsoft Store](https://aka.ms/wslstore) and select your favorite Linux distribution.</span></span>

    ![Ansicht der Linux-Verteilungen im Microsoft Store](media/store.png)

    <span data-ttu-id="abe01-128">Über die folgenden Links wird die Seite des Microsoft Store für jede Distribution geöffnet:</span><span class="sxs-lookup"><span data-stu-id="abe01-128">The following links will open the Microsoft store page for each distribution:</span></span>

    - [<span data-ttu-id="abe01-129">Ubuntu 16.04 LTS</span><span class="sxs-lookup"><span data-stu-id="abe01-129">Ubuntu 16.04 LTS</span></span>](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    - [<span data-ttu-id="abe01-130">Ubuntu 18.04 LTS</span><span class="sxs-lookup"><span data-stu-id="abe01-130">Ubuntu 18.04 LTS</span></span>](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    - [<span data-ttu-id="abe01-131">openSUSE Leap 15.1</span><span class="sxs-lookup"><span data-stu-id="abe01-131">openSUSE Leap 15.1</span></span>](https://www.microsoft.com/store/apps/9NJFZK00FGKV)
    - [<span data-ttu-id="abe01-132">SUSE Linux Enterprise Server 12 SP5</span><span class="sxs-lookup"><span data-stu-id="abe01-132">SUSE Linux Enterprise Server 12 SP5</span></span>](https://www.microsoft.com/store/apps/9MZ3D1TRP8T1)
    - [<span data-ttu-id="abe01-133">SUSE Linux Enterprise Server 15 SP1</span><span class="sxs-lookup"><span data-stu-id="abe01-133">SUSE Linux Enterprise Server 15 SP1</span></span>](https://www.microsoft.com/store/apps/9PN498VPMF3Z)
    - [<span data-ttu-id="abe01-134">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="abe01-134">Kali Linux</span></span>](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    - [<span data-ttu-id="abe01-135">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="abe01-135">Debian GNU/Linux</span></span>](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    - [<span data-ttu-id="abe01-136">Fedora Remix for WSL</span><span class="sxs-lookup"><span data-stu-id="abe01-136">Fedora Remix for WSL</span></span>](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    - [<span data-ttu-id="abe01-137">Pengwin</span><span class="sxs-lookup"><span data-stu-id="abe01-137">Pengwin</span></span>](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    - [<span data-ttu-id="abe01-138">Pengwin Enterprise</span><span class="sxs-lookup"><span data-stu-id="abe01-138">Pengwin Enterprise</span></span>](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    - [<span data-ttu-id="abe01-139">Alpine WSL</span><span class="sxs-lookup"><span data-stu-id="abe01-139">Alpine WSL</span></span>](https://www.microsoft.com/store/apps/9p804crf0395)

2. <span data-ttu-id="abe01-140">Wählen Sie auf der Seite der Verteilung die Option „Get“ (Abrufen) aus.</span><span class="sxs-lookup"><span data-stu-id="abe01-140">From the distribution's page, select "Get".</span></span>

    ![Linux-Verteilungen im Microsoft Store](media/UbuntuStore.png)

## <a name="set-up-a-new-distribution"></a><span data-ttu-id="abe01-142">Einrichten einer neuen Verteilung</span><span class="sxs-lookup"><span data-stu-id="abe01-142">Set up a new distribution</span></span>

<span data-ttu-id="abe01-143">Wenn Sie eine neu installierte Linux-Verteilung zum ersten Mal starten, wird ein Konsolenfenster geöffnet, und Sie werden aufgefordert, ein oder zwei Minuten zu warten, bis die Dateien dekomprimiert und auf dem PC gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="abe01-143">The first time you launch a newly installed Linux distribution, a console window will open and you'll be asked to wait for a minute or two for files to de-compress and be stored on your PC.</span></span> <span data-ttu-id="abe01-144">Alle zukünftigen Starts sollten weniger als eine Sekunde in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="abe01-144">All future launches should take less than a second.</span></span>

<span data-ttu-id="abe01-145">Anschließend müssen Sie [ein Benutzerkonto und Kennwort für Ihre neue Linux-Verteilung erstellen](./user-support.md).</span><span class="sxs-lookup"><span data-stu-id="abe01-145">You will then need to [create a user account and password for your new Linux distribution](./user-support.md).</span></span>

![Entpacken von Ubuntu in der Windows-Konsole](media/UbuntuInstall.png)

## <a name="set-your-distribution-version-to-wsl-1-or-wsl-2"></a><span data-ttu-id="abe01-147">Festlegen der Verteilungsversion auf WSL 1 oder WSL 2</span><span class="sxs-lookup"><span data-stu-id="abe01-147">Set your distribution version to WSL 1 or WSL 2</span></span>

<span data-ttu-id="abe01-148">Sie können die den einzelnen installierten Linux-Verteilungen zugewiesenen WSL-Version überprüfen, indem Sie die PowerShell-Befehlszeile öffnen und den folgenden Befehl (nur verfügbar in [Windows Build 19041 oder höher](ms-settings:windowsupdate)) eingeben: `wsl -l -v`</span><span class="sxs-lookup"><span data-stu-id="abe01-148">You can check the WSL version assigned to each of the Linux distributions you have installed by opening the PowerShell command line and entering the command (only available in [Windows Build 19041 or higher](ms-settings:windowsupdate)): `wsl -l -v`</span></span>

```bash
wsl --list --verbose
```

<span data-ttu-id="abe01-149">Um eine Verteilung so einzurichten, dass sie von einer der beiden WSL-Versionen unterstützt wird, führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="abe01-149">To set a distribution to be backed by either version of WSL please run:</span></span>

```bash
wsl --set-version <distribution name> <versionNumber>
```

<span data-ttu-id="abe01-150">Ersetzen Sie hierbei `<distribution name>` durch den tatsächlichen Namen Ihrer Verteilung und `<versionNumber>` durch die Ziffer „1“ oder „2“.</span><span class="sxs-lookup"><span data-stu-id="abe01-150">Make sure to replace `<distribution name>` with the actual name of your distribution and `<versionNumber>` with the number '1' or '2'.</span></span> <span data-ttu-id="abe01-151">Sie können jederzeit zu WSL 1 zurückwechseln, indem sie denselben Befehl wie oben ausführen, aber die 2 durch eine 1 ersetzen.</span><span class="sxs-lookup"><span data-stu-id="abe01-151">You can change back to WSL 1 at anytime by running the same command as above but replacing the '2' with a '1'.</span></span>

<span data-ttu-id="abe01-152">Wenn Sie WSL 2 als Ihre Standardarchitektur festlegen möchten, ist dies über diesen Befehl möglich:</span><span class="sxs-lookup"><span data-stu-id="abe01-152">Additionally, if you want to make WSL 2 your default architecture you can do so with this command:</span></span>

```bash
wsl --set-default-version 2
```

<span data-ttu-id="abe01-153">Dadurch wird die Version jeder neu installierten Verteilung auf WSL 2 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="abe01-153">This will set the version of any new distribution installed to WSL 2.</span></span>

## <a name="troubleshooting-installation"></a><span data-ttu-id="abe01-154">Problembehandlung bei der Installation</span><span class="sxs-lookup"><span data-stu-id="abe01-154">Troubleshooting installation</span></span>

<span data-ttu-id="abe01-155">Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="abe01-155">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="abe01-156">Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="abe01-156">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

- <span data-ttu-id="abe01-157">**Installation failed with error 0x80070003 (Installationsfehler mit Fehlercode 0x80070003)**</span><span class="sxs-lookup"><span data-stu-id="abe01-157">**Installation failed with error 0x80070003**</span></span>
  - <span data-ttu-id="abe01-158">Das Windows-Subsystem für Linux wird nur auf dem Systemlaufwerk ausgeführt (in der Regel ist dies Ihr Laufwerk `C:`).</span><span class="sxs-lookup"><span data-stu-id="abe01-158">The Windows Subsystem for Linux only runs on your system drive (usually this is your `C:` drive).</span></span> <span data-ttu-id="abe01-159">Stellen Sie sicher, dass die Verteilungen auf dem Systemlaufwerk gespeichert sind:</span><span class="sxs-lookup"><span data-stu-id="abe01-159">Make sure that distributions are stored on your system drive:</span></span>  
  - <span data-ttu-id="abe01-160">Öffnen Sie **Einstellungen** -> **Speicher** -> **Weitere Speichereinstellungen: Ändern Sie den Speicherort für neue Inhalte**
    ![Abbildung der Systemeinstellungen für die Installation von Apps auf dem Laufwerk C:](media/AppStorage.png)</span><span class="sxs-lookup"><span data-stu-id="abe01-160">Open **Settings** -> **Storage** -> **More Storage Settings: Change where new content is saved**
![Picture of system settings to install apps on C: drive](media/AppStorage.png)</span></span>

- <span data-ttu-id="abe01-161">**WslRegisterDistribution failed with error 0x8007019e (WslRegisterDistribution-Fehler mit Fehlercode 0x8007019e)**</span><span class="sxs-lookup"><span data-stu-id="abe01-161">**WslRegisterDistribution failed with error 0x8007019e**</span></span>
  - <span data-ttu-id="abe01-162">Die optionale Komponente des Windows-Subsystems für Linux ist nicht aktiviert:</span><span class="sxs-lookup"><span data-stu-id="abe01-162">The Windows Subsystem for Linux optional component is not enabled:</span></span>
  - <span data-ttu-id="abe01-163">Öffnen Sie **Systemsteuerung** -> **Programme und Funktionen** -> **Windows-Funktion aktivieren oder deaktivieren**. Aktivieren Sie die Option **Windows-Subsystem für Linux**, oder verwenden Sie das PowerShell-Cmdlet, das am Anfang dieses Artikels erwähnt wurde.</span><span class="sxs-lookup"><span data-stu-id="abe01-163">Open **Control Panel** -> **Programs and Features** -> **Turn Windows Feature on or off** -> Check **Windows Subsystem for Linux** or using the PowerShell cmdlet mentioned at the begining of this article.</span></span>

- <span data-ttu-id="abe01-164">**Fehler 0x80070003 oder Fehler 0x80370102 während der Installation**</span><span class="sxs-lookup"><span data-stu-id="abe01-164">**Installation failed with error 0x80070003 or error 0x80370102**</span></span>
  - <span data-ttu-id="abe01-165">Stellen Sie sicher, dass im BIOS Ihres Computers die Virtualisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="abe01-165">Please make sure that virtualization is enabled inside of your computer's BIOS.</span></span> <span data-ttu-id="abe01-166">Die Anweisungen zur Aktivierung variieren je nach Computer. Die entsprechenden Optionen befinden sich wahrscheinlich in den CPU-bezogenen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="abe01-166">The instructions on how to do this will vary from computer to computer, and will most likely be under CPU related options.</span></span>

- <span data-ttu-id="abe01-167">**Fehler beim Upgradeversuch: `Invalid command line option: wsl --set-version Ubuntu 2`**</span><span class="sxs-lookup"><span data-stu-id="abe01-167">**Error when trying to upgrade: `Invalid command line option: wsl --set-version Ubuntu 2`**</span></span>
  - <span data-ttu-id="abe01-168">Stellen Sie sicher, dass das Windows-Subsystem für Linux aktiviert wurde und Sie Windows-Build 19041 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="abe01-168">Please make sure that you have the Windows Subsystem for Linux enabled, and that you're using Windows Build version 19041 or higher.</span></span> <span data-ttu-id="abe01-169">Führen Sie zum Aktivieren von WSL in einer PowerShell-Eingabeaufforderung mit Administratorberechtigungen diesen Befehl aus: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span><span class="sxs-lookup"><span data-stu-id="abe01-169">To enable WSL run this command in a Powershell prompt with admin privileges: `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`.</span></span> <span data-ttu-id="abe01-170">Die vollständigen Anweisungen zur WSL-Installation finden Sie [hier](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="abe01-170">You can find the full WSL install instructions [here](./install-win10.md).</span></span>

- <span data-ttu-id="abe01-171">**Der angeforderte Vorgang konnte aufgrund einer Einschränkung des virtuellen Dateisystems nicht abgeschlossen werden. Dateien für virtuelle Festplatten müssen unkomprimiert und unverschlüsselt sein und dürfen keine geringe Dichte aufweisen.**</span><span class="sxs-lookup"><span data-stu-id="abe01-171">**The requested operation could not be completed due to a virtual disk system limitation. Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.**</span></span>
  - <span data-ttu-id="abe01-172">Bitte prüfen Sie den [WSL Github-Thread #4103](https://github.com/microsoft/WSL/issues/4103), der diesem Thema gewidmet ist, auf aktualisierte Informationen.</span><span class="sxs-lookup"><span data-stu-id="abe01-172">Please check [WSL Github thread #4103](https://github.com/microsoft/WSL/issues/4103) where this issue is being tracked for updated information.</span></span>

- <span data-ttu-id="abe01-173">**Der Ausdruck 'wsl' wurde nicht als Name eines Cmdlets, einer Funktion, einer Skriptdatei oder eines ausführbaren Programms erkannt.**</span><span class="sxs-lookup"><span data-stu-id="abe01-173">**The term 'wsl' is not recognized as the name of a cmdlet, function, script file, or operable program.**</span></span>
  - <span data-ttu-id="abe01-174">Vergewissern Sie sich, dass die [optionale Komponente Windows-Subsystem für Linux installiert ist](./install-win10.md#enable-the-virtual-machine-platform-optional-component).</span><span class="sxs-lookup"><span data-stu-id="abe01-174">Ensure that the [Windows Subsystem for Linux Optional Component is installed](./install-win10.md#enable-the-virtual-machine-platform-optional-component).</span></span> <span data-ttu-id="abe01-175">Außerdem wird dieser Fehler angezeigt, wenn Sie ein Arm64-Gerät verwenden und diesen Befehl aus PowerShell ausführen.</span><span class="sxs-lookup"><span data-stu-id="abe01-175">Additionally, if you are using an Arm64 device and running this command from PowerShell, you will receive this error.</span></span> <span data-ttu-id="abe01-176">Führen Sie stattdessen `wsl.exe` in [PowerShell Core](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6) oder einer Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="abe01-176">Instead run `wsl.exe` from [PowerShell Core](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6), or Command Prompt.</span></span>
