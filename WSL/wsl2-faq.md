---
title: WSL 2 – häufig gestellte Fragen
description: Häufig gestellte Fragen zum Windows-Subsystem für Linux 2
keywords: Installieren Sie BashOnWindows, Bash, Wsl, wsl2, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 84805278abaeb6334c662e1dfab1bced3e0ddb0b
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67038090"
---
# <a name="wsl-2-faq"></a>WSL 2 FAQ

Im folgenden finden eine Liste mit häufig gestellten Fragen (FAQ) zum Windows-Subsystem für Linux 2 ein.

## <a name="does-wsl-2-use-hyper-v-will-it-be-available-on-windows-10-home"></a>Werden WSL 2 wird Hyper-V verwendet? Ist es auf Windows 10 Home erhältlich?

WSL 2 werden auf alle SKUs verfügbar, in denen WSL derzeit verfügbar ist, einschließlich Windows 10 Home.

Die neueste Version von WSL verwendet Hyper-V-Architektur, um Virtualisierung zu aktivieren. Diese Architektur wird in eine optionale Komponente verfügbar sein, die eine Teilmenge der Hyper-V-Funktion. Diese optionale Komponente wird auf alle SKUs verfügbar sein. Sie erwarten können hier erfahren mehr über diese Benutzeroberfläche schnell, wie wir näher auf die WSL-2-Version erhalten.

## <a name="what-will-happen-to-wsl-1-will-it-be-abandoned"></a>Was geschieht mit WSL 1? Wird sie werden verworfen?

Wir stellen Ihnen derzeit keine Pläne WSL 1 als veraltet markiert. Sie können WSL-1 und 2 von WSL Distributionen nebeneinander ausgeführt und können Upgrades bzw. Downgrades-Distribution, die alle zu einem beliebigen Zeitpunkt. Hinzufügen von WSL 2 als eine neue Architektur bietet eine bessere Plattform für das Team WSL um bereitzustellen, die WSL eine fantastische Möglichkeit zum Ausführen von einer Linux-Umgebung in Windows machen.

## <a name="will-i-be-able-to-run-wsl-2-and-other-3rd-party-virtualization-tools-such-as-vmware-or-virtualbox"></a>Werden WSL-2 und andere 3rd Party Virtualisierungstools z. B. VMware, VirtualBox oder ausgeführt?

Einige 3rd Party-Anwendungen funktioniert nicht, wenn Hyper-V verwendet, wird dies bedeutet, dass sie nicht werden ausgeführt, wenn die WSL 2 aktiviert ist. Dies schließt leider ein VMware und Versionen von VirtualBox vor VirtualBox-6 (VirtualBox 6.0.0 veröffentlicht im Dezember 2018 [unterstützt nun Hyper-V als einen Kern fallback Ausführung auf einem Windows-Host] [ 1]!)

Wir untersuchen Methoden, um dieses Problem zu beheben. Z. B. machen wir eine Reihe von APIs, die aufgerufen [Hypervisorplattform] [ 2] , Anbieter von Drittanbietern verwenden können, um ihre Software mit Hyper-V kompatibel zu machen Dies ermöglicht es Anwendungen, die die Hyper-V-Architektur für die Netzwerkemulation verwenden, z. B. [der Google Android Emulator][3], und VirtualBox, 6 und höher die jetzt mit Hyper-V kompatibel sind.

## <a name="can-i-access-the-gpu-in-wsl-2-are-there-plans-to-increase-hardware-support"></a>Kann ich die GPU in WSL 2 zugreifen? Gibt es Pläne, um die Hardware-Unterstützung zu erhöhen?

In der ursprünglichen Version von WSL 2 Hardwarezugriff Unterstützung ist beschränkt, z.B.: Sie werden nicht den Zugriff der GPU, serielle oder USB sehr. Hinzufügen von Unterstützung für bessere Geräte ist jedoch in unserem Backlog, hoch, wie viele weitere Anwendungsfälle für Entwickler wird geöffnet, die mit diesen Geräten interagieren möchten. In der Zwischenzeit können Sie immer WSL 1 verwenden, an der seriellen Anschluss und USB-Zugriff verfügt. Sie bleiben auf dem laufenden, die für diesen Blog und WSL-Teammitglieder auf Twitter, um über die neuesten Funktionen für Insider informiert zu bleiben erstellt und wenden Sie sich an uns Feedback für welche Geräte Sie interagieren möchten!

## <a name="will-wsl-2-be-able-to-use-networking-applications"></a>Wird WSL 2 netzwerkanwendungen verwenden kann?

Ja, im Allgemeinen netzwerkanwendungen wird schneller und besser funktionieren, da wir die vollständige systemüberprüfung Kompatibilität aufgerufen haben. Allerdings verwendet die neue Architektur virtualisierte Netzwerkkomponenten. Verhält sich das heißt, die in der ersten Vorschau WSL 2 baut auf ähnliche Weise mehr an einen virtuellen Computer, z.B.: WSL 2 müssen eine andere IP-Adresse als der Hostcomputer. Wir haben sich verpflichtet, wodurch WSL 2 können Sie die WSL 1 identisch, und enthält unsere Netzwerke Geschichte zu verbessern. Wir erwarten, dass Verbesserungen so schnell wie möglich, z. B. Zugriff auf alle Netzwerke apps unter Linux oder Windows mithilfe von "localhost", werden hinzufügen. Wir veröffentlichen werden weitere Details zu unserem Netzwerk Story und Verbesserungen, wie wir die Veröffentlichung von WSL-2-Ansatz.

## <a name="can-i-run-wsl-2-in-a-virtual-machine"></a>Kann ich WSL 2 auf einem virtuellen Computer ausführen?

Ja! Sie müssen sicherstellen, dass die virtuelle Maschine Virtualisierung aktiviert geschachtelte werden. Dies kann in Hyper-V aktiviert werden, durch den folgenden Befehl in einem PowerShell-Fenster mit Administratorrechten ausführen:

`Set-VMProcessor -VMName <VMName> -ExposeVirtualizationExtensions $true`

Achten Sie darauf, ersetzen Sie "&lt;VMName&gt;" mit dem Namen des virtuellen Computers.

 [1]: https://www.virtualbox.org/wiki/Changelog-6.0
 [2]: https://docs.microsoft.com/en-us/virtualization/api/
 [3]: https://devblogs.microsoft.com/visualstudio/hyper-v-android-emulator-support/