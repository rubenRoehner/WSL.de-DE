---
title: Initialisieren einer neuen WSL-Linux-Distribution
description: Nach dem Installieren einer Linux-Distribution für WSL führen Sie die folgenden einfachen Schritte aus, um die Initialisierung abzuschließen.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: e544dc461913c6e044c70f39103cced62167c4b8
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122712"
---
# <a name="initializing-a-newly-installed-distro"></a>Initialisieren einer neu installierten Distribution
Nachdem Sie Ihre Distribution heruntergeladen und installiert haben, müssen Sie die Initialisierung der neuen Distribution abgeschlossen haben:

## <a name="launch-a-distro"></a>Hiermit wird eine Distribution gestartet.
Um die Initialisierung der neu installierten Distribution abzuschließen, starten Sie eine neue-Instanz. Klicken Sie hierzu in der Microsoft Store-App auf die Schaltfläche "starten", oder starten Sie die Distribution über das Startmenü:

> Tipp: Möglicherweise möchten Sie Ihre am häufigsten verwendeten Distributionen an das Startmenü und/oder an die Taskleiste anheften.

![Starten von Distributionen über das Startmenü](media/start-menu.png)

> Unter Windows Server können Sie die ausführbare Datei des ausführbaren `<distro>.exe` Programms Ihrer Distribution über den Installationsordner "Distribution" starten.

Wenn eine neu installierte Distribution zum ersten Mal ausgeführt wird, wird ein Konsolenfenster geöffnet, und Sie werden aufgefordert, bis zum Abschluss der Installation eine Minute oder zwei Minuten zu warten.

> In dieser letzten Phase der Installation werden die Dateien der Distribution dekomprimiert und auf Ihrem PC gespeichert, einsatzbereit. Dies kann je nach Leistung der Speichergeräte Ihres PCs etwa eine Minute oder länger dauern. Diese erste Installationsphase ist nur erforderlich, wenn eine Distribution bereinigt ist. alle zukünftigen Starts sollten weniger als eine Sekunde in Anspruch nehmen.

## <a name="setting-up-a-new-linux-user-account"></a>Einrichten eines neuen Linux-Benutzerkontos

Nach Abschluss der Installation werden Sie aufgefordert, ein neues Benutzerkonto (und das zugehörige Kennwort) zu erstellen. 

![Ubuntu-Entpacken in der Windows-Konsole](media/UbuntuInstall.png)

Dieses Benutzerkonto gilt für den normalen Benutzer ohne Administratorrechte, bei dem Sie beim Starten einer Distribution standardmäßig angemeldet werden.

> Sie können einen beliebigen Benutzernamen und ein Kennwort auswählen, und Sie haben keinen Einfluss auf Ihren Windows-Benutzernamen. 

Wenn Sie eine neue Instanz von Distribution öffnen, werden Sie nicht zur Eingabe Ihres Kennworts aufgefordert. **Wenn Sie jedoch einen Prozess mit `sudo`herauf Stufen, müssen Sie Ihr Kennwort eingeben**. Stellen Sie also sicher, dass Sie ein Kennwort auswählen, das Sie sich leicht merken können. Weitere Informationen finden Sie auf der Seite [Benutzer Support](user-support.md) .

## <a name="update--upgrade-your-distros-packages"></a>Aktualisieren & Aktualisieren der Pakete Ihrer Distribution

Die meisten Distributionen werden mit einem leeren/minimalen Paket Katalog ausgeliefert. Es wird dringend empfohlen, den Paket Katalog regelmäßig zu aktualisieren und die installierten Pakete mit dem bevorzugten Paket-Manager Ihrer Distribution zu aktualisieren. Unter Debian/Ubuntu verwenden Sie APT:

```bash
sudo apt update && sudo apt upgrade
```

> Ihre Linux-Distributionen werden von Windows nicht automatisch aktualisiert oder aktualisiert: Dies ist eine Aufgabe, die die Linux-Benutzer vorziehen, sich selbst zu steuern.

Fertig! Profitieren Sie von der Verwendung ihrer neuen Linux-Distribution auf WSL! Weitere Informationen zu WSL finden Sie unter WSL [docs](https://aka.ms/wsldocs)(WSL-Dokumentation) oder auf der Seite mit den [WSL-Lernressourcen](https://aka.ms/learnwsl).

![Nutzen Sie Linux auf WSL](media/linux-on-wsl.png)

## <a name="troubleshooting"></a>Problembehandlung

Im folgenden finden Sie verwandte Fehler und empfohlene Korrekturen. Weitere häufige Fehler und deren Lösungen finden Sie auf der [WSL-Seite zur Problem](troubleshooting.md) Behandlung.

> **Fehler bei der Installation (Fehler 0x8007007e** ). Dieser Fehler tritt auf, wenn das System Linux nicht aus dem Store unterstützt.  Stellen Sie Folgendes sicher:
> * Sie führen Windows Build 16215 oder höher aus. [Überprüfen Sie den Build](troubleshooting.md#check-your-build-number).
> * Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.  [Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).
