---
title: Windows-Subsystem für Linux-Befehlsreferenz
description: Liste der Befehle, die das Windows-Subsystem für Linux verwalten
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, ubuntu
author: scooley
ms.author: scooley
ms.date: 07/31/2017
ms.topic: article
ms.assetid: 82908295-a6bd-483c-a995-613674c2677e
ms.custom: seodec18
ms.openlocfilehash: 978a35d593e37877949c24cbd833a519888d54bf
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063578"
---
# <a name="command-reference-for-windows-subsystem-for-linux"></a><span data-ttu-id="ef41a-104">Befehlsreferenz für Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="ef41a-104">Command Reference for Windows Subsystem for Linux</span></span>

> `lxrun.exe` <span data-ttu-id="ef41a-105">ist als veraltet markierte seit Windows 10-Version 1803 und höher.</span><span class="sxs-lookup"><span data-stu-id="ef41a-105">is deprecated as of Windows 10 1803 and later.</span></span>

<span data-ttu-id="ef41a-106">Der Befehl `lxrun.exe` kann verwendet werden, für die Interaktion mit der [Windows-Subsystem für Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) direkt.</span><span class="sxs-lookup"><span data-stu-id="ef41a-106">The command `lxrun.exe` can be used to interact with the [Windows Subsystem for Linux (WSL)](https://msdn.microsoft.com/en-us/commandline/wsl/faq#what-windows-subsystem-for-linux-wsl-) directly.</span></span>  <span data-ttu-id="ef41a-107">Diese Befehle werden installiert, in der `\Windows\System32` Verzeichnis und ggf. einer Windows-Eingabeaufforderung oder in PowerShell ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ef41a-107">These commands are installed into the `\Windows\System32` directory and may be run within a Windows command prompt or in PowerShell.</span></span>

* `lxrun.exe` <span data-ttu-id="ef41a-108">Dient zum Verwalten von WSL.</span><span class="sxs-lookup"><span data-stu-id="ef41a-108">is used to manage WSL.</span></span>  <span data-ttu-id="ef41a-109">Dieser Befehl kann zum Installieren oder deinstallieren das Ubuntu-Image verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ef41a-109">This command can be used to install or uninstall the Ubuntu image.</span></span>


| <span data-ttu-id="ef41a-110">Befehl</span><span class="sxs-lookup"><span data-stu-id="ef41a-110">Command</span></span>                     | <span data-ttu-id="ef41a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef41a-111">Description</span></span>                     |
|:----------------------------|:---------------------------|
| `bash`                      | <span data-ttu-id="ef41a-112">Startet die Bash-Shell im aktuellen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="ef41a-112">Launches the Bash shell in the current directory.</span></span>  <span data-ttu-id="ef41a-113">Wenn die Bash-Shell nicht automatisch installiert wird ausgeführt</span><span class="sxs-lookup"><span data-stu-id="ef41a-113">If the Bash shell is not installed automatically runs</span></span> `lxrun /install` |
| `bash ~`                    | <span data-ttu-id="ef41a-114">Startet die Bash-Shell in Ubuntu-Basisverzeichnis des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="ef41a-114">Launches the bash shell into the user's Ubuntu home directory.</span></span>  <span data-ttu-id="ef41a-115">Ähnlich wie beim Ausführen von cd ~</span><span class="sxs-lookup"><span data-stu-id="ef41a-115">Similar to running cd ~</span></span>            |
| `bash -c "<command>"`       | <span data-ttu-id="ef41a-116">Führt den Befehl und druckt die Ausgabe an der Eingabeaufforderung von Windows beendet wird.</span><span class="sxs-lookup"><span data-stu-id="ef41a-116">Runs the command, prints the output and exits back to the Windows command prompt.</span></span> <br/> <br/> <span data-ttu-id="ef41a-117">Beispiel: **bash -c "ls"**</span><span class="sxs-lookup"><span data-stu-id="ef41a-117">Example:  **bash -c "ls"**</span></span> |

<p>

| <span data-ttu-id="ef41a-118">Befehl</span><span class="sxs-lookup"><span data-stu-id="ef41a-118">Command</span></span>                     | <span data-ttu-id="ef41a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef41a-119">Description</span></span>                     |
|:----------------------------|:---------------------------|
| `lxrun`                     | <span data-ttu-id="ef41a-120">Der Befehl Lxrun wird verwendet, zum Verwalten der WSL-Instanz.</span><span class="sxs-lookup"><span data-stu-id="ef41a-120">The lxrun command is used to manage the WSL instance.</span></span> |
| `lxrun /install`            | <span data-ttu-id="ef41a-121">Der Download gestartet und die Installation.</span><span class="sxs-lookup"><span data-stu-id="ef41a-121">Starts the download and install process.</span></span> <br/> <span data-ttu-id="ef41a-122">**/ y** können hinzugefügt werden, um alle eingabeaufforderungen zu umgehen.</span><span class="sxs-lookup"><span data-stu-id="ef41a-122">**/y** may be added to bypass all prompts.</span></span>  <span data-ttu-id="ef41a-123">Die bestätigungsaufforderung wird automatisch akzeptiert, und der Standardbenutzer als Stamm festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ef41a-123">The confirmation prompt is automatically accepted and the default user is set to root.</span></span>          |
| `lxrun /uninstall`          | <span data-ttu-id="ef41a-124">Deinstalliert, und löscht das Ubuntu-Image.</span><span class="sxs-lookup"><span data-stu-id="ef41a-124">Uninstalls and deletes the Ubuntu image.</span></span>  <span data-ttu-id="ef41a-125">Standardmäßig wird dadurch nicht die Ubuntu-Basisverzeichnis des Benutzers entfernt.</span><span class="sxs-lookup"><span data-stu-id="ef41a-125">By default this does not remove the user's Ubuntu home directory.</span></span> <br/> <span data-ttu-id="ef41a-126">**/ y** können hinzugefügt werden, um automatisch die bestätigungsaufforderung akzeptieren</span><span class="sxs-lookup"><span data-stu-id="ef41a-126">**/y** may be added to automatically accept the confirmation prompt</span></span> <br/><span data-ttu-id="ef41a-127">**/ vollständiges** deinstalliert, und löscht die Ubuntu-Basisverzeichnis des Benutzers</span><span class="sxs-lookup"><span data-stu-id="ef41a-127">**/full** uninstalls and deletes the user's Ubuntu home directory</span></span>         |
| `lxrun /setdefaultuser <userName>`     | <span data-ttu-id="ef41a-128">Die Standardeinstellung Bash festgelegt auf Ubuntu-Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ef41a-128">Sets the default Bash on Ubuntu user.</span></span> <span data-ttu-id="ef41a-129">Wird für ein Kennwort angefordert werden, wenn der angegebene Benutzer nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ef41a-129">Will prompt for a password if the specified user does not exist.</span></span>  <span data-ttu-id="ef41a-130">Weitere Informationen finden Sie unter: https://aka.ms/wslusers.</span><span class="sxs-lookup"><span data-stu-id="ef41a-130">For more information visit: https://aka.ms/wslusers.</span></span> <br/> <span data-ttu-id="ef41a-131">**/ y** umgehungen Promping für das Kennwort.</span><span class="sxs-lookup"><span data-stu-id="ef41a-131">**/y** Bypasses promping for the password.</span></span>  <span data-ttu-id="ef41a-132">Ohne Angabe eines Kennworts wird der Benutzer erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="ef41a-132">The user will be created without a password.</span></span>|
| `lxrun /update`            | <span data-ttu-id="ef41a-133">Aktualisiert das Subsystem des Paket-index</span><span class="sxs-lookup"><span data-stu-id="ef41a-133">Updates the subsystem's package index</span></span>          |
