---
title: Initialisiert eine neue WSL-Linux-Distribution
description: Schließen Sie nach der Installation einer Linux-Distribution für WSL Initialisierung, indem Sie die folgenden einfachen Schritte
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 7f1ce521b248c873fa7f81c6363eb506c0363fed
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2019
ms.locfileid: "59902047"
---
# <a name="initializing-a-newly-installed-distro"></a><span data-ttu-id="b9684-104">Initialisiert eine neu installierte Distribution</span><span class="sxs-lookup"><span data-stu-id="b9684-104">Initializing a newly installed distro</span></span>
<span data-ttu-id="b9684-105">Nachdem Ihre Distribution heruntergeladen und installiert wurde, müssen Sie zum Abschließen der Initialisierung der neuen Distribution:</span><span class="sxs-lookup"><span data-stu-id="b9684-105">Once your distro has been downloaded and installed, you'll need to complete initialization of the new distro:</span></span>

## <a name="launch-a-distro"></a><span data-ttu-id="b9684-106">Starten Sie eine Distribution</span><span class="sxs-lookup"><span data-stu-id="b9684-106">Launch a distro</span></span>
<span data-ttu-id="b9684-107">Um die Initialisierung von Ihrer Distribution, die neu installierte abgeschlossen haben, starten Sie eine neue Instanz.</span><span class="sxs-lookup"><span data-stu-id="b9684-107">To complete the initialization of your newly installed distro, launch a new instance.</span></span> <span data-ttu-id="b9684-108">Sie erreichen dies durch Klicken auf die Startschaltfläche "" in der Windows Store-app, oder starten Sie den-Distribution, die über das Startmenü zugreifen:</span><span class="sxs-lookup"><span data-stu-id="b9684-108">You can do this by clicking the "launch" button in the Windows Store app, or launching the distro from the Start menu:</span></span>

> <span data-ttu-id="b9684-109">Tipp: Sie möchten Ihre am häufigsten verwendeten Distributionen Startmenü und/oder die Taskleiste anheften.</span><span class="sxs-lookup"><span data-stu-id="b9684-109">Tip: You might want to pin your most frequently used distros to your Start menu, and/or to your taskbar!</span></span>

![Distributionen über das Startmenü starten](media/start-menu.png)

> <span data-ttu-id="b9684-111">In Windows Server, starten Sie Ihre Distribution des-Startprogramms `<distro>.exe` aus dem Installationsordner der Distribution.</span><span class="sxs-lookup"><span data-stu-id="b9684-111">On Windows Server, you can launch your distro's launcher executable `<distro>.exe` from the distro installation folder.</span></span>

<span data-ttu-id="b9684-112">Erstmals eine neu installierte Distribution ausgeführt wird, eine Konsole Fenster geöffnet wird, und werden Sie aufgefordert, ein oder zwei Minuten zum Abschluss der Installation warten.</span><span class="sxs-lookup"><span data-stu-id="b9684-112">The first time a newly installed distro runs, a Console window will open, and you'll be asked to wait for a minute or two for the installation to complete.</span></span>

> <span data-ttu-id="b9684-113">In dieser letzten Phase der Installation werden die Distribution Dateien aufheben komprimiert und gespeichert, die auf Ihrem PC, die zur Verwendung bereit.</span><span class="sxs-lookup"><span data-stu-id="b9684-113">During this final stage of installation, the distro's files are de-compressed and stored on your PC, ready for use.</span></span> <span data-ttu-id="b9684-114">Dies kann zu eine Minute oder länger, je nach die Leistung Ihres Computers Speichergeräte dauern.</span><span class="sxs-lookup"><span data-stu-id="b9684-114">This may take around a minute or more depending on the performance of your PC's storage devices.</span></span> <span data-ttu-id="b9684-115">In dieser Phase der Erstinstallation ist nur erforderlich, wenn eine Distribution, die neu installierten - ist alle auf zukünftig gestartete dauert weniger als eine Sekunde.</span><span class="sxs-lookup"><span data-stu-id="b9684-115">This initial installation phase is only required when a distro is clean-installed - all future launches should take less than a second.</span></span>

## <a name="setting-up-a-new-linux-user-account"></a><span data-ttu-id="b9684-116">Das Einrichten eines neuen Linux-Benutzerkontos</span><span class="sxs-lookup"><span data-stu-id="b9684-116">Setting up a new Linux user account</span></span>

<span data-ttu-id="b9684-117">Nach Abschluss der Installation werden Sie aufgefordert werden, erstellen Sie ein neues Benutzerkonto (und das Kennwort).</span><span class="sxs-lookup"><span data-stu-id="b9684-117">Once installation is complete, you will be prompted to create a new user account (and its password).</span></span> 

![Ubuntu, die in der Windows-Konsole Entpacken](media/UbuntuInstall.png)

<span data-ttu-id="b9684-119">Dieses Benutzerkonto ist für den normalen nicht-Admin-Benutzer, dass Sie angemeldet als standardmäßig beim Starten von einer Distribution.</span><span class="sxs-lookup"><span data-stu-id="b9684-119">This user account is for the normal non-admin user that you'll be logged-in as by default when launching a distro.</span></span>

> <span data-ttu-id="b9684-120">Sie können einen beliebigen Benutzernamen und das Kennwort werden sollen – sie haben keinen Einfluss auf Ihren Windows-Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="b9684-120">You can choose any username and password you wish - they have no bearing on your Windows username.</span></span> 

<span data-ttu-id="b9684-121">Wenn Sie eine neue Instanz der Distribution öffnen, werden Sie nicht aufgefordert für Ihr Kennwort jedoch **, wenn Sie einen Prozess mit erhöhen `sudo`, Sie müssen Ihr Kennwort eingeben**, stellen Sie sicher, dass ein Kennwort wählen Sie Sie leicht merken können!</span><span class="sxs-lookup"><span data-stu-id="b9684-121">When you open a new distro instance, you won't be prompted for your password, but **if you elevate a process using `sudo`, you will need to enter your password**, so make sure you choose a password you can easily remember!</span></span> <span data-ttu-id="b9684-122">Finden Sie unter den [Benutzersupport](user-support.md) Seite Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="b9684-122">See the [User Support](user-support.md) page for more info.</span></span>

## <a name="update--upgrade-your-distros-packages"></a><span data-ttu-id="b9684-123">Aktualisieren und Ihre Distribution Pakete aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9684-123">Update & upgrade your distro's packages</span></span>

<span data-ttu-id="b9684-124">Die meisten Distributionen, die mit einer leeren/minimale Paketkatalog ausgeliefert werden.</span><span class="sxs-lookup"><span data-stu-id="b9684-124">Most distros ship with an empty/minimal package catalog.</span></span> <span data-ttu-id="b9684-125">Es wird dringend empfohlen, Ihr Paketkatalog regelmäßig aktualisiert, und aktualisieren Ihre installierten Pakete, die mit Ihrer Distribution des bevorzugten Paket-Manager.</span><span class="sxs-lookup"><span data-stu-id="b9684-125">We strongly recommend regularly updating your package catalog, and upgrading your installed packages using your distro's preferred package manager.</span></span> <span data-ttu-id="b9684-126">Unter Debian/Ubuntu verwenden Sie apt:</span><span class="sxs-lookup"><span data-stu-id="b9684-126">On Debian/Ubuntu, you use apt:</span></span>

```bash
sudo apt update && sudo apt upgrade
```

> <span data-ttu-id="b9684-127">Windows nicht automatisch zu aktualisieren oder aktualisieren Sie Ihre Linux-Distro(s): Dies ist eine Aufgabe, die das Linux-Benutzer lieber selbst steuern.</span><span class="sxs-lookup"><span data-stu-id="b9684-127">Windows does not automatically update or upgrade your Linux distro(s): This is a task that the Linux users prefer to control themselves.</span></span>

<span data-ttu-id="b9684-128">Fertig!</span><span class="sxs-lookup"><span data-stu-id="b9684-128">You're done!</span></span> <span data-ttu-id="b9684-129">Nutzen Sie Ihre neue Linux-Distribution für WSL!</span><span class="sxs-lookup"><span data-stu-id="b9684-129">Enjoy using your new Linux distro on WSL!</span></span> <span data-ttu-id="b9684-130">Weitere Informationen zu WSL finden Sie in den anderen [WSL-Dokumentation](https://aka.ms/wsldocs), oder die [WSL Lernressourcenseite](https://aka.ms/learnwsl).</span><span class="sxs-lookup"><span data-stu-id="b9684-130">To learn more about WSL, review the other [WSL docs](https://aka.ms/wsldocs), or the [WSL learning resources page](https://aka.ms/learnwsl).</span></span>

![Profitieren Sie mit Linux in WSL](media/linux-on-wsl.png)

## <a name="troubleshooting"></a><span data-ttu-id="b9684-132">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="b9684-132">Troubleshooting</span></span>

<span data-ttu-id="b9684-133">Im folgenden finden Sie zugehörige Fehler und Vorschläge zur Behebung.</span><span class="sxs-lookup"><span data-stu-id="b9684-133">Below are related errors and suggested fixes.</span></span> <span data-ttu-id="b9684-134">Finden Sie in der [WSL Problembehandlungsseite](troubleshooting.md) andere häufig auftretende Fehler und ihre Lösungen.</span><span class="sxs-lookup"><span data-stu-id="b9684-134">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

> <span data-ttu-id="b9684-135">**Fehler bei der Installation Fehler 0x8007007e** dieser Fehler tritt auf, wenn es sich bei Ihrem System Linux aus dem Speicher nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9684-135">**Installation failed with error 0x8007007e** This error occurs when your system doesn't support Linux from the store.</span></span>  <span data-ttu-id="b9684-136">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="b9684-136">Make sure that:</span></span>
> * <span data-ttu-id="b9684-137">Sie können Windows Build 16215 oder höher ausführen.</span><span class="sxs-lookup"><span data-stu-id="b9684-137">You're running Windows build 16215 or later.</span></span> <span data-ttu-id="b9684-138">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="b9684-138">[Check your build](troubleshooting.md#check-your-build-number).</span></span>
> * <span data-ttu-id="b9684-139">Das Windows-Subsystem für Linux optionale Komponente aktiviert ist, und der Computer neu gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="b9684-139">The Windows Subsystem for Linux optional component is enabled and the computer has restarted.</span></span>  <span data-ttu-id="b9684-140">[WSL aktiviert](troubleshooting.md#confirm-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="b9684-140">[Make sure WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled).</span></span>
