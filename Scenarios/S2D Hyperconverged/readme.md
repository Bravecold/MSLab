<!-- TOC -->

- [Scenario Description](#scenario-description)
- [Scenario requirements](#scenario-requirements)
- [Screenshots](#screenshots)
    - [Howto](#howto)
    - [Result](#result)
- [How it looks like end-to-end (when you just paste the script).](#how-it-looks-like-end-to-end-when-you-just-paste-the-script)

<!-- /TOC -->

# Scenario Description

> Note: Scenario is bit obsolete. Use [AzSHCI Deployment Scenario](https://github.com/microsoft/MSLab/tree/master/Scenarios/AzSHCI%20Deployment) for deployment instead (just skip Azure Registration)

* In this scenario 2-16 node S2D cluster can be created.
* It is just simulation "how it would look like". Performance is not a subject here - it is just to test look and feel
* Script is well tested, on both real and simulated environments. However if you need assist, ask your Premier Field Engineer
* you can also use Nano Servers (its eating less resources). However as communicated [here](https://blogs.technet.microsoft.com/hybridcloud/2017/06/15/delivering-continuous-innovation-with-windows-server/), our focus is Core Server for physical infrastructure servers
* Deploy script finishes in ~5 minutes. Scenario script finishes in ~37 minutes.
* [S2D Cluster Validation Report](/Scenarios/S2D%20Hyperconverged/Screenshots/ValidationReport.zip)

# Scenario requirements

* Windows 10 1511 with enabled Hyper-V or Windows 10 1607+ (if nested virtualization is enabled)
* 8GB Memory or 20GB if nested virtualization is used (for 4 node configuration)
* SSD (with HDD it is really slow)

# Screenshots

## Howto

**Deploy.ps1 result**

![](/Scenarios/S2D%20Hyperconverged/Screenshots/DeployResultOverview.png)

**Collapsed scenario script in DC (ctrl+m)**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/CollapsedScenarioScriptInDC.png)

**Script configuring the scenario (copied to PowerShell script just by right-clicking into the window)**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/ScenarioScriptPastedIntoPosh.png)

## Result

**Scenario script finished in 37minutes**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/ScenarioScriptFinished.png)

**Server Manager (you need to add servers manually)**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/ServerManager.png)

**Failover Cluster Manager Summary**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerSummary.png)

**Failover Cluster Manager Roles**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerRoles.png)

**Failover Cluster Manager Nodes**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerNodes.png)

**Failover Cluster Manager Disks**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerDisks.png)

**Failover Cluster Manager Pool**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerPool.png)

**Failover Cluster Manager Networks**
![](/Scenarios/S2D%20Hyperconverged/Screenshots/FailoverClusterManagerNetworks.png)

# How it looks like end-to-end (when you just paste the script). 
Note, there are small differences as I did it a while ago.

![](/Scenarios/S2D%20Hyperconverged/Screenshots/s2d_Hyperconverged.gif)
