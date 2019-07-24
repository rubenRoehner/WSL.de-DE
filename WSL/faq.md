---
title: Häufig gestellte Fragen
description: Häufig gestellte Fragen zum Windows-Subsystem für Linux.
keywords: Bashonwindows, bash, WSL, Windows, windowssubsystem, FAQ
author: taraj
ms.author: taraj
ms.date: 9/4/2018
ms.topic: article
ms.assetid: 129101ed-b88a-43c2-b6a2-cd2c4ff6fee1
ms.openlocfilehash: 2bbcec661146fcb570209fd895e6543657e98996
ms.sourcegitcommit: 939fe561d178454219adbee96c0ad3f768db2208
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2019
ms.locfileid: "67237387"
---
# <a name="frequently-asked-questions-about-windows-subsystem-for-linux"></a>Häufig gestellte Fragen zum Windows-Subsystem für Linux

## <a name="what-is-windows-subsystem-for-linux-wsl"></a>Was ist das Windows-Subsystem für Linux (WSL)?
Das Windows-Subsystem für Linux (WSL) ist ein neues Feature von Windows 10, mit dem Sie native Linux-Befehlszeilen Tools direkt auf Windows ausführen können, zusammen mit herkömmlichen Windows Desktop-und modernen Store-Apps.

Weitere Informationen finden Sie auf der [Seite](./about.md) "Info".

## <a name="who-is-wsl-for"></a>Für wen gilt WSL?
Dies ist in erster Linie ein Tool für Entwickler, insbesondere Webentwickler und Anwendungen, die an oder mit Open Source-Projekten arbeiten. Dies ermöglicht es Benutzern, die bash, gängige Linux-Tools (`sed`, `awk`usw.) und viele Linux-First-Tools (Ruby, python usw.) verwenden möchten, um Ihre Toolkette unter Windows zu verwenden.

## <a name="what-can-i-do-with-wsl"></a>Was kann ich mit WSL tun?
WSL bietet eine Anwendung mit dem Namen bash. exe, die eine Windows-Konsole mit der bash-Shell öffnet, wenn Sie gestartet wird. Mithilfe von bash können Sie Befehlszeilen-Linux-Tools und-apps ausführen. Geben Sie z `lsb_release -a` . b. ein, und drücken Sie die EINGABETASTE. es werden Details zu der derzeit laufenden Linux-Distribution angezeigt:

![Screenshot der Details der Distribution](media/distro.png)

Sie können auch über die Linux bash-Shell auf das Dateisystem des lokalen Computers zugreifen – Sie finden die lokalen Laufwerke, die `/mnt` im Ordner bereitgestellt werden. Das `C:` Laufwerk wird beispielsweise unter `/mnt/c`:  

![Screenshot des eingebundenen C-Laufwerks](media/ls.png)

## <a name="what-is-bash"></a>Was ist bash?
[Bash](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) ist eine beliebte, textbasierte Shell und Befehlssprache. Dabei handelt es sich um die Standardshell, die in Ubuntu und anderen Linux-Distributionen und macOS enthalten ist. Benutzer geben Befehle in eine Shell ein, um Skripts auszuführen und/oder Befehle und Tools auszuführen, um viele Aufgaben auszuführen.

## <a name="how-does-this-work"></a>Wie funktioniert das?
Sehen Sie sich unseren [Blog](https://blogs.msdn.microsoft.com/wsl/) an, in dem wir uns ausführlich über die zugrunde liegende Technologie informieren.

## <a name="why-would-i-use-wsl-rather-than-linux-in-a-vm"></a>Warum sollte ich WSL anstelle von Linux auf einem virtuellen Computer verwenden?
WSL erfordert weniger Ressourcen (CPU, Arbeitsspeicher und Speicher) als ein vollständiger virtueller Computer. WSL ermöglicht Ihnen außerdem das Ausführen von Linux-Befehlszeilen Tools und-apps neben Ihren Windows-Befehlszeilen-, Desktop-und Store-Apps und den Zugriff auf Ihre Windows-Dateien aus Linux. Auf diese Weise können Sie Windows-apps und Linux-Befehlszeilen Tools für denselben Satz von Dateien verwenden, wenn Sie möchten.

## <a name="why-would-i-use-for-example-ruby-on-linux-instead-of-on-windows"></a>Warum würde ich beispielsweise Ruby on Linux anstelle von Windows verwenden?
Einige plattformübergreifende Tools wurden unter der Annahme erstellt, dass sich die Umgebung, in der Sie ausgeführt werden, wie Linux verhält. Einige Tools nehmen z. b. an, dass Sie in der Lage sind, auf sehr lange Dateipfade zuzugreifen, oder dass bestimmte Dateien/Ordner vorhanden sind. Dies verursacht häufig Probleme unter Windows, die sich häufig anders als Linux Verhalten.

Viele Sprachen wie Ruby und Node werden häufig in Windows portiert und hervorragend ausgeführt. Allerdings portieren nicht alle ruby Gem oder Node/NPM-Bibliotheks Besitzer ihre Bibliotheken, um Windows zu unterstützen, und viele verfügen über Linux-spezifische Abhängigkeiten. Dies kann häufig dazu führen, dass Systeme erstellt werden, die mit Tools und Bibliotheken erstellt werden, die von Build und manchmal Laufzeitfehlern oder unerwünschten Verhalten unter Windows erstellt werden

Dies sind nur einige Probleme, die dazu geführt haben, dass viele Benutzer Microsoft aufgefordert haben, die Befehlszeilen Tools von Windows zu verbessern, und was wir an Partner mit Canonical weitergeleitet haben, um native bash-und Linux-Befehlszeilen Tools für die Unterstützung von Windows zu aktivieren

## <a name="what-does-this-mean-for-powershell"></a>Was bedeutet dies für PowerShell?
Beim Arbeiten mit OSS-Projekten gibt es viele Szenarios, in denen es äußerst nützlich ist, in bash von einer PowerShell-Eingabeaufforderung zu löschen. Die bash-Unterstützung ist ergänzend und stärkt den Wert der Befehlszeile unter Windows, sodass PowerShell und die PowerShell-Community andere gängige Technologien nutzen können.

Weitere Informationen finden Sie im PowerShell- [Teamblog: bash für Windows: Warum es großartig ist und was es für PowerShell bedeutet](https://blogs.msdn.microsoft.com/powershell/2016/04/01/bash-for-windows-why-its-awesome-and-what-it-means-for-powershell/)

## <a name="can-i-run-all-linux-apps-in-wsl"></a>Kann ich alle Linux-apps in WSL ausführen?
Nein! WSL ist ein Tool zum Aktivieren von Benutzern, die diese benötigen, um bash-und Core Linux-Befehlszeilen Tools unter Windows auszuführen. 

WSL zielt **nicht** darauf ab, GUI-Desktops oder-Anwendungen (z. b. gnome, KDE usw.) zu unterstützen.  

Auch wenn Sie viele beliebte Server Anwendungen (z. b. redis) ausführen können, empfiehlt es sich nicht, WSL zum Hosten von Produktions Diensten zu verwenden – Microsoft bietet eine Vielzahl von Lösungen für die Ausführung von Linux-Workloads in Azure, Hyper-V und Docker. 

## <a name="what-windows-skus-is-wsl-included-in"></a>In welchen Windows-SKUs ist WSL enthalten?
Das Windows-Subsystem für Linux ist in der Desktop Version von Windows für Windows 10 Anniversary und Creators Update oder höher verfügbar.

Beginnend mit dem Fall Creators Update ist WSL auf den Desktop-und Server-SKUs von Windows verfügbar.

## <a name="what-processors-does-wsl-support"></a>Welche Prozessoren werden von WSL unterstützt?
WSL unterstützt x64-und ARM-CPUs.

## <a name="how-do-i-access-my-c-drive"></a>Gewusst wie auf mein Laufwerk "C:" zugreifen?
Einstellungspunkte für Festplatten auf dem lokalen Computer werden automatisch erstellt und ermöglichen einen einfachen Zugriff auf das Windows-Dateisystem. 
 
**im\<Laufwerk Buchstabe >/**
 
`cd /mnt/c` Beispiel für den Zugriff auf c:\

## <a name="how-do-i-use-a-windows-file-with-a-linux-app"></a>Gewusst wie eine Windows-Datei mit einer Linux-App verwenden?

Einer der Vorteile von WSL besteht darin, dass Sie über Windows-und Linux-Apps oder-Tools auf Ihre Dateien zugreifen können. 

WSL stellt die Festplattenlaufwerke Ihres Computers unter dem `/mnt/<drive>` Ordner in Ihren Linux-Distributionen bereit. Beispielsweise wird das `C:` Laufwerk unter`/mnt/c/` 

Mit den bereitgestellten Laufwerken können Sie Code in `C:\dev\myproj\` z. b. mithilfe von [Visual Studio](https://visualstudio.microsoft.com/vs/) /oder [vs Code](https://code.visualstudio.com/)bearbeiten und den Code in Linux erstellen und testen, indem Sie über `/mnt/c/dev/myproj`auf die gleichen Dateien zugreifen.

> **WICHTIGER HINWEIS**: Eine der wichtigsten Einschränkungen bei der Verwendung von WSL besteht darin, dass der direkte Zugriff auf/das Ändern von Dateien im Dateisystem von Linux-Distributionen mithilfe von Windows-Apps oder-Tools nicht unterstützt wird. Thema [Ändern Sie Linux-Dateien nicht mithilfe von Windows-apps und-Tools.](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/)

## <a name="are-files-in-the-linux-drive-different-from-the-mounted-windows-drive"></a>Unterscheiden sich die Dateien im Linux-Laufwerk vom bereitgestellten Windows-Laufwerk?

1. Dateien unter dem Linux-Stamm (d.h. `/`) werden von WSL gesteuert, was das Linux-spezifische Verhalten imitiert, einschließlich, aber nicht beschränkt auf:
   * Dateien, die ungültige Windows-Dateinamen Zeichen enthalten
   * Für Benutzer ohne Administratorrechte erstellte symlinks
   * Ändern von Dateiattributen über chmod und chown
   * Unterscheidung nach Groß-/Kleinschreibung

2. Dateien in bereitgestellten Laufwerken werden von Windows gesteuert und weisen folgendes Verhalten auf:
   * Unterscheidung von Unterstützung
   * Alle Berechtigungen sind so festgelegt, dass Sie die Windows-Berechtigungen bestmöglich

## <a name="why-are-there-so-many-errors-when-i-run-apt-get-upgrade"></a>Warum gibt es so viele Fehler, wenn ich apt-get-Upgrade führe?
In einigen Paketen werden Features verwendet, die noch nicht implementiert wurden. `udev`wird z. b. noch nicht unterstützt und `apt-get upgrade` verursacht mehrere Fehler.

Führen Sie die folgenden Schritte `udev`aus, um Probleme im Zusammenhang mit zu beheben:

1. Schreiben Sie Folgendes in `/usr/sbin/policy-rc.d` , und speichern Sie die Änderungen.

    ```bash
    #!/bin/sh
    exit 101
    ```

2. Ausführungs Berechtigungen hinzufügen zu`/usr/sbin/policy-rc.d`

    ```bash
    chmod +x /usr/sbin/policy-rc.d
    ```
  
2. Führen Sie die folgenden Befehle aus:

    ```bash
    dpkg-divert --local --rename --add /sbin/initctl
    ln -s /bin/true /sbin/initctl
    ```

## <a name="how-do-i-uninstall-a-wsl-distribution"></a>Gewusst wie Deinstallieren einer WSL-Distribution?

Öffnen Sie in Builds vor 1709 (16299) eine Eingabeaufforderung, und führen Sie Folgendes aus:
  ```batchfile
  lxrun /uninstall /full
  ```
  
WSL-Distributionen, die aus dem Speicher installiert werden, können wie jede andere Windows-APP deinstalliert werden, indem Sie mit der rechten Maustaste auf die APP-Kachel klicken und auf Deinstallieren oder mithilfe des [ `Remove-AppxPackage` -Cmdlets](https://technet.microsoft.com/en-us/library/hh856038.aspx)über PowerShell klicken.

## <a name="why-does-ping-generate-permission-denied-errors"></a>Warum werden bei der Ping-Berechtigung Fehler verweigert?
In WSL-Builds < 14926 erforderte der Ping-Befehl, dass WSL über eine Konsole mit erhöhten Rechten ausgeführt wird. Dieses Problem wurde in Build 14926 und höher behoben.

## <a name="how-do-i-run-an-openssh-server"></a>Gewusst wie einen OpenSSH-Server ausführen?
Zum Ausführen von OpenSSH in WSL sind Administrator Rechte in Windows erforderlich. Wenn Sie einen OpenSSH-Server ausführen möchten, führen Sie bash unter Ubuntu unter Windows als Administrator aus, oder führen Sie bash. exe von einer cmd-/PowerShell-Eingabeaufforderung mit Administratorrechten aus.

## <a name="why-do-i-get-error-0x80040306-when-i-try-to-install"></a>Warum erhalte ich einen Fehler: 0x80040306 "beim Versuch, zu installieren?
WSL unterstützt die Ausführung in einer Legacy Konsole nicht. So deaktivieren Sie die Legacy Konsole:

1. Öffnen von WSL, PowerShell oder cmd
1. Klicken Sie mit der rechten Maustaste auf Titelleiste-> Eigenschaften > deaktivieren Sie die Option "Legacy Konsole verwenden".
1. Auf "OK" klicken

## <a name="why-do-i-get-error-0x80040154-when-i-run-bashexe-after-upgrading-windows"></a>Warum erhalte ich einen Fehler: 0x80040154 "beim Ausführen von bash. exe nach dem Upgrade von Windows?
Das Feature "Windows-Subsystem für Linux" ist möglicherweise während eines Windows-Updates deaktiviert. Wenn dies der Fall ist, muss das Windows-Feature erneut aktiviert werden. Anweisungen zum Aktivieren des Features "Windows-Subsystem für Linux" finden Sie im [Installationshandbuch](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui).

## <a name="how-do-i-change-the-display-language-of-wsl"></a>Gewusst wie die Anzeige Sprache von WSL ändern?
Die WSL-Installation versucht, das Ubuntu-Gebiets Schema automatisch so zu ändern, dass es dem Gebiets Schema Ihrer Windows-Installation entspricht. Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl ausführen, um das Ubuntu-Gebiets Schema zu ändern, nachdem die Installation abgeschlossen wurde. Sie müssen bash. exe neu starten, damit diese Änderung wirksam wird.

Im folgenden Beispiel wird "locale" in "en-US" geändert:
```bash
sudo update-locale LANG=en_US.UTF8
```

## <a name="why-do-i-not-have-internet-access-from-wsl"></a>Warum habe ich keinen Internet Zugriff von WSL?
Einige Benutzer haben Probleme mit bestimmten Firewallanwendungen gemeldet, die den Internet Zugriff in WSL blockieren. Die gemeldeten Firewalls lauten wie folgt:

1. Kaspersky
1. AVG
1. Avast

In einigen Fällen ermöglicht das Ausschalten der Firewall den Zugriff. In einigen Fällen, in denen die Firewall einfach installiert ist, wird der Zugriff von blockiert.

## <a name="how-do-i-access-a-port-from-wsl-in-windows"></a>Gewusst wie auf einen Port von WSL in Windows zugreifen?
WSL nutzt die IP-Adresse von Windows, da Sie unter Windows ausgeführt wird. Daher können Sie auf alle Ports auf "localhost" zugreifen, z. b. Wenn Sie Webinhalte an https://localhost:1234 Port 1234 haben, können Sie in Ihren Windows-Browser gelangen.

## <a name="how-can-i-back-up-my-wsl-distros"></a>Wie kann ich meine WSL-Distributionen sichern?

Die beste Möglichkeit zum Sichern Ihrer Distributionen ist in Windows Version 1809 und höher verfügbar. Sie können die gesamte Verteilung mithilfe des `wsl --export` Befehls in einen Tarball exportieren. Anschließend können Sie diese Distribution mithilfe des Befehls wieder in WSL importieren `wsl --import` , sodass Sie die Zustände ihrer WSL-Distributionen sichern und speichern können. 

Beachten Sie, dass herkömmliche Sicherungsdienste, die Dateien in ihren APPDATA-Ordnern (z. b. Windows-Sicherung) sichern, Ihre Linux-Dateien nicht beschädigen. 



## <a name="where-can-i-provide-feedback"></a>Wo kann ich Feedback geben?

Sie können Feedback freigeben und Fragen über mehrere Kanäle stellen: Feedback und Fragen sollten wie folgt geleitet werden:
* Unsere [GitHub-Problem](https://github.com/Microsoft/BashOnWindows/issues) Verfolgung
* Unser [Befehlszeilen-UserVoice-Portal](https://wpdev.uservoice.com/forums/266908-command-prompt/filters/top)
* Unser [Befehlszeilen-Teamblog](https://blogs.msdn.microsoft.com/commandline/)
* Über Twitter. Weitere Informationen zu Neuigkeiten, Updates usw. finden Sie [unterTwitter.@richturn_ms](https://twitter.com/richturn_MS)
