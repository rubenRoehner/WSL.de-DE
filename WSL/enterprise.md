---
title: Windows-Subsystem für Linux für Unternehmen
description: Ressourcen und Anweisungen zur optimalen Verwendung des Windows-Subsystems für Linux in einer Unternehmensumgebung.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10, Enterprise, Bereitstellung, offline, Verpacken, speichern, Vertrieb, Installation, Installation
ms.date: 09/04/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: c32d62267c77d87fb200cfe43b8e6f43b4e3a56d
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269858"
---
# <a name="windows-subsystem-for-linux-for-enterprise"></a><span data-ttu-id="ea75e-104">Windows-Subsystem für Linux für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="ea75e-104">Windows Subsystem for Linux for Enterprise</span></span>

<span data-ttu-id="ea75e-105">Die Microsoft Store für Unternehmen bietet verschiedene Lösungen für Unternehmen, die WSL in Ihrem Unternehmen bereitstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="ea75e-105">The Microsoft Store for Business offers a variety of solutions to Enterprises who want to deploy WSL to their company.</span></span> <span data-ttu-id="ea75e-106">Die [Online](https://docs.microsoft.com/en-us/microsoft-store/) Dokumentation für die Microsoft Store für Unternehmen ist eine großartige Ressource, um allgemeine Informationen über die Speichernutzung zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="ea75e-106">The [online docs](https://docs.microsoft.com/en-us/microsoft-store/) for the Microsoft Store for Business are a great resource to find out general information about the Store experience.</span></span>

<span data-ttu-id="ea75e-107">Wenn Sie ein Unternehmen sind, das nur für die Bereitstellung von WSL eingerichtet werden soll, können Sie die folgenden Schritte ausführen, die in den Microsoft Store docs erläutert werden:</span><span class="sxs-lookup"><span data-stu-id="ea75e-107">If you’re a company that’s just looking to get set up to start deploying WSL you can follow these steps, which are explained inside of the Microsoft Store docs:</span></span>

* [<span data-ttu-id="ea75e-108">Registrieren Sie sich für die Microsoft Store für Unternehmen, und starten Sie</span><span class="sxs-lookup"><span data-stu-id="ea75e-108">Sign up for the Microsoft Store for Business and get started</span></span>](https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business-overview)
* <span data-ttu-id="ea75e-109">[Verwalten Sie Ihre Produkte und Dienste (einschließlich der Benutzer, die auf die apps in Ihrem privaten Store zugreifen können)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span><span class="sxs-lookup"><span data-stu-id="ea75e-109">[Manage your products and services (including who can access which apps in your private store)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview).</span></span> <span data-ttu-id="ea75e-110">Hier können Sie dem Store WSL-Distributionen hinzufügen und Steuern, wer Sie installieren kann.</span><span class="sxs-lookup"><span data-stu-id="ea75e-110">Here you can add WSL distros to your store and control who can install them</span></span>
* [<span data-ttu-id="ea75e-111">Verwenden Sie eine Verteilungsmethode Ihrer Wahl, um die Software in Ihrem Unternehmen bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="ea75e-111">Use a distribution method of your choice to deploy the software to your company</span></span>](https://docs.microsoft.com/en-us/microsoft-store/distribute-apps-to-your-employees-microsoft-store-for-business)
* <span data-ttu-id="ea75e-112">Kommunizieren Sie mit Benutzern, die Zugriff auf WSL-Distributionen haben, dass Sie [diese Schritte](https://docs.microsoft.com/en-us/windows/wsl/install-win10) zum Installieren der Distribution oder der Distribution Ihrer Wahl verwenden können.</span><span class="sxs-lookup"><span data-stu-id="ea75e-112">Communicate to users who have access to WSL distros that they can [use these steps](https://docs.microsoft.com/en-us/windows/wsl/install-win10) to install the distro or distros of their choice</span></span> 

## <a name="how-to-distribute-a-distro-offline"></a><span data-ttu-id="ea75e-113">So verteilen Sie eine Distribution offline</span><span class="sxs-lookup"><span data-stu-id="ea75e-113">How to Distribute a Distro Offline</span></span>

<span data-ttu-id="ea75e-114">Wenn die Computer in Ihrem Unternehmen keinen Zugriff auf die Microsoft Store oder die Microsoft Store für Unternehmen haben, können Sie das Installationsprogramm einer Linux-Distribution mit einer Offline Lizenz herunterladen, indem Sie die folgenden Schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="ea75e-114">If the computers in your company don’t have access to the Microsoft Store or the Microsoft Store for Business, then you can download the installer of a Linux distro that has an offline license by following these steps.</span></span> 

### <a name="set-up-an-azure-active-directory-ad-account"></a><span data-ttu-id="ea75e-115">Einrichten eines Azure Active Directory Kontos (AD)</span><span class="sxs-lookup"><span data-stu-id="ea75e-115">Set up an Azure Active Directory (AD) Account</span></span> 

<span data-ttu-id="ea75e-116">Sie müssen über ein Azure AD Konto verfügen und der globale Administrator für Ihre Organisation sein, um das Installationsprogramm für Microsoft Store-Apps zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ea75e-116">You need to have an Azure AD account and be the global administrator for your organization to get the installer of Microsoft Store apps.</span></span> <span data-ttu-id="ea75e-117">Wenn Sie bereits über ein Konto verfügen, können Sie diesen Schritt überspringen.</span><span class="sxs-lookup"><span data-stu-id="ea75e-117">If you already have an account, you can skip this step.</span></span>

<span data-ttu-id="ea75e-118">Die Anweisungen zum Registrieren eines Kontos finden Sie hier: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business</span><span class="sxs-lookup"><span data-stu-id="ea75e-118">The instructions to register an account can be found here: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business</span></span>

### <a name="sign-into-the-store-for-business-and-go-to-the-homepage"></a><span data-ttu-id="ea75e-119">Melden Sie sich beim Store für Unternehmen an, und wechseln Sie zur Homepage.</span><span class="sxs-lookup"><span data-stu-id="ea75e-119">Sign into the Store for Business and go to the homepage</span></span>
<span data-ttu-id="ea75e-120">Melden Sie sich hier an: www.Microsoft.com/Business-Store</span><span class="sxs-lookup"><span data-stu-id="ea75e-120">Sign in here: www.microsoft.com/business-store</span></span>

![MS Store für Unternehmen-Startseite](media/offlineinstallscreens/1-screen.png)

### <a name="go-to-manage-settings-and-enable-show-offline-apps"></a><span data-ttu-id="ea75e-122">Wechseln Sie zu Manage-> Settings, und aktivieren Sie "Offline-Apps anzeigen".</span><span class="sxs-lookup"><span data-stu-id="ea75e-122">Go to Manage->Settings and enable 'Show offline apps'</span></span>

![Seite "Einstellungen" für MS Store für Unternehmen](media/offlineinstallscreens/2-screen.png)

### <a name="go-back-to-the-main-page-by-clicking-shop-for-my-group"></a><span data-ttu-id="ea75e-124">Wechseln Sie zurück zur Hauptseite, indem Sie auf "für meine Gruppe einkaufen" klicken.</span><span class="sxs-lookup"><span data-stu-id="ea75e-124">Go back to the main page by clicking 'Shop for my group'</span></span>

![MS Store für Unternehmen-Startseite](media/offlineinstallscreens/1-screen.png)

### <a name="search-for-your-desired-distro-and-select-it"></a><span data-ttu-id="ea75e-126">Suchen Sie nach der gewünschten Distribution, und wählen Sie Sie aus.</span><span class="sxs-lookup"><span data-stu-id="ea75e-126">Search for your desired distro and select it</span></span>

![MS Store für Unternehmen-Startseite mit aktiver Suche](media/offlineinstallscreens/3-screen.png)

### <a name="select-an-offline-license-in-the-license-type-dropdown-menu-and-click-get-the-app"></a><span data-ttu-id="ea75e-128">Wählen Sie im Dropdown Menü "Lizenztyp" eine Offline Lizenz aus, und klicken Sie auf "APP herunter schalten".</span><span class="sxs-lookup"><span data-stu-id="ea75e-128">Select an ‘Offline’ license in the License type dropdown menu and click ‘Get the app’</span></span>

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/4-screen.png)

<span data-ttu-id="ea75e-130">Beachten Sie: einige Distributionen haben möglicherweise die Wahl, dass keine Offline Lizenz vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ea75e-130">Please note: some distros may elect not to have an offline license</span></span>

### <a name="click-the-manage-button-to-get-to-the-apps-product-page"></a><span data-ttu-id="ea75e-131">Klicken Sie auf die Schaltfläche "verwalten", um zur Produktseite der APP zu gelangen.</span><span class="sxs-lookup"><span data-stu-id="ea75e-131">Click the ‘Manage’ button to get to the app’s product page</span></span>

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/5-screen.png)

### <a name="select-your-architecture-and-download-the-package-for-offline-use"></a><span data-ttu-id="ea75e-133">Auswählen der Architektur und Herunterladen des Pakets für die Offline Verwendung</span><span class="sxs-lookup"><span data-stu-id="ea75e-133">Select your architecture and download the package for offline use</span></span>

![MS Store for Business-Ubuntu-Produktdetailseite](media/offlineinstallscreens/6-screen.png)

<span data-ttu-id="ea75e-135">Dieser Installer kann dann an jeden Computer verteilt werden, auf dem Sie WSL installieren möchten.</span><span class="sxs-lookup"><span data-stu-id="ea75e-135">This installer can then be distributed to any computer where you would like to install WSL.</span></span>