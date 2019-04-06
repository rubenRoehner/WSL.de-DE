---
title: Windows-Subsystem für Linux für Unternehmen
description: Ressourcen und Anleitungen zum am besten verwenden das Windows-Subsystem für Linux in einer unternehmensumgebung.
keywords: Installieren Sie BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10, Enterprise, Bereitstellung, offline, Verpacken, Speicher, Verteilung, installation
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 09/04/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 9d867654d1b66fc14b58bc5e111986a7d38ef79c
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063278"
---
# <a name="windows-subsystem-for-linux-for-enterprise"></a><span data-ttu-id="5ddd7-104">Windows-Subsystem für Linux für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="5ddd7-104">Windows Subsystem for Linux for Enterprise</span></span>

<span data-ttu-id="5ddd7-105">Die Microsoft Store für Unternehmen bietet eine Vielzahl von Lösungen bis hin zu Unternehmen, die WSL in ihrem Unternehmen bereitstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-105">The Microsoft Store for Business offers a variety of solutions to Enterprises who want to deploy WSL to their company.</span></span> <span data-ttu-id="5ddd7-106">Die [Onlinedokumentation](https://docs.microsoft.com/en-us/microsoft-store/) für den Microsoft Store für Unternehmen sind eine hervorragende Ressource aus, um herauszufinden, allgemeine Informationen über die Store-Benutzeroberfläche.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-106">The [online docs](https://docs.microsoft.com/en-us/microsoft-store/) for the Microsoft Store for Business are a great resource to find out general information about the Store experience.</span></span>

<span data-ttu-id="5ddd7-107">Haben ein Unternehmen, die nur zum Abrufen oder Festlegen der sieht können Sie zum Starten der Bereitstellung von WSL Sie, folgendermaßen die innerhalb der Microsoft Store-Dokumentation erläutert werden:</span><span class="sxs-lookup"><span data-stu-id="5ddd7-107">If you’re a company that’s just looking to get set up to start deploying WSL you can follow these steps, which are explained inside of the Microsoft Store docs:</span></span>

* [<span data-ttu-id="5ddd7-108">Melden Sie sich für den Microsoft Store für Unternehmen und erste Schritte</span><span class="sxs-lookup"><span data-stu-id="5ddd7-108">Sign up for the Microsoft Store for Business and get started</span></span>](https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business-overview)
* <span data-ttu-id="5ddd7-109">[Verwalten Sie Ihre Produkte und Dienste (einschließlich, wer auf welche apps in Ihrem privaten Store zugreifen können)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span><span class="sxs-lookup"><span data-stu-id="5ddd7-109">[Manage your products and services (including who can access which apps in your private store)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span></span> <span data-ttu-id="5ddd7-110">Hier können Sie WSL-Distributionen auf Speicher und steuern, wer die Installation hinzufügen</span><span class="sxs-lookup"><span data-stu-id="5ddd7-110">Here you can add WSL distros to your store and control who can install them</span></span>
* [<span data-ttu-id="5ddd7-111">Verwenden Sie zum Bereitstellen der Software für Ihr Unternehmen eine Verteilungsmethode Ihrer Wahl</span><span class="sxs-lookup"><span data-stu-id="5ddd7-111">Use a distribution method of your choice to deploy the software to your company</span></span>](https://docs.microsoft.com/en-us/microsoft-store/distribute-apps-to-your-employees-microsoft-store-for-business)
* <span data-ttu-id="5ddd7-112">Kommunizieren Sie mit der Benutzer mit Zugriff auf die WSL-Distributionen, die Sie [verwenden Sie diese Schritte](https://docs.microsoft.com/en-us/windows/wsl/install-win10) , die Distribution oder die Distributionen ihrer Wahl installieren</span><span class="sxs-lookup"><span data-stu-id="5ddd7-112">Communicate to users who have access to WSL distros that they can [use these steps](https://docs.microsoft.com/en-us/windows/wsl/install-win10) to install the distro or distros of their choice</span></span> 

## <a name="how-to-distribute-a-distro-offline"></a><span data-ttu-id="5ddd7-113">Wie Sie eine Offline-Distribution zu verteilen.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-113">How to Distribute a Distro Offline</span></span>

<span data-ttu-id="5ddd7-114">Wenn die Computer in Ihrem Unternehmen Zugriff auf den Microsoft Store oder den Microsoft Store für Unternehmen haben, können Sie das Installationsprogramm aus, der eine Linux-Distribution herunterladen, die über eine offline-Lizenz verfügt, mit folgenden Schritten.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-114">If the computers in your company don’t have access to the Microsoft Store or the Microsoft Store for Business, then you can download the installer of a Linux distro that has an offline license by following these steps.</span></span> 

### <a name="set-up-an-azure-active-directory-ad-account"></a><span data-ttu-id="5ddd7-115">Richten Sie ein Konto für Azure Active Directory (AD)</span><span class="sxs-lookup"><span data-stu-id="5ddd7-115">Set up an Azure Active Directory (AD) Account</span></span> 

<span data-ttu-id="5ddd7-116">Sie müssen Azure AD-Kontos und der globale Administrator für Ihre Organisation, um das Installationsprogramm der Microsoft Store-apps zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-116">You need to have an Azure AD account and be the global administrator for your organization to get the installer of Microsoft Store apps.</span></span> <span data-ttu-id="5ddd7-117">Wenn Sie bereits über ein Konto verfügen, können Sie diesen Schritt überspringen.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-117">If you already have an account, you can skip this step.</span></span>

<span data-ttu-id="5ddd7-118">Die Anweisungen zum Registrieren eines Kontos finden Sie hier: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business</span><span class="sxs-lookup"><span data-stu-id="5ddd7-118">The instructions to register an account can be found here: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business</span></span>

### <a name="sign-into-the-store-for-business-and-go-to-the-homepage"></a><span data-ttu-id="5ddd7-119">Melden Sie sich den Store für Unternehmen, und rufen Sie die Startseite</span><span class="sxs-lookup"><span data-stu-id="5ddd7-119">Sign into the Store for Business and go to the homepage</span></span>
<span data-ttu-id="5ddd7-120">Melden Sie sich hier: www.microsoft.com/business-store</span><span class="sxs-lookup"><span data-stu-id="5ddd7-120">Sign in here: www.microsoft.com/business-store</span></span>

![MS Store für Unternehmen-Homepage](media/offlineinstallscreens/1-screen.png)

### <a name="go-to-manage-settings-and-enable-show-offline-apps"></a><span data-ttu-id="5ddd7-122">Wechseln Sie zum Verwalten >-Einstellungen, und aktivieren Sie "Show offline-apps"</span><span class="sxs-lookup"><span data-stu-id="5ddd7-122">Go to Manage->Settings and enable 'Show offline apps'</span></span>

![MS Store für Unternehmen-Seite "Einstellungen"](media/offlineinstallscreens/2-screen.png)

### <a name="go-back-to-the-main-page-by-clicking-shop-for-my-group"></a><span data-ttu-id="5ddd7-124">Wechseln Sie zur Hauptseite zurück, indem Sie auf "Kaufen Sie meine Gruppe"</span><span class="sxs-lookup"><span data-stu-id="5ddd7-124">Go back to the main page by clicking 'Shop for my group'</span></span>

![MS Store für Unternehmen-Homepage](media/offlineinstallscreens/1-screen.png)

### <a name="search-for-your-desired-distro-and-select-it"></a><span data-ttu-id="5ddd7-126">Suchen Sie nach Ihrer gewünschten Distribution, und wählen Sie Sie</span><span class="sxs-lookup"><span data-stu-id="5ddd7-126">Search for your desired distro and select it</span></span>

![MS Store für die geschäftliche Homepage mit active-Suche](media/offlineinstallscreens/3-screen.png)

### <a name="select-an-offline-license-in-the-license-type-dropdown-menu-and-click-get-the-app"></a><span data-ttu-id="5ddd7-128">Wählen Sie im Dropdownmenü Lizenz Typ eine Lizenz "Offline", und klicken Sie auf "App abrufen"</span><span class="sxs-lookup"><span data-stu-id="5ddd7-128">Select an ‘Offline’ license in the License type dropdown menu and click ‘Get the app’</span></span>

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/4-screen.png)

<span data-ttu-id="5ddd7-130">Bitte beachten Sie: Einige Distributionen können festlegen, ob es sich nicht um eine offline-Lizenz</span><span class="sxs-lookup"><span data-stu-id="5ddd7-130">Please note: some distros may elect not to have an offline license</span></span>

### <a name="click-the-manage-button-to-get-to-the-apps-product-page"></a><span data-ttu-id="5ddd7-131">Klicken Sie auf die Schaltfläche "Verwalten", um die app Seite mit den Produktdetails zu erhalten</span><span class="sxs-lookup"><span data-stu-id="5ddd7-131">Click the ‘Manage’ button to get to the app’s product page</span></span>

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/5-screen.png)

### <a name="select-your-architecture-and-download-the-package-for-offline-use"></a><span data-ttu-id="5ddd7-133">Wählen Sie die Architektur und herunterladen das Paket für die Offlineverwendung</span><span class="sxs-lookup"><span data-stu-id="5ddd7-133">Select your architecture and download the package for offline use</span></span>

![MS Store für Unternehmen Ubuntu Seite für Produktdetails](media/offlineinstallscreens/6-screen.png)

<span data-ttu-id="5ddd7-135">Dieses Installationsprogramm können Sie dann auf jedem Computer verteilt werden, in dem Sie WSL installieren möchten.</span><span class="sxs-lookup"><span data-stu-id="5ddd7-135">This installer can then be distributed to any computer where you would like to install WSL.</span></span>