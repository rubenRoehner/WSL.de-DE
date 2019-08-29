---
title: Problembehandlung beim Windows-Subsystem für Linux
description: Bietet ausführliche Informationen zu häufigen Fehlern und Problemen, die bei der Ausführung von Linux im Windows-Subsystem für Linux auftreten.
keywords: Bashonwindows, bash, WSL, Windows, windowssubsystem, Ubuntu
author: scooley
ms.author: scooley
ms.date: 11/15/2017
ms.topic: article
ms.assetid: 6753f1b2-200e-49cc-93a5-4323e1117246
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 6a5fec8b8e054b4d3399ee9bcd903acebca7aace
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122690"
---
# <a name="troubleshooting-windows-subsystem-for-linux"></a>Problembehandlung bei Windows-Subsystem für Linux

### <a name="bash-loses-network-connectivity-once-connected-to-a-vpn"></a>Bash verliert nach dem Herstellen einer Verbindung mit einem VPN die Netzwerk Konnektivität

Wenn bash nach dem Herstellen einer Verbindung mit einem VPN unter Windows die Netzwerk Konnektivität verliert, können Sie diese Problem Umgehung innerhalb von bash testen. Mit dieser Problem Umgehung können Sie die DNS-Auflösung durch manuell `/etc/resolv.conf`überschreiben.

1. Notieren Sie sich den DNS-Server des VPN.`ipconfig.exe /all`
2. Erstellen Sie eine Kopie der vorhandenen Datei "resolv. conf".`sudo cp /etc/resolv.conf /etc/resolv.conf.new`
3. Verknüpfung der aktuellen resolv. con aufheben`sudo unlink /etc/resolv.conf`
4. `sudo mv /etc/resolv.conf.new /etc/resolv.conf`
5. Öffnen `/etc/resolv.conf` Sie und. <br/>
   a. Löschen Sie die erste Zeile aus der Datei, die besagt\# , dass diese Datei automatisch von WSL generiert wurde. Um die automatische Generierung dieser Datei zu verhindern, entfernen Sie diese Zeile. ". <br/>
   b. Fügen Sie den DNS-Eintrag aus (1) oben als ersten Eintrag in der Liste der DNS-Server hinzu. <br/>
   c. Schließen Sie die Datei. <br/>

Nachdem Sie die Verbindung mit dem VPN getrennt haben, müssen Sie die Änderungen auf `/etc/resolv.conf`zurücksetzen. Gehen Sie hierzu wie folgt vor:
1. `cd /etc`
2. `sudo mv resolv.conf resolv.conf.new`
3. `sudo ln -s ../run/resolvconf/resolv.conf resolv.conf`

### <a name="starting-wsl-or-installing-a-distribution-returns-an-error-code"></a>Beim Starten von WSL oder beim Installieren einer Distribution wird ein Fehlercode zurückgegeben

Befolgen Sie [diese Anweisungen](https://github.com/Microsoft/WSL/blob/master/CONTRIBUTING.md#8-detailed-logs) , um detaillierte Protokolle zu erfassen und ein Problem auf unserem GitHub zu melden.

### <a name="updating-bash-on-ubuntu-on-windows"></a>Aktualisieren von bash unter Ubuntu unter Windows

Es gibt zwei Komponenten von bash unter Ubuntu unter Windows, die aktualisiert werden können. 

1. Das Windows-Subsystem für Linux
  
   Durch das Upgrade dieses Teils von bash auf Ubuntu unter Windows werden alle neuen Korrekturen in den [Anmerkungen](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes)zu dieser Version aktiviert. Stellen Sie sicher, dass Sie das Windows Insider-Programm abonniert haben und dass der Build auf dem neuesten Stand ist. Wenn Sie ein feineres Steuerelement wie das Zurücksetzen Ihrer Ubuntu-Instanz einrichten, sehen Sie sich die [Befehlsreferenz Seite](https://msdn.microsoft.com/en-us/commandline/wsl/reference)

2. Die Ubuntu-Benutzer Binärdateien 

   Durch das Upgrade dieses Teils von bash auf Ubuntu unter Windows werden alle Updates der Ubuntu-Benutzer Binärdateien einschließlich der Anwendungen installiert, die Sie über apt-get installiert haben. Führen Sie die folgenden Befehle in bash aus, um das Update auszuführen:
  
   1. `apt-get update`
   2. `apt-get upgrade`
  
### <a name="apt-get-upgrade-errors"></a>Apt-get-Upgradefehler
In einigen Paketen werden Features verwendet, die noch nicht implementiert wurden. `udev`wird z. b. noch nicht unterstützt und `apt-get upgrade` verursacht mehrere Fehler.

Führen Sie die folgenden Schritte `udev`aus, um Probleme im Zusammenhang mit zu beheben:

1. Schreiben Sie Folgendes in `/usr/sbin/policy-rc.d` , und speichern Sie die Änderungen.
  
   ``` BASH
   #!/bin/sh
   exit 101
   ```
  
2. Ausführungs Berechtigungen hinzufügen zu`/usr/sbin/policy-rc.d`
   ``` BASH
   chmod +x /usr/sbin/policy-rc.d
   ```
  
3. Führen Sie die folgenden Befehle aus:
   ``` BASH
   dpkg-divert --local --rename --add /sbin/initctl
   ln -s /bin/true /sbin/initctl
   ```
  
### <a name="error-0x80040306-on-installation"></a>Zeit 0x80040306 "bei Installation
Dies ist mit der Tatsache zu tun, dass die Legacy Konsole nicht unterstützt wird.
So deaktivieren Sie die Legacy Konsole:

1. Öffnen Sie "cmd. exe"
1. Klicken Sie mit der rechten Maustaste auf Titelleiste-> Eigenschaften-> deaktivieren Sie ältere Konsole verwenden.
1. Auf "OK" klicken

### <a name="error-0x80040154-after-windows-update"></a>Zeit 0x80040154 "nach Windows Update
Das Windows-Subsystem für Linux ist während eines Windows-Updates möglicherweise deaktiviert. Wenn dies der Fall ist, muss das Windows-Feature erneut aktiviert werden. Anweisungen zum Aktivieren des Windows-Subsystems für Linux finden Sie im [Installationshandbuch](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui).

### <a name="changing-the-display-language"></a>Ändern der Anzeige Sprache
Die WSL-Installation versucht, das Ubuntu-Gebiets Schema automatisch so zu ändern, dass es dem Gebiets Schema Ihrer Windows-Installation entspricht.  Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl ausführen, um das Ubuntu-Gebiets Schema zu ändern, nachdem die Installation abgeschlossen wurde.  Sie müssen bash. exe neu starten, damit diese Änderung wirksam wird.

Im folgenden Beispiel wird "locale" in "en-US" geändert:
``` BASH
sudo update-locale LANG=en_US.UTF8
```

### <a name="installation-issues-after-windows-system-restore"></a>Installationsprobleme nach der Windows-Systemwiederherstellung
1.  Löschen Sie `%windir%\System32\Tasks\Microsoft\Windows\Windows Subsystem for Linux` den Ordner. <br/>
  **Hinweis: Dies ist nicht der Fall, wenn das optionale Feature vollständig installiert ist und funktioniert.**
2.  Aktivieren Sie das optionale WSL-Feature (falls noch nicht geschehen).
3.  Neustart
4.  lxrun/Uninstall/Full
5.  Installieren von bash

### <a name="no-internet-access-in-wsl"></a>Kein Internet Zugriff in WSL
Einige Benutzer haben Probleme mit bestimmten Firewallanwendungen gemeldet, die den Internet Zugriff in WSL blockieren.  Die gemeldeten Firewalls lauten wie folgt:

1. Kaspersky
1. AVG
1. Avast

In einigen Fällen ermöglicht das Ausschalten der Firewall den Zugriff.  In einigen Fällen, in denen die Firewall einfach installiert ist, wird der Zugriff von blockiert.

### <a name="permission-denied-error-when-using-ping"></a>Berechtigungs Verweigerungs Fehler bei Verwendung von Ping.
#### <a name="anniversary-updatehttpsmsdnmicrosoftcomen-uscommandlinewslrelease_notesbuild-14388-to-windows-10-anniversary-update"></a>[Anniversary Update](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes#build-14388-to-windows-10-anniversary-update) 

Zum Ausführen von Ping in WSL sind Administrator Rechte in Windows erforderlich.  Zum Ausführen von Ping führen Sie bash unter Ubuntu unter Windows als Administrator aus, oder führen Sie bash. exe von einer cmd-/PowerShell-Eingabeaufforderung mit Administratorrechten aus.

#### <a name="build-14926httpsmsdnmicrosoftcomen-uscommandlinewslrelease_notesbuild-14926"></a>[Build 14926 +](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes#build-14926)
  Administrator Rechte sind nicht mehr erforderlich.

### <a name="bash-is-hung"></a>Bash ist nicht reagiert.
Wenn Sie mit Bash arbeiten, stellen Sie fest, dass bash nicht reagiert (oder blockiert) ist und nicht auf Eingaben antwortet, uns bei der Diagnose des Problems helfen, indem Sie ein Speicher Abbild erfassen und melden. Beachten Sie, dass diese Schritte zu einem Absturz Ihres Systems führt. Tun Sie dies nicht, wenn Sie damit nicht vertraut sind, oder speichern Sie Ihre Arbeit, bevor Sie dies tun.  <br/>
So erfassen Sie ein Speicher Abbild:
1. Ändern Sie den Typ des Speicher Abbilds in "Complete Memory Dump". Beachten Sie beim Ändern des dumptyps den aktuellen Typ.
2. Verwenden Sie die [Schritte](https://blogs.technet.microsoft.com/askpfeplat/2015/04/05/how-to-force-a-diagnostic-memory-dump-when-a-computer-hangs/) zum Konfigurieren von Abstürzen mithilfe der Tastatursteuerung.
3. Gibt den Absturz oder Deadlock zurück.
4. Abstürzen Sie das System mithilfe der Schlüssel Sequenz von (2).
5. Das System stürzt ab und sammelt das Speicher Abbild.
6. Nachdem das System neu gestartet wurde, melden Sie die Datei "Memory secure@microsoft.com. dmp" an. Der Standard Speicherort der Dumpdatei ist%SystemRoot%\Memory.dmp oder c:\WINDOWS\MEMORY.dmp, wenn C: das Systemlaufwerk ist. Beachten Sie in der e-Mail, dass das Abbild für das WSL-oder bash on Windows-Team gilt.
7. Stellen Sie den Speicher Abbild Speichertyp in der ursprünglichen Einstellung wieder her.

### <a name="check-your-build-number"></a>Überprüfen der Buildnummer

Um die Architektur des PCs und die Windows-Buildnummer zu ermitteln, öffnen Sie  
**Einstellungs** >  **System**Info > 

Suchen Sie nach den Feldern **Betriebs systembuild** und **Systemtyp** .  
    ![Screenshot der Felder "Build" und "Systemtyp"](media/system.png) 


Führen Sie Folgendes in PowerShell aus, um die Windows Server-Buildnummer zu ermitteln:  
``` PowerShell
systeminfo | Select-String "^OS Name","^OS Version"
```

### <a name="confirm-wsl-is-enabled"></a>Bestätigen, dass WSL aktiviert ist
Sie können überprüfen, ob das Windows-Subsystem für Linux aktiviert ist, indem Sie Folgendes in PowerShell ausführen:  
``` PowerShell
Get-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

### <a name="openssh-server-connection-issues"></a>OpenSSH-Server-Verbindungsprobleme
Fehler beim Versuch, den SSH-Server zu verbinden: "Die Verbindung wurde von 127.0.0.1 Port 22 geschlossen."
1. Stellen Sie sicher, dass der OpenSSH-Server ausgeführt wird:
   ``` BASH
   sudo service ssh status
   ```
   und Sie haben dieses Tutorial befolgt: https://help.ubuntu.com/lts/serverguide/openssh-server.html.en
2. Starten Sie den sshd-Dienst, und starten Sie sshd im Debugmodus:
   ``` BASH
   sudo service ssh stop
   sudo /usr/sbin/sshd -d
   ```
3. Überprüfen Sie die Start Protokolle, und stellen Sie sicher, dass die Host Schlüssel verfügbar sind, und es werden keine Protokollmeldungen wie:
   ```
   debug1: sshd version OpenSSH_7.2, OpenSSL 1.0.2g  1 Mar 2016
   debug1: key_load_private: incorrect passphrase supplied to decrypt private key
   debug1: key_load_public: No such file or directory
   Could not load host key: /etc/ssh/ssh_host_rsa_key
   debug1: key_load_private: No such file or directory
   debug1: key_load_public: No such file or directory
   Could not load host key: /etc/ssh/ssh_host_dsa_key
   debug1: key_load_private: No such file or directory
   debug1: key_load_public: No such file or directory
   Could not load host key: /etc/ssh/ssh_host_ecdsa_key
   debug1: key_load_private: No such file or directory
   debug1: key_load_public: No such file or directory
   Could not load host key: /etc/ssh/ssh_host_ed25519_key
   ```

Wenn solche Meldungen angezeigt werden und die Schlüssel unter `/etc/ssh/`fehlen, müssen Sie die Schlüssel neu generieren oder einfach & OpenSSH-Server installieren:
```BASH
sudo apt-get purge openssh-server
sudo apt-get install openssh-server
```

