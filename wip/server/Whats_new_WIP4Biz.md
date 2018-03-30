---
title: What’s New in Windows Server 2019 Insider Preview
description: new features for you to test
ms.author: dawnwood
ms.date: 4/5/2018
---
#What’s New in Windows Server 2019 Insider Preview
The features listed below have been made available in preview builds of Windows Server 2019 via the Windows Server Insider Program.  To obtain the Insider software downloads, registered Insiders may navigate directly to the [Windows Server Insider Preview download page](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewserver).  If you have not yet registered as an Insider, see [GETTING STARTED WITH SERVER](https://insider.windows.com/en-us/for-business-getting-started-server/) on the [Windows Insiders for Business](https://insider.windows.com/ForBusiness) portal. We also encourage you to visit the [Windows Server Insiders space](https://techcommunity.microsoft.com/t5/Windows-Server-Insiders/bd-p/WindowsServerInsiders) on the [Microsoft Tech Communities forum](https://techcommunity.microsoft.com/) to collaborate, share and learn from experts.

Validation for every preview: There are two major areas that we would like you to try out in each preview release and report back any issues: 
* <b>In-place OS Upgrade </b> (from Windows Server 2012 R2, Windows Server 2016) 
* <b>Application compatibility </b> Let us know if any server roles or applications stops working or fails to function as it used to. 

<b>Extending your Clusters with Cluster Sets</b>

“Cluster Sets” is the new cloud scale-out technology in this Preview release that increases cluster node count in a single SDDC (Software-Defined Data Center) cloud by orders of magnitude. A Cluster Set is a loosely-coupled grouping of multiple Failover Clusters: compute, storage or hyper-converged. Cluster Sets technology enables virtual machine fluidity across member clusters within a Cluster Set and a unified storage namespace across the "set" in support of virtual machine fluidity.  While preserving existing Failover Cluster management experiences on member clusters, a Cluster Set instance additionally offers key use cases around lifecycle management of a Cluster Set at the aggregate.

<b>Windows Defender Advanced Threat Protection</b>

We provide deep platform sensors and response actions, providing visibility to memory and kernel level attacker activities and abilities to take actions on compromised machines in response to incidents such as remote collection of additional forensic data, remediating malicious files, terminating malicious processes etc. 
 
If you’re already using Windows Defender Advanced Threat Protection (ATP), preview these features by simply installing the latest preview build of Windows Server, and onboard it to Windows Defender ATP. 

Otherwise, sign up for the Windows Defender ATP trial on [Windows
Defender Advanced Threat
Protection](https://www.microsoft.com/en-us/windowsforbusiness/windows-atp).

<b>Windows Defender ATP Exploit Guard</b>

Windows Defender ATP Exploit Guard is a new set of host-intrusion
prevention capabilities. The four components of Windows Defender Exploit
Guard are designed to lock down the device against a wide variety of
attack vectors and block behaviors commonly used in malware attacks,
while enabling enterprises to balance their security risk and
productivity requirements.

-   <b><a href="https://docs.microsoft.com/en-us/windows/threat-protection/windows-defender-exploit-guard/attack-surface-reduction-exploit-guard?ocid=cx-blog-mmpc">Attack Surface Reduction
    (ASR)</a></b>:
    A set of controls that enterprises can enable to prevent malware
    from getting on the machine by blocking suspicious malicious files
    (for example, Office files), scripts, lateral movement, ransomware
    behavior, and email-based threats.

-   [**Network
    protection**](https://docs.microsoft.com/en-us/windows/threat-protection/windows-defender-exploit-guard/network-protection-exploit-guard?ocid=cx-blog-mmpc):
    Protects the endpoint against web-based threats by blocking any
    outbound process on the device to untrusted hosts/IP addresses
    through Windows Defender SmartScreen.

-   [**Controlled folder
    access**](https://blogs.technet.microsoft.com/mmpc/2017/10/23/stopping-ransomware-where-it-counts-protecting-your-data-with-controlled-folder-access?ocid=cx-blog-mmpc):
    Protects sensitive data from ransomware by blocking untrusted
    processes from accessing your protected folders.

-   [**Exploit
    protection**](https://docs.microsoft.com/en-us/windows/threat-protection/windows-defender-exploit-guard/exploit-protection-exploit-guard?ocid=cx-blog-mmpc):
    A set of mitigations for vulnerability exploits (replacing EMET)
    that can be easily configured to protect your system and
    applications.

To deploy a default set of Exploit Guard policy on Windows Server, run
the following cmdlets:
<pre>
Set-MpPreference -EnableControlledFolderAccess Enabled

Set-MpPreference -EnableNetworkProtection Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
75668C1F-73B5-4CF0-BB93-3ECF5CB7CC84
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
3B576869-A4EC-4529-8536-B80A7769E899
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
D4F940AB-401B-4EfC-AADC-AD5F3C50688A
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
D3E037E1-3EB8-44C8-A917-57927947596D
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
5BEB7EFE-FD9A-4556-801D-275E5FFC04CC
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
BE9BA2D9-53EA-4CDC-84E5-9B1EEEE46550
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
92E97FA1-2EDF-4476-BDD6-9DD0B4DDDC7B
-AttackSurfaceReductionRules\_Actions Enabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
D1E49AAC-8F56-4280-B9BA-993A6D77406C
-AttackSurfaceReductionRules\_Actions Disabled

Add-MpPreference -AttackSurfaceReductionRules\_Ids
01443614-cd74-433a-b99e-2ecdc07bfc25
-AttackSurfaceReductionRules\_Actions Enabled

$url = 'https://demo.wd.microsoft.com/Content/ProcessMitigation.xml'

Invoke-WebRequest $url -OutFile ProcessMitigation.xml

Write-Host "Enabling Exploit Protection"

Set-ProcessMitigation -PolicyFilePath ProcessMitigation.xml
</pre>


<b>Windows Defender Application Control</b>

Windows Defender Application Control—also known as Code Integrity (CI) policy—was released in Windows Server 2016. Customer feedback has suggested that it is a great concept, but hard to deploy. To address this, we are building default CI policies, which will allow all Windows in-box files and Microsoft applications, such as SQL Server, and block known executables that can bypass CI.  
You can download the default policies at: [https://developer.microsoft.com/en-us/dashboard/collaborate/packages/4265](https://developer.microsoft.com/en-us/dashboard/collaborate/packages/4265).

The package contains an audit version and an enforced version. If the server doesn’t require additional drivers/applications, you can deploy the enforced version. Otherwise, you can use the audit policy, check uncovered executables, and then merge them into the default CI policy. 

To deploy the default code integrity policy, run the following commands:

Copy-Item C:\\CI\\ServerDefault-EnforcedCI.bin
C:\\Windows\\System32\\CodeIntegrity\\SiPolicy.p7b

Reboot the server to allow code integrity service to load the policy.


<b>Failover Cluster removing use of NTLM authentication</b>

Windows Server Failover Clusters no longer use NTLM authentication by exclusively using Kerberos and certificate based authentication.  There are no changes required by the user, or deployment tools,  to take advantage of this security enhancement.  It also allows failover clusters to be deployed in environments where NTLM has been disabled. 

<b>Shielded virtual machines – Offline mode, VMConnect and Linux support</b>

You can now run [shielded virtual
machines](https://docs.microsoft.com/en-us/windows-server/virtualization/guarded-fabric-shielded-vm/guarded-fabric-and-shielded-vms)
on machines with intermittent connectivity to the Host Guardian Service
by leveraging the new fallback HGS and offline mode features. Fallback
HGS allows you to configure a second set of URLs for Hyper-V to try if
it can't reach your primary HGS server. To see how this can be used in a
branch-office scenario, see [Improved branch office support for shielded
VMs in Windows Server, version
1709](https://blogs.technet.microsoft.com/datacentersecurity/2017/11/15/improved-branch-office-support-for-shielded-vms-in-windows-server-version-1709/)
on our blog. [Offline
mode](https://docs.microsoft.com/en-us/windows-server/virtualization/guarded-fabric-shielded-vm/guarded-fabric-manage-branch-office#offline-mode)
allows you to continue to start up your shielded VMs, even if HGS can't
be reached, as long as the VM has started successfully once, and the
host's security configuration has not changed. (To enable offline mode,
run the following command on the Host Guardian Service:
**Set-HgsKeyProtectionConfiguration –AllowKeyMaterialCaching**.)

We've also made it easier to troubleshoot your shielded virtual machines
by enabling support for VMConnect Enhanced Session Mode and PowerShell
Direct. These tools are particularly useful if you've lost network
connectivity to your VM and need to update its configuration to restore
access. These features do not need to be configured, and they will
automatically become available when a shielded VM is placed on a Hyper-V
host running build 17040 or later.

For customers who run mixed-OS environments, we now support running
Ubuntu, Red Hat Enterprise Linux, and SUSE Linux Enterprise Server
inside shielded virtual machines. Try it out—[Create a Linux shielded VM
template
disk](https://docs.microsoft.com/en-us/windows-server/virtualization/guarded-fabric-shielded-vm/guarded-fabric-create-a-linux-shielded-vm-template)—and
send us your feedback in the Feedback Hub.

<b>Encrypted Network in SDN</b>

Network traffic going out from a VM host can be snooped on and/or
manipulated by anyone with access to the physical fabric. While shielded
VMs protect VM data from theft and manipulation, similar protection is
required for network traffic to and from a VM. While the tenant can
setup protection such as IPSEC, this is difficult due to configuration
complexity and heterogeneous environments.

Encrypted Networks is a feature which provides simple to configure
DTLS-based encryption using the Network Controller to manage the
end-to-end encryption and protect data as it travels through the wires
and network devices between the hosts It is configured by the
Administrator on a per-subnet basis.  This enables the VM to VM traffic
within the VM subnet to be automatically encrypted as it leaves the host
and prevents snooping and manipulation of traffic on the wire. This is
done without requiring any configuration changes in the VMs themselves.
Try it out—[Configure Encryption for a Virtual
Subnet](https://docs.microsoft.com/en-us/windows-server/networking/sdn/vnet-encryption/sdn-config-vnet-encryption)—and
send us your feedback in the Feedback Hub.

If you are using Storage Spaces Direct, take a look at another area to
explore for this release: performance history for Storage Spaces Direct.

<b>Software Defined Datacenter</b>
If you are using Storage Spaces Direct, take a look at  performance history for Storage Spaces Direct. 

<b>Performance history for Storage Spaces Direct</b>

Administrators of [Storage Spaces
Direct](https://docs.microsoft.com/windows-server/storage/storage-spaces/storage-spaces-direct-overview)
can now get easy access to historical performance and capacity data from
their cluster. *Did CPU usage spike last night? When did this drive
become slow? Which virtual machine used the most memory last month? Is
network activity trending up or down? The cluster is pushing 1,000,000
IOPS – is that my new record?* Previously, you'd need external tooling
to answer these questions. No more!

Beginning in build 17090, beautiful new charts in [Project
Honolulu](https://docs.microsoft.com/en-us/windows-server/manage/honolulu/honolulu-manage-hci)
(and new PowerShell cmdlets, for those so inclined) empower you to
answer these questions. There's nothing to install, configure, or
start—it's built-in and always-on. Learn more at
<https://aka.ms/clusterperformancehistory>.

<img src="C:\repos\release_notes\rs5\server\prime\17609.1001_Windows_Server_vNext_LTSC_Preview\images\chart.gif" style="width:6.5in;height:3.65625in" />

*Caption: New charts in Project Honolulu, powered by built-in cluster
performance history.*

## Available Content
<b>Windows Server 2019 LTSC Build 17623</b> is available in ISO format in 18 languages. This build and all future pre-release builds will require use of activation keys during setup. The following keys allow for unlimited activations:
<table>
    <tr>
        <td>Datacenter Edition
        </td>
        <td>6XBNX-4JQGW-QX6QG-74P76-72V67
        </td>
    </tr>
    <tr>
        <td>Standard Edition
        </td>
        <td>MFY9F-XBN2F-TYFMP-CCV49-RMYVH
        </td>
    </tr>
</table>
<b>Windows Server vNext Semi-Annual Build 17623</b> The Server Core Edition is available in English only, in ISO or VHDX format. The images are pre-keyed –  no need to enter a key during setup.
<b>Symbols</b> are available on the public symbol server – see [Update on Microsoft’s Symbol Server](https://blogs.msdn.microsoft.com/windbg/2017/10/18/update-on-microsofts-symbol-server/) blog post and [Using the Microsoft Symbol Server](https://msdn.microsoft.com/library/windows/desktop/ee416588(v=vs.85).aspx#using_the_microsoft_symbol_server). As before, matching Windows Server container images will be available via Docker Hub. For more information about Windows Server containers and Insider builds, click [here](http://aka.ms/containers/insiders).

This build will expire July 2nd, 2018.

## How to download
To obtain the Insider software downloads, registered Insiders may navigate directly to the [Windows Server Insider Preview download page](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewserver).  If you have not yet registered as an Insider, see [GETTING STARTED WITH SERVER](https://insider.windows.com/en-us/for-business-getting-started-server/) on the [Windows Insiders for Business portal](https://insider.windows.com/ForBusiness).

## It's all about your feedback!
The most important part of a frequent release cycle is to hear what’s working and what needs to be improved, so your feedback is extremely valued. Use your registered Windows 10 Insider device and use the Feedback Hub application. In the app, choose the <b>Server</b> category and then the appropriate subcategory for your feedback. Please indicate what <b>build number</b> you are providing feedback on. We also encourage you to visit the [Windows Server Insiders](https://techcommunity.microsoft.com/t5/Windows-Server-Insiders/bd-p/WindowsServerInsiders) space on the [Microsoft Tech Communities](https://techcommunity.microsoft.com/) forum to collaborate, share and learn from experts.