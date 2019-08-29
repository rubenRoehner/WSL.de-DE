---
title: Verwalten von Linux-Distributionen
description: Referenz zum Auflisten und Konfigurieren mehrerer Linux-Distributionen, die auf dem Windows-Subsystem für Linux ausgeführt werden.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, windowssubsystem, Ubuntu, WSL. conf, wslconfig
author: scooley
ms.author: scooley
ms.date: 02/7/2018
ms.topic: article
ms.assetid: 7ca59bd7-d9d3-4f6d-8b92-b8faa9bcf250
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: ca65cf6fde3e0ba4750ffc44f5aec542be6cfabf
ms.sourcegitcommit: 7af6b7a3f8cfa66cb25115bc26f44aa64ef22811
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2019
ms.locfileid: "70122705"
---
# <a name="manage-and-configure-windows-subsystem-for-linux"></a>Verwalten und Konfigurieren des Windows-Subsystems für Linux

> Gilt für Windows 10 Fall Creators Update und höher.  Weitere Informationen zu neuen Verwaltungs Features und zum Ausführen mehrerer Linux-Distributionen aus dem Microsoft Store finden Sie in unserem aktualisierten [Installationshandbuch](./install_guide.md) .

## <a name="ways-to-run-wsl"></a>Möglichkeiten zum Ausführen von WSL

Es gibt viele Möglichkeiten, Linux mit dem Windows-Subsystem für Linux auszuführen.

1. `[distro]`Zum Beispiel`ubuntu`
1. `wsl.exe` oder `bash.exe`
1. `wsl [command]` oder `bash -c [command]`

Welche Methode Sie verwenden sollten, hängt davon ab, was Sie gerade tun.

### <a name="launch-wsl-by-distribution"></a>Starten von WSL nach Verteilung

Durch das Ausführen einer Verteilung mit der IT-spezifischen Anwendung wird diese Distribution im eigenen Konsolenfenster gestartet.

![Starten von WSL über das Startmenü](media/start-launch.png)

Dies entspricht dem Klicken auf "starten" im Microsoft Store.

![Starten von WSL aus dem Microsoft Store](media/store-launch.png)

Sie können die Verteilung auch über die Befehlszeile ausführen, indem `[distribution].exe`Sie ausführen.

Der Nachteil der Ausführung einer Verteilung von der Befehlszeile auf diese Weise besteht darin, dass das Arbeitsverzeichnis automatisch vom aktuellen Verzeichnis in das Basisverzeichnis der Distribution geändert wird.

**Beispiel:**

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> ubuntu

scooley@scooley-elmer:~$ pwd
/home/scooley
scooley@scooley-elmer:~$ exit
logout

PS C:\Users\sarah>
```

### <a name="wsl-and-wsl-command"></a>WSL und WSL [Befehl]

Die beste Methode zum Ausführen von WSL von der Befehlszeile aus `wsl.exe`ist die Verwendung von.

**Beispiel:**

```console
PS C:\Users\sarah> pwd

Path
----
C:\Users\sarah

PS C:\Users\sarah> wsl

scooley@scooley-elmer:/mnt/c/Users/sarah$ pwd
/mnt/c/Users/sarah
```

Das aktuelle Arbeits `wsl` Verzeichnis wird nicht nur auf dem neuesten Stand gehalten, sondern Sie können auch einen einzelnen Befehl entlang von Windows-Befehlszeilen ausführen.

**Beispiel:**

```console
PS C:\Users\sarah> Get-Date

Sunday, March 11, 2018 7:54:05 PM

PS C:\Users\sarah> wsl
scooley@scooley-elmer:/mnt/c/Users/sarah$ date
Sun Mar 11 19:56:57 DST 2018
scooley@scooley-elmer:/mnt/c/Users/sarah$ exit
logout

PS C:\Users\sarah> wsl date
Sun Mar 11 19:55:47 DST 2018
```

**Beispiel:**

```console
PS C:\Users\sarah> Get-VM

Name            State CPUUsage(%) MemoryAssigned(M) Uptime   Status
----            ----- ----------- ----------------- ------   ------
Server17093     Off   0           0                 00:00:00 Opera...
Ubuntu          Off   0           0                 00:00:00 Opera...
Ubuntu (bionic) Off   0           0                 00:00:00 Opera...
Windows         Off   0           0                 00:00:00 Opera...


PS C:\Users\sarah> Get-VM | wsl grep "Ubuntu"
Ubuntu          Off   0           0                 00:00:00 Opera...
Ubuntu (bionic) Off   0           0                 00:00:00 Opera...
PS C:\Users\sarah>
```


## <a name="managing-multiple-linux-distributions"></a>Verwalten mehrerer Linux-Distributionen

### <a name="windows-10-version-1903-and-later"></a>Windows 10, Version 1903 und höher

Sie können verwenden `wsl.exe` , um die Verteilungen im Windows-Subsystem für Linux (WSL) zu verwalten, einschließlich der Auflistung verfügbarer Verteilungen, dem Festlegen einer Standardverteilung und der Deinstallieren von Verteilungen.

Jede Linux-Distribution verwaltet unabhängig seine eigenen Konfigurationen. Führen `[distro.exe] /?`Sie aus, um Verteilungs spezifische Befehle anzuzeigen.  Beispiel: `ubuntu /?`.

#### <a name="list-distributions"></a>Verteilungen auflisten

`wsl -l`,`wsl --list`  
Listet verfügbare Linux-Distributionen für WSL auf.  Wenn eine Distribution aufgeführt ist, ist Sie installiert und einsatzbereit.

`wsl --list --all`   
Listet alle Verteilungen auf, einschließlich derjenigen, die derzeit nicht verwendbar sind.  Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.  

`wsl --list --running`   
Listet alle Verteilungen auf, die zurzeit ausgeführt werden.

#### <a name="set-a-default-distribution"></a>Festlegen einer Standardverteilung

Die standardmäßige WSL-Verteilung ist die, die ausgeführt wird `wsl` , wenn Sie in einer Befehlszeile ausführen.

`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`

Legt die Standardverteilung auf `<DistributionName>`fest.

**Beispiel:**  
`wsl -s Ubuntu`legt die Standardverteilung auf Ubuntu fest.  Wenn die Anwendung ausgeführt `wsl npm init` wird, wird Sie jetzt in Ubuntu ausgeführt.  Wenn ich das `wsl` ausführen, wird eine Ubuntu-Sitzung geöffnet.

#### <a name="unregister-and-reinstall-a-distribution"></a>Aufheben der Registrierung und Neuinstallation einer Verteilung

Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.  Die WSL-Konfiguration ermöglicht die Registrierung/Deinstallieren von Distributionen.

Durch die Aufhebung der Registrierung können auch Verteilungen erneut installiert werden.

> **Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Software, die dieser Verteilung zugeordnet sind, dauerhaft verloren.  Bei der erneuten Installation aus dem Speicher wird eine saubere Kopie der Verteilung installiert.

`wsl --unregister <DistributionName>`  
Hebt die Registrierung der Verteilung bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.

Beispiel: `wsl --unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Verteilungen entfernen.  Beim Ausführen `wsl --list` wird der Dienst nicht aufgelistet.

Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie "starten" aus.

#### <a name="run-as-a-specific-user"></a>Ausführen als bestimmter Benutzer

`wsl -u <Username>`, `wsl --user <Username>`

Führen Sie WSL als den angegebenen Benutzer aus. Beachten Sie, dass der Benutzer in der WSL-Distribution vorhanden sein muss.

#### <a name="run-a-specific-distribution"></a>Ausführen einer bestimmten Verteilung

`wsl --d <DistributionName>`, `wsl --distribution <DistributionName>`

Führen Sie eine angegebene Distribution von WSL aus, die zum Senden von Befehlen an eine bestimmte Distribution verwendet werden kann, ohne den Standardwert ändern zu müssen.

### <a name="versions-earlier-than-windows-10-version-1903"></a>Frühere Versionen als Windows 10, Version 1903

WSL config (`wslconfig.exe`) ist ein Befehlszeilen Tool zum Verwalten von Linux-Distributionen, die unter dem Windows-Subsystem für Linux (WSL) ausgeführt werden.  Damit können Sie verfügbare Distributionen auflisten, eine Standardverteilung festlegen und Verteilungen deinstallieren.

Während die WSL-Konfiguration für Einstellungen nützlich ist, die Verteilungen überspannen oder koordinieren, verwaltet jede Linux-Distribution unabhängig seine eigenen Konfigurationen.  Führen `[distro.exe] /?`Sie aus, um Verteilungs spezifische Befehle anzuzeigen.  Beispiel: `ubuntu /?`.

Um alle verfügbaren Optionen für wslconfig anzuzeigen, führen Sie Folgendes aus:`wslconfig /?`

```console
wslconfig.exe
Performs administrative operations on Windows Subsystem for Linux

Usage:
    /l, /list [/all] - Lists registered distributions.
        /all - Optionally list all distributions, including distributions that
               are currently being installed or uninstalled.
    /s, /setdefault <DistributionName> - Sets the specified distribution as the default.
    /u, /unregister <DistributionName> - Unregisters a distribution.
```

#### <a name="list-distributions"></a>Verteilungen auflisten

`wslconfig /list`  
Listet verfügbare Linux-Distributionen für WSL auf.  Wenn eine Distribution aufgeführt ist, ist Sie installiert und einsatzbereit.

`wslconfig /list /all`  
Listet alle Verteilungen auf, einschließlich derjenigen, die derzeit nicht verwendbar sind.  Sie werden möglicherweise gerade installiert, deinstalliert oder sind beschädigt.  

#### <a name="set-a-default-distribution"></a>Festlegen einer Standardverteilung

Die standardmäßige WSL-Verteilung ist die, die ausgeführt wird `wsl` , wenn Sie in einer Befehlszeile ausführen.

`wslconfig /setdefault <DistributionName>`

Legt die Standardverteilung auf `<DistributionName>`fest.

**Beispiel:**  
`wslconfig /setdefault Ubuntu`legt die Standardverteilung auf Ubuntu fest.  Wenn die Anwendung ausgeführt `wsl npm init` wird, wird Sie jetzt in Ubuntu ausgeführt.  Wenn ich das `wsl` ausführen, wird eine Ubuntu-Sitzung geöffnet.

#### <a name="unregister-and-reinstall-a-distribution"></a>Aufheben der Registrierung und Neuinstallation einer Verteilung

Obwohl Linux-Distributionen über den Microsoft Store installiert werden können, können Sie nicht über den Store deinstalliert werden.  Die WSL-Konfiguration ermöglicht die Registrierung/Deinstallieren von Distributionen.

Durch die Aufhebung der Registrierung können auch Verteilungen erneut installiert werden.

> **Vorsicht:** Nachdem die Registrierung aufgehoben wurde, gehen alle Daten, Einstellungen und Software, die dieser Verteilung zugeordnet sind, dauerhaft verloren.  Bei der erneuten Installation aus dem Speicher wird eine saubere Kopie der Verteilung installiert.

`wslconfig /unregister <DistributionName>`  
Hebt die Registrierung der Verteilung bei WSL auf, damit Sie erneut installiert oder bereinigt werden kann.

Beispiel: `wslconfig /unregister Ubuntu` würde Ubuntu aus den in WSL verfügbaren Verteilungen entfernen.  Beim Ausführen `wslconfig /list` wird der Dienst nicht aufgelistet.

Zum erneuten Installieren suchen Sie die Distribution im Microsoft Store, und wählen Sie "starten" aus.

## <a name="set-wsl-launch-settings"></a>Festlegen der WSL-Start Einstellungen

> **Verfügbar in Windows Insider Build 17093 und höher**

Konfigurieren Sie automatisch bestimmte Funktionen in WSL, die jedes Mal angewendet werden, wenn Sie das `wsl.conf`Subsystem mithilfe von starten. 

Zurzeit umfasst dies automatische Optionen und Netzwerkkonfiguration.

`wsl.conf`befindet sich in jeder Linux-Distribution `/etc/wsl.conf`in. Wenn die Datei nicht vorhanden ist, können Sie Sie selbst erstellen. WSL erkennt das vorhanden sein der Datei und liest ihren Inhalt. Wenn die Datei fehlt oder falsch formatiert ist (d. h. eine falsche Markup Formatierung), wird WSL weiterhin normal gestartet.

Im folgenden finden Sie `wsl.conf` eine Beispieldatei, die Sie ihren Distributionen hinzufügen können:

```console
# Enable extra metadata options by default
[automount]
enabled = true
root = /windir/
options = "metadata,umask=22,fmask=11"
mountFsTab = false

# Enable DNS – even though these are turned on by default, we’ll specify here just to be explicit.
[network]
generateHosts = true
generateResolvConf = true
```

### <a name="configuration-options"></a>Konfigurationsoptionen

In Übereinstimmung mit ini-Konventionen werden Schlüssel in einem Abschnitt deklariert. 

WSL unterstützt zwei Abschnitte `automount` : `network`und.

#### <a name="automount"></a>automatischen Bereitstellung

Sektions`[automount]`


| Key        | Wert                          | default      | Anmerkungen                                                                                                                                                                                                                                                                                                                          |
|:-----------|:-------------------------------|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| aktiviert    | boolean                        | true         | `true`verursacht Festplattenlaufwerke (d. h. `C:/`oder `D:/`) für die automatische Bereitstellung mit drvfs `/mnt`unter.  `false`bedeutet, dass Laufwerke nicht automatisch bereitgestellt werden, aber Sie können Sie trotzdem manuell `fstab`oder über bereitstellen.                                                                                                             |
| mountfstab | boolean                        | true         | `true`auf `/etc/fstab` dem WSL-Start zu verarbeitende Sätze. bei "/etc/fstab" handelt es sich um eine Datei, in der Sie andere Dateisysteme wie eine SMB-Freigabe deklarieren können. Daher können Sie diese Dateisysteme beim Start automatisch in WSL einbinden.                                                                                                                |
| fasst       | Zeichenfolge                         | `/mnt/`      | Legt das Verzeichnis fest, in dem Festplattenlaufwerke automatisch bereitgestellt werden. Wenn Sie z. b. ein Verzeichnis in WSL bei `/windir/` haben und Sie als Stammverzeichnis angeben, erwarten Sie, dass die Festplattenlaufwerke unter`/windir/c`                                                                                              |
| options    | durch Trennzeichen getrennte Liste von Werten | leere Zeichenfolge | Dieser Wert wird an die Standard Zeichenfolge der drvfs-Einfügeoptionen angehängt. **Es können nur drvfs-spezifische Optionen angegeben werden.** Optionen, die die Einbindungs Binärdatei normalerweise in ein Flag analysieren würde, werden nicht unterstützt. Wenn Sie diese Optionen explizit angeben möchten, müssen Sie jedes Laufwerk, für das Sie dies tun möchten, in "/etc/fstab" einschließen. |

Standardmäßig legt WSL die UID und die gid auf den Wert des Standard Benutzers fest (in Ubuntu-Distribution wird der Standardbenutzer mit UID = 1000, gid = 1000 erstellt). Wenn der Benutzer eine GID-oder UID-Option explizit über diesen Schlüssel angibt, wird der zugehörige Wert überschrieben. Andernfalls wird der Standardwert immer angefügt.

**Hinweis**: Diese Optionen werden als Einstellungsoptionen für alle automatisch bereitgestellten Laufwerke angewendet. Verwenden Sie stattdessen "/etc/fstab", um die Optionen für ein bestimmtes Laufwerk zu ändern.

#### <a name="network"></a>Netzwerk

Abschnitts Bezeichnung:`[network]`

| Key | Wert | default | Anmerkungen|
|:----|:----|:----|:----|
| generatehosts | boolean | `true` | `true`legt fest, dass WSL generiert `/etc/hosts`wird. Die `hosts` Datei enthält eine statische Zuordnung der Hostnamen der entsprechenden IP-Adresse. |
| generateresolvconf | boolean | `true` | `true`Legen Sie WSL auf `/etc/resolv.conf`Generate fest. Die `resolv.conf` enthält eine DNS-Liste, die einen angegebenen Hostnamen in seine IP-Adresse auflösen können. | 

#### <a name="interop"></a>Interop

Abschnitts Bezeichnung:`[interop]`

Diese Optionen sind in Insider Build 17713 und höher verfügbar.

| Key | Wert | default | Anmerkungen|
|:----|:----|:----|:----|
| aktiviert | boolean | `true` | Durch Festlegen dieses Schlüssels wird festgelegt, ob WSL das Starten von Windows-Prozessen unterstützt. |
| appendwindowspath | boolean | `true` | Wenn dieser Schlüssel festgelegt wird, wird festgelegt, ob WSL der $PATH-Umgebungsvariablen Windows-Pfad Elemente hinzufügt. | 
