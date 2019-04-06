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
# <a name="windows-subsystem-for-linux-for-enterprise"></a>Windows-Subsystem für Linux für Unternehmen

Die Microsoft Store für Unternehmen bietet eine Vielzahl von Lösungen bis hin zu Unternehmen, die WSL in ihrem Unternehmen bereitstellen möchten. Die [Onlinedokumentation](https://docs.microsoft.com/en-us/microsoft-store/) für den Microsoft Store für Unternehmen sind eine hervorragende Ressource aus, um herauszufinden, allgemeine Informationen über die Store-Benutzeroberfläche.

Haben ein Unternehmen, die nur zum Abrufen oder Festlegen der sieht können Sie zum Starten der Bereitstellung von WSL Sie, folgendermaßen die innerhalb der Microsoft Store-Dokumentation erläutert werden:

* [Melden Sie sich für den Microsoft Store für Unternehmen und erste Schritte](https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business-overview)
* [Verwalten Sie Ihre Produkte und Dienste (einschließlich, wer auf welche apps in Ihrem privaten Store zugreifen können)](https://docs.microsoft.com/en-us/microsoft-store/manage-apps-microsoft-store-for-business-overview). Hier können Sie WSL-Distributionen auf Speicher und steuern, wer die Installation hinzufügen
* [Verwenden Sie zum Bereitstellen der Software für Ihr Unternehmen eine Verteilungsmethode Ihrer Wahl](https://docs.microsoft.com/en-us/microsoft-store/distribute-apps-to-your-employees-microsoft-store-for-business)
* Kommunizieren Sie mit der Benutzer mit Zugriff auf die WSL-Distributionen, die Sie [verwenden Sie diese Schritte](https://docs.microsoft.com/en-us/windows/wsl/install-win10) , die Distribution oder die Distributionen ihrer Wahl installieren 

## <a name="how-to-distribute-a-distro-offline"></a>Wie Sie eine Offline-Distribution zu verteilen.

Wenn die Computer in Ihrem Unternehmen Zugriff auf den Microsoft Store oder den Microsoft Store für Unternehmen haben, können Sie das Installationsprogramm aus, der eine Linux-Distribution herunterladen, die über eine offline-Lizenz verfügt, mit folgenden Schritten. 

### <a name="set-up-an-azure-active-directory-ad-account"></a>Richten Sie ein Konto für Azure Active Directory (AD) 

Sie müssen Azure AD-Kontos und der globale Administrator für Ihre Organisation, um das Installationsprogramm der Microsoft Store-apps zu erhalten. Wenn Sie bereits über ein Konto verfügen, können Sie diesen Schritt überspringen.

Die Anweisungen zum Registrieren eines Kontos finden Sie hier: https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business

### <a name="sign-into-the-store-for-business-and-go-to-the-homepage"></a>Melden Sie sich den Store für Unternehmen, und rufen Sie die Startseite
Melden Sie sich hier: www.microsoft.com/business-store

![MS Store für Unternehmen-Homepage](media/offlineinstallscreens/1-screen.png)

### <a name="go-to-manage-settings-and-enable-show-offline-apps"></a>Wechseln Sie zum Verwalten >-Einstellungen, und aktivieren Sie "Show offline-apps"

![MS Store für Unternehmen-Seite "Einstellungen"](media/offlineinstallscreens/2-screen.png)

### <a name="go-back-to-the-main-page-by-clicking-shop-for-my-group"></a>Wechseln Sie zur Hauptseite zurück, indem Sie auf "Kaufen Sie meine Gruppe"

![MS Store für Unternehmen-Homepage](media/offlineinstallscreens/1-screen.png)

### <a name="search-for-your-desired-distro-and-select-it"></a>Suchen Sie nach Ihrer gewünschten Distribution, und wählen Sie Sie

![MS Store für die geschäftliche Homepage mit active-Suche](media/offlineinstallscreens/3-screen.png)

### <a name="select-an-offline-license-in-the-license-type-dropdown-menu-and-click-get-the-app"></a>Wählen Sie im Dropdownmenü Lizenz Typ eine Lizenz "Offline", und klicken Sie auf "App abrufen"

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/4-screen.png)

Bitte beachten Sie: Einige Distributionen können festlegen, ob es sich nicht um eine offline-Lizenz

### <a name="click-the-manage-button-to-get-to-the-apps-product-page"></a>Klicken Sie auf die Schaltfläche "Verwalten", um die app Seite mit den Produktdetails zu erhalten

![MS Store für Unternehmen-Ubuntu-Produktseite](media/offlineinstallscreens/5-screen.png)

### <a name="select-your-architecture-and-download-the-package-for-offline-use"></a>Wählen Sie die Architektur und herunterladen das Paket für die Offlineverwendung

![MS Store für Unternehmen Ubuntu Seite für Produktdetails](media/offlineinstallscreens/6-screen.png)

Dieses Installationsprogramm können Sie dann auf jedem Computer verteilt werden, in dem Sie WSL installieren möchten.