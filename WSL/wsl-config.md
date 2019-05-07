---
title: Verwalten von Linux-Distributionen
description: Verweisen auf auflisten und Konfigurieren von mehreren Linux-Distributionen, die auf dem Windows-Subsystem für Linux ausführen.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, wsl.conf, wslconfig
author: scooley
ms.author: scooley
ms.date: 02/7/2018
ms.topic: article
ms.assetid: 7ca59bd7-d9d3-4f6d-8b92-b8faa9bcf250
ms.custom: seodec18
ms.openlocfilehash: c806552750f413fcb75f989d868a57cc939af64a
ms.sourcegitcommit: ae0956bc0543b1c45765f3620ce9a55c9afe55da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/18/2019
ms.locfileid: "59063498"
---
# <a name="manage-and-configure-windows-subsystem-for-linux"></a>Verwalten und Konfigurieren von Windows-Subsystem für Linux

> Gilt für Windows 10 Fall Creators Update und höher.  Finden Sie in unserer aktualisierten [Installationshandbuch](./install_guide.md) , neue Features zu starten, Ausführen von mehreren Linux-Distributionen aus dem Windows Store.

## <a name="ways-to-run-wsl"></a>Möglichkeiten zum Ausführen von WSL

Es gibt viele Möglichkeiten zum Ausführen von Linux mit dem Windows-Subsystem für Linux.

1. `[distro]` ie `ubuntu`
1. `wsl.exe` oder `bash.exe`
1. `wsl [command]` oder `bash -c [command]`

Welche Methode Sie verwenden sollten, hängt davon ab, was Sie tun.

### <a name="launch-wsl-by-distribution"></a>Starten Sie von der Verteilung von WSL

Eine Distribution mit distributionsspezifische Anwendung ausführt, wird dieser Verteilung in seinem eigenen Konsolenfenster gestartet.

![Starten Sie im Startmenü WSL](media/start-launch.png)

Es ist identisch mit dem "Start" klicken, in der Windows Store.

![Starten Sie die WSL aus dem Windows Store](media/store-launch.png)

Sie können auch die Verteilung über die Befehlszeile ausführen, mit `[distribution].exe`.

Der Nachteil der Ausführung einer Verteilungs über die Befehlszeile auf diese Weise ist, dass es automatisch Ihrem Arbeitsverzeichnis aus dem aktuellen Verzeichnis in der Distribution-Basisverzeichnis ändert.

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

### <a name="wsl-and-wsl-command"></a>Wsl und Wsl [Befehl]

Die beste Möglichkeit zum Ausführen von WSL über die Befehlszeile verwendet `wsl.exe`.

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

Nicht nur `wsl` behalten Sie das aktuelle Arbeitsverzeichnis vorhanden, sie können einen einzelnen Befehl auf der Seite Windows-Befehle ausführen.

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


## <a name="managing-multiple-linux-distributions"></a>Verwalten von mehreren Linux-Distributionen

### <a name="windows-10-version-1903-and-later"></a>Windows 10-Version 1903 und höher

Sie können `wsl.exe` Ihre Distributionen im Windows-Subsystem für Linux (WSL), einschließlich der verfügbare Distributionen auflisten, Festlegen von einer standardverteilung und Deinstallieren von Verteilungen zu verwalten.

Jede Linux-Distribution verwaltet unabhängig voneinander eine eigene Konfigurationen. Führen Sie zum Anzeigen der Verteilung spezifischen Befehle `[distro.exe] /?`.  Beispiel: `ubuntu /?`.

#### <a name="list-distributions"></a>Liste von Verteilungen

`wsl -l` , `wsl --list`  
Listet die verfügbaren Linux-Distributionen für WSL verfügbar.  Wenn eine Verteilung aufgeführt ist, wird installiert und bereit für die Verwendung.

`wsl --list --all`   
Listet alle Verteilungen, einschließlich jener, die nicht derzeit verwendbar sind.  Sie möglicherweise während der Installation, Deinstallation oder in einem fehlerhaften Zustand befinden.  

`wsl --list --running`   
Listet alle Verteilungen, die derzeit ausgeführt werden.

#### <a name="set-a-default-distribution"></a>Legen Sie eine standardverteilung

Die standardverteilung von WSL ist diejenige, die ausgeführt, beim Ausführen von wird `wsl` in einer Befehlszeile.

`wsl -s <DistributionName>`, `wsl --setdefault <DistributionName>`

Legt die standardverteilung auf `<DistributionName>`.

**Beispiel:**  
`wsl -s Ubuntu` Meine standardverteilung würde auf Ubuntu festgelegt werden.  Wenn ich jetzt ausführen `wsl npm init` wird es in Ubuntu ausgeführt.  Wenn ich ausführe `wsl` eine Ubuntu-Sitzung wird geöffnet.

#### <a name="unregister-and-reinstall-a-distribution"></a>Aufheben der Registrierung, und installieren Sie eine Verteilung neu.

Speichern bei Linux, auf die Verteilungen, die durch die Windows installiert werden können, sie können nicht deinstalliert werden, über den Store.  WSL Config können Verteilungen, deren Registrierung aufgehoben/deinstalliert werden.

Aufheben der Registrierung können auch Distributionen neu installiert werden.

> **Vorsicht:** Nach deren Registrierung aufgehoben wird, werden alle Daten, Einstellungen und Software, die dieser Verteilung zugeordneten dauerhaft verloren.  Neu aus dem Store installieren, installieren Sie eine Neuinstallation der Verteilung.

`wsl --unregister <DistributionName>`  
Hebt die Registrierung auf der Verteilung von WSL, damit sie neu installiert oder bereinigt werden kann.

Zum Beispiel: `wsl -unregister Ubuntu` Ubuntu die Verteilungen in WSL verfügbar entfernt.  Beim Ausführen `wsl --list` wird es nicht aufgeführt werden.

Suchen Sie die Verteilung in der Windows Store, und wählen Sie die "Start", um erneut zu installieren.

#### <a name="run-as-a-specific-user"></a>Führen Sie als ein bestimmter Benutzer

`wsl -u <Username>`, `wsl --user <Username>`

Führen Sie WSL, als der angegebene Benutzer. Beachten Sie, dass dieser Benutzer in der Verteilung WSL vorhanden sein muss.

#### <a name="run-a-specific-distribution"></a>Führen Sie eine bestimmte Verteilung

`wsl --d <DistributionName>`, `wsl --distribution <DistributionName>`

Führen Sie eine angegebene Verteilung von WSL, können verwendet werden, um Befehle an einer bestimmten Verteilung zu senden, ohne den Standardwert zu ändern.

### <a name="versions-earlier-than-windows-10-version-1903"></a>Versionen vor Windows 10, Version 1903

WSL Config (`wslconfig.exe`) ist ein Befehlszeilentool zum Verwalten von Linux-Distributionen, die auf dem Windows-Subsystem für Linux (WSL) ausgeführt wird.  Sie können Sie die Liste der verfügbaren Distributionen, legen Sie eine standardverteilung und Deinstallieren von Verteilungen.

Während die WSL-Konfiguration für Einstellungen hilfreich ist, umfassen oder Verteilungen zu koordinieren, verwaltet jede Linux-Distribution unabhängig eigene Konfigurationen.  Führen Sie zum Anzeigen der Verteilung spezifischen Befehle `[distro.exe] /?`.  Beispiel: `ubuntu /?`.

Um alle verfügbaren Optionen für Wslconfig anzuzeigen, führen Sie Folgendes aus:  `wslconfig /?`

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

#### <a name="list-distributions"></a>Liste von Verteilungen

`wslconfig /list`  
Listet die verfügbaren Linux-Distributionen für WSL verfügbar.  Wenn eine Verteilung aufgeführt ist, wird installiert und bereit für die Verwendung.

`wslconfig /list /all`  
Listet alle Verteilungen, einschließlich jener, die nicht derzeit verwendbar sind.  Sie möglicherweise während der Installation, Deinstallation oder in einem fehlerhaften Zustand befinden.  

#### <a name="set-a-default-distribution"></a>Legen Sie eine standardverteilung

Die standardverteilung von WSL ist diejenige, die ausgeführt, beim Ausführen von wird `wsl` in einer Befehlszeile.

`wslconfig /setdefault <DistributionName>`

Legt die standardverteilung auf `<DistributionName>`.

**Beispiel:**  
`wslconfig /setdefault Ubuntu` Meine standardverteilung würde auf Ubuntu festgelegt werden.  Wenn ich jetzt ausführen `wsl npm init` wird es in Ubuntu ausgeführt.  Wenn ich ausführe `wsl` eine Ubuntu-Sitzung wird geöffnet.

#### <a name="unregister-and-reinstall-a-distribution"></a>Aufheben der Registrierung, und installieren Sie eine Verteilung neu.

Speichern bei Linux, auf die Verteilungen, die durch die Windows installiert werden können, sie können nicht deinstalliert werden, über den Store.  WSL Config können Verteilungen, deren Registrierung aufgehoben/deinstalliert werden.

Aufheben der Registrierung können auch Distributionen neu installiert werden.

> **Vorsicht:** Nach deren Registrierung aufgehoben wird, werden alle Daten, Einstellungen und Software, die dieser Verteilung zugeordneten dauerhaft verloren.  Neu aus dem Store installieren, installieren Sie eine Neuinstallation der Verteilung.

`wslconfig /unregister <DistributionName>`  
Hebt die Registrierung auf der Verteilung von WSL, damit sie neu installiert oder bereinigt werden kann.

Zum Beispiel: `wslconfig /unregister Ubuntu` Ubuntu die Verteilungen in WSL verfügbar entfernt.  Beim Ausführen `wslconfig /list` wird es nicht aufgeführt werden.

Suchen Sie die Verteilung in der Windows Store, und wählen Sie die "Start", um erneut zu installieren.

## <a name="set-wsl-launch-settings"></a>Starteinstellungen für den WSL festlegen

> **In Windows-Insider-Build-17093 und höher verfügbar**

Konfigurieren Sie automatisch bestimmte Funktionen in WSL, die jedes Mal, wenn Sie das Subsystem mit starten angewendet werden `wsl.conf`. 

Rechts umfasst dies nun, automatische Optionen und Netzwerkkonfiguration.

`wsl.conf` befindet sich im einzelnen Linux-Distribution `/etc/wsl.conf`. Wenn die Datei nicht vorhanden ist, können Sie ihn selbst erstellen. WSL erkennt, dass das Vorhandensein der Datei und liest den Inhalt. Wenn die Datei fehlt oder ist falsch formatiert ist (d. h. eine ungültige Markup formatieren), WSL weiterhin normal zu starten.

Hier ist ein Beispiel `wsl.conf` Datei, die Sie in Ihrem Distributionen hinzufügen können:

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

Gemäß der INI-Konventionen werden die Schlüssel unter einem Abschnitt deklariert. 

WSL unterstützt zwei Abschnitte: `automount` und `network`.

#### <a name="automount"></a>Automatische Bereitstellung

Abschnitt: `[automount]`


| key        | Wert                          | default      | Anmerkungen zu dieser Version                                                                                                                                                                                                                                                                                                                          |
|:-----------|:-------------------------------|:-------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| enabled    | boolean                        | true         | `true` bewirkt, dass Festplattenlaufwerke (d.h.) `C:/` oder `D:/`) mit DrvFs unter automatisch eingebunden werden `/mnt`.  `false` bedeutet, dass Laufwerke wird nicht automatisch bereitgestellt werden, aber Sie dennoch bereitstellen können, manuell oder über `fstab`.                                                                                                             |
| mountFsTab | boolean                        | true         | `true` Legt `/etc/fstab` zu verarbeitenden WSL starten. / etc/fstab handelt es sich um eine Datei, in dem Sie andere Dateisysteme, wie eine SMB-Freigabe deklarieren können. Daher können Sie diese Dateisysteme in WSL beim Start automatisch nach oben bereitstellen.                                                                                                                |
| Stammverzeichnis       | Zeichenfolge                         | `/mnt/`      | Legt das Verzeichnis, in denen feste Laufwerke automatisch eingebunden werden. Für, wenn Sie z. B. ein Verzeichnis in WSL am `/windir/` und angeben, dass als Wurzel an, Sie Ihre Festplattenlaufwerke bereitgestellt erwarten: `/windir/c`                                                                                              |
| Optionen    | durch Trennzeichen getrennte Liste von Werten | Leere Zeichenfolge | Dieser Wert wird an die standardmäßige DrvFs Mount-Optionen-Zeichenfolge angefügt. **Nur DrvFs-spezifische Optionen können angegeben werden.** Optionen, die die Bereitstellung, die binäre normalerweise in einem Flag analysieren würde, werden nicht unterstützt. Wenn Sie diese Optionen explizit angeben möchten, müssen Sie alle Laufwerke einschließen, die für die Sie dazu in/etc/fstab möchten. |

Standardmäßig legt WSL die Uid und Gid auf den Wert des Standardbenutzers (im Ubuntu-Distribution, die Standardbenutzer ist mit einer Uid zwischen erstellt = 1000, Gid = 1000). Wenn der Benutzer eine Gruppen-ID oder die Uid-Option explizit über diesen Schlüssel angegeben ist, wird der zugehörige Wert überschrieben. Andernfalls wird der Standardwert immer angefügt.

**Hinweis**: Diese Optionen werden als die Bereitstellungsoption für alle automatisch bereitgestellte Laufwerke angewendet. Um die Optionen für die nur ein bestimmtes Laufwerk ändern möchten, verwenden Sie stattdessen/etc/fstab.

#### <a name="network"></a>Netzwerk

Abschnittsbeschriftung: `[network]`

| key | Wert | default | Anmerkungen zu dieser Version|
|:----|:----|:----|:----|
| generateHosts | boolean | `true` | `true` Legt die WSL generieren `/etc/hosts`. Die `hosts` -Datei enthält von Hostnamen entsprechende IP-Adresse eine statische Karte. |
| generateResolvConf | boolean | `true` | `true` Legen Sie die WSL generieren `/etc/resolv.conf`. Die `resolv.conf` enthält eine DNS-Serverliste, die einen bestimmten Hostnamen in seine IP-Adresse auflösen können. | 

#### <a name="interop"></a>Interop

Abschnittsbeschriftung: `[interop]`

Diese Optionen sind in Insider-Build 17713 und höher verfügbar.

| key | Wert | default | Anmerkungen zu dieser Version|
|:----|:----|:----|:----|
| enabled | boolean | `true` | Einstellung, die diesem Schlüssel bestimmen, ob WSL beim Starten von Windows-Prozesse unterstützt wird. |
| appendWindowsPath | boolean | `true` | Einstellung, die diesem Schlüssel bestimmen, ob WSL Windows Pfadelemente die Umgebungsvariable $PATH hinzufügen möchten. | 
