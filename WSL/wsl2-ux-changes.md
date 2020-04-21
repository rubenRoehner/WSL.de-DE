---
title: Änderungen der Benutzeroberfläche zwischen WSL 1 und WSL 2
description: Änderungen der Benutzeroberfläche zwischen WSL 1 und WSL 2
keywords: BashOnWindows, Bash, WSL, WSL2, Windows, Windows-Subsystem für Linux, Windows-Subsystem, Ubuntu, Debian, Suse, Windows 10
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 1965a22a2e290777b207d9ded099ce4a79e1ed38
ms.sourcegitcommit: 0a001ada2131f80dd77b114fc14f2fde43c947ad
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/25/2020
ms.locfileid: "80256333"
---
# <a name="user-experience-changes-between-wsl-1-and-wsl-2"></a>Änderungen der Benutzeroberfläche zwischen WSL 1 und WSL 2

Auf dieser Seite werden die Unterschiede bei der Benutzeroberfläche zwischen WSL 1 und der WSL 2-Vorschauversion behandelt. Dies sind die wichtigsten Änderungen, die Sie beachten sollten:

- Platzieren Sie Dateien, auf die Ihre Linux-Apps zugreifen, in Ihrem Linux-Stammdateisystem, um einen schnelleren Dateizugriff zu ermöglichen
- In anfänglichen Builds der WSL 2-Vorschauversion müssen Sie über eine IP-Adresse auf Netzwerkanwendungen zugreifen und können nicht localhost verwenden

Nachfolgend finden Sie eine vollständige Liste mit sonstigen Änderungen, die Sie möglicherweise bemerken:

- WSL 2 verwendet einen [virtuellen Hardwaredatenträger](https://en.wikipedia.org/wiki/VHD_(file_format)) (VHD) zum Speichern von Dateien. Wenn Sie dessen maximale Größe erreichen, müssen Sie ihn möglicherweise erweitern
- Beim Starten verwendet WSL 2 jetzt einen kleinen Anteil des Arbeitsspeichers
- Die betriebssystemübergreifende Zugriffsgeschwindigkeit auf Dateien ist bei den ersten Vorschaubuilds langsamer

## <a name="place-your-linux-files-in-your-linux-root-file-system"></a>Platzieren Ihrer Linux-Dateien in Ihrem Linux-Stammdateisystem
Achten Sie darauf, Dateien, auf die Sie häufig mit Linux-Anwendungen zugreifen, in Ihrem Linux-Stammdateisystem zu speichern, um die Vorteile bei der Dateileistung zu nutzen. Diese Dateien müssen sich im Linux-Stammdateisystem befinden, um einen schnelleren Zugriff auf das Dateisystem zu erreichen. Außerdem haben wir für Windows-Apps den Zugriff auf das Linux-Stammdateisystem ermöglicht (etwa dem Datei-Explorer! Versuchen Sie, `explorer.exe .` im Stammverzeichnis Ihrer Linux-Distribution auszuführen, und sehen Sie, was geschieht), wodurch sich diese Umstellung erheblich vereinfacht. 

## <a name="accessing-network-applications"></a>Zugriff auf Netzwerkanwendungen
In den anfänglichen Builds der WSL 2-Vorschauversion müssen Sie unter Linux mithilfe der IP-Adresse des Hostcomputers auf Windows-Server zugreifen.

### <a name="accessing-windows-applications-from-linux"></a>Zugreifen auf Windows-Anwendungen unter Linux
Um auf eine Windows-Netzwerkanwendung zuzugreifen, müssen Sie die IP-Adresse Ihres Hostcomputers verwenden. Dies können Sie anhand der folgenden Schritten tun:

- Rufen Sie die IP-Adresse Ihres Hostcomputers ab, indem Sie den Befehl `cat /etc/resolv.conf` ausführen und die IP-Adresse kopieren, die sich an den Ausdruck `nameserver` anschließt. 
- Stellen Sie mithilfe der kopierten IP-Adresse eine Verbindung zu jedem beliebigen Windows-Server her.

Die Abbildung zeigt ein Beispiel dafür – hier wird über curl eine Verbindung mit einem Node.js-Server hergestellt, der unter Windows ausgeführt wird. 

![Zugreifen auf Linux-Netzwerkanwendungen aus Windows](media/wsl2-network-l2w.png)

### <a name="accessing-linux-applications-from-windows"></a>Zugreifen auf Windows-Anwendungen aus Linux

Je nach der von Ihnen verwendeten Windows-Version müssen Sie möglicherweise die IP-Adresse des virtuellen Computers abrufen. Wenn Sie einen Build mit der Nummer 18945 oder höher benutzen, können Sie einfach wie gewohnt `localhost` verwenden. 

#### <a name="accessing-linux-on-builds-lower-than-18945"></a>Zugriff auf Linux aus Builds mit Nummern unter [18945](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/)

Wenn Sie einen Server in einer WSL-Distribution verwenden, müssen Sie die IP-Adresse des virtuellen Computers ermitteln, der Ihre Distribution ausführt, und mithilfe dieser IP-Adresse eine Verbindung mit ihm herstellen. Sie können dazu diese Schritte ausführen:

- Rufen Sie die IP-Adresse Ihrer Distribution ab, indem Sie den Befehl `ip addr` in Ihrer WSL-Distribution ausführen und die Adresse unter dem `inet`-Wert der `eth0`-Schnittstelle finden.
   - Sie können sich die Suche erleichtern, indem Sie die Ausgabe des Befehls mithilfe von grep filtern, wie hier zu sehen: `ip addr | grep eth0`.
- Stellen Sie eine Verbindung mit Ihrem Linux-Server mithilfe der oben ermittelten IP-Adresse her.

Die Abbildung zeigt ein Beispiel dafür – hier wird mithilfe des Microsoft Edge-Browsers eine Verbindung mit einem Node.js-Server hergestellt.

![Zugreifen auf Linux-Netzwerkanwendungen aus Windows](media/wsl2-network-w2l.jpg)

### <a name="other-networking-considerations"></a>Weitere Netzwerküberlegungen

#### <a name="connecting-via-remote-ip-addresses"></a>Verbinden über Remote-IP-Adressen

Wenn Sie Remote-IP-Adressen verwenden, um Verbindungen mit Ihren Anwendungen herzustellen, werden diese als Verbindungen aus dem LAN (Local Area Network) behandelt. Dies bedeutet, Sie müssen sicherstellen, dass Ihre Anwendung LAN-Verbindungen akzeptieren kann, d. h.: Möglicherweise müssen Sie Ihre Anwendung an `0.0.0.0` statt an `127.0.0.1` binden. Beispielsweise kann das in Python mithilfe von Flask und diesem Befehl erfolgen: `app.run(host='0.0.0.0')`. Bitte beachten Sie bei diesen Änderungen die Sicherheit, da sie Verbindungen aus Ihrem LAN zulassen. 

#### <a name="accessing-a-wsl2-distro-from-your-local-area-network-lan"></a>Zugreifen auf eine WSL 2-Distribution aus Ihrem LAN (Local Area Network)

Wenn Sie eine WSL 1-Distribution verwenden und Ihr Computer im LAN so eingerichtet wurde, dass auf ihn zugegriffen wird, kann auf Anwendungen, die in WSL ausgeführt werden, in Ihrem LAN ebenfalls zugegriffen werden. Dies ist standardmäßig in WSL 2 nicht der Fall, da WSL 2 über einen virtualisierten Ethernetadapter mit eigener IP-Adresse verfügt. Um diesen Workflow zu aktivieren, müssen Sie aktuell die gleichen Schritte wie bei einem gewöhnlichen virtuellen Computer durchlaufen. Wir untersuchen Möglichkeiten, dieses Verhalten zu verbessern!

#### <a name="ipv6-access"></a>IPv6-Zugriff

WSL 2-Distributionen können aktuell keine reinen IPv6-Adressen erreichen. Wir arbeiten daran, diese Funktion hinzuzufügen.

## <a name="understanding-wsl-2-uses-a-vhd-and-what-to-do-if-you-reach-its-max-size"></a>WSL 2 verwendet jetzt eine VHD, und so kann man vorgehen, wenn deren maximale Größe erreicht ist
WSL 2 speichert alle Ihre Linux-Dateien auf einer VHD, die das Ext4-Dateisystem verwendet. Diese VHD passt ihre Größe automatisch an, um Ihren Speicheranforderungen zu genügen. Diese VHD weist außerdem anfänglich eine maximale Größe von 256 GB auf. Wenn Ihre Distribution über die Größe von 256 GB anwächst, werden Ihnen Fehler angezeigt, die besagen, dass kein Speicherplatz mehr zur Verfügung steht. Sie können dieses Problem beheben, indem Sie die Größe der VHD heraufsetzen. Anweisungen dazu finden Sie unten:

1. Beenden Sie alle WSL-Instanzen mit dem `wsl --shutdown`-Befehl
2. Suchen Sie das Installationspaket Ihrer Distribution mit dem Namen ‚PackageFamilyName‘
   - Geben Sie an einer PowerShell-Eingabeaufforderung (in der ‚distro‘ für den Namen Ihrer Distribution steht) ein:
      - `Get-AppxPackage -Name "*<distro>*" | Select PackageFamilyName`
3. Suchen Sie den vollständigen Pfad der VHD-Datei, die von Ihrer WSL 2-Installation verwendet wird, dies ist Ihr ‚pathToVHD‘:
     - `%LOCALAPPDATA%\Packages\<PackageFamilyName>\LocalState\<disk>.vhdx`
4. Ändern Sie die Größe Ihrer WSL 2-VHD, indem Sie die folgenden Befehle ausführen
   - Öffnen Sie ein Eingabeaufforderungsfenster mit Administratorrechten, und führen Sie die folgenden Befehle aus:
      - `diskpart`
      - `Select vdisk file="<pathToVHD>"`
      - `expand vdisk maximum="<sizeInMegaBytes>"`
5. Starten Sie Ihre WSL-Distribution
6. WSL darüber informieren, dass es die Größe seines Dateisystems erweitern kann
   - Führen Sie diese Befehle in Ihrer WSL-Distribution aus:
      - `sudo mount -t devtmpfs none /dev`
      - `mount | grep ext4`
         - Kopieren Sie den Namen dieses Eintrags, der diese Form hat: /dev/sdXX (wobei X für ein beliebiges anderes Zeichen steht)
      - `sudo resize2fs /dev/sdXX`
         - Achten Sie darauf, den Wert zu verwenden, den Sie zuvor kopiert hatten, und möglicherweise müssen Sie `apt install resize2fs` verwenden.

Bitte beachten: Im Allgemeinen sollten Sie die WSL-bezogenen Dateien, die sich in Ihrem AppData-Ordner befinden, nicht mithilfe von Windows-Tools oder-Editoren ändern, verschieben oder darauf zugreifen. Dies könnte zu einer Beschädigung Ihrer Linux-Distribution führen.

## <a name="wsl-2-will-use-some-memory-on-startup"></a>WSL 2 belegt beim Starten eine gewisse Menge Arbeitsspeicher
WSL 2 verwendet eine schlanke VM mit Hilfsprogrammen unter einem echten Linux-Kernel, um hervorragende Dateisystemleistung und vollständige Kompatibilität von Systemaufrufen zu bieten und dabei die Schlankheit, Schnelligkeit, Integration und Reaktionsfähigkeit von WSL 1 beizubehalten. Diese Hilfsprogramm-VM weist einen geringen Arbeitsspeicherbedarf auf und weist beim Starten von virtuellen Adressen gestützten Arbeitsspeicher zu. Sie ist so konfiguriert, dass sie mit einem kleinen Anteil Ihres gesamten Arbeitsspeichers startet.

## <a name="cross-os-file-speed-will-be-slower-in-initial-preview-builds"></a>Die betriebssystemübergreifende Zugriffsgeschwindigkeit auf Dateien ist bei den ersten Vorschaubuilds langsamer
Beim Zugriff auf Windows-Dateien aus einer Linux-Anwendung werden Sie im Vergleich zu WSL 1 geringere Zugriffsgeschwindigkeiten feststellen. Dies ist ein Ergebnis der Architekturänderungen in WSL 2 und stellt einen Punkt dar, den das WSL-Team aktiv untersucht, um eine Verbesserung dieses Verhaltens zu erreichen.
