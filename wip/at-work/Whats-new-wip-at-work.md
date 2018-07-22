---
title: What's new in the Windows Server 2019 Insider Preview Builds
description: New features to use and test in the Windows Insider Program for Server 2019 Preview Builds
services: WIP-at-work
author: dawn.wood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 04/10/2018
ms.author: dawn.wood
---

# What’s New in Windows Server 2019 Insider Preview Builds 

The features listed below are available in preview builds of Windows Server 2019 via the Windows Insider Program for Server. To obtain the Insider software downloads, registered Insiders may navigate directly to the [Windows Server Insider Preview download page](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewserver). If you have not yet registered as an Insider, see [Getting started with Server](https://insider.windows.com/en-us/for-business-getting-started-server/). 


We also encourage you to visit the [Windows Server Insiders space](https://techcommunity.microsoft.com/t5/Windows-Server-Insiders/bd-p/WindowsServerInsiders) on the [Microsoft Tech Communities forum](https://techcommunity.microsoft.com/) to collaborate, share, and learn from experts.

## Containers
### Group Managed Service Accounts 
We’ve improved the scalability and reliability of containers that use group managed service accounts (gMSA) to access network resources. You should see fewer authentication errors when using a single gMSA with multiple container instances. Additionally, you no longer need to set the container's host name to be the same as the gMSA. We also fixed a bug that prevented you from using gMSAs with Hyper-V isolated containers.  

### New Container base image: Windows 
We added a new base image to the Windows Server container collection. In addition to nanoserver and windowsservercore container images, the new windows image is now available. This image carries even more components than its nanoserver and servercore siblings, meaning it can support applications that have additional API dependencies. To learn more and get started, go to https://aka.ms/windowscontainer. 

## Delimit volume allocation with Storage Spaces Direct

New cmdlets simplify the management of volumes with delimited allocation. Use Get-StorageScaleUnit to see fault domains; follow associations to/from Get-VirtualDisk to see the current allocation; and set or modify allocation by using friendly names for fault domains. For more details, see the links under "Insider Preview content" on [aka.ms/StorageSpacesDirect](https://docs.microsoft.com/en-us/windows-server/storage/storage-spaces/storage-spaces-direct-overview).

## Encrypted Network in SDN

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

## Extending your Clusters with Cluster Sets

“Cluster Sets” is the new cloud scale-out technology that increases cluster node count in a single SDDC (Software-Defined Data Center) cloud by orders of magnitude. A Cluster Set is a loosely-coupled grouping of multiple Failover Clusters: compute, storage or hyper-converged. Cluster Sets technology enables virtual machine fluidity across member clusters within a Cluster Set and a unified storage namespace across the "set" in support of virtual machine fluidity.  While preserving existing Failover Cluster management experiences on member clusters, a Cluster Set instance additionally offers key use cases around lifecycle management of a Cluster Set at the aggregate.

## Failover clustering: file share witness

One of the witness options available for failover clustering, File Share Witness, has two new enhancements. 

The first enhancement blocks the use of a Distributed File System (DFS) share as a location. Adding a File Share Witness (FSW) to a DFS share can cause stability issues for your cluster, and this configuration has never been supported. So, we added logic to detect if a share uses DFS, and if DFS is detected, Failover Cluster Manager blocks creation of the witness and displays an error message about not being supported.

The second enhancement enables use of an FSW for several scenarios that were previously not supported: 
*  Absent or extremely poor Internet access because of a remote location, preventing the use of a cloud witness. 
*  Lack of shared drives for a disk witness. This could be a Storage Spaces Direct hyperconverged configuration, a SQL Server Always On Availability Groups (AG), or an *  Exchange Database Availability Group (DAG), none of which use shared disks. 
*  Lack of a domain controller connection due to the cluster being behind a DMZ. 
*  A workgroup or cross-domain cluster for which there is no Active Directory cluster name object (CNO). Find out more about these enhancements in the following post in Server & Management Blogs: [Failover Cluster File Share Witness and DFS](https://blogs.msdn.microsoft.com/clustering/2018/04/13/failover-cluster-file-share-witness-and-dfs/).

## Failover clustering: moving clusters between domains 
Moving a cluster from one domain to another has always been a daunting task because you must destroy the cluster to move it.  Depending on the roles in the cluster, that role must also be removed and recreated.  The following are two common scenarios:
Company A purchases Company B and must move all servers to Company A's domain 
Main office builds a cluster and ships it to another location 
We have added two new PowerShell commandlets to quickly take you from one domain to another without the need to destroy it.  For more information about this new capability, see [How to Switch a Failover Cluster to a New Domain](https://blogs.msdn.microsoft.com/clustering/2018/01/09/how-to-switch-a-failover-cluster-to-a-new-domain/) in Server & Management blogs. 

## In place upgrades

In-place upgrade allows an administrator to upgrade an existing installation of Windows Server to a newer version, retaining settings and installed features. The LTSC versions and editions of Windows Server that are supported for in-place upgrade are shown in the following table.

<br/>

|CURRENTLY INSTALLED OPERATING SYSTEM |AVAILABLE UPGRADE VERSION & EDITION |
|--- |--- |
|Windows Server 2016 Standard |Windows Server 2019 Standard or Datacenter |
|Windows Server 2016 Datacenter | Windows Server 2019 Datacenter|
|Windows Server 2012 R2 Standard| Windows Server 2019 Standard or Datacenter|
|Windows Server 2012 R2 Datacenter | Windows Server 2019 Datacenter|

## Microsoft Hyper-V 2019 Preview
This is the first Insider Preview of Microsoft Hyper-V 2019. Microsoft Hyper-V Server is a stand-alone product that contains only the Windows hypervisor, a Windows Server driver model, and virtualization components. It provides a simple and reliable virtualization solution to help you improve your server utilization and reduce costs.

The Windows hypervisor technology in Microsoft Hyper-V Server is the same as what's in the Hyper-V role on Windows Server. So, much of the content available for the Hyper-V role on Windows Server 2016 also applies to Microsoft Hyper-V Server.

## Remote Desktop Session Host (RDSH)

RD Session Host is a Remote Desktop Services role service that enables users to share Windows-based programs or the full Windows desktop. Users can connect to an RD Session Host server to run programs, save files, and use network resources on that server. Because of a bug, the RDSH role was missing in previous releases of Windows Server 2019 – this build fixes that. 

## Server Core App Compatibility Feature on Demand
App Compatibility, a Feature on Demand (FoD), has been updated with additional features and two additional components: Event Viewer and File Explorer.
This FoD significantly improves the app compatibility of Windows Server Core by including a set of binaries and packages from Windows Server with Desktop, without adding any of the Windows Server Desktop GUI or Windows 10 GUI experiences. The FoD package is available on a separate ISO and installs on Windows Server Core only.

Important   Please try out this FoD, and verify that current applications and tools run on the preview release as expected. Also, try any server app (from Microsoft or not) that you want to use on Server Core but currently cannot use, and please let us know about any successes or failures.
Operating system components that are available with this update:
* Event Viewer (Eventvwr.msc)
* Performance Monitor (PerfMon.exe)
* Resource Monitor (Resmon.exe)
* Device Manager (Devmgmt.msc)
* Microsoft Management Console (mmc.exe)
* File Explorer (Explorer.exe)
* Windows PowerShell (Powershell_ISE.exe)
* Failover Cluster Manager (CluAdmin.msc)

These components come with support for SQL Server Management Studio (SSMS), version 16 and 17, which must be installed separately from SQL Server via command line.

To install Failover Cluster Manager, launch PowerShell, and then enter the following command:
		Install-WindowsFeature -Name Failover-Clustering -IncludeManagementTools
To run Failover Cluster Manager, enter cluadmin at a regular command prompt.
The following installation procedure uses Deployment Image Servicing and Management (DISM.exe), a command-line tool. For more information about DISM commands, see [DISM Capabilities Package Servicing Command-Line Options](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/dism-capabilities-package-servicing-command-line-options).

To install Server Core with FoD binaries
1. Download the FoD ISO, and copy the ISO to a shared folder on your local network.
2. Download the ISO of the matching preview release of Windows Server, and install the operating system. Do not choose Desktop Experience options; the FoD is for Server Core only.
3. Sign in as administrator on the newly installed preview release of Server Core.
4. Use net use, or some other method, to connect to the location of the FoD ISO.
5. Copy the FoD ISO to a local folder of your choosing.
6. Start PowerShell by entering powershell.exe at a command prompt.
7. Mount the FoD ISO by using the following command:
Mount-DiskImage -ImagePath drive_letter:\folder_where_ISO_is_saved
8. Enter exit to exit PowerShell.
9. Enter the following command:
DISM /Online /Add-Capability /CapabilityName:Server.Appcompat~~~~0.0.1.0 /Source:drive_letter_of_mounted_ISO: /LimitAccess
10. After the progress bar completes, restart the operating system at the prompt.

## Storage Spaces Direct
Storage Spaces Direct uses industry-standard servers with local-attached drives to create highly available, highly scalable software-defined storage at a fraction of the cost of traditional SAN or NAS arrays. Its converged or hyper-converged architecture radically simplifies procurement and deployment, while features such as caching, storage tiers, and erasure coding, together with the latest hardware innovations such as RDMA networking and NVMe drives, deliver unrivaled efficiency and performance. 

### Performance history for Storage Spaces Direct

* The Get-ClusterPerf cmdlet includes self-diagnosis logic: if the cmdlet finds nothing to report, it looks for common issues that would prevent performance history from working properly (for example, if its storage is missing) so that the cmdlet can provide clear error text.

* New cmdlets, Start-ClusterPerformanceHistory and Stop-ClusterPerformanceHistory, that are provided in this build make it easy to remediate such issues by cleaning up and/or re-provisioning performance history.

* New series records how much Storage Spaces Direct data needs to repair/resync per server. 

* The Get-ClusterPerformanceHistory cmdlet is more scripting-friendly. It’s now convenient to pipe performance history into utility cmdlets like Sort-Object, Where-Object, and Measure-Object so you can quickly find the average or peak value, filter values, plot trend lines, run outlier detection, and more. You can see examples with these cmdlets in the topics linked under "Insider Preview content" on [aka.ms/StorageSpacesDirect](https://docs.microsoft.com/en-us/windows-server/storage/storage-spaces/storage-spaces-direct-overview.

* Performance history for the Storage Spaces Direct cache for reads (% hit rate) and writes (% full), as well as the CSV in-memory read cache (% hit rate), is now available. These new series are available per-server and in aggregate.

* Some performance history series have changed names for greater clarity and consistency—for example, Node.Cpu.Usage is now ClusterNode.Cpu.Usage. Note that this change will result in some blank charts in Windows Admin Center until its next update.

* Administrators of [Storage Spaces
Direct](https://docs.microsoft.com/windows-server/storage/storage-spaces/storage-spaces-direct-overview)
can now get easy access to historical performance and capacity data from
their cluster. *Did CPU usage spike last night? When did this drive
become slow? Which virtual machine used the most memory last month? Is
network activity trending up or down? The cluster is pushing 1,000,000
IOPS – is that my new record?* Previously, you'd need external tooling
to answer these questions. No more!

* Beautiful new charts in [Project
Honolulu](https://docs.microsoft.com/en-us/windows-server/manage/honolulu/honolulu-manage-hci)
(and new PowerShell cmdlets, for those so inclined) empower you to
answer these questions. There's nothing to install, configure, or
start—it's built-in and always-on. Learn more at
<https://aka.ms/clusterperformancehistory>.

![alt text](images/Hyper-Converged-in-Honolulu.png "New charts in Project Honolulu, powered by built-in cluster
performance history.")

## Storage Migration Service

A common issue around Windows Server is a lack of data migration options from older operating systems and storage platforms. Many customers run Windows Server 2012 R2, Windows Server 2008 R2, or even Windows Server 2003 simply because in-place upgrades were impossible and manual data migrations were slow and likely to cause significant service interruption or even loss of access to users and applications.

Windows Server 2019 introduces the Storage Migration Service (SMS), a new role included in Windows Server Standard and Datacenter editions. SMS is a job-based orchestration and proxy that:
 
* Allows administrators to inventory existing servers for their data, security, and network settings.
* Migrates that data, security, and network settings to a new, modern target by using the SMB protocol.
* Takes over the identity of the old server completely, while decommissioning the original source, in such a way that users and applications are unaffected and unaware that migration has taken place. 

SMS provides orchestrated workflow with a Honolulu-based graphical management system, allowing scalable migrations of many servers simultaneously to new targets running on premises or in Azure.

![alt text](images/scalable-migrations.png "Scalable migrations")

SMS handles common problems and subtleties of a migration, including in-use files, share settings, security settings, network addresses and names, local security principals, encrypted data, and more. All of this is available from an intuitive graphical interface, which is backed by robust PowerShell automation.

SMS is under active development, and you will see many changes and improvements with each preview. Furthermore, the use of the Honolulu management system enables out-of-band changes through its extension manager system, allowing us to act on your feedback more frequently than the Windows Server preview mechanism allows.

For more information on deploying and using the Storage Migration Service, please visit [https://aka.ms/stormigser](https://aka.ms/stormigser)

## Storage Replica
<b>Storage Replica (SR)</b> was first released as a technology for Windows Server 2016 Datacenter Edition. SR enables synchronous and asynchronous block replication of volumes between servers or clusters for disaster recovery. SR also enables you to create stretch failover clusters that span two sites, with all nodes staying in sync. 
Beginning with Windows Server 2019, responding to customer requests, we've added the following improvement to SR: 
 
Storage Replica Standard. SR is available on Windows Server 2019 Standard Edition, not just on Datacenter Edition. When installed on servers running Standard Edition, SR has the following limitations: 
 
*  SR replicates a single volume instead of an unlimited number of volumes.  
*  Volumes can have one partnership instead of an unlimited number of partners.  
*  Volumes can have a size of up to 2 TB instead of an unlimited size. 
 
We will continue to listen to your feedback and evaluate these settings through our telemetry during Insider previews of Windows Server 2019. These limitations may change several times during the preview phase and at RTM. 
For more information about Storage Replica, visit [http://aka.ms/StorageReplica](http://aka.ms/StorageReplica).  

## System Insights
System Insights is a new feature available in Windows Server 2019 that brings local predictive analytics capabilities natively to Windows Server. These predictive capabilities—each backed by a machine-learning model—locally analyze Windows Server system data, such as performance counters and events, providing insight into the functioning of your deployments and helping you reduce the operational expenses associated with monitoring your Windows Server instances.

Because each of these capabilities runs locally, all your data is collected, persisted, and analyzed directly on your Windows Server instance, allowing you to use predictive analytics capabilities without any cloud connectivity. In Windows Server 2019, System Insights introduces a set of capabilities focused on capacity forecasting, predicting future usage for compute, networking, and storage.

![alt text](images/system-insights.png "System Insights")

You can manage System Insights through an intuitive Windows Admin Center extension or directly through PowerShell, and System Insights allows you to manage each capability individually. This includes configuring custom schedules to run each capability and adding remediation scripts to automatically address any issue detected by a capability.

For more information about System Insights, please visit [aka.ms/SystemInsights](https://aka.ms/SystemInsights).

## Windows Admin Center Preview 1806
For full details, see the [Windows Admin Center Preview 1806 Announcement](https://aka.ms/WACPreview1806-InsiderBlog).

## Windows Defender Advanced Threat Protection

We provide deep platform sensors and response actions, providing visibility to memory and kernel level attacker activities and abilities to take actions on compromised machines in response to incidents such as remote collection of additional forensic data, remediating malicious files, terminating malicious processes etc. 
 
If you’re already using Windows Defender Advanced Threat Protection (ATP), preview these features by simply installing the latest preview build of Windows Server, and onboard it to Windows Defender ATP. 

Otherwise, sign up for the Windows Defender ATP trial on [Windows
Defender Advanced Threat
Protection](https://www.microsoft.com/en-us/windowsforbusiness/windows-atp).

## Windows Defender ATP Exploit Guard

Windows Defender ATP Exploit Guard is a new set of host-intrusion
prevention capabilities. The four components of Windows Defender Exploit
Guard are designed to lock down the device against a wide variety of
attack vectors and block behaviors commonly used in malware attacks,
while enabling enterprises to balance their security risk and
productivity requirements.

- <a href="https://docs.microsoft.com/en-us/windows/threat-protection/windows-defender-exploit-guard/attack-surface-reduction-exploit-guard?ocid=cx-blog-mmpc">Attack Surface Reduction
    (ASR)</a>:
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


## Windows Defender Application Control

Windows Defender Application Control—also known as Code Integrity (CI) policy—was released in Windows Server 2016. Customer feedback has suggested that it is a great concept, but hard to deploy. To address this, we are building default CI policies, which will allow all Windows in-box files and Microsoft applications, such as SQL Server, and block known executables that can bypass CI.  

The package contains an audit version and an enforced version. If the server doesn’t require additional drivers/applications, you can deploy the enforced version. Otherwise, you can use the audit policy, check uncovered executables, and then merge them into the default CI policy. 

To deploy the default code integrity policy, run the following commands:

<pre>
Copy-Item C:\\CI\\ServerDefault-EnforcedCI.bin<br/>
C:\\Windows\\System32\\CodeIntegrity\\SiPolicy.p7b
</pre>


Reboot the server to allow code integrity service to load the policy.


## Failover Cluster removing use of NTLM authentication

Windows Server Failover Clusters no longer use NTLM authentication by exclusively using Kerberos and certificate based authentication.  There are no changes required by the user, or deployment tools,  to take advantage of this security enhancement.  It also allows failover clusters to be deployed in environments where NTLM has been disabled. 

## Shielded virtual machines – Offline mode, VMConnect and Linux support

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

