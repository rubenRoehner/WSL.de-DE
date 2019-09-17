---
title: Häufig gestellte Fragen zu WSL 2
description: Häufig gestellte Fragen zum Windows-Subsystem für Linux 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
author: craigloewen-msft
ms.author: crloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: ea6a1e4fc813ec80393a0c4e2beb89e9a40fb68e
ms.sourcegitcommit: ed5cf72d5ceb92edd50cf9260ac31fd4d95a02c8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/16/2019
ms.locfileid: "71020926"
---
# <a name="wsl-2-faq"></a>FAQ ZU WSL 2

Im folgenden finden Sie eine Liste mit häufig gestellten Fragen (FAQ) zum Windows-Subsystem für Linux 2.

## <a name="does-wsl-2-use-hyper-v-will-it-be-available-on-windows-10-home"></a>Verwendet WSL 2 Hyper-V? Ist es unter Windows 10 Home verfügbar?

WSL 2 steht für alle SKUs zur Verfügung, auf denen zurzeit WSL verfügbar ist, einschließlich Windows 10 Home.

Die neueste Version von WSL verwendet die Hyper-V-Architektur, um die Virtualisierung zu ermöglichen. Diese Architektur wird in der optionalen Komponente "VM Platform" verfügbar sein. Diese optionale Komponente ist für alle SKUs verfügbar. Sie können erwarten, dass Sie weitere Details zu dieser Umgebung sehen, sobald wir die Version von WSL 2 näher betrachten.

## <a name="what-will-happen-to-wsl-1-will-it-be-abandoned"></a>Was geschieht mit WSL 1? Wird der Vorgang abgebrochen?

Es ist zurzeit nicht geplant, WSL 1 als veraltet zu kennzeichnen. Sie können WSL 1 und WSL 2-Distributionen nebeneinander ausführen und jederzeit ein Upgrade und Downgrade für jede Distribution durchführen. Das Hinzufügen von WSL 2 als neue Architektur bietet dem WSL-Team eine bessere Plattform zum Bereitstellen von Features, die WSL eine beeindruckende Möglichkeit zum Ausführen einer Linux-Umgebung in Windows darstellen.

## <a name="will-i-be-able-to-run-wsl-2-and-other-3rd-party-virtualization-tools-such-as-vmware-or-virtualbox"></a>Kann ich WSL 2 und andere Virtualisierungstools von Drittanbietern, z. b. VMware oder VirtualBox, ausführen?

Einige Anwendungen von Drittanbietern können nicht funktionieren, wenn Hyper-V verwendet wird. Dies bedeutet, dass Sie nicht ausgeführt werden können, wenn WSL 2 aktiviert ist. Leider umfasst dies VMware und Versionen von VirtualBox vor VirtualBox 6 (VirtualBox 6.0.0, die im Dezember 2018 veröffentlicht wurde, [unterstützt nun Hyper-V als Fall Back Ausführungs Kern auf einem Windows-Host][1]!)

Wir untersuchen Möglichkeiten, dieses Problem zu beheben. Wir stellen beispielsweise einen Satz von APIs namens [Hypervisor Platform][2] zur Verfügung, mit denen Drittanbieter-Virtualisierungsanbieter Ihre Software mit Hyper-V kompatibel machen können. Dies ermöglicht es Anwendungen, die Hyper-v-Architektur für Ihre Emulation zu verwenden, wie z. b. [Google Android-Emulator][3]und VirtualBox 6 und höher, die beide jetzt mit Hyper-v kompatibel sind.

## <a name="can-i-access-the-gpu-in-wsl-2-are-there-plans-to-increase-hardware-support"></a>Kann ich auf die GPU in WSL 2 zugreifen? Gibt es Pläne, den Hardware Support zu erhöhen?

In den ersten Releases des WSL 2 ist die Hardwarezugriffsunterstützung eingeschränkt. Sie können z. B. nicht auf die GPU, die serielle Schnittstelle oder die USB-Schnittstelle zugreifen. Das Hinzufügen verbesserter Geräteunterstützung steht jedoch in unserem Backlog ganz oben, da sich dadurch viele weitere Anwendungsfälle für Entwickler eröffnen, die mit diesen Geräten interagieren möchten. In der Zwischenzeit können Sie weiterhin das WSL 1 verwenden, das einen seriellen Anschluss und USB-Zugriff bietet. Verfolgen Sie diesen Blog, und folgen Sie den Mitgliedern des WSL-Teams auf Twitter, um sich über die neuesten Features von Insider-Builds zu informieren und uns mitzuteilen, mit welchen Geräten Sie interagieren möchten.

## <a name="will-wsl-2-be-able-to-use-networking-applications"></a>Kann WSL 2 Netzwerkanwendungen verwenden?

Ja, in der Regel sind Netzwerkanwendungen schneller und können besser funktionieren, da wir eine vollständige System aufrufskompatibilität haben. Die neue Architektur verwendet jedoch virtualisierte Netzwerkkomponenten. Dies bedeutet, dass sich WSL 2 in der ersten Vorschau ähnlich wie ein virtueller Computer verhält, z. b.: WSL 2 hat eine andere IP-Adresse als der Host Computer. Wir sind bestrebt, das Aussehen von WSL 2 mit WSL 1 und das verbessern unserer Netzwerk Geschichte zu vereinfachen. Wir erwarten, dass Sie Verbesserungen so schnell wie möglich hinzufügen, z. b. durch den Zugriff auf alle Netzwerk-apps unter Linux oder Windows mithilfe von localhost. Wir werden weitere Details über unsere Netzwerk Geschichte und Verbesserungen veröffentlichen, wenn wir uns mit der Veröffentlichung von WSL 2 in Verbindung treten.

## <a name="can-i-run-wsl-2-in-a-virtual-machine"></a>Kann ich WSL 2 auf einem virtuellen Computer ausführen?

Ja! Sie müssen sicherstellen, dass die aktivierte aktivierte Virtualisierung auf dem virtuellen Computer aktiviert ist. Dies kann in ihrem übergeordneten Hyper-V-Host aktiviert werden, indem Sie den folgenden Befehl in einem PowerShell-Fenster mit Administrator Rechten ausführen:

`Set-VMProcessor -VMName <VMName> -ExposeVirtualizationExtensions $true`

Stellen Sie sicher, dass&lt;Sie "&gt;VMName" durch den Namen des virtuellen Computers ersetzen.

## <a name="can-i-use-wslconf-in-wsl-2"></a>Kann ich WSL. conf in WSL 2 verwenden?

WSL 2 unterstützt dieselbe WSL. conf-Datei, die von WSL 1 verwendet wird. Dies bedeutet, dass alle Konfigurationsoptionen, die Sie in einer WSL 1-Distribution festgelegt haben, z. b. das Automatisieren von Windows-Laufwerken, das Aktivieren oder Deaktivieren von Interop, das Ändern des Verzeichnisses, in dem Windows-Laufwerke bereitgestellt werden, in WSL 2 funktionieren. Weitere Informationen zu den Konfigurationsoptionen in WSL finden Sie auf der [Verwaltungs](./wsl-config.md) Seite für die Distribution. 

 [1]: https://www.virtualbox.org/wiki/Changelog-6.0
 [2]: https://docs.microsoft.com/en-us/virtualization/api/
 [3]: https://devblogs.microsoft.com/visualstudio/hyper-v-android-emulator-support/
