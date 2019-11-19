---
title: Informationen zu WSL 2
description: Informationen zu WSL 2 die neue Architektur für das Windows-Subsystem für Linux
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10, Installation, installieren
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 7122fcbd73e064871eba2ac80c727178aaf3ca7b
ms.sourcegitcommit: 5c92b820f84de57a04ab11faf4dd0d24fff6b320
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/18/2019
ms.locfileid: "74161482"
---
# <a name="about-wsl-2"></a>Informationen zu WSL 2

WSL 2 ist eine neue Version der Architektur, die das Windows-Subsystem für Linux für das Ausführen von ELF64-Linux-Binärdateien unter Windows unterstützt. Die wichtigsten Ziele sind das Erhöhen der Dateisystem Leistung sowie das Hinzufügen von vollständiger System aufrufskompatibilität. Diese neue Architektur ändert, wie diese Linux-Binärdateien mit Windows und der Hardware Ihres Computers interagieren, bietet aber immer noch die gleiche Benutzer Leistung wie in WSL 1 (die aktuelle allgemein verfügbare Version). Einzelne Linux-Distributionen können entweder als WSL 1-Distribution oder als WSL 2-Distribution ausgeführt werden. Sie können jederzeit aktualisiert oder heruntergestuft werden, und Sie können WSL 1 und WSL 2-Distributionen nebeneinander ausführen. WSL 2 verwendet eine völlig neue Architektur, die einen echten Linux-Kernel verwendet.

## <a name="linux-kernel-in-wsl-2"></a>Linux-Kernel in WSL 2

Der Linux-Kernel in WSL 2 ist auf der Grundlage der unter Kernel.org verfügbaren Quelle auf der Grundlage der aktuellen stabilen Verzweigung integriert. Dieser Kernel wurde speziell für WSL 2 optimiert. Es wurde für die Größe und die Leistung optimiert, um unter Windows eine beeindruckende Linux-Darstellung zu bieten, und wird über Windows-Updates gewartet, was bedeutet, dass Sie die neuesten Sicherheitskorrekturen und Kernel Verbesserungen erhalten, ohne Sie selbst verwalten zu müssen.

Außerdem ist dieser Kernel Open Source. Den vollständigen Quellcode für den Linux-Kernel finden Sie [hier](https://github.com/microsoft/WSL2-Linux-Kernel). Weitere Informationen zu diesem Kernel finden Sie in [diesem Blogbeitrag](https://devblogs.microsoft.com/commandline/shipping-a-linux-kernel-with-windows/) , der vom Team verfasst wurde, das es erstellt hat.

## <a name="brief-overview-of-the-wsl-2-architecture"></a>Kurze Übersicht über die Architektur von WSL 2

WSL 2 verwendet die neueste und größte in der Virtualisierungstechnologie, um den Linux-Kernel innerhalb eines virtuellen Lightweight-Hilfsprogramms (Virtual Machine, VM) auszuführen. WSL 2 ist jedoch keine herkömmliche VM-Darstellung. Eine herkömmliche VM-Benutzeroberflächen kann langsam gestartet werden, ist isoliert, beansprucht viele Ressourcen und benötigt Ihre Zeit für deren Verwaltung. WSL 2 verfügt nicht über diese Attribute. Sie bietet weiterhin die bemerkenswerten Vorteile von WSL 1: ein hohes Maß an Integration zwischen Windows und Linux, extrem schnelle Startzeiten, geringen Ressourcenbedarf und das beste daran, dass keine VM-Konfiguration oder-Verwaltung erforderlich ist. Während WSL 2 einen virtuellen Computer verwendet, wird er verwaltet und im Hintergrund ausgeführt, sodass Sie die gleiche Benutzer Darstellung wie WSL 1 haben.

## <a name="increased-file-io-performance"></a>Erweiterte Datei-e/a

Datei intensive Vorgänge wie `git clone`, `npm install`, `apt update`, `apt upgrade`und vieles mehr werden deutlich schneller. Die tatsächliche Geschwindigkeitssteigerung hängt davon ab, welche app Sie ausführen und wie Sie mit dem Dateisystem interagiert. Anfängliche Versionen von WSL 2 werden im Vergleich zu WSL 1 bis zu 20-mal schneller ausgeführt, wenn ein gezippte Tarball entpackt und bei Verwendung von `git clone`, `npm install` und `cmake` in verschiedenen Projekten um 2-5x beschleunigt werden.

## <a name="full-system-call-compatibility"></a>Vollständige System aufrufskompatibilität

Bei Linux-Binärdateien werden Systemaufrufe verwendet, um viele Funktionen wie den Zugriff auf Dateien, das Anfordern von Speicher, das Erstellen von Prozessen und vieles mehr auszuführen. Während WSL 1 eine Übersetzungs Schicht verwendet hat, die vom WSL-Team erstellt wurde, enthält WSL 2 seinen eigenen Linux-Kernel mit vollständiger System aufrufskompatibilität. Dadurch wird ein ganz neuer Satz von apps eingeführt, die Sie in WSL ausführen können, wie z. b. docker und mehr. Darüber hinaus können Updates des Linux-Kernels sofort bereit zum Hinzufügen zu Ihrem Computer sein, anstatt darauf zu warten, dass das WSL-Team die Änderungen implementiert und Sie dann hinzugefügt hat.