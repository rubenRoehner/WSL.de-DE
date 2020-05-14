---
title: Windows-Subsystem für Linux für Unternehmen
description: Ressourcen und Anweisungen zur optimalen Verwendung des Windows-Subsystems für Linux in einer Unternehmensumgebung.
keywords: BashOnWindows, Bash, WSL, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Unternehmen, Bereitstellung, offline, Paket, Store, Verteilung, Installation, installieren
ms.date: 05/15/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: 02f4ff41614f78c0e588f329c777a87f8b416233
ms.sourcegitcommit: 3fb40fd65b34a5eb26b213a0df6a3b2746b7a9b4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2020
ms.locfileid: "83235831"
---
# <a name="set-up-windows-subsystem-for-linux-for-your-enterprise-company"></a><span data-ttu-id="57be2-104">Einrichten des Windows-Subsystems für Linux für Ihr Unternehmen</span><span class="sxs-lookup"><span data-stu-id="57be2-104">Set up Windows Subsystem for Linux for your enterprise company</span></span>

<span data-ttu-id="57be2-105">Der Microsoft Store für Unternehmen bietet verschiedene Unternehmenslösungen, die WSL in Ihrem Unternehmen bereitstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="57be2-105">The Microsoft Store for Business offers a variety of solutions to Enterprises who want to deploy WSL to their company.</span></span> <span data-ttu-id="57be2-106">Die [Dokumentation im Microsoft Store für Unternehmen und Bildungseinrichtungen](https://docs.microsoft.com/microsoft-store/) stellt eine gute Ressource für allgemeine Informationen über die Store-Benutzeroberfläche dar.</span><span class="sxs-lookup"><span data-stu-id="57be2-106">The [Microsoft Store for Business and Education docs](https://docs.microsoft.com/microsoft-store/) are a great resource to find out general information about the Store experience.</span></span>

<span data-ttu-id="57be2-107">Als Unternehmen, das nur sein System für die Bereitstellung von WSL einrichten möchte, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="57be2-107">If you're a company that's just looking to get set up to start deploying WSL, follow these steps:</span></span>

* <span data-ttu-id="57be2-108">[Registrieren für Microsoft Store für Unternehmen und erste Schritte](https://docs.microsoft.com/microsoft-store/sign-up-microsoft-store-for-business-overview).</span><span class="sxs-lookup"><span data-stu-id="57be2-108">[Sign up for the Microsoft Store for Business and get started](https://docs.microsoft.com/microsoft-store/sign-up-microsoft-store-for-business-overview)</span></span>
* <span data-ttu-id="57be2-109">[Verwalten Sie Ihre Produkte und Dienste (einschließlich der Benutzer, die auf die Apps in Ihrem privaten Store zugreifen können)](https://docs.microsoft.com/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span><span class="sxs-lookup"><span data-stu-id="57be2-109">[Manage your products and services (including who can access which apps in your private store)](https://docs.microsoft.com/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span></span> <span data-ttu-id="57be2-110">Hier können Sie Ihrem Store WSL-Verteilungen hinzufügen und steuern, wer diese installieren kann.</span><span class="sxs-lookup"><span data-stu-id="57be2-110">Here you can add WSL distros to your store and control who can install them</span></span>
* [<span data-ttu-id="57be2-111">Verwenden einer Verteilungsmethode Ihrer Wahl, um die Software in Ihrem Unternehmen bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="57be2-111">Use a distribution method of your choice to deploy the software to your company</span></span>](https://docs.microsoft.com/microsoft-store/distribute-apps-to-your-employees-microsoft-store-for-business)
* <span data-ttu-id="57be2-112">Informieren Sie die Mitarbeiter Ihres Unternehmens, dass sie diesen Dokumentationslink zum Installieren von WSL verwenden können: [Installieren des Windows-Subsystems für Linux](./install-win10.md)</span><span class="sxs-lookup"><span data-stu-id="57be2-112">Communicate to the employees of your company that they can use this documentation link to install WSL: [Install the Windows Subsystem for Linux](./install-win10.md)</span></span>

## <a name="how-to-distribute-a-linux-distribution-on-windows-offline"></a><span data-ttu-id="57be2-113">Offlineverteilen einer Linux-Verteilung unter Windows</span><span class="sxs-lookup"><span data-stu-id="57be2-113">How to distribute a Linux distribution on Windows offline</span></span>

<span data-ttu-id="57be2-114">Wenn die Computer in Ihrem Unternehmen keinen Zugriff auf den Microsoft Store oder den Microsoft Store für Unternehmen haben, können Sie das Installationsprogramm einer Linux-Verteilung mit einer Offline Lizenz herunterladen, indem Sie die folgenden Schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="57be2-114">If the computers in your company don't have access to the Microsoft Store or the Microsoft Store for Business, then you can download the installer of a Linux distribution that has an offline license by following these steps.</span></span>

### <a name="set-up-an-azure-active-directory-account"></a><span data-ttu-id="57be2-115">Einrichten eines Azure Active Directory-Kontos</span><span class="sxs-lookup"><span data-stu-id="57be2-115">Set up an Azure Active Directory account</span></span>

<span data-ttu-id="57be2-116">Sie müssen sich [für ein Azure AD-Konto registrieren](https://docs.microsoft.com/azure/active-directory/fundamentals/sign-up-organization?WT.mc_id=windows-c9-niner) und der globale Administrator für Ihre Organisation sein, um das Installationsprogramm für Microsoft Store-Apps zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="57be2-116">You need to [sign up for an Azure AD account](https://docs.microsoft.com/azure/active-directory/fundamentals/sign-up-organization?WT.mc_id=windows-c9-niner) and be the global administrator for your organization to get the installer of Microsoft Store apps.</span></span> <span data-ttu-id="57be2-117">Wenn Sie bereits ein Konto haben, können Sie diesen Schritt überspringen.</span><span class="sxs-lookup"><span data-stu-id="57be2-117">If you already have an account, you can skip this step.</span></span>

### <a name="set-up-wsl-using-your-microsoft-store-for-business-account"></a><span data-ttu-id="57be2-118">Einrichten von WSL mithilfe Ihres Microsoft Store für Unternehmen-Kontos</span><span class="sxs-lookup"><span data-stu-id="57be2-118">Set up WSL using your Microsoft Store for Business account</span></span>

<span data-ttu-id="57be2-119">Die Anweisungen zum Registrieren eines Kontos finden Sie hier: https://docs.microsoft.com/microsoft-store/sign-up-microsoft-store-for-business</span><span class="sxs-lookup"><span data-stu-id="57be2-119">The instructions to register an account are found here: https://docs.microsoft.com/microsoft-store/sign-up-microsoft-store-for-business</span></span>

1. <span data-ttu-id="57be2-120">Melden Sie sich beim Store für Unternehmen an, und wechseln Sie zur Startseite: https://www.microsoft.com/business-store</span><span class="sxs-lookup"><span data-stu-id="57be2-120">Sign into the Store for Business and go to the homepage: https://www.microsoft.com/business-store</span></span>

    ![Microsoft Store für Unternehmen – Startseite](media/offlineinstallscreens/1-screen.png)

2. <span data-ttu-id="57be2-122">Wechseln Sie zu „Verwalten“ > „Einstellungen“, und aktivieren Sie „Offline-Apps anzeigen“.</span><span class="sxs-lookup"><span data-stu-id="57be2-122">Go to Manage > Settings and enable 'Show offline apps'.</span></span>

    ![Seite mit den Einstellungen für den Microsoft Store für Unternehmen](media/offlineinstallscreens/2-screen.png)

3. <span data-ttu-id="57be2-124">Wechseln Sie zurück zur Hauptseite, indem Sie „Für meine Gruppe einkaufen“ auswählen.</span><span class="sxs-lookup"><span data-stu-id="57be2-124">Go back to the main page by selecting 'Shop for my group'.</span></span>

    ![Microsoft Store für Unternehmen – Startseite](media/offlineinstallscreens/1-screen.png)

4. <span data-ttu-id="57be2-126">Suchen Sie nach der gewünschten Verteilung, und wählen Sie sie aus.</span><span class="sxs-lookup"><span data-stu-id="57be2-126">Search for your desired distribution and select it.</span></span>

    ![Microsoft Store für Unternehmen – Startseite mit aktiver Suche](media/offlineinstallscreens/3-screen.png)

5. <span data-ttu-id="57be2-128">Wählen Sie im Dropdownmenü „Lizenztyp“ eine Offlinelizenz und dann „App abrufen“ aus.</span><span class="sxs-lookup"><span data-stu-id="57be2-128">Select an 'Offline' license in the License type dropdown menu and select 'Get the app'.</span></span> <span data-ttu-id="57be2-129">(Einige Linux-Verteilungen bieten möglicherweise keine Offlinelizenzen.)</span><span class="sxs-lookup"><span data-stu-id="57be2-129">(Some Linux distributions may elect not to provide an offline license).</span></span>

    ![Microsoft Store für Unternehmen – Ubuntu-Produktseite](media/offlineinstallscreens/4-screen.png)

6. <span data-ttu-id="57be2-131">Wählen Sie die Schaltfläche „Verwalten“ aus, um zur Produktseite der App zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="57be2-131">Select the 'Manage' button to get to the app's product page.</span></span>

    ![Microsoft Store für Unternehmen – Ubuntu-Produktseite](media/offlineinstallscreens/5-screen.png)

7. <span data-ttu-id="57be2-133">Wählen Sie Ihre Architektur aus, und laden Sie das Paket zur Offlineverwendung herunter.</span><span class="sxs-lookup"><span data-stu-id="57be2-133">Select your architecture and download the package for offline use.</span></span>

    ![Microsoft Store für Unternehmen – Seite der Ubuntu-Produktdetails](media/offlineinstallscreens/6-screen.png)

<span data-ttu-id="57be2-135">Dieses Installationsprogramm kann dann an jeden Computer verteilt werden, auf dem Sie WSL installieren möchten.</span><span class="sxs-lookup"><span data-stu-id="57be2-135">This installer can then be distributed to any computer where you would like to install WSL.</span></span>
