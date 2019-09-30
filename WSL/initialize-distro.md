---
title: Initialisieren einer neuen WSL Linux-Distribution
description: Nach dem Installieren einer Linux-Distribution für WSL führen Sie die folgenden einfachen Schritte aus, um die Initialisierung abzuschließen.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: e544dc461913c6e044c70f39103cced62167c4b8
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122712"
---
# <a name="initializing-a-newly-installed-distro"></a>Initialisieren einer neu installierten Distribution
Nachdem Sie Ihre Distribution heruntergeladen und installiert haben, müssen Sie die Initialisierung der neuen Distribution abschließen:

## <a name="launch-a-distro"></a>Starten einer Distribution
Um die Initialisierung der neu installierten Distribution abzuschließen, starten Sie eine neue Instanz. Klicken Sie hierzu in der Microsoft Store-App auf die Schaltfläche „Starten“, oder starten Sie die Distribution über das Startmenü:

> Tipp: Möglicherweise möchten Sie Ihre am häufigsten verwendeten Distributionen an das Startmenü und/oder an die Taskleiste anheften.

![Starten von Distributionen über das Startmenü](media/start-menu.png)

> Unter Windows Server können Sie die ausführbare Startprogrammdatei `<distro>.exe` Ihrer Distribution über dem Distributionsinstallationsordner starten.

Wenn eine neu installierte Distribution zum ersten Mal ausgeführt wird, wird ein Konsolenfenster geöffnet, und Sie werden aufgefordert, bis zum Abschluss der Installation wenige Minuten zu warten.

> In dieser letzten Phase der Installation werden die Dateien der Distribution dekomprimiert und auf Ihrem PC gespeichert. Sie sind dann einsatzbereit. Dies kann je nach Leistung der Speichergeräte Ihres PCs etwa eine Minute oder ggf. auch länger dauern. Diese erste Installationsphase ist nur erforderlich, wenn eine „saubere“ Distribution installiert wird. Alle zukünftigen Starts sollten weniger als eine Sekunde in Anspruch nehmen.

## <a name="setting-up-a-new-linux-user-account"></a>Einrichten eines neuen Linux-Benutzerkontos

Nach Abschluss der Installation werden Sie aufgefordert, ein neues Benutzerkonto (und das zugehörige Kennwort) zu erstellen. 

![Entpacken von Ubuntu in der Windows-Konsole](media/UbuntuInstall.png)

Dieses Benutzerkonto gilt für den normalen Benutzer ohne Administratorrechte, als der Sie beim Starten einer Distribution standardmäßig angemeldet werden.

> Sie können einen beliebigen Benutzernamen und ein gewünschtes Kennwort auswählen. Beides hat keinen Einfluss auf Ihren Windows-Benutzernamen. 

Wenn Sie eine neue Distributionsinstanz öffnen, werden Sie nicht zur Eingabe Ihres Kennworts aufgefordert. Wenn Sie jedoch **einen Prozess mit `sudo` heraufstufen, müssen Sie Ihr Kennwort eingeben**. Stellen Sie also sicher, dass Sie ein Kennwort auswählen, das Sie sich leicht merken können. Weitere Informationen finden Sie auf der Seite [Benutzersupport](user-support.md).

## <a name="update--upgrade-your-distros-packages"></a>Aktualisieren und Upgraden der Pakete Ihrer Distribution

Die meisten Distributionen werden mit einem leeren/minimalen Paketkatalog ausgeliefert. Es wird dringend empfohlen, den Paketkatalog regelmäßig zu aktualisieren und ein Upgrade der installierten Pakete mit dem bevorzugten Paket-Manager Ihrer Distribution auszuführen. Unter Debian/Ubuntu verwenden Sie apt:

```bash
sudo apt update && sudo apt upgrade
```

> Windows führt für Ihre Linux-Distributionen nicht automatisch eine Aktualisierung oder ein Upgrade aus: Linux-Benutzer ziehen es vor, diese Aufgabe selbst zu steuern.

Fertig! Viel Spaß bei der Verwendung Ihrer neuen Linux-Distribution unter WSL! Weitere Informationen zu WSL finden Sie in der weiteren [WSL-Dokumentation](https://aka.ms/wsldocs) oder auf der [Seite mit den WSL-Lernressourcen](https://aka.ms/learnwsl).

![Viel Spaß bei der Verwendung von Linux unter WSL!](media/linux-on-wsl.png)

## <a name="troubleshooting"></a>Problembehandlung

Nachfolgend werden einige Fehler und vorgeschlagene Korrekturen beschrieben. Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).

> **Fehler bei der Installation: 0x8007007e**: Dieser Fehler tritt auf, wenn das System Linux aus dem Store nicht unterstützt.  Stellen Sie Folgendes sicher:
> * Sie führen Windows-Build 16215 oder höher aus. [Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).
> * Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.  [Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).
