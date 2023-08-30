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

<p align="center"

![Geo API](https://github.com/jlam744/SentinelGeo_lab/assets/95711303/4ab2eb9a-9db6-44b0-b487-55217de0ea23)
![RDP Heat Map](https://github.com/jlam744/SentinelGeo_lab/assets/95711303/6b4c6dd8-3f5b-448a-828b-2948154cbbc8)


</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer
![Powershell script](https://github.com/jlam744/SentinelGeo_lab/assets/95711303/3faedbc4-c5d8-44d2-9c46-f3cf6e023a63)


<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API
![Powershell to API ](https://github.com/jlam744/SentinelGeo_lab/assets/95711303/4fa4ff8f-029a-4cb1-bb7a-6659632b3c70)

<h2>Attacks from China coming in; Custom logs being output with geodata</h2>

<p align="center">

</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://imgur.com/a/xuixRB4.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
