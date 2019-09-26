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
# <a name="windows-subsystem-for-linux-for-enterprise"></a>Windows-Subsystem für Linux für Unternehmen

Die Microsoft Store für Unternehmen bietet verschiedene Lösungen für Unternehmen, die WSL in Ihrem Unternehmen bereitstellen möchten. Die [Online](https://docs.microsoft.com/en-us/microsoft-store/) Dokumentation für die Microsoft Store für Unternehmen ist eine großartige Ressource, um allgemeine Informationen über die Speichernutzung zu ermitteln.

Wenn Sie ein Unternehmen sind, das nur für die Bereitstellung von WSL eingerichtet werden soll, können Sie die folgenden Schritte ausführen, die in den Microsoft Store docs erläutert werden:

* [Registrieren Sie sich für die Microsoft Store für Unternehmen, und starten Sie](https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business-overview)
* [Verwalten Sie Ihre Produkte und Dienste (einschließlich der Benutzer, die auf die apps in Ihrem privaten Store zugreifen können)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview). Hier können Sie dem Store WSL-Distributionen hinzufügen und Steuern, wer Sie installieren kann.
* [Verwenden Sie eine Verteilungsmethode Ihrer Wahl, um die Software in Ihrem Unternehmen bereitzustellen.](https://docs.microsoft.com/en-us/microsoft-store/distribute-apps-to-your-employees-microsoft-store-for-business)
* Kommunizieren Sie mit Benutzern, die Zugriff auf WSL-Distributionen haben, dass Sie [diese Schritte](https://docs.microsoft.com/en-us/windows/wsl/install-win10) zum Installieren der Distribution oder der Distribution Ihrer Wahl verwenden können. 

## <a name="how-to-distribute-a-distro-offline"></a>So verteilen Sie eine Distribution offline

Wenn die Computer in Ihrem Unternehmen keinen Zugriff auf die Microsoft Store oder die Microsoft Store für Unternehmen haben, können Sie das Installationsprogramm einer Linux-Distribution mit einer Offline Lizenz herunterladen, indem Sie die folgenden Schritte ausführen. 

### <a name="set-up-an-azure-active-directory-ad-account"></a>Einrichten eines Azure Active Directory Kontos (AD) 

Sie müssen über ein Azure AD Konto verfügen und der globale Administrator für Ihre Organisation sein, um das Installationsprogramm für Microsoft Store-Apps zu erhalten. Wenn Sie bereits über ein Konto verfügen, können Sie diesen Schritt überspringen.

Die Anweisungen zum Registrieren eines Kontos finden Sie hier: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business

### <a name="sign-into-the-store-for-business-and-go-to-the-homepage"></a>Melden Sie sich beim Store für Unternehmen an, und wechseln Sie zur Homepage.
Melden Sie sich hier an: www.Microsoft.com/Business-Store

![MS Store für Unternehmen-Startseite](media/offlineinstallscreens/1-screen.png)

### <a name="go-to-manage-settings-and-enable-show-offline-apps"></a>Wechseln Sie zu Manage-> Settings, und aktivieren Sie "Offline-Apps anzeigen".

![Seite "Einstellungen" für MS Store für Unternehmen](media/offlineinstallscreens/2-screen.png)

### <a name="go-back-to-the-main-page-by-clicking-shop-for-my-group"></a>Wechseln Sie zurück zur Hauptseite, indem Sie auf "für meine Gruppe einkaufen" klicken.

![MS Store für Unternehmen-Startseite](media/offlineinstallscreens/1-screen.png)

### <a name="search-for-your-desired-distro-and-select-it"></a>Suchen Sie nach der gewünschten Distribution, und wählen Sie Sie aus.

![MS Store für Unternehmen-Startseite mit aktiver Suche](media/offlineinstallscreens/3-screen.png)

### <a name="select-an-offline-license-in-the-license-type-dropdown-menu-and-click-get-the-app"></a>Wählen Sie im Dropdown Menü "Lizenztyp" eine Offline Lizenz aus, und klicken Sie auf "APP herunter schalten".

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/4-screen.png)

Beachten Sie: einige Distributionen haben möglicherweise die Wahl, dass keine Offline Lizenz vorhanden ist.

### <a name="click-the-manage-button-to-get-to-the-apps-product-page"></a>Klicken Sie auf die Schaltfläche "verwalten", um zur Produktseite der APP zu gelangen.

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/5-screen.png)

### <a name="select-your-architecture-and-download-the-package-for-offline-use"></a>Auswählen der Architektur und Herunterladen des Pakets für die Offline Verwendung

![MS Store for Business-Ubuntu-Produktdetailseite](media/offlineinstallscreens/6-screen.png)

Dieser Installer kann dann an jeden Computer verteilt werden, auf dem Sie WSL installieren möchten.