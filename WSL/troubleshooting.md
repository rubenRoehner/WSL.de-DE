---
title: Problembehandlung bei der Windows-Susbystem für Linux
description: Enthält ausführliche Informationen zu häufigen Fehlern und Personen, die auftreten, Probleme bei der Ausführung von Linux in der Windows-Susbystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, ubuntu
author: scooley
ms.author: scooley
ms.date: 11/15/2017
ms.topic: article
ms.assetid: 6753f1b2-200e-49cc-93a5-4323e1117246
ms.custom: seodec18
ms.openlocfilehash: feb9e25da73eeb0d7f0cef4014221a42e2ca179b
ms.sourcegitcommit: db69625e26bc141ea379a830790b329e51ed466b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/13/2019
ms.locfileid: "67040843"
---
# <a name="troubleshooting-windows-subsystem-for-linux"></a>Problembehandlung bei Windows-Subsystem für Linux

### <a name="bash-loses-network-connectivity-once-connected-to-a-vpn"></a>Bash verliert die Netzwerkverbindung, die einmal mit einem VPN verbunden.

Wenn Bash nach dem Herstellen einer Verbindung mit einem VPN für Windows, über eine Netzwerkverbindung verliert, versuchen Sie diese problemumgehung aus in Bash. Diese problemumgehung können Sie die DNS-Auflösung über manuell überschreiben `/etc/resolv.conf`.

1. Notieren der DNS-Server das VPN aus dadurch `ipconfig.exe /all`
2. Erstellen einer Kopie der vorhandenen "resolv.conf" `sudo cp /etc/resolv.conf /etc/resolv.conf.new`
3. Die aktuelle resolv.con aufheben `sudo unlink /etc/resolv.conf`
4. `sudo mv /etc/resolv.conf.new /etc/resolv.conf`
5. Open `/etc/resolv.conf` und <br/>
   a. Löschen Sie die erste Zeile aus der Datei, die besagt, dass "\# dieser Datei durch WSL automatisch generiert wurde. Um die automatische Generierung von dieser Datei zu beenden, entfernen Sie diese Zeile. ". <br/>
   b. Fügen Sie den DNS-Eintrag oben als der erste Eintrag in der Liste der DNS-Server aus (1) hinzu. <br/>
   c. Schließen Sie die Datei an. <br/>

Nachdem Sie das VPN getrennt haben, müssen Sie die Änderungen zurücksetzen `/etc/resolv.conf`. Zu diesem Zweck führen Sie aus:
1. `cd /etc`
2. `sudo mv resolv.conf resolv.conf.new`
3. `sudo ln -s ../run/resolvconf/resolv.conf resolv.conf`

### <a name="starting-wsl-or-installing-a-distribution-returns-an-error-code"></a>WSL Installation oder einer Verteilungs wird ein Fehlercode zurückgegeben.

Führen Sie [diese Anweisungen](https://github.com/Microsoft/WSL/blob/master/CONTRIBUTING.md#8-detailed-logs) ausführliche Protokolle erfassen und melden ein Problem auf GitHub.

### <a name="updating-bash-on-ubuntu-on-windows"></a>Aktualisieren Bash auf Ubuntu unter Windows

Es gibt zwei Komponenten von Bash auf Ubuntu unter Windows, die aktualisiert werden können. 

1. Die Windows-Subsystem für Linux
  
   Aktualisieren diesen Teil Bash auf Ubuntu unter Windows können neuen Fehlerbehebungen sind in der [Anmerkungen zu dieser Version](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes). Stellen Sie sicher, dass Sie das Windows-Insider-Programm abonniert haben und der Build auf dem neuesten Stand ist. Sehen Sie sich für eine differenzierte Steuerung, darunter das Zurücksetzen Ihrer Ubuntu-Instanz die [Befehl Referenzseite](https://msdn.microsoft.com/en-us/commandline/wsl/reference).

2. Die Ubuntu-Benutzer-Binärdateien 

   Aktualisieren diesen Teil Bash auf Ubuntu unter Windows installiert alle Updates mit den Ubuntu-Benutzer-Binärdateien einschließlich Anwendungen, die Sie über apt-Get installiert haben. Die folgenden Befehle aus, aktualisieren Sie die Ausführung in Bash:
  
   1. `apt-get update`
   2. `apt-get upgrade`
  
### <a name="apt-get-upgrade-errors"></a>Apt-Get-Upgrade-Fehler
Einige Pakete verwenden Funktionen, die wir noch nicht implementiert haben. `udev`, z. B. wird nicht noch unterstützt und bewirkt, dass mehrere `apt-get upgrade` Fehler.

Zum Beheben von Problemen im Zusammenhang mit `udev`, befolgen Sie die folgenden Schritte aus:

1. Schreiben Sie folgenden Code zum `/usr/sbin/policy-rc.d` und die Änderungen zu speichern.
  
   ``` BASH
   #!/bin/sh
   exit 101
   ```
  
2. Hinzufügen Ausführungsberechtigungen `/usr/sbin/policy-rc.d`
   ``` BASH
   chmod +x /usr/sbin/policy-rc.d
   ```
  
3. Führen Sie die folgenden Befehle
   ``` BASH
   dpkg-divert --local --rename --add /sbin/initctl
   ln -s /bin/true /sbin/initctl
   ```
  
### <a name="error-0x80040306-on-installation"></a>"Fehler: 0x80040306 "in-Installation
Dies hat, führen mit der Tatsache, dass wir keine legacykonsole unterstützen.
So deaktivieren legacy-Konsole ein:

1. Öffnen von cmd.exe
1. Klicken Sie mit der rechten Maustaste auf Title bar -> Eigenschaften -> legacykonsole verwenden deaktivieren
1. Auf "OK" klicken

### <a name="error-0x80040154-after-windows-update"></a>"Fehler: 0 x 80040154 "nach dem update von Windows
Das Windows-Subsystem für Linux-Funktion möglicherweise deaktiviert, während eines Windows-Updates. In diesem Fall muss das Windows-Feature erneut aktiviert werden. Anweisungen zum Aktivieren der Windows-Subsystem für Linux Sie in finden der [Installationshandbuch](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui).

### <a name="changing-the-display-language"></a>Ändern der Anzeigesprache
Installieren von WSL versucht, die automatisch das Ubuntu-Gebietsschema entsprechend das Gebietsschema des der Windows-Installation zu ändern.  Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl, um die Ubuntu-Benutzergebietsschema ändern, nachdem die Installation abgeschlossen ist ausführen.  Sie müssen bash.exe für diese Änderung wirksam wird neu zu starten.

Das folgenden Beispiel ändert sich auf dem Gebietsschema En-US:
``` BASH
sudo update-locale LANG=en_US.UTF8
```

### <a name="installation-issues-after-windows-system-restore"></a>Probleme bei der Installation nach Windows-Systemwiederherstellung
1.  Löschen der `%windir%\System32\Tasks\Microsoft\Windows\Windows Subsystem for Linux` Ordner. <br/>
  **Hinweis: Verwenden Sie keine, wenn das optionale Feature vollständig installiert wurde und funktioniert.**
2.  Aktivieren Sie die optionale WSL-Funktion (falls noch nicht geschehen)
3.  Neustart
4.  Lxrun / uninstall/vollständiges
5.  Installieren von bash

### <a name="no-internet-access-in-wsl"></a>Kein Zugriff auf das Internet in WSL
Einige Benutzer haben Probleme mit der bestimmte Firewall-Anwendungen, die Zugriff auf das Internet in WSL blockieren gemeldet.  Die Firewalls, die gemeldet werden:

1. Kaspersky
1. AVG
1. Avast

In einigen Fällen können durch das Deaktivieren der Firewalls für den Zugriff.  In einigen Fällen sucht das einfach dadurch, dass die installierte Firewall zum Blockieren des Zugriffs.

### <a name="permission-denied-error-when-using-ping"></a>Berechtigung verweigert bei Verwendung von ping
#### <a name="anniversary-updatehttpsmsdnmicrosoftcomen-uscommandlinewslreleasenotesbuild-14388-to-windows-10-anniversary-update"></a>[Anniversary-Update](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes#build-14388-to-windows-10-anniversary-update) 

Berechtigungen in Windows sind zum Ausführen von Ping in WSL erforderlich.  Führen Sie Ping, Ausführen von Bash unter Ubuntu unter Windows als Administrator oder bash.exe einer CMD/PowerShell-Eingabeaufforderung mit Administratorrechten ausführen.

#### <a name="build-14926httpsmsdnmicrosoftcomen-uscommandlinewslreleasenotesbuild-14926"></a>[Build 14926+](https://msdn.microsoft.com/en-us/commandline/wsl/release_notes#build-14926)
  Administratorrechte mehr erforderlich.

### <a name="bash-is-hung"></a>Bash ist nicht reagiert.
Wenn bei der Arbeit mit Bash, Sie finden, Bash hängen geblieben ist (oder Deadlocks) und reagiert nicht auf Eingaben, helfen Sie uns, das Problem zu diagnostizieren, indem sammeln und melden ein Speicherabbild. Beachten Sie, dass diese Schritte das System abstürzt. Verwenden Sie keine Wenn Sie nicht vertraut sind, oder speichern Sie Ihre Arbeit, bevor Sie auf diese Weise.  <br/>
Um ein Speicherabbild sammeln:
1. Ändern Sie den Speichertyp für die Sicherung in "vollständiges Speicherabbild" ein. Nehmen Sie beim Ändern des Dump-Typs, notieren Sie den aktuellen Typ.
2. Verwenden der [Schritte](https://blogs.technet.microsoft.com/askpfeplat/2015/04/05/how-to-force-a-diagnostic-memory-dump-when-a-computer-hangs/) Absturz konfigurieren mithilfe der Tastatur steuern.
3. Reproduktion, die nicht mehr reagiert oder einen Deadlock.
4. Stürzt ab, das System über die Tastenkombination von (2).
5. Das System stürzt ab und Speicherabbild erfassen.
6. Sobald das System neu startet, melden die memory.dmp zu secure@microsoft.com. Der Standardspeicherort der Dumpdatei ist %SystemRoot%\memory.dmp oder C:\Windows\memory.dmp, wenn c das Systemlaufwerk ist. In der e-Mail, beachten Sie, dass das Speicherabbild für die WSL oder Bash für Windows-Team.
7. Stellen Sie den Speichertyp für die Sicherung auf die ursprüngliche Einstellung wieder her.

### <a name="check-your-build-number"></a>Überprüfen Sie Ihre Buildnummer

Öffnen Sie, um herauszufinden, dass der PC Architektur und Windows-Buildnummer  
**Einstellungen** > **System** > **zu**

Suchen Sie nach der **Betriebssystembuild** und **Systemtyp** Felder.  
    ![Screenshot des erstellen und Typ-Felder](media/system.png) 


Um Ihre Windows Server-Build-Nummer zu suchen, führen Sie Folgendes in PowerShell aus:  
``` PowerShell
systeminfo | Select-String "^OS Name","^OS Version"
```

### <a name="confirm-wsl-is-enabled"></a>Vergewissern Sie sich, dass WSL aktiviert ist
Sie können bestätigen, dass die Windows-Subsystem für Linux durch Ausführen des folgenden Befehls in PowerShell aktiviert ist:  
``` PowerShell
Get-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

### <a name="openssh-server-connection-issues"></a>OpenSSH-Server-Verbindungsprobleme
Ihre SSH-Server eine Verbindung herstellen möchten, ist mit folgendem Fehler fehlgeschlagen: "Verbindung beendet durch 127.0.0.1 port 22".
1. Stellen Sie sicher, dass Ihre OpenSSH-Server ausgeführt wird:
   ``` BASH
   sudo service ssh status
   ```
   und Sie in diesem Tutorial befolgt haben: https://help.ubuntu.com/lts/serverguide/openssh-server.html.en
2. Beenden Sie den Sshd-Dienst aus, und starten Sie Sshd im Debugmodus befindet:
   ``` BASH
   sudo service ssh stop
   sudo /usr/sbin/sshd -d
   ```
3. Überprüfen Sie die startaufgabenprotokolle, und stellen Sie sicher für Host-Schlüssel verfügbar sind und keine protokollmeldungen wie angezeigt werden:
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

Wenn Sie diese Nachrichten sehen und die Schlüssel unter fehlen `/etc/ssh/`, müssen Sie den Schlüssel neu generieren oder einfach löschen & Openssh-Server zu installieren:
```BASH
sudo apt-get purge openssh-server
sudo apt-get install openssh-server
```

