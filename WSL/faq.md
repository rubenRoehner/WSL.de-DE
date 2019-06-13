---
title: Häufig gestellte Fragen
description: Häufig gestellte Fragen zum Windows-Subsystem für Linux.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, faq
author: taraj
ms.author: taraj
ms.date: 9/4/2018
ms.topic: article
ms.assetid: 129101ed-b88a-43c2-b6a2-cd2c4ff6fee1
ms.openlocfilehash: 07461f7db4a351f5b79ab0c5179d3d917ef1bdf7
ms.sourcegitcommit: bb88269eb37405192625fa81ff91162393fb491f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67035062"
---
# <a name="frequently-asked-questions-about-windows-subsystem-for-linux"></a>Häufig gestellte Fragen zu Windows-Subsystem für Linux

## <a name="what-is-windows-subsystem-for-linux-wsl"></a>Was ist Windows-Subsystem für Linux (WSL)?
Das Windows-Subsystem für Linux (WSL) ist eine neue Windows 10-Funktion, mit der Sie native Linux-Befehlszeilentools direkt auf Windows auszuführen, die zusammen mit dem herkömmlichen Windows-Desktop und moderne store-apps.

Finden Sie unter den [Infoseite](./about.md) Weitere Details.

## <a name="who-is-wsl-for"></a>Wer ist WSL für?
Dies ist in erster Linie ein Tool für Entwickler – insbesondere Webentwickler und diejenigen, die auf oder mit open Source-Projekten arbeiten. Dadurch können diejenigen, die möchten/müssen, verwenden Sie Bash, häufig verwendete Linux-Tools (`sed`, `awk`usw.) und viele Linux-First-Tools (Ruby, Python usw.), ihre toolkette auf Windows zu verwenden.

## <a name="what-can-i-do-with-wsl"></a>Was kann ich mit WSL tun?
WSL bietet die eine Anwendung Bash.exe, die beim Starten, öffnet einer Windows-Konsole die Bash-Shell ausgeführt. Bei Verwendung von Bash, können Sie Linux-Befehlszeilenprogramme und apps ausführen. Geben Sie z. B. `lsb_release -a` , und drücken Sie die EINGABETASTE; Sie sehen die Details der Linux-Distribution, die derzeit ausgeführt wird:

![Screenshot der Distribution-details](media/distro.png)

Sie können auch Ihr Dateisystem des lokalen Computers aus in der Linux-Bash-Shell zugreifen – finden Sie Ihren lokalen Laufwerken, die die Bereitstellung unter der `/mnt` Ordner. Angenommen, Ihre `C:` Laufwerk erfolgt die Bereitstellung unter `/mnt/c`:  

![Screenshot der bereitgestellten C-Laufwerk](media/ls.png)

## <a name="what-is-bash"></a>Was ist Bash?
[Bash-](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) ist eine beliebte textorientierten Shell und Befehlssprache. Es ist die Standardshell enthalten, innerhalb von Ubuntu und andere Linux-Distributionen und in MacOS. Benutzer geben Sie Befehle in einer Shell zum Ausführen von Skripts und/oder die Ausführung von Befehlen und Tools, um viele Aufgaben ausgeführt werden.

## <a name="how-does-this-work"></a>Wie funktioniert das?
Sehen Sie sich unsere [Blog](https://blogs.msdn.microsoft.com/wsl/) wobei wir uns in die Details der zugrunde liegende Technologie.

## <a name="why-would-i-use-wsl-rather-than-linux-in-a-vm"></a>Warum sollte ich WSL anstelle von Linux auf einem virtuellen Computer verwenden?
WSL erfordert weniger Ressourcen (CPU, Arbeitsspeicher und Speicher) als einen vollständigen virtuellen Computer. WSL können Sie die zum Ausführen von Linux-Befehlszeilentools und apps gemeinsam mit Ihren Windows-Befehlszeile, Desktop und Store-apps, und klicken Sie auf Ihrem Windows-Dateien in Linux. Dadurch können Sie apps für Windows und Linux-Befehlszeilenprogramme auf den gleichen Satz von Dateien verwenden, wenn Sie möchten.

## <a name="why-would-i-use-for-example-ruby-on-linux-instead-of-on-windows"></a>Warum sollte ich, z. B. Ruby unter Linux nicht in Windows verwenden?
Einige plattformübergreifende Tools erstellt wurden, vorausgesetzt, dass die Umgebung, in der sie ausgeführt werden, wie Linux verhält. Nehmen wir beispielsweise an einige Tools, oder, dass sie sehr lange Dateipfade zugreifen können, dass bestimmte Dateien bzw. Ordner vorhanden sind. Dies bewirkt, dass häufig Probleme auf Windows, die häufig verhält sich unterschiedlich unter Linux.

Viele Sprachen wie Ruby und Knoten werden häufig zu portiert, und Sie gut auf Windows führen. Allerdings nicht alle Ruby, Gem oder Besitzer von Knoten und NPM-Bibliothek Portieren ihrer Bibliotheken zur Unterstützung von Windows, und viele Linux-spezifische Abhängigkeiten aufweisen. Dies kann häufig in Systemen, die mithilfe von Tools und Bibliotheken, die aus dem Build und manchmal Laufzeitfehler oder unerwünschte Verhaltensweisen auf Windows leidet erstellt führen.

Dies sind nur einige der Probleme, die viele Leute Fragen von Microsoft zur Verbesserung der Windows Befehlszeilentools und was wir mit Canonical, um native Bash als auch Linux-Befehlszeilentools zur Ausführung auf Windows aktivieren einen verursacht.

## <a name="what-does-this-mean-for-powershell"></a>Was bedeutet dies für PowerShell?
Beim Arbeiten mit Projekte (OSS), gibt es zahlreiche Szenarios, in denen es immens nützlich zum Löschen in Bash aus einem PowerShell Eingabeaufforderung. Bash-Unterstützung ist eine Ergänzung und erhöht den Wert von der Befehlszeile auf Windows, sodass PowerShell und der PowerShell-Community andere gängigen Technologien nutzen.

Erfahren Sie mehr im PowerShell-Teamblog – [Bash für Windows: Warum ist es großartig, und was es bedeutet für PowerShell](https://blogs.msdn.microsoft.com/powershell/2016/04/01/bash-for-windows-why-its-awesome-and-what-it-means-for-powershell/)

## <a name="can-i-run-all-linux-apps-in-wsl"></a>Kann ich alle Linux-apps in WSL ausführen?
Nein! WSL ist ein Tool zur ermöglicht den Benutzern, die sie zum Ausführen von Bash sowie der wichtigsten Linux-Befehlszeilenprogramme für Windows. 

Wird von WSL **nicht** GUI-Desktops und Anwendungen (z. B. Gnome, KDE usw.) unterstützen.  

Darüber hinaus, obwohl Sie werden zu viele beliebte serveranwendungen ausgeführt werden (z. B. Redis), wir empfehlen nicht WSL für das Hosten von Produktionsdienste – Microsoft bietet eine Vielzahl von Lösungen für die Produktion Linux-Workloads in Azure ausgeführt wird, Hyper-V und Docker. 

## <a name="what-windows-skus-is-wsl-included-in"></a>Welche Windows-SKUs umfasst WSL?
Windows-Subsystem für Linux ist auf die desktop-Version von Windows für Windows 10 Anniversary- und Creators Update oder höher verfügbar.

Ab dem Fall Creators werden Update WSL auf dem Desktop und dem Server-SKUs von Windows verfügbar.

## <a name="what-processors-does-wsl-support"></a>Welche Prozessoren unterstützt WSL?
WSL unterstützt X64 und ARM-CPUs.

## <a name="how-do-i-access-my-c-drive"></a>Wie greife ich auf Mein Laufwerk "c:"?
Bereitstellungspunkte für die Festplatten auf dem lokalen Computer werden automatisch erstellt und bieten einfachen Zugriff auf das Windows-Dateisystem. 
 
**/mnt/\<Laufwerkbuchstabe > /**
 
Beispiel für die Verwendung wäre `cd /mnt/c` auf c:\

## <a name="how-do-i-use-a-windows-file-with-a-linux-app"></a>Wie verwende ich eine Windows-Datei mit einer Linux-app?

Einer der Vorteile von WSL wird Zugriff auf Ihre Dateien sowohl Windows und Linux-Anwendungen oder Tools. 

WSL bindet die Festplattenlaufwerke des Computers, unter dem `/mnt/<drive>` Ordner in Ihrem Linux-Distributionen. Angenommen, Ihre `C:` Laufwerk eingebunden ist, klicken Sie unter `/mnt/c/` 

Verwenden die bereitgestellten Laufwerke, können Sie Code bearbeiten, z. B. `C:\dev\myproj\` mit [Visual Studio](https://visualstudio.microsoft.com/vs/) / oder [VS Code](https://code.visualstudio.com/), und erstellen/Testen dieses Codes in Linux durch den Zugriff auf die gleichen Dateien über `/mnt/c/dev/myproj`.

> **WICHTIGER HINWEIS**: Die Einschränkungen der Verwendung von WSL ist, dass direkt den Zugriff auf/Ändern von Dateien in Ihrer Linux-Distributionen Dateisystem mithilfe von Windows-apps oder Tools nicht unterstützt wird. Thema [Wirken Sie sich nicht auf Linux-Dateien, die mithilfe von Windows-apps und -tools](https://blogs.msdn.microsoft.com/commandline/2016/11/17/do-not-change-linux-files-using-windows-apps-and-tools/)

## <a name="are-files-in-the-linux-drive-different-from-the-mounted-windows-drive"></a>Unterscheiden sich Dateien in das Linux-Laufwerk aus dem bereitgestellten Windows-Laufwerk?

1. Dateien unter dem Linux-Stamm (d. h. `/`) werden von WSL die Linux bestimmtes Verhalten führen, einschließlich aber nicht beschränkt auf imitiert gesteuert:
   * Dateien, die ungültige Zeichen im Dateinamen Windows enthalten.
   * Symbolische Verknüpfungen erstellt, die für Benutzer ohne Administratorrechte
   * Ändern die Attribute der Datei durch Chmod und chown
   * Datei/Ordner Groß-/Kleinschreibung

2. Dateien in die bereitgestellten Laufwerke werden durch Windows gesteuert, und weisen folgende Verhaltensweisen:
   * Unterstützung von Groß-/Kleinschreibung
   * Alle Berechtigungen sind entsprechend der am besten die Windows-Berechtigungen festgelegt

## <a name="why-are-there-so-many-errors-when-i-run-apt-get-upgrade"></a>Warum gibt es so viele Fehler beim Upgrade von apt-Get ausführen?
Einige Pakete verwenden Funktionen, die wir noch nicht implementiert haben. `udev`, z. B. wird nicht noch unterstützt und bewirkt, dass mehrere `apt-get upgrade` Fehler.

Zum Beheben von Problemen im Zusammenhang mit `udev`, befolgen Sie die folgenden Schritte aus:

1. Schreiben Sie folgenden Code zum `/usr/sbin/policy-rc.d` und die Änderungen zu speichern.

    ```bash
    #!/bin/sh
    exit 101
    ```

2. Hinzufügen Ausführungsberechtigungen `/usr/sbin/policy-rc.d`

    ```bash
    chmod +x /usr/sbin/policy-rc.d
    ```
  
2. Führen Sie die folgenden Befehle

    ```bash
    dpkg-divert --local --rename --add /sbin/initctl
    ln -s /bin/true /sbin/initctl
    ```

## <a name="how-do-i-uninstall-a-wsl-distribution"></a>Wie deinstalliere ich eine Verteilung WSL?

Auf builds vor 1709 (16299) öffnen eine Eingabeaufforderung, und führen Sie aus:
  ```batchfile
  lxrun /uninstall /full
  ```
  
WSL-Verteilungen aus dem Store installiert können wie jede andere Windows-app deinstalliert werden, mit der rechten Maustaste auf die Kachel der app, und klicken Sie auf Deinstallieren oder über PowerShell mit der [ `Remove-AppxPackage` Cmdlet](https://technet.microsoft.com/en-us/library/hh856038.aspx).

## <a name="why-does-ping-generate-permission-denied-errors"></a>Warum wird Ping Zugriff verweigert-Fehler generiert?
In WSL builds < 14926, Ping erforderlich WSL, über eine Konsole mit erhöhten Rechten auszuführen. Dieses Problem wurde in Build 14926 und höher behoben.

## <a name="how-do-i-run-an-openssh-server"></a>Wie führe ich ein OpenSSH-Server aus?
Berechtigungen in Windows sind erforderlich, OpenSSH in WSL ausgeführt wird. Klicken Sie zum Ausführen eines OpenSSH-Servers Ausführen von Bash unter Ubuntu unter Windows als Administrator, oder führen Sie bash.exe CMD/PowerShell-Eingabeaufforderung mit Administratorrechten aus.

## <a name="why-do-i-get-error-0x80040306-when-i-try-to-install"></a>Warum erhalte ich "Fehler: 0x80040306 "beim versuch, Sie installieren?
WSL unterstützt nicht die in einer legacy-Konsole ausgeführt wird. So deaktivieren legacy-Konsole ein:

1. Öffnen Sie WSL, PowerShell oder Cmd
1. Klicken Sie mit der rechten Maustaste auf Title bar -> Eigenschaften -> deaktivieren Sie "Legacykonsole verwenden"
1. Auf "OK" klicken

## <a name="why-do-i-get-error-0x80040154-when-i-run-bashexe-after-upgrading-windows"></a>Warum erhalte ich "Fehler: 0 x 80040154 "beim bash.exe nach dem Upgrade von Windows ausführen?
Die Funktion "Windows-Subsystem für Linux" möglicherweise deaktiviert werden, während eines Windows-Updates. In diesem Fall muss das Windows-Feature erneut aktiviert werden. Anweisungen zum Aktivieren des Features "Windows-Subsystem für Linux" finden Sie in der [Installationshandbuch](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui https://msdn.microsoft.com/en-us/commandline/wsl/install_guide#enable-the-windows-subsystem-for-linux-feature-gui).

## <a name="how-do-i-change-the-display-language-of-wsl"></a>Wie ändere ich die Anzeigesprache des WSL?
Installieren von WSL versucht, die automatisch das Ubuntu-Gebietsschema entsprechend das Gebietsschema des der Windows-Installation zu ändern. Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl, um die Ubuntu-Benutzergebietsschema ändern, nachdem die Installation abgeschlossen ist ausführen. Sie müssen bash.exe für diese Änderung wirksam wird neu zu starten.

Das folgenden Beispiel ändert sich auf dem Gebietsschema En-US:
```bash
sudo update-locale LANG=en_US.UTF8
```

## <a name="why-do-i-not-have-internet-access-from-wsl"></a>Warum habe ich kein Internetzugriff von WSL?
Einige Benutzer haben Probleme mit der bestimmte Firewall-Anwendungen, die Zugriff auf das Internet in WSL blockieren gemeldet. Die Firewalls, die gemeldet werden:

1. Kaspersky
1. AVG
1. Avast

In einigen Fällen können durch das Deaktivieren der Firewalls für den Zugriff. In einigen Fällen sucht das einfach dadurch, dass die installierte Firewall zum Blockieren des Zugriffs.

## <a name="how-do-i-access-a-port-from-wsl-in-windows"></a>Wie greife ich auf einen Port aus WSL in Windows?
WSL gibt Windows, die IP-Adresse an, wie sie auf dem Windows ausgeführt wird. Daher es stehen keine Ports auf "localhost" z. B. Wenn Sie Web-Inhalte an Port 1234 haben, Sie können https://localhost:1234 in Ihren Windows-Browser.

## <a name="where-can-i-provide-feedback"></a>Wo kann ich Feedback Geben?

Sie können die Teilen Sie uns Feedback und fragen sich über mehrere Kanäle: Feedback und Ihre Fragen bitte an:
* Unsere [GitHub-problemverfolgung](https://github.com/Microsoft/BashOnWindows/issues)
* Unsere [Befehlszeilen UserVoice-Portal](https://wpdev.uservoice.com/forums/266908-command-prompt/filters/top)
* Unsere [Befehlszeilen-Teamblog](https://blogs.msdn.microsoft.com/commandline/)
* Via Twitter. Führen Sie [ @richturn_ms ](https://twitter.com/richturn_MS) usw. auf Twitter, um Neuigkeiten, Updates, Informationen zu.
