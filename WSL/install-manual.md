---
title: Manuelles Herunterladen von WSL-Distributionen (Windows-Subsystem für Linux)
description: Anweisungen zum manuellen Herunterladen von Distributionen des Windows-Subsystems für Linux.
keywords: BashOnWindows, Bash, wsl, Windows, Windows-Subsystem für Linux, WSL, Windows-Subsystem, Distribution, ubuntu, openSUSE, SLES, debian, kali
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 37d8ad589d0108534c27137614a005c0c0ac55bc
ms.sourcegitcommit: 39d3a2f0f4184eaec8d8fec740aff800e8ea9ac7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/24/2020
ms.locfileid: "80256373"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a>Manuelles Herunterladen von Distributionspaketen des Windows-Subsystems für Linux

Es gibt eine Reihe von Szenarien, in denen Sie möglicherweise nicht in der Lage sind, Distributionen von WSL Linux über den Microsoft Store zu installieren, oder dies nicht wünschen. Insbesondere kann dies eintreten, wenn Sie eine SKU von Windows Server oder eines LTSC-Desktopbetriebssystems (Long-Term Servicing) ausführen, die den Microsoft Store nicht unterstützt, oder die Netzwerkrichtlinien Ihres Unternehmens und/oder die Administratoren die Nutzung des Microsoft Stores in Ihrer Umgebung nicht erlauben.

Wie können Sie in diesen Fällen, wenn das eigentliche WSL verfügbar ist, Linux-Distributionen herunterladen und in WSL installieren, wenn Sie nicht auf den Store zugreifen können?

> Hinweis: **Befehlszeilenshellumgebungen, einschließlich Cmd, PowerShell und Linux/WSL-Distributionen, dürfen im Windows 10 S-Modus nicht ausgeführt werden**. Diese Einschränkung wurde implementiert, um die Integritäts- und Sicherheitsziele des S-Modus sicherzustellen: Weitere Informationen finden Sie in [diesem Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/).

## <a name="downloading-distros"></a>Herunterladen von Distributionen

Wenn die Microsoft Store-App nicht verfügbar ist, können Sie Linux-Distributionen manuell herunterladen und installieren, indem Sie auf die folgenden Links klicken:
* [Ubuntu 18.04](https://aka.ms/wsl-ubuntu-1804)
* [Ubuntu 18.04 ARM](https://aka.ms/wsl-ubuntu-1804-arm)
* [Ubuntu 16.04](https://aka.ms/wsl-ubuntu-1604)
* [Debian GNU/Linux](https://aka.ms/wsl-debian-gnulinux)
* [Kali Linux](https://aka.ms/wsl-kali-linux-new)
* [OpenSUSE Leap 42](https://aka.ms/wsl-opensuse-42)
* [SUSE Linux Enterprise Server 12](https://aka.ms/wsl-sles-12)
* [Fedora Remix for WSL](https://github.com/WhitewaterFoundry/WSLFedoraRemix/releases/)

Dies bewirkt den Download der `<distro>.appx`-Pakete in einen Ordner Ihrer Wahl. Befolgen Sie die [Installationsanweisungen](#installing-your-distro), um die heruntergeladenen Distributionen zu installieren.

## <a name="downloading-distros-via-the-command-line"></a>Herunterladen von Distributionen über die Befehlszeile
Wenn Sie möchten, können Sie Ihre bevorzugten Distributionen auch über die Befehlszeile herunterladen:

 ### <a name="download-using-powershell"></a>Herunterladen mithilfe von PowerShell
 Zum Herunterladen von Distributionen mithilfe von PowerShell verwenden Sie das [Invoke-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest)-Cmdlet. Hier sehen Sie eine Beispielanweisung zum Herunterladen von Ubuntu 16.04.

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> Wenn der Download sehr lange dauert, deaktivieren Sie die Statusanzeige, indem Sie `$ProgressPreference = 'SilentlyContinue'` festlegen.

### <a name="download-using-curl"></a>Herunterladen mit curl
Das Windows 10-Update aus Frühjahr 2018 (oder höher) umfasst das beliebte [curl-Befehlszeilenhilfsprogramm](https://curl.haxx.se/), mit dem Sie Webanforderungen (d. h. Befehle der Art HTTP GET, POST, PUT usw.) von der Befehlszeile aus aufrufen können. Mit `curl.exe` können Sie die oben genannten Distributionen herunterladen:

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

Im Beispiel oben wird `curl.exe` ausgeführt (nicht einfach `curl`), um sicherzustellen, dass in PowerShell die echte curl-Programmdatei aufgerufen wird, nicht der curl-Alias von PowerShell für [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)

> Hinweis: Die Verwendung von `curl` kann Vorteile bieten, wenn Sie mithilfe der Cmd-Shell und/oder `.bat` / `.cmd` Schritte zum Herunterladen aufrufen/skripten müssen.

## <a name="installing-your-distro"></a>Installieren der Distribution
Wenn Sie Windows 10 verwenden, können Sie Ihre Distribution mit PowerShell installieren. Navigieren Sie einfach zu dem Ordner, der die oben heruntergeladene Distribution enthält, und führen Sie in diesem Verzeichnis den folgenden Befehl aus, wobei `app_name` für den Namen der APPX-Datei Ihrer Distribution steht.  
```Powershell
Add-AppxPackage .\app_name.appx
```

Wenn Sie Windows Server verwenden, finden Sie die Installationsanweisungen auf der [Windows Server](install-on-server.md)-Dokumentationsseite.

Nachdem Sie Ihre Distribution installiert haben, lesen Sie die Seite [Initialisierungsschritte](initialize-distro.md), um Ihre neue Distribution zu initialisieren.
