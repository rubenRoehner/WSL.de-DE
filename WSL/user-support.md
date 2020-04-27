---
title: Erstellen und Aktualisieren von Benutzerkonten für WSL-Verteilungen
description: Referenz für Benutzerkonten und Berechtigungsverwaltung mit dem Windows-Subsystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, user accounts
ms.date: 01/20/2020
ms.topic: article
ms.assetid: f70e685f-24c6-4908-9546-bf4f0291d8fd
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 30dea11adb68639f645ca800a695b0404661845a
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "76973680"
---
# <a name="create-and-update-user-accounts-for-wsl-distributions"></a><span data-ttu-id="60467-104">Erstellen und Aktualisieren von Benutzerkonten für WSL-Verteilungen</span><span class="sxs-lookup"><span data-stu-id="60467-104">Create and update user accounts for WSL distributions</span></span>

<span data-ttu-id="60467-105">Nachdem Sie WSL aktiviert und eine Linux-Verteilung aus dem Microsoft Store installiert haben, werden Sie beim Öffnen Ihrer neu installierten Linux-Verteilung zunächst aufgefordert, ein Konto zu erstellen, einschließlich **Benutzername** und **Kennwort**.</span><span class="sxs-lookup"><span data-stu-id="60467-105">Once you have enabled WSL and installed a Linux distribution from the Microsoft Store, the first step you will be asked to complete when opening your newly installed Linux distribution is to create an account, including a **User Name** and **Password**.</span></span>

- <span data-ttu-id="60467-106">Diese Kombination aus **Benutzername** und **Kennwort** ist spezifisch für Ihre Linux-Verteilung und hat keinen Einfluss auf Ihren Windows-Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="60467-106">This **User Name** and **Password** is specific to your Linux distribution and has no bearing on your Windows user name.</span></span>

- <span data-ttu-id="60467-107">Nachdem Sie den **Benutzernamen** und das **Kennwort** erstellt haben, ist das Konto Ihr Standardbenutzer für die Verteilung und wird beim Start automatisch angemeldet.</span><span class="sxs-lookup"><span data-stu-id="60467-107">Once you create this **User Name** and **Password**, the account will be your default user for the distribution and automatically sign-in on launch.</span></span>

- <span data-ttu-id="60467-108">Dieses Konto wird als Linux-Administrator angesehen, mit der Möglichkeit, administrative `sudo` (Super User Do)-Befehle auszuführen.</span><span class="sxs-lookup"><span data-stu-id="60467-108">This account will be considered the Linux administrator, with the ability to run `sudo` (Super User Do) administrative commands.</span></span>

- <span data-ttu-id="60467-109">Jede Linux-Distribution, die unter dem Windows-Subsystem für Linux ausgeführt wird, verfügt über eigene Linux-Benutzerkonten und -Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="60467-109">Each Linux distribution running on the Windows Subsystem for Linux has its own Linux user accounts and passwords.</span></span>  <span data-ttu-id="60467-110">Jedes Mail, wenn Sie eine Verteilung hinzufügen, erneut installieren oder zurücksetzen, müssen Sie ein Linux-Benutzerkonto konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="60467-110">You will have to configure a Linux user account every time you add a distribution, reinstall, or reset.</span></span>

## <a name="reset-your-linux-password"></a><span data-ttu-id="60467-111">Zurücksetzen Ihres Linux-Kennworts</span><span class="sxs-lookup"><span data-stu-id="60467-111">Reset your Linux password</span></span>

<span data-ttu-id="60467-112">Um Ihr Kennwort zu ändern, öffnen Sie Ihre Linux-Verteilung (z. B. Ubuntu), und geben Sie den Befehl `passwd` ein.</span><span class="sxs-lookup"><span data-stu-id="60467-112">To change your password, open your Linux distribution (Ubuntu for example) and enter the command: `passwd`</span></span>

<span data-ttu-id="60467-113">Sie werden aufgefordert, Ihr aktuelles Kennwort und Ihr neues Kennwort einzugeben und anschließend Ihr neues Kennwort zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="60467-113">You will be asked to enter your current password, then asked to enter your new password, and then to confirm your new password.</span></span>

### <a name="forgot-your-password"></a><span data-ttu-id="60467-114">Haben Sie Ihr Kennwort vergessen?</span><span class="sxs-lookup"><span data-stu-id="60467-114">Forgot your password</span></span>

<span data-ttu-id="60467-115">Wenn Sie das Kennwort für Ihre Linux-Verteilung vergessen haben:</span><span class="sxs-lookup"><span data-stu-id="60467-115">If you forgot the password for your Linux distribution:</span></span>

1. <span data-ttu-id="60467-116">Öffnen Sie PowerShell, und geben Sie mit dem Befehl `wsl -u root` das Stammverzeichnis Ihrer Standard-WSL-Verteilung ein.</span><span class="sxs-lookup"><span data-stu-id="60467-116">Open PowerShell and enter the root of your default WSL distribution using the command: `wsl -u root`</span></span>

> <span data-ttu-id="60467-117">Wenn Sie das vergessene Kennwort für eine Verteilung aktualisieren müssen, die nicht Ihre Standardverteilung ist, verwenden Sie den Befehl `wsl -d Debian -u root`, wobei Sie `Debian` durch den Namen Ihrer Zielverteilung ersetzen.</span><span class="sxs-lookup"><span data-stu-id="60467-117">If you need to update the forgotten password on a distribution that is not your default, use the command: `wsl -d Debian -u root`, replacing `Debian` with the name of your targeted distribution.</span></span>

2. <span data-ttu-id="60467-118">Sobald Ihre WSL-Verteilung auf der Root-Ebene innerhalb von PowerShell geöffnet wurde, können Sie den Befehl `passwd` verwenden, um Ihr Kennwort zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="60467-118">Once your WSL distribution has been opened at the root level inside PowerShell, you can use this command to update your password: `passwd`</span></span>

3. <span data-ttu-id="60467-119">Sie werden aufgefordert, ein neues UNIX-Kennwort einzugeben und dieses Kennwort anschließend zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="60467-119">You will be prompted to enter a new UNIX password and then confirm that password.</span></span> <span data-ttu-id="60467-120">Sobald Ihnen mitgeteilt wird, dass das Kennwort erfolgreich aktualisiert wurde, schließen Sie WSL in PowerShell mithilfe des Befehls `exit`.</span><span class="sxs-lookup"><span data-stu-id="60467-120">Once you're told that the password has updated successfully, close WSL inside of PowerShell using the command: `exit`</span></span>

> [!NOTE]
> <span data-ttu-id="60467-121">Wenn Sie eine frühe Version des Windows-Betriebssystems ausführen, wie z. B. 1703 (Creators Update) oder 1709 (Fall Creators Update), finden Sie weitere Informationen in der [Dokumentation zur archivierten Version dieses Benutzerkontoupdates](./user-support-archived.md).</span><span class="sxs-lookup"><span data-stu-id="60467-121">If you are running an early version of Windows operating system, like 1703 (Creators Update) or 1709 (Fall Creators Update), see the [archived version of this user account update doc](./user-support-archived.md).</span></span>
