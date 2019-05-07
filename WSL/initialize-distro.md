---
title: Initialisiert eine neue WSL-Linux-Distribution
description: Schließen Sie nach der Installation einer Linux-Distribution für WSL Initialisierung, indem Sie die folgenden einfachen Schritte
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 7f1ce521b248c873fa7f81c6363eb506c0363fed
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2019
ms.locfileid: "59902047"
---
# <a name="initializing-a-newly-installed-distro"></a>Initialisiert eine neu installierte Distribution
Nachdem Ihre Distribution heruntergeladen und installiert wurde, müssen Sie zum Abschließen der Initialisierung der neuen Distribution:

## <a name="launch-a-distro"></a>Starten Sie eine Distribution
Um die Initialisierung von Ihrer Distribution, die neu installierte abgeschlossen haben, starten Sie eine neue Instanz. Sie erreichen dies durch Klicken auf die Startschaltfläche "" in der Windows Store-app, oder starten Sie den-Distribution, die über das Startmenü zugreifen:

> Tipp: Sie möchten Ihre am häufigsten verwendeten Distributionen Startmenü und/oder die Taskleiste anheften.

![Distributionen über das Startmenü starten](media/start-menu.png)

> In Windows Server, starten Sie Ihre Distribution des-Startprogramms `<distro>.exe` aus dem Installationsordner der Distribution.

Erstmals eine neu installierte Distribution ausgeführt wird, eine Konsole Fenster geöffnet wird, und werden Sie aufgefordert, ein oder zwei Minuten zum Abschluss der Installation warten.

> In dieser letzten Phase der Installation werden die Distribution Dateien aufheben komprimiert und gespeichert, die auf Ihrem PC, die zur Verwendung bereit. Dies kann zu eine Minute oder länger, je nach die Leistung Ihres Computers Speichergeräte dauern. In dieser Phase der Erstinstallation ist nur erforderlich, wenn eine Distribution, die neu installierten - ist alle auf zukünftig gestartete dauert weniger als eine Sekunde.

## <a name="setting-up-a-new-linux-user-account"></a>Das Einrichten eines neuen Linux-Benutzerkontos

Nach Abschluss der Installation werden Sie aufgefordert werden, erstellen Sie ein neues Benutzerkonto (und das Kennwort). 

![Ubuntu, die in der Windows-Konsole Entpacken](media/UbuntuInstall.png)

Dieses Benutzerkonto ist für den normalen nicht-Admin-Benutzer, dass Sie angemeldet als standardmäßig beim Starten von einer Distribution.

> Sie können einen beliebigen Benutzernamen und das Kennwort werden sollen – sie haben keinen Einfluss auf Ihren Windows-Benutzernamen. 

Wenn Sie eine neue Instanz der Distribution öffnen, werden Sie nicht aufgefordert für Ihr Kennwort jedoch **, wenn Sie einen Prozess mit erhöhen `sudo`, Sie müssen Ihr Kennwort eingeben**, stellen Sie sicher, dass ein Kennwort wählen Sie Sie leicht merken können! Finden Sie unter den [Benutzersupport](user-support.md) Seite Weitere Informationen.

## <a name="update--upgrade-your-distros-packages"></a>Aktualisieren und Ihre Distribution Pakete aktualisieren

Die meisten Distributionen, die mit einer leeren/minimale Paketkatalog ausgeliefert werden. Es wird dringend empfohlen, Ihr Paketkatalog regelmäßig aktualisiert, und aktualisieren Ihre installierten Pakete, die mit Ihrer Distribution des bevorzugten Paket-Manager. Unter Debian/Ubuntu verwenden Sie apt:

```bash
sudo apt update && sudo apt upgrade
```

> Windows nicht automatisch zu aktualisieren oder aktualisieren Sie Ihre Linux-Distro(s): Dies ist eine Aufgabe, die das Linux-Benutzer lieber selbst steuern.

Fertig! Nutzen Sie Ihre neue Linux-Distribution für WSL! Weitere Informationen zu WSL finden Sie in den anderen [WSL-Dokumentation](https://aka.ms/wsldocs), oder die [WSL Lernressourcenseite](https://aka.ms/learnwsl).

![Profitieren Sie mit Linux in WSL](media/linux-on-wsl.png)

## <a name="troubleshooting"></a>Problembehandlung

Im folgenden finden Sie zugehörige Fehler und Vorschläge zur Behebung. Finden Sie in der [WSL Problembehandlungsseite](troubleshooting.md) andere häufig auftretende Fehler und ihre Lösungen.

> **Fehler bei der Installation Fehler 0x8007007e** dieser Fehler tritt auf, wenn es sich bei Ihrem System Linux aus dem Speicher nicht unterstützt.  Stellen Sie Folgendes sicher:
> * Sie können Windows Build 16215 oder höher ausführen. [Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).
> * Das Windows-Subsystem für Linux optionale Komponente aktiviert ist, und der Computer neu gestartet wurde.  [WSL aktiviert](troubleshooting.md#confirm-wsl-is-enabled).
