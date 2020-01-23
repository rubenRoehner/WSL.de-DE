---
title: UX-Änderungen zwischen WSL 1 und WSL 2
description: Änderungen der Benutzeroberflächen zwischen WSL 1 und WSL 2
keywords: Bashonwindows, bash, WSL, wsl2, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, Debian, SuSE, Windows 10
ms.date: 05/30/2019
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.openlocfilehash: a8f298a69acf44f152da626a0ba571f6bba1970c
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520559"
---
# <a name="user-experience-changes-between-wsl-1-and-wsl-2"></a>Änderungen der Benutzeroberflächen zwischen WSL 1 und WSL 2

Auf dieser Seite werden die Unterschiede bei der Benutzer Darstellung zwischen WSL 1 und der WSL 2-Vorschau angezeigt. Beachten Sie die folgenden wichtigen Änderungen:

- Platzieren von Dateien, auf die Ihre Linux-apps in Ihrem Linux-Stammdatei System zugreifen, um die Geschwindigkeit der Datei Leistung zu beschleunigen
- In anfänglichen Builds der WSL 2-Vorschauversion müssen Sie über eine IP-Adresse auf Netzwerkanwendungen zugreifen und dürfen nicht localhost verwenden.

Und im folgenden finden Sie eine vollständige Liste mit anderen Änderungen, die Sie möglicherweise bemerken:

- WSL 2 verwendet einen virtuellen Hardware Datenträger ( [Virtual Hard Disk](https://en.wikipedia.org/wiki/VHD_(file_format)) , VHD) zum Speichern von Dateien. Wenn Sie die maximale Größe erreichen, müssen Sie Sie möglicherweise erweitern.
- Beim Starten von WSL 2 wird jetzt ein kleiner Anteil des Speichers verwendet.
- Die systemübergreifende Datei Zugriffsgeschwindigkeit wird bei der ersten Vorschau der Builds langsamer

## <a name="place-your-linux-files-in-your-linux-root-file-system"></a>Platzieren Sie Ihre Linux-Dateien in Ihrem Linux-Stammdatei System.
Stellen Sie sicher, dass Sie die Dateien, auf die Sie häufig zugreifen werden, mit Linux-Anwendungen in Ihrem Linux-Stammdatei System speichern, um die Vorteile der Datei Leistung zu nutzen. Diese Dateien müssen sich im Linux-Stammdatei System befinden, um den Zugriff auf das Dateisystem zu beschleunigen. Außerdem haben wir es Windows-Apps ermöglicht, auf das Linux-Stammdatei System zuzugreifen (z. b. Datei-Explorer). Führen Sie Folgendes aus: `explorer.exe .` im Stammverzeichnis Ihrer Linux-Distribution, und sehen Sie sich an, was passiert), wodurch diese Umstellung erheblich vereinfacht wird. 

## <a name="accessing-network-applications"></a>Zugreifen auf Netzwerkanwendungen
In den anfänglichen Builds von WSL 2 Preview müssen Sie unter Linux unter Verwendung der IP-Adresse des Host Computers auf jeden Windows-Server zugreifen.

### <a name="accessing-windows-applications-from-linux"></a>Zugreifen auf Windows-Anwendungen unter Linux
Für den Zugriff auf eine Windows-Netzwerk Anwendung müssen Sie die IP-Adresse des Host Computers verwenden. Dies können Sie mit den folgenden Schritten tun:

- Rufen Sie die IP-Adresse des Host Computers ab, indem Sie den Befehl `cat /etc/resolv.conf` ausführen und die IP-Adresse nach dem Begriff `nameserver`kopieren. 
- Stellen Sie mithilfe der kopierten IP-Adresse eine Verbindung mit einem beliebigen Windows Server

Die folgende Abbildung zeigt ein Beispiel hierfür, indem eine Verbindung mit einem Node. js-Server hergestellt wird, der unter Windows über curl ausgeführt wird. 

![Zugreifen auf Linux-Netzwerkanwendungen über Windows](media/wsl2-network-l2w.png)

### <a name="accessing-linux-applications-from-windows"></a>Zugreifen auf Linux-Anwendungen von Windows aus

Je nachdem, welche Windows-Version Sie verwenden, müssen Sie möglicherweise die IP-Adresse des virtuellen Computers abrufen. Wenn Ihr Build 18945 oder höher ist, können Sie `localhost` wie gewohnt verwenden. 

#### <a name="accessing-linux-on-builds-lower-than-18945httpsblogswindowscomwindowsexperience20190726announcing-windows-10-insider-preview-build-18945"></a>Der Zugriff auf Linux auf Builds unter [18945](https://blogs.windows.com/windowsexperience/2019/07/26/announcing-windows-10-insider-preview-build-18945/)

Wenn Sie über einen Server in einer WSL-Distribution verfügen, müssen Sie die IP-Adresse des virtuellen Computers ermitteln, der Ihre Distribution verwendet, und mit dieser IP-Adresse eine Verbindung mit ihm herstellen. Führen Sie dazu die folgenden Schritte aus:

- Rufen Sie die IP-Adresse Ihrer Distribution ab, indem Sie den Befehl `ip addr` in ihrer WSL-Distribution ausführen und ihn unter dem `inet` Wert der `eth0`-Schnittstelle finden.
   - Dies können Sie leichter finden, indem Sie die Ausgabe des Befehls mit grep wie folgt filtern: `ip addr | grep eth0`.
- Stellen Sie mithilfe der oben gefundenen IP-Adresse eine Verbindung mit dem Linux-Server her.

Die folgende Abbildung zeigt ein Beispiel dafür, dass Sie mithilfe des Edge-Browsers eine Verbindung mit einem Node. js-Server herstellen.

![Zugreifen auf Linux-Netzwerkanwendungen über Windows](media/wsl2-network-w2l.jpg)

### <a name="other-networking-considerations"></a>Weitere Netzwerk Aspekte

#### <a name="connecting-via-remote-ip-addresses"></a>Verbinden über Remote-IP-Adressen

Wenn Sie Remote-IP-Adressen verwenden, um eine Verbindung mit Ihren Anwendungen herzustellen, werden diese als Verbindungen aus dem LAN (Local Area Network) behandelt. Dies bedeutet, dass Sie sicherstellen müssen, dass Ihre Anwendung LAN-Verbindungen akzeptiert, d. h., Sie müssen die Anwendung möglicherweise an `0.0.0.0` anstatt an `127.0.0.1`binden. Beispielsweise kann in python mithilfe von Flask der folgende Befehl ausgeführt werden: `app.run(host='0.0.0.0')`. Behalten Sie die Sicherheit bei, wenn Sie diese Änderungen vornehmen, da dadurch Verbindungen von Ihrem LAN zugelassen werden. 

#### <a name="accessing-a-wsl2-distro-from-your-local-area-network-lan"></a>Zugreifen auf eine WSL2-Distribution über Ihr lokales Netzwerk (LAN)

Wenn Sie eine WSL1-Distribution verwenden und Ihr Computer so eingerichtet wurde, dass in Ihrem LAN auf zugegriffen wird, können Sie auch in Ihrem LAN auf Anwendungen zugreifen, die in WSL ausgeführt werden. Dies ist nicht der Standardfall in WSL2, da WSL2 über einen virtualisierten Ethernet-Adapter mit einer eigenen IP-Adresse verfügt. Um diesen Workflow zu aktivieren, müssen Sie derzeit die gleichen Schritte durchlaufen wie bei einem regulären virtuellen Computer. Wir untersuchen Möglichkeiten, dieses Verhalten zu verbessern.

#### <a name="ipv6-access"></a>IPv6-Zugriff

WSL2 Distributionen können derzeit nur IPv6-Adressen erreichen. Wir arbeiten daran, diese Funktion hinzuzufügen.

## <a name="understanding-wsl-2-uses-a-vhd-and-what-to-do-if-you-reach-its-max-size"></a>Verständnis von WSL 2 verwendet eine virtuelle Festplatte und was Sie tun sollten, wenn Sie die maximale Größe erreichen
WSL 2 speichert alle Ihre Linux-Dateien in einer VHD, die das Ext4-Dateisystem verwendet. Diese VHD wird automatisch angepasst, um Ihre Speicheranforderungen zu erfüllen. Diese VHD weist auch eine anfängliche maximale Größe von 256 GB auf. Wenn sich Ihre Distribution um mehr als 256 GB vergrößert, werden Fehler angezeigt, die darauf hinweisen, dass kein Speicherplatz mehr zur Verfügung steht. Sie können diese Probleme beheben, indem Sie die VHD-Größe erweitern. Anweisungen dazu finden Sie unten:

1. Alle WSL-Instanzen mit dem `wsl --shutdown` Befehl beenden
2. Suchen Sie den Namen des Distribution-Installationspakets "packagefamilyname".
   - Geben Sie in einer PowerShell-Eingabeaufforderung (bei der "Distro" ihren Verteilungs Namen ist) Folgendes ein:
      - `Get-AppxPackage -Name "*<distro>*" | Select PackageFamilyName`
3. Suchen Sie den vollständigen Pfad der VHD-Datei, der von der WSL 2-Installation verwendet wird. Dies ist Ihre "pathtovhd":
     - `%LOCALAPPDATA%\Packages\<PackageFamilyName>\LocalState\<disk>.vhdx`
4. Ändern Sie die Größe der WSL 2-VHD, indem Sie die folgenden Befehle ausführen:
   - Öffnen Sie ein Eingabe Aufforderungs Fenster mit Administrator Berechtigungen, und führen Sie die folgenden Befehle aus:
      - `diskpart`
      - `Select vdisk file="<pathToVHD>"`
      - `expand vdisk maximum="<sizeInMegaBytes>"`
5. Starten Sie Ihre WSL-Distribution.
6. Legen Sie fest, dass WSL seine Größe des Dateisystems erweitern kann.
   - Führen Sie diese Befehle in ihrer WSL-Distribution aus:
      - `sudo mount -t devtmpfs none /dev`
      - `mount | grep ext4`
         - Kopieren Sie den Namen dieses Eintrags, der wie folgt aussieht:/dev/sdXX (wobei das X ein beliebiges anderes Zeichen darstellt).
      - `sudo resize2fs /dev/sdXX`
         - Stellen Sie sicher, dass Sie den Wert verwenden, den Sie zuvor kopiert haben, und Sie müssen möglicherweise Folgendes verwenden: `apt install resize2fs`.

Hinweis: im Allgemeinen können Sie die mit WSL verknüpften Dateien, die sich in Ihrem AppData-Ordner befinden, nicht mithilfe von Windows-Tools oder-Editoren ändern, verschieben oder darauf zugreifen. Dies könnte dazu führen, dass Ihre Linux-Distribution beschädigt wird.

## <a name="wsl-2-will-use-some-memory-on-startup"></a>WSL 2 verwendet Arbeitsspeicher beim Start
WSL 2 verwendet einen einfachen virtuellen Computer für das Hilfsprogramm in einem echten Linux-Kernel, um eine hohe Leistung des Dateisystems und die vollständige System aufrufskompatibilität zu gewährleisten und gleichzeitig genauso schnell, schnell, integriert und reaktionsfähig wie WSL 1 Diese VM für das Hilfsprogramm weist eine geringe Speicher Beanspruchung auf und belegt beim Start den virtuellen Adress gesicherten Speicher. Er ist so konfiguriert, dass er mit einem kleinen Anteil des gesamten Arbeitsspeichers gestartet wird.

## <a name="cross-os-file-speed-will-be-slower-in-initial-preview-builds"></a>Die Kreuz Betriebssystem-Datei Geschwindigkeit wird bei der ersten Vorschau der Builds langsamer
Beim Zugriff auf Windows-Dateien aus einer Linux-Anwendung oder beim Zugriff auf Linux-Dateien aus einer Windows-Anwendung bemerken Sie, dass im Vergleich zu WSL 1 langsamer Datei Geschwindigkeiten angezeigt werden. Das Ergebnis der Architektur Änderungen in WSL 2 ist, dass das WSL-Team aktiv untersucht, wie wir diese Vorgehensweise verbessern können.
