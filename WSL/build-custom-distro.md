---
title: Erstellen Sie eine benutzerdefinierte Linux-Distribution für WSL
description: Erfahren Sie, wie eine benutzerdefinierte Linux-Distribution für Windows-Subsystem für Linux zu erstellen.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem, -Distribution, Benutzerdefiniert
author: taraj
ms.author: taraj
ms.date: 03/27/2018
ms.topic: article
ms.assetid: a5095219-0c82-4ce5-9a6d-5c2fc00835a3
ms.custom: seodec18
ms.openlocfilehash: b98101c19d7d450548531521c3f8ee15ce62f9f1
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59063258"
---
# <a name="creating-a-custom-linux-distro-for-wsl"></a>Erstellen eine benutzerdefinierte Linux-Distribution für WSL

Verwenden Sie unsere open-Source WSL-Beispiel, das Erstellen von Paketen für WSL-Distribution, die für den Microsoft Store und/oder zum Erstellen von benutzerdefinierten Linux-Distribution, die Pakete für das querladen. Sie finden die [Distribution Startprogramm Repository](https://github.com/Microsoft/WSL-DistroLauncher) auf GitHub.

Dieses Projekt ermöglicht:
* Linux-Verteilung Verwalter zu packen und senden eine Linux-Distribution als eine AppX-Datei, die für WSL ausgeführt wird.
* Entwicklern das Erstellen von benutzerdefinierter Linux-Distributionen, die auf ihrem Entwicklungscomputer sein können

## <a name="background"></a>Hintergrund
Wir verteilen als UWP-Anwendungen über den Microsoft Store-Linux-Distributionen für WSL. Sie können diese Anwendungen installieren, die dann für WSL - das Subsystem ausgeführt wird, die sich im Windows-Kernel befindet. Dieser Mechanismus hat viele Vorteile, wie in einem früheren Blogbeitrag beschrieben.

## <a name="sideloading-a-custom-linux-distro-package"></a>Querladen eines benutzerdefinierten virtuellen Linux-Distribution-Pakets
Sie können ein benutzerdefiniertes Paket von Linux-Distribution, die als eine Anwendung zum Sideloaden auf Ihr persönlicher Computer erstellen. Bitte beachten Sie, dass das benutzerdefinierte Paket nicht über den Microsoft Store verteilt werden würde, es sei denn, Sie Maintainer Verteilung übermitteln.
Zum Einrichten von Ihrem Computers, Apps querzuladen, müssen Sie dies in den Systemeinstellungen, unter "Für Entwickler" zu ermöglichen.  Achten Sie darauf, dass Sie entweder den Entwicklermodus oder querladen von apps ausgewählt haben

## <a name="for-linux-distro-maintainers"></a>Für die Verwalter von Linux-Distribution
Um an den Store übermitteln, müssen Sie die Arbeit mit uns auf die Genehmigung zur Veröffentlichung zu erhalten. Wenn Sie interessiert, Hinzufügen von Ihrer Distribution zu den Microsoft Store-Besitzer einer Linux-Verteilung sind, wenden Sie sich an wslpartners@microsoft.com.

## <a name="getting-started"></a>Erste Schritte
Befolgen Sie die Anweisungen auf der [Distribution Startprogramm-GitHub-Repository](https://github.com/Microsoft/WSL-DistroLauncher) zum Erstellen eines benutzerdefinierten Linux-Distribution-Pakets.

 
## <a name="team-blogs"></a>Team-Blogs
*  [Öffnen Sie ein Beispiel für WSL-Sourcing für die Verwalter von Linux-Verteilung und Querladen benutzerdefinierte Linux-Distributionen](https://blogs.msdn.microsoft.com/commandline/2018/03/26/wsl-distro-launcher/)
* [Befehlszeilen-blog](https://blogs.msdn.microsoft.com/commandline/)

## <a name="provide-feedback"></a>Senden von Feedback
* [Repository der Distribution-Startprogramm Gitub](https://github.com/Microsoft/WSL-DistroLauncher)
* [GitHub-problemverfolgung für WSL](https://github.com/Microsoft/BashOnWindows/issues)
* [Befehlszeile UserVoice-portal](https://wpdev.uservoice.com/forums/266908-command-prompt-console-bash-on-ubuntu-on-windo/category/161892-bash)
