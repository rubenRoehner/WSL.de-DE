---
title: Manuelles Herunterladen von Windows-Subsystem für Linux (WSL)
description: Anweisungen zum manuellen Herunterladen des Windows-Subsystems für Linux-Distributionen.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, WSL, Windows-Subsystem, Distribution, Ubuntu, openSUSE, SLES, Debian, Kali
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: aa0b42748115045105bb4e6eae91493bfee11d09
ms.sourcegitcommit: 467b6c8e9716d1a60dbf9f7658fd9579da365b58
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2020
ms.locfileid: "77624924"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a>Manuelles Herunterladen von Windows-Subsystem für Linux-Distribution-Pakete

Es gibt mehrere Szenarios, in denen Sie möglicherweise nicht in der Lage sind, WSL-Linux-Distributionen über die Microsoft Store zu installieren (oder möchten). Vor allem können Sie eine Windows Server-oder eine LTSC-Desktop-SKU (Long-Term Wartung) ausführen, die keine Microsoft Store unterstützt, oder Ihre Unternehmensnetzwerk Richtlinien und/oder Administratoren, um die Verwendung von Microsoft Store in Ihrer Umgebung nicht zuzulassen.

Wie können Sie in diesen Fällen, während WSL selbst verfügbar ist, Linux-Distributionen in WSL herunterladen und installieren, wenn Sie nicht auf den Store zugreifen können?

> Hinweis: **befehlszeilenshellumgebungen, einschließlich cmd, PowerShell und Linux/WSL-Distributionen, dürfen im Windows 10 S-Modus nicht ausgeführt werden**. Diese Einschränkung ist vorhanden, um die Integritäts-und Sicherheitsziele des S-Modus sicherzustellen: Lesen Sie [diesen Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) , um weitere Informationen zu erhalten.

## <a name="downloading-distros"></a>Herunterladen von Distributionen

Wenn die Microsoft Store-App nicht verfügbar ist, können Sie Linux-Distributionen herunterladen und manuell installieren, indem Sie auf die folgenden Links klicken:
<!-- * [Ubuntu 18.04](https://aka.ms/wsl-ubuntu-1804)
* [Ubuntu 18.04 ARM](https://aka.ms/wsl-ubuntu-1804-arm) -->
* Ubuntu 18,04
* Ubuntu 18,04 Arm
* [Ubuntu 16,04](https://aka.ms/wsl-ubuntu-1604)
* [Debian GNU/Linux](https://aka.ms/wsl-debian-gnulinux)
* [Kali Linux](https://aka.ms/wsl-kali-linux-new)
* [OpenSUSE Leap 42](https://aka.ms/wsl-opensuse-42)
* [SUSE Linux Enterprise Server 12](https://aka.ms/wsl-sles-12)
* [Fedora Remix for WSL](https://github.com/WhitewaterFoundry/WSLFedoraRemix/releases/)

Dies bewirkt, dass die `<distro>.appx` Pakete in einen Ordner Ihrer Wahl heruntergeladen werden. Befolgen Sie die [Installationsanweisungen](#installing-your-distro) , um die heruntergeladenen Distributionen zu installieren.

## <a name="downloading-distros-via-the-command-line"></a>Herunterladen von Distributionen über die Befehlszeile
Wenn Sie möchten, können Sie Ihre bevorzugten Distributionen auch über die Befehlszeile herunterladen:

 ### <a name="download-using-powershell"></a>Herunterladen mithilfe von PowerShell
 Verwenden Sie das Cmdlet "Start [-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) ", um Distributionen mithilfe von PowerShell herunterzuladen. Im folgenden finden Sie eine Beispiel Anweisung zum Herunterladen von Ubuntu 16,04.

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> Wenn der Download lange dauert, deaktivieren Sie die Statusanzeige, indem Sie festlegen `$ProgressPreference = 'SilentlyContinue'`

### <a name="download-using-curl"></a>Download mithilfe von curl
Windows 10 Spring 2018 Update (oder höher) umfasst das beliebte [curl-Befehlszeilen Dienstprogramm](https://curl.haxx.se/) , mit dem Sie Webanforderungen (z. b. HTTP Get-, Post-, Put-usw.-Befehle) von der Befehlszeile aus aufrufen können. Mit `curl.exe` können Sie die obigen Distributionen herunterladen:

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

Im obigen Beispiel wird `curl.exe` (nicht nur `curl`) ausgeführt, um sicherzustellen, dass in PowerShell die ausführbare Datei "Real curl" aufgerufen wird, nicht der PowerShell-curl-Alias für " [Aufruf-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6) ".

> Hinweis: das Verwenden von `curl` ist möglicherweise vorzuziehen, wenn Sie Download Schritte mithilfe der CMD-Shell und/oder `.bat` / `.cmd` Skripts aufrufen/ausführen müssen.

## <a name="installing-your-distro"></a>Installieren der Distribution
Wenn Sie Windows 10 verwenden, können Sie Ihre Distribution mit PowerShell installieren. Navigieren Sie einfach zum Ordner, der die zuvor heruntergeladene Distribution enthält, und führen Sie in diesem Verzeichnis den folgenden Befehl aus, wobei `app_name` der Name der Datei "Distribution. AppX" ist.  
```Powershell
Add-AppxPackage .\app_name.appx
```

Wenn Sie Windows Server verwenden, finden Sie die Installationsanweisungen auf der [Windows Server](install-on-server.md) -Dokumentationsseite.

Nachdem Sie Ihre Distribution installiert haben, lesen Sie die Seite [Initialisierungs Schritte](initialize-distro.md) , um Ihre neue Distribution zu initialisieren.
