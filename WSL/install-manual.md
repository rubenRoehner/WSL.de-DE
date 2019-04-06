---
title: Manuelles Herunterladen von Windows-Subsystem für Linux (WSL)-Distributionen
description: Anweisungen zum Manuelles Herunterladen von Windows-Subsystem für Linux-Distributionen.
keywords: BashOnWindows, Bash, Wsl, Windows, Windows-Subsystem für Linux, WSL, Windows-Subsystem, -Distribution, Ubuntu, OpenSUSE, SLES, debian, Kali
author: taraj
ms.author: taraj
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: be1c1331183317d4f970696464110b9968208d21
ms.sourcegitcommit: ca08a78925880ed3eccf88edb30def16c83f2543
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/04/2019
ms.locfileid: "59063568"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a>Manuelles Herunterladen von Windows-Subsystem für Linux-Distribution-Pakete

Es gibt mehrere Szenarios, in dem darf nicht in der Lage (oder möchten), WSL-Linux-Distributionen, über den Microsoft Store zu installieren. Insbesondere können Sie ausgeführt werden, einem Windows Server- oder Long-term Servicing (LTSB/LTSC) Desktop-Betriebssystem-SKU, die Microsoft Store, oder Ihre zum Zulassen von Microsoft Store-Verwendung in Ihrer Umgebung nicht Unternehmensnetzwerk Richtlinien und/oder Administratoren nicht unterstützt.

In diesen Fällen WSL selbst zur Verfügung steht, wie Sie herunterladen und installieren Linux-Distributionen in WSL, wenn Sie nicht den Speicher zugreifen können?

> Hinweis: **Befehlszeilenshell Umgebungen Cmd, PowerShell und Linux/WSL Distributionen einschließlich dürfen nicht auf Windows 10 S-Modus ausführen**. Diese Einschränkung gilt, um sicherzustellen, dass die Integrität und Sicherheit Ziele, die S-Modus bietet: Lesen [diesen Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) für Weitere Informationen.

## <a name="downloading-distros"></a>Herunterladen von Distributionen

Wenn die Microsoft Store-app nicht verfügbar ist, können Sie herunterladen und installieren Linux-Distributionen manuell durch Klicken auf diese Links:
* [Ubuntu 18.04](https://aka.ms/wsl-ubuntu-1804)
* [Ubuntu 18.04 ARM](https://aka.ms/wsl-ubuntu-1804-arm)
* [Ubuntu 16.04](https://aka.ms/wsl-ubuntu-1604)
* [Debian GNU/Linux](https://aka.ms/wsl-debian-gnulinux)
* [Kali Linux](https://aka.ms/wsl-kali-linux)
* [OpenSUSE](https://aka.ms/wsl-opensuse-42)
* [SLES](https://aka.ms/wsl-sles-12)

Dies bewirkt, dass die `<distro>.appx` Pakete in einen Ordner Ihrer Wahl herunterladen. Führen Sie die [installationsanweisungen](#installing-your-distro) um Ihre heruntergeladene Distro(s) zu installieren.

## <a name="downloading-distros-via-the-command-line"></a>Herunterladen von Distributionen über die Befehlszeile
Falls gewünscht, können Sie auch Ihre bevorzugte Distro(s) über die Befehlszeile herunterladen:

 ### <a name="download-using-powershell"></a>Laden Sie mithilfe von PowerShell
 Verwenden Sie zum Herunterladen mithilfe von PowerShell Distributionen die [Invoke-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) Cmdlet. Hier ist eine Beispiel-Anleitung zum Herunterladen von Ubuntu 16.04.

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> Wenn der Download sehr lange dauert, deaktivieren Sie die Statusanzeige festlegen `$ProgressPreference = 'SilentlyContinue'`

### <a name="download-using-curl"></a>Laden Sie mithilfe von curl
Windows 10 Frühjahr 2018 Update (oder höher) enthält das beliebte [curl-Befehlszeilen-Hilfsprogramm](https://curl.haxx.se/) mit dem Sie webanforderungen (d. h. HTTP-GET, POST, PUT, Befehle von usw.) über die Befehlszeile aufrufen können. Sie können `curl.exe` zum Herunterladen von der oben aufgeführten Distributionen:

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

Im obigen Beispiel `curl.exe` ausgeführt wird (nicht nur `curl`) sicherstellen, dass in PowerShell ist die echten Curl ausführbare Datei aufgerufen wird, nicht PowerShell Curl alias für [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)

> Hinweis: Mithilfe von `curl` kann vorteilhafter sein, wenn man Download-Schritte, die mithilfe des Cmd-Shell aufrufen bzw. das Skript bzw. `.bat`  /  `.cmd` Skripts.

## <a name="installing-your-distro"></a>Installieren von Ihrer Distribution
Anweisungen dazu, wie Sie Ihre heruntergeladene Distro(s) installieren, finden Sie in der [Windows Desktop](install-win10.md) oder [WindowsServer](install-on-server.md) installationsanweisungen.
