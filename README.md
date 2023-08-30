<h1>Honey pot, RDP Failure to IP Geolocation Information</h1>

<h2>Description</h2>
<b>Utilized Windows Powershell script which is responsible for pushing out Windows Event Log information (Security Event 4625) for failed RDP attacks and using a third party API to collect information on the attackers location.
</b>
<br />
<br />
Azure Sentinel (SIEM) is set up and connects to a live virtual machine acting as a honey pot.
(RDP Brute Force) from all around the world is displayed. PowerShell script
looks up the attackers Geolocation information and plots it on Azure Sentinel Map.
<br />
<br />

<p align="center">
<img src="[https://i.imgur.com/3d3CEwZ.png](https://imgur.com/a/JUQuQKf)" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from China coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://i.imgur.com/LhDCRz4.jpeg" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/krRFrK5.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
