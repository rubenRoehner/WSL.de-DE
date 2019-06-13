---
title: Installieren von WSL 2
description: Installationsanweisungen für WSL 2
keywords: Installieren Sie BashOnWindows, Bash, Wsl, wsl2, Windows, Windows-Subsystem für Linux, Windowssubsystem, Ubuntu, Debian, Suse, Windows 10
author: mscraigloewen
ms.author: mscraigloewen
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: 2af43a046333fc8c7b4142cdc5077cdfbf29fea7
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67038080"
---
# <a name="installation-instructions-for-wsl-2"></a>Installationsanweisungen für WSL 2

Führen Sie zum Installieren und nutzen Sie WSL 2 die folgenden Schritte aus:

- Aktivieren Sie die "VM-Plattform" optionale Komponente
- Legen Sie eine Distribution, die durch die WSL-2, die über die Befehlszeile unterstützt werden
- Überprüfen Sie, welche Versionen von WSL Ihre Distributionen verwenden

## <a name="enable-the-virtual-machine-platform-optional-component"></a>Aktivieren Sie die "VM-Plattform" optionale Komponente

Öffnen Sie PowerShell als Administrator, und führen Sie aus:

`Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform`

Nachdem diese Änderungen aktiviert sind, müssen Sie den Computer neu starten.

## <a name="set-a-distro-to-be-backed-by-wsl-2-using-the-command-line"></a>Legen Sie eine Distribution, die durch die WSL-2, die über die Befehlszeile unterstützt werden

In PowerShell ausführen:

`wsl --set-version <Distro> 2`

und achten Sie darauf, ersetzen Sie dies `<Distro>` durch den tatsächlichen Namen von Ihrer Distribution. (Sie finden diese mit dem Befehl: `wsl -l`). Sie können an WSL 1 auf jederzeit ändern, indem den gleichen Befehl wie oben ausführen, aber ersetzen die "2" mit "1".

Darüber hinaus sollten Sie WSL 2 Stellen Sie die Standardarchitektur können Sie mit diesem Befehl dafür:

`wsl --set-default-version 2`

Dies veranlasst alle neuen-Distribution, die Sie installieren, als eine Distribution WSL 2 initialisiert.

## <a name="finish-with-verifying-what-versions-of-wsl-your-distro-are-using"></a>Beim Überprüfen, welche Versionen von WSL Ihre Distribution verwenden, sind abgeschlossen

So überprüfen, welche Versionen von WSL jede Distribution verwendet den folgenden Befehl verwenden:

`wsl --list --verbose` oder `wsl -l -v`

Die Distribution, der Sie oben ausgewählt haben, sollte nun eine "2" in der Spalte "Version" anzeigen. Nun, da Sie danach können Sie beim Einstieg in Ihre WSL-2-Distribution! 