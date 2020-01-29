---
title: Problembehandlung des Windows-Subsystems für Linux
description: Bietet ausführliche Informationen zu häufigen Fehlern und Problemen, die bei der Ausführung von Linux im Windows-Subsystem für Linux auftreten.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, ubuntu
ms.date: 01/20/2020
ms.topic: article
ms.localizationpriority: high
ms.openlocfilehash: ec456c314ac4a1588ccb5c1aa35e22a2d33a39b0
ms.sourcegitcommit: 07eb5f2e1f4517928165dda4510012599b0d0e1e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/22/2020
ms.locfileid: "76520529"
---
# <a name="troubleshooting-windows-subsystem-for-linux"></a><span data-ttu-id="6a351-104">Problembehandlung des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="6a351-104">Troubleshooting Windows Subsystem for Linux</span></span>

<span data-ttu-id="6a351-105">Unterstützung bei Fragen im Zusammenhang mit WSL finden Sie in unserem GitHub-Repository:</span><span class="sxs-lookup"><span data-stu-id="6a351-105">For support with issues related to WSL, please see our GitHub repo:</span></span>

## <a name="search-for-any-existing-issues-related-to-your-problem"></a><span data-ttu-id="6a351-106">Suchen nach vorhandenen Themen zu Ihrem Problem</span><span class="sxs-lookup"><span data-stu-id="6a351-106">Search for any existing issues related to your problem</span></span>

<span data-ttu-id="6a351-107">Verwenden Sie für technische Probleme das Produktrepository: https://github.com/Microsoft/wsl/issues</span><span class="sxs-lookup"><span data-stu-id="6a351-107">For technical issues, use the product repo: https://github.com/Microsoft/wsl/issues</span></span>

<span data-ttu-id="6a351-108">Verwenden Sie für Probleme im Zusammenhang mit dem Inhalt dieser Dokumentation das Dokumentrepository: https://github.com/MicrosoftDocs/wsl/issues</span><span class="sxs-lookup"><span data-stu-id="6a351-108">For issues related to the contents of this documentation, use the docs repo: https://github.com/MicrosoftDocs/wsl/issues</span></span>

## <a name="submit-a-bug-report"></a><span data-ttu-id="6a351-109">Senden eines Fehlerberichts</span><span class="sxs-lookup"><span data-stu-id="6a351-109">Submit a bug report</span></span>

<span data-ttu-id="6a351-110">Bei Fehlern im Zusammenhang mit WSL-Funktionen oder -Features melden Sie ein Problem im Produktrepository: https://github.com/Microsoft/wsl/issues</span><span class="sxs-lookup"><span data-stu-id="6a351-110">For bugs related to WSL functions or features, file an issue in the product repo: https://github.com/Microsoft/wsl/issues</span></span>

## <a name="submit-a-feature-request"></a><span data-ttu-id="6a351-111">Übermitteln einer Featureanforderung</span><span class="sxs-lookup"><span data-stu-id="6a351-111">Submit a feature request</span></span>

<span data-ttu-id="6a351-112">Um ein neues Feature im Zusammenhang mit der WSL-Funktionalität oder -Kompatibilität anzufordern, melden Sie ein Problem im Produktrepository: https://github.com/Microsoft/wsl/issues</span><span class="sxs-lookup"><span data-stu-id="6a351-112">To request a new feature related to WSL functionality or compatibility, file an issue in the product repo: https://github.com/Microsoft/wsl/issues</span></span>

## <a name="contribute-to-the-docs"></a><span data-ttu-id="6a351-113">Beiträge zu den Dokumenten leisten</span><span class="sxs-lookup"><span data-stu-id="6a351-113">Contribute to the docs</span></span>

<span data-ttu-id="6a351-114">Um einen Beitrag zur WSL-Dokumentation zu leisten, senden Sie ein Pull Request im Dokumentrepository: https://github.com/MicrosoftDocs/wsl/issues</span><span class="sxs-lookup"><span data-stu-id="6a351-114">To contribute to the WSL documentation, submit a pull request in the docs repo: https://github.com/MicrosoftDocs/wsl/issues</span></span>

## <a name="terminal-or-command-line"></a><span data-ttu-id="6a351-115">Terminal oder Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="6a351-115">Terminal or Command Line</span></span>

<span data-ttu-id="6a351-116">Wenn sich Ihr Problem auf den Windows-Terminal, die Windows-Konsole oder die Befehlszeilenschnittstelle bezieht, verwenden Sie schließlich das Windows-Terminal-Repository: https://github.com/microsoft/terminal</span><span class="sxs-lookup"><span data-stu-id="6a351-116">Lastly, if your issue is related to the Windows Terminal, Windows Console, or the command-line UI, use the Windows terminal repo: https://github.com/microsoft/terminal</span></span>

## <a name="common-issues"></a><span data-ttu-id="6a351-117">Allgemeine Probleme</span><span class="sxs-lookup"><span data-stu-id="6a351-117">Common issues</span></span>

### <a name="bash-loses-network-connectivity-once-connected-to-a-vpn"></a><span data-ttu-id="6a351-118">Bash verliert nach dem Herstellen einer Verbindung mit einem VPN die Netzwerkkonnektivität</span><span class="sxs-lookup"><span data-stu-id="6a351-118">Bash loses network connectivity once connected to a VPN</span></span>

<span data-ttu-id="6a351-119">Wenn Bash nach dem Herstellen einer Verbindung mit einem VPN unter Windows die Netzwerkkonnektivität verliert, können Sie diese Problemumgehung innerhalb von Bash versuchen.</span><span class="sxs-lookup"><span data-stu-id="6a351-119">If after connecting to a VPN on Windows, bash loses network connectivity, try this workaround from within bash.</span></span> <span data-ttu-id="6a351-120">Mit dieser Problemumgehung können Sie die DNS-Auflösung manuell durch `/etc/resolv.conf` außer Kraft setzen.</span><span class="sxs-lookup"><span data-stu-id="6a351-120">This workaround will allow you to manually override the DNS resolution through `/etc/resolv.conf`.</span></span>

1. <span data-ttu-id="6a351-121">Notieren Sie sich den DNS-Server des VPN (`ipconfig.exe /all`).</span><span class="sxs-lookup"><span data-stu-id="6a351-121">Take a note of the DNS server of the VPN from doing `ipconfig.exe /all`</span></span>
2. <span data-ttu-id="6a351-122">Erstellen Sie eine Kopie der vorhandenen Datei „resolv.conf“ (`sudo cp /etc/resolv.conf /etc/resolv.conf.new`).</span><span class="sxs-lookup"><span data-stu-id="6a351-122">Make a copy of the existing resolv.conf `sudo cp /etc/resolv.conf /etc/resolv.conf.new`</span></span>
3. <span data-ttu-id="6a351-123">Heben Sie die Verknüpfung der aktuellen Datei „resolv.conf“ auf (`sudo unlink /etc/resolv.conf`).</span><span class="sxs-lookup"><span data-stu-id="6a351-123">Unlink the current resolv.conf `sudo unlink /etc/resolv.conf`</span></span>
4. `sudo mv /etc/resolv.conf.new /etc/resolv.conf`
5. <span data-ttu-id="6a351-124">Öffnen Sie `/etc/resolv.conf` und</span><span class="sxs-lookup"><span data-stu-id="6a351-124">Open `/etc/resolv.conf` and</span></span> <br/>
   <span data-ttu-id="6a351-125">ein.</span><span class="sxs-lookup"><span data-stu-id="6a351-125">a.</span></span> <span data-ttu-id="6a351-126">Löschen Sie die erste Zeile aus der Datei, die Folgendes besagt: „\#This file was automatically generated by WSL.</span><span class="sxs-lookup"><span data-stu-id="6a351-126">Delete the first line from the file, which says "\# This file was automatically generated by WSL.</span></span> <span data-ttu-id="6a351-127">To stop automatic generation of this file, remove this line.“ (Diese Datei wurde automatisch von WSL generiert. Um die automatische Generierung dieser Datei zu beenden, entfernen Sie diese Zeile.)</span><span class="sxs-lookup"><span data-stu-id="6a351-127">To stop automatic generation of this file, remove this line.".</span></span> <br/>
   <span data-ttu-id="6a351-128">b.</span><span class="sxs-lookup"><span data-stu-id="6a351-128">b.</span></span> <span data-ttu-id="6a351-129">Fügen Sie den DNS-Eintrag aus (1) oben als ersten Eintrag in der Liste der DNS-Server hinzu.</span><span class="sxs-lookup"><span data-stu-id="6a351-129">Add the DNS entry from (1) above as the very first entry in the list of DNS servers.</span></span> <br/>
   <span data-ttu-id="6a351-130">c.</span><span class="sxs-lookup"><span data-stu-id="6a351-130">c.</span></span> <span data-ttu-id="6a351-131">Schließen Sie die Datei.</span><span class="sxs-lookup"><span data-stu-id="6a351-131">Close the file.</span></span> <br/>

<span data-ttu-id="6a351-132">Nachdem Sie die Verbindung mit dem VPN getrennt haben, müssen Sie die Änderungen auf `/etc/resolv.conf` zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="6a351-132">Once you have disconnected the VPN, you will have to revert the changes to `/etc/resolv.conf`.</span></span> <span data-ttu-id="6a351-133">Gehen Sie dazu folgendermaßen vor:</span><span class="sxs-lookup"><span data-stu-id="6a351-133">To do this, do:</span></span>

1. `cd /etc`
2. `sudo mv resolv.conf resolv.conf.new`
3. `sudo ln -s ../run/resolvconf/resolv.conf resolv.conf`

### <a name="starting-wsl-or-installing-a-distribution-returns-an-error-code"></a><span data-ttu-id="6a351-134">Beim Starten von WSL oder beim Installieren einer Distribution wird ein Fehlercode zurückgegeben</span><span class="sxs-lookup"><span data-stu-id="6a351-134">Starting WSL or installing a distribution returns an error code</span></span>

<span data-ttu-id="6a351-135">Befolgen Sie [diese Anweisungen](https://github.com/Microsoft/WSL/blob/master/CONTRIBUTING.md#8-detailed-logs), um detaillierte Protokolle zu erfassen und ein Issue auf GitHub zu melden.</span><span class="sxs-lookup"><span data-stu-id="6a351-135">Follow [these instructions](https://github.com/Microsoft/WSL/blob/master/CONTRIBUTING.md#8-detailed-logs) to collect detailed logs and file an issue on our GitHub.</span></span>

### <a name="updating-bash-on-ubuntu-on-windows"></a><span data-ttu-id="6a351-136">Aktualisieren von Bash unter Ubuntu unter Windows</span><span class="sxs-lookup"><span data-stu-id="6a351-136">Updating Bash on Ubuntu on Windows</span></span>

<span data-ttu-id="6a351-137">Es gibt zwei Komponenten von Bash unter Ubuntu unter Windows, die eine Aktualisierung erfordern.</span><span class="sxs-lookup"><span data-stu-id="6a351-137">There are two components of Bash on Ubuntu on Windows that can require updating.</span></span>

1. <span data-ttu-id="6a351-138">Das Windows-Subsystem für Linux</span><span class="sxs-lookup"><span data-stu-id="6a351-138">The Windows Subsystem for Linux</span></span>
  
   <span data-ttu-id="6a351-139">Durch das Upgrade dieses Teils von Bash unter Ubuntu unter Windows werden alle neuen Problembehandlungen aktiviert, die in den [Anmerkungen zu dieser Version](./release-notes.md) beschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="6a351-139">Upgrading this portion of Bash on Ubuntu on Windows will enable any new fixes outlines in the [release notes](./release-notes.md).</span></span> <span data-ttu-id="6a351-140">Stellen Sie sicher, dass Sie das Windows-Insider-Programm abonniert haben und dass Ihr Build auf dem neuesten Stand ist.</span><span class="sxs-lookup"><span data-stu-id="6a351-140">Ensure that you are subscribed to the Windows Insider Program and that your build is up to date.</span></span> <span data-ttu-id="6a351-141">Informationen zu einer genaueren Steuerung (einschließlich des Zurücksetzens der Ubuntu-Instanz) finden Sie auf der [Befehlsreferenzseite](./reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a351-141">For finer grain control including resetting your Ubuntu instance check out the [command reference page](./reference.md).</span></span>

2. <span data-ttu-id="6a351-142">Die Ubuntu-Benutzerbinärdateien</span><span class="sxs-lookup"><span data-stu-id="6a351-142">The Ubuntu user binaries</span></span>

   <span data-ttu-id="6a351-143">Durch das Upgrade dieses Teils von Bash unter Ubuntu unter Windows werden alle Updates der Ubuntu-Benutzerbinärdateien einschließlich der Anwendungen installiert, die Sie über apt-get installiert haben.</span><span class="sxs-lookup"><span data-stu-id="6a351-143">Upgrading this portion of Bash on Ubuntu on Windows will install any updates to the Ubuntu user binaries including applications that you have installed via apt-get.</span></span> <span data-ttu-id="6a351-144">Führen Sie die folgenden Befehle in Bash aus, um das Update auszuführen:</span><span class="sxs-lookup"><span data-stu-id="6a351-144">To update run the following commands in Bash:</span></span>
  
   1. `apt-get update`
   2. `apt-get upgrade`
  
### <a name="apt-get-upgrade-errors"></a><span data-ttu-id="6a351-145">Apt-get-Upgradefehler</span><span class="sxs-lookup"><span data-stu-id="6a351-145">Apt-get upgrade errors</span></span>

<span data-ttu-id="6a351-146">In einigen Paketen werden Features verwendet, die noch nicht implementiert wurden.</span><span class="sxs-lookup"><span data-stu-id="6a351-146">Some packages use features that we haven't implemented yet.</span></span> <span data-ttu-id="6a351-147">`udev` wird z.B. noch nicht unterstützt und verursacht mehrere `apt-get upgrade`-Fehler.</span><span class="sxs-lookup"><span data-stu-id="6a351-147">`udev`, for example, isn't supported yet and causes several `apt-get upgrade` errors.</span></span>

<span data-ttu-id="6a351-148">Führen Sie die folgenden Schritte aus, um Probleme im Zusammenhang mit `udev` zu beheben:</span><span class="sxs-lookup"><span data-stu-id="6a351-148">To fix issues related to `udev`, follow the following steps:</span></span>

1. <span data-ttu-id="6a351-149">Schreiben Sie Folgendes in `/usr/sbin/policy-rc.d`, und speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="6a351-149">Write the following to `/usr/sbin/policy-rc.d` and save your changes.</span></span>
  
   ``` BASH
   #!/bin/sh
   exit 101
   ```
  
2. <span data-ttu-id="6a351-150">Fügen Sie `/usr/sbin/policy-rc.d` Ausführungsberechtigungen hinzu:</span><span class="sxs-lookup"><span data-stu-id="6a351-150">Add execute permissions to `/usr/sbin/policy-rc.d`:</span></span>

   ``` BASH
   chmod +x /usr/sbin/policy-rc.d
   ```
  
3. <span data-ttu-id="6a351-151">Führen Sie die folgenden Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="6a351-151">Run the following commands:</span></span>

   ``` BASH
   dpkg-divert --local --rename --add /sbin/initctl
   ln -s /bin/true /sbin/initctl
   ```
  
### <a name="error-0x80040306-on-installation"></a><span data-ttu-id="6a351-152">„Error: 0x80040306“ bei der Installation</span><span class="sxs-lookup"><span data-stu-id="6a351-152">"Error: 0x80040306" on installation</span></span>

<span data-ttu-id="6a351-153">Dies hat mit der Tatsache zu tun, dass die Legacykonsole nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="6a351-153">This has to do with the fact that we do not support legacy console.</span></span>
<span data-ttu-id="6a351-154">So deaktivieren Sie die Legacykonsole:</span><span class="sxs-lookup"><span data-stu-id="6a351-154">To turn off legacy console:</span></span>

1. <span data-ttu-id="6a351-155">Öffnen Sie „cmd. exe“.</span><span class="sxs-lookup"><span data-stu-id="6a351-155">Open cmd.exe</span></span>
1. <span data-ttu-id="6a351-156">Klicken Sie mit der rechten Maustaste auf der Titelleiste auf „Eigenschaften“. Deaktivieren Sie die Option „Legacykonsole verwenden“.</span><span class="sxs-lookup"><span data-stu-id="6a351-156">Right click title bar -> Properties -> Uncheck Use legacy console</span></span>
1. <span data-ttu-id="6a351-157">Auf "OK" klicken</span><span class="sxs-lookup"><span data-stu-id="6a351-157">Click OK</span></span>

### <a name="error-0x80040154-after-windows-update"></a><span data-ttu-id="6a351-158">„Error: 0x80040154“ nach Windows-Update</span><span class="sxs-lookup"><span data-stu-id="6a351-158">"Error: 0x80040154" after Windows update</span></span>

<span data-ttu-id="6a351-159">Das Feature „Windows-Subsystem für Linux“ ist möglicherweise während eines Windows-Updates deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6a351-159">The Windows Subsystem for Linux feature may be disabled during a Windows update.</span></span> <span data-ttu-id="6a351-160">Wenn dies der Fall ist, muss das Windows-Feature erneut aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="6a351-160">If this happens the Windows feature must be re-enabled.</span></span> <span data-ttu-id="6a351-161">Anweisungen zum Aktivieren des Windows-Subsystems für Linux finden Sie im [Installationsleitfaden](./install-win10.md).</span><span class="sxs-lookup"><span data-stu-id="6a351-161">Instructions for enabling the Windows Subsystem for Linux can be found in the [Installation Guide](./install-win10.md).</span></span>

### <a name="changing-the-display-language"></a><span data-ttu-id="6a351-162">Ändern der Anzeigesprache</span><span class="sxs-lookup"><span data-stu-id="6a351-162">Changing the display language</span></span>

<span data-ttu-id="6a351-163">Die WSL-Installation versucht, das Ubuntu-Gebietsschema automatisch so zu ändern, dass es dem Gebietsschema Ihrer Windows-Installation entspricht.</span><span class="sxs-lookup"><span data-stu-id="6a351-163">WSL install will try to automatically change the Ubuntu locale to match the locale of your Windows install.</span></span>  <span data-ttu-id="6a351-164">Wenn Sie dieses Verhalten nicht wünschen, können Sie diesen Befehl ausführen, um das Ubuntu-Gebietsschema zu ändern, nachdem die Installation abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="6a351-164">If you do not want this behavior you can run this command to change the Ubuntu locale after install completes.</span></span>  <span data-ttu-id="6a351-165">Sie müssen „bash.exe“ neu starten, damit diese Änderung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="6a351-165">You will have to relaunch bash.exe for this change to take effect.</span></span>

<span data-ttu-id="6a351-166">Im folgenden Beispiel wird das Gebietsschema in „en-US“ geändert:</span><span class="sxs-lookup"><span data-stu-id="6a351-166">The below example changes to locale to en-US:</span></span>

``` BASH
sudo update-locale LANG=en_US.UTF8
```

### <a name="installation-issues-after-windows-system-restore"></a><span data-ttu-id="6a351-167">Installationsprobleme nach der Windows-Systemwiederherstellung</span><span class="sxs-lookup"><span data-stu-id="6a351-167">Installation issues after Windows system restore</span></span>

1. <span data-ttu-id="6a351-168">Löschen Sie den Ordner `%windir%\System32\Tasks\Microsoft\Windows\Windows Subsystem for Linux`.</span><span class="sxs-lookup"><span data-stu-id="6a351-168">Delete the `%windir%\System32\Tasks\Microsoft\Windows\Windows Subsystem for Linux` folder.</span></span> <br/>
  <span data-ttu-id="6a351-169">**Hinweis: Unterlassen Sie dies, wenn Ihre optionale Funktion vollständig installiert und funktionsfähig ist.**</span><span class="sxs-lookup"><span data-stu-id="6a351-169">**Note: Do not do this if your optional feature is fully installed and working.**</span></span>
2. <span data-ttu-id="6a351-170">Aktivieren Sie das optionale WSL-Feature (falls noch nicht geschehen).</span><span class="sxs-lookup"><span data-stu-id="6a351-170">Enable the WSL optional feature (if not already)</span></span>
3. <span data-ttu-id="6a351-171">Neustart</span><span class="sxs-lookup"><span data-stu-id="6a351-171">Reboot</span></span>
4. <span data-ttu-id="6a351-172">lxrun/uninstall/full</span><span class="sxs-lookup"><span data-stu-id="6a351-172">lxrun /uninstall /full</span></span>
5. <span data-ttu-id="6a351-173">Installieren von Bash</span><span class="sxs-lookup"><span data-stu-id="6a351-173">Install bash</span></span>

### <a name="no-internet-access-in-wsl"></a><span data-ttu-id="6a351-174">Kein Internetzugriff in WSL</span><span class="sxs-lookup"><span data-stu-id="6a351-174">No internet access in WSL</span></span>

<span data-ttu-id="6a351-175">Einige Benutzer haben Probleme mit bestimmten Firewallanwendungen gemeldet, die den Internetzugriff in WSL blockieren.</span><span class="sxs-lookup"><span data-stu-id="6a351-175">Some users have reported issues with specific firewall applications blocking internet access in WSL.</span></span>  <span data-ttu-id="6a351-176">Die gemeldeten Firewalls sind:</span><span class="sxs-lookup"><span data-stu-id="6a351-176">The firewalls reported are:</span></span>

1. <span data-ttu-id="6a351-177">Kaspersky</span><span class="sxs-lookup"><span data-stu-id="6a351-177">Kaspersky</span></span>
2. <span data-ttu-id="6a351-178">AVG</span><span class="sxs-lookup"><span data-stu-id="6a351-178">AVG</span></span>
3. <span data-ttu-id="6a351-179">Avast</span><span class="sxs-lookup"><span data-stu-id="6a351-179">Avast</span></span>

<span data-ttu-id="6a351-180">In einigen Fällen ermöglicht das Deaktivieren der Firewall den Zugriff.</span><span class="sxs-lookup"><span data-stu-id="6a351-180">In some cases turning off the firewall allows for access.</span></span>  <span data-ttu-id="6a351-181">In einigen Fällen sieht es so aus, als ob bereits die Installation der Firewall den Zugriff blockiert.</span><span class="sxs-lookup"><span data-stu-id="6a351-181">In some cases simply having the firewall installed looks to block access.</span></span>

### <a name="permission-denied-error-when-using-ping"></a><span data-ttu-id="6a351-182">Fehler des Typs „Berechtigung verweigert“ bei Verwendung von Ping</span><span class="sxs-lookup"><span data-stu-id="6a351-182">Permission Denied error when using ping</span></span>

<span data-ttu-id="6a351-183">Für [Windows Anniversary Update, Version 1607](./release-notes.md#build-14388-to-windows-10-anniversary-update), sind **Administratorberechtigungen** in Windows erforderlich, um Ping in WSL auszuführen.</span><span class="sxs-lookup"><span data-stu-id="6a351-183">For [Windows Anniversary Update, version 1607](./release-notes.md#build-14388-to-windows-10-anniversary-update), **administrator privileges** in Windows are required to run ping in WSL.</span></span>  <span data-ttu-id="6a351-184">Um Ping auszuführen, führen Sie Bash unter Ubuntu unter Windows als Administrator aus, oder starten Sie „bash.exe“ über eine CMD-/PowerShell-Eingabeaufforderung mit Administratorrechten.</span><span class="sxs-lookup"><span data-stu-id="6a351-184">To run ping, run Bash on Ubuntu on Windows as an administrator, or run bash.exe from a CMD/PowerShell prompt with administrator privileges.</span></span>

<span data-ttu-id="6a351-185">Für spätere Versionen von Windows, [ab Build 14926](./release-notes.md#build-14926), sind Administratorberechtigungen nicht mehr erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a351-185">For later versions of Windows, [Build 14926+](./release-notes.md#build-14926), administrator privileges are no longer required.</span></span>

### <a name="bash-is-hung"></a><span data-ttu-id="6a351-186">Bash reagiert nicht</span><span class="sxs-lookup"><span data-stu-id="6a351-186">Bash is hung</span></span>

<span data-ttu-id="6a351-187">Wenn Sie beim Arbeiten mit Bash feststellen, dass Bash hängt (oder blockiert ist) und nicht mehr auf Eingaben reagiert, helfen Sie uns, das Problem zu diagnostizieren, indem Sie ein Speicherabbild erfassen und melden.</span><span class="sxs-lookup"><span data-stu-id="6a351-187">If while working with bash, you find that bash is hung (or deadlocked) and not responding to inputs, help us diagnose the issue by collecting and reporting a memory dump.</span></span> <span data-ttu-id="6a351-188">Beachten Sie, dass diese Schritte zu einem Absturz Ihres Systems führen.</span><span class="sxs-lookup"><span data-stu-id="6a351-188">Note that these steps will crash your system.</span></span> <span data-ttu-id="6a351-189">Unterlassen Sie dies, wenn Sie damit nicht einverstanden sind, oder speichern Sie Ihre Arbeit zuvor.</span><span class="sxs-lookup"><span data-stu-id="6a351-189">Do not do this if you are not comfortable with that or save your work prior to doing this.</span></span>

<span data-ttu-id="6a351-190">So erfassen Sie ein Speicherabbild</span><span class="sxs-lookup"><span data-stu-id="6a351-190">To collect a memory dump</span></span>

1. <span data-ttu-id="6a351-191">Ändern Sie den Typ des Speicherabbilds in „Vollständiges Speicherabbild“.</span><span class="sxs-lookup"><span data-stu-id="6a351-191">Change the memory dump type to "complete memory dump".</span></span> <span data-ttu-id="6a351-192">Notieren Sie sich den aktuellen Typ, bevor Sie den Speicherabbildtyp ändern.</span><span class="sxs-lookup"><span data-stu-id="6a351-192">While changing the dump type, take a note of your current type.</span></span>

2. <span data-ttu-id="6a351-193">Verwenden Sie diese [Schritte](https://techcommunity.microsoft.com/t5/Core-Infrastructure-and-Security/How-to-Force-a-Diagnostic-Memory-Dump-When-a-Computer-Hangs/ba-p/257809) zum Konfigurieren von Abstürzen mithilfe der Tastatursteuerung.</span><span class="sxs-lookup"><span data-stu-id="6a351-193">Use the [steps](https://techcommunity.microsoft.com/t5/Core-Infrastructure-and-Security/How-to-Force-a-Diagnostic-Memory-Dump-When-a-Computer-Hangs/ba-p/257809) to configure crash using keyboard control.</span></span>

3. <span data-ttu-id="6a351-194">Reproduzieren Sie das Hängen oder die Blockade.</span><span class="sxs-lookup"><span data-stu-id="6a351-194">Repro the hang or deadlock.</span></span>

4. <span data-ttu-id="6a351-195">Lassen Sie das System mithilfe der Tastensequenz aus (2) abstürzen.</span><span class="sxs-lookup"><span data-stu-id="6a351-195">Crash the system using the key sequence from (2).</span></span>

5. <span data-ttu-id="6a351-196">Das System stürzt ab und erfasst das Speicherabbild.</span><span class="sxs-lookup"><span data-stu-id="6a351-196">The system will crash and collect the memory dump.</span></span>

6. <span data-ttu-id="6a351-197">Nachdem das System neu gestartet wurde, übermitteln Sie die Datei „memory.dmp“ an secure@microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="6a351-197">Once the system reboots, report the memory.dmp to secure@microsoft.com.</span></span> <span data-ttu-id="6a351-198">Der Standardspeicherort der Speicherabbilddatei ist „%SystemRoot%\memory.dmp“ oder „C:\Windows\memory.dmp“, wenn „C:“ das Systemlaufwerk ist.</span><span class="sxs-lookup"><span data-stu-id="6a351-198">The default location of the dump file is %SystemRoot%\memory.dmp or C:\Windows\memory.dmp if C: is the system drive.</span></span> <span data-ttu-id="6a351-199">Geben Sie in der E-Mail an, dass das Speicherabbild für das WSL- oder Bash unter Windows-Team vorgesehen ist.</span><span class="sxs-lookup"><span data-stu-id="6a351-199">In the email, note that the dump is for the WSL or Bash on Windows team.</span></span>

7. <span data-ttu-id="6a351-200">Stellen Sie die ursprünglichen Einstellung für den Speicherabbildtyp wieder her.</span><span class="sxs-lookup"><span data-stu-id="6a351-200">Restore the memory dump type to the original setting.</span></span>

### <a name="check-your-build-number"></a><span data-ttu-id="6a351-201">Überprüfen der Buildnummer</span><span class="sxs-lookup"><span data-stu-id="6a351-201">Check your build number</span></span>

<span data-ttu-id="6a351-202">Um die Architektur des PCs und die Windows-Buildnummer zu ermitteln, öffnen Sie</span><span class="sxs-lookup"><span data-stu-id="6a351-202">To find your PC's architecture and Windows build number, open</span></span>  
<span data-ttu-id="6a351-203">**Einstellungen** > **System** > **Info**</span><span class="sxs-lookup"><span data-stu-id="6a351-203">**Settings** > **System** > **About**</span></span>

<span data-ttu-id="6a351-204">Suchen Sie nach den Feldern **Betriebssystembuild** und **Systemtyp**.</span><span class="sxs-lookup"><span data-stu-id="6a351-204">Look for the **OS Build** and **System Type** fields.</span></span>  
    <span data-ttu-id="6a351-205">![Screenshot der Felder „Betriebssystembuild“ und „Systemtyp“](media/system.png)</span><span class="sxs-lookup"><span data-stu-id="6a351-205">![Screenshot of Build and System Type fields](media/system.png)</span></span>

<span data-ttu-id="6a351-206">Führen Sie Folgendes in PowerShell aus, um die Windows Server-Buildnummer zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="6a351-206">To find your Windows Server build number, run the following in PowerShell:</span></span>  

``` PowerShell
systeminfo | Select-String "^OS Name","^OS Version"
```

### <a name="confirm-wsl-is-enabled"></a><span data-ttu-id="6a351-207">Bestätigen, dass WSL aktiviert ist</span><span class="sxs-lookup"><span data-stu-id="6a351-207">Confirm WSL is enabled</span></span>

<span data-ttu-id="6a351-208">Sie können bestätigen, dass das Windows-Subsystem für Linux aktiviert ist, indem Sie Folgendes in PowerShell ausführen:</span><span class="sxs-lookup"><span data-stu-id="6a351-208">You can confirm that the Windows Subsystem for Linux is enabled by running the following in PowerShell:</span></span>  

``` PowerShell
Get-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

### <a name="openssh-server-connection-issues"></a><span data-ttu-id="6a351-209">Verbindungsprobleme des OpenSSH-Servers</span><span class="sxs-lookup"><span data-stu-id="6a351-209">OpenSSH-Server connection issues</span></span>

<span data-ttu-id="6a351-210">Beim Versuch, den SSH-Server zu verbinden, tritt ein Fehler auf: „Connection closed by 127.0.0.1 port 22“ (Verbindung wurde durch 127.0.0.1 Port 22 geschlossen).</span><span class="sxs-lookup"><span data-stu-id="6a351-210">Trying to connect your SSH server is failed with the following error: "Connection closed by 127.0.0.1 port 22".</span></span>

1. <span data-ttu-id="6a351-211">Stellen Sie sicher, dass der OpenSSH-Server ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="6a351-211">Make sure your OpenSSH Server is running:</span></span>

   ``` BASH
   sudo service ssh status
   ```

   <span data-ttu-id="6a351-212">und Sie dieses Tutorial befolgt haben: https://help.ubuntu.com/lts/serverguide/openssh-server.html.en</span><span class="sxs-lookup"><span data-stu-id="6a351-212">and you've followed this tutorial: https://help.ubuntu.com/lts/serverguide/openssh-server.html.en</span></span>

2. <span data-ttu-id="6a351-213">Beenden Sie den sshd-Dienst, und starten Sie sshd im Debugmodus:</span><span class="sxs-lookup"><span data-stu-id="6a351-213">Stop the sshd service and start sshd in debug mode:</span></span>

   ``` BASH
   sudo service ssh stop
   sudo /usr/sbin/sshd -d
   ```

3. <span data-ttu-id="6a351-214">Überprüfen Sie die Startprotokolle, und stellen Sie sicher, dass HostKeys verfügbar sind und keine Protokollmeldungen wie die folgenden angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="6a351-214">Check the startup logs and make sure HostKeys are available and you don't see log messages such as:</span></span>

   ```BASH
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

<span data-ttu-id="6a351-215">Wenn solche Meldungen angezeigt werden und die Schlüssel unter `/etc/ssh/` fehlen, müssen Sie die Schlüssel neu generieren oder openssh-server einfach bereinigen und installieren:</span><span class="sxs-lookup"><span data-stu-id="6a351-215">If you do see such messages and the keys are missing under `/etc/ssh/`, you will have to regenerate the keys or just purge&install openssh-server:</span></span>

```BASH
sudo apt-get purge openssh-server
sudo apt-get install openssh-server
```

### <a name="the-referenced-assembly-could-not-be-found-when-enabling-the-wsl-optional-feature"></a><span data-ttu-id="6a351-216">"Die referenzierte Assembly konnte nicht gefunden werden."</span><span class="sxs-lookup"><span data-stu-id="6a351-216">"The referenced assembly could not be found."</span></span> <span data-ttu-id="6a351-217">beim Aktivieren des optionalen WSL-Features</span><span class="sxs-lookup"><span data-stu-id="6a351-217">when enabling the WSL optional feature</span></span>

<span data-ttu-id="6a351-218">Dieser Fehler bezieht sich auf einen fehlerhaften Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="6a351-218">This error is related to being in a bad install state.</span></span> <span data-ttu-id="6a351-219">Führen Sie die folgenden Schritte aus, um eine Behebung dieses Problems zu versuchen:</span><span class="sxs-lookup"><span data-stu-id="6a351-219">Please complete the following steps to try and fix this issue:</span></span>

- <span data-ttu-id="6a351-220">Wenn Sie den Befehl zum Aktivieren des WSL-Features aus PowerShell ausführen, versuchen Sie stattdessen, die grafische Benutzeroberfläche zu verwenden, indem Sie das Startmenü öffnen, nach „Windows-Features aktivieren oder deaktivieren“ suchen und dann in der Liste „Windows Subsystem für Linux“ auswählen, wodurch die optionale Komponente installiert wird.</span><span class="sxs-lookup"><span data-stu-id="6a351-220">If you are running the enable WSL feature command from PowerShell, try using the GUI instead by opening the start menu, searching for 'Turn Windows features on or off' and then in the list select 'Windows Subsystem for Linux' which will install the optional component.</span></span>

- <span data-ttu-id="6a351-221">Aktualisieren Sie Ihre Windows-Version, indem Sie zu „Einstellungen“, „Updates“ wechseln und dann auf „Nach Updates suchen“ klicken</span><span class="sxs-lookup"><span data-stu-id="6a351-221">Update your version of Windows by going to Settings, Updates, and clicking 'Check for Updates'</span></span>

- <span data-ttu-id="6a351-222">Wenn beide Versuche erfolglos bleiben und Sie auf WSL zugreifen müssen, erwägen Sie, ein lokales Upgrade auszuführen, indem Sie Windows 10 mithilfe der Installationsmedien erneut installieren und „Alles beibehalten“ auswählen, um sicherzustellen, dass Ihre Apps und Dateien erhalten bleiben.</span><span class="sxs-lookup"><span data-stu-id="6a351-222">If both of those fail and you need to access WSL please consider upgrading in place by reinstalling Windows 10 using installation media and selecting 'Keep Everything' to ensure your apps and files are preserved.</span></span> <span data-ttu-id="6a351-223">Anweisungen dazu finden Sie auf der Seite [Erneutes Installieren von Windows 10](https://support.microsoft.com/help/4000735/windows-10-reinstall).</span><span class="sxs-lookup"><span data-stu-id="6a351-223">You can find instructions on how to do so at the [Reinstall Windows 10 page](https://support.microsoft.com/help/4000735/windows-10-reinstall).</span></span>
