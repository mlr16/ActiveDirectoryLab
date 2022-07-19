<h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](URL)

<h2>Description</h2>
This Lab consists of walkthrough on installing Server 2019 and Microsoft Windows 10 in a virtual machine (Virtualbox). The steps will also demonstate installation of DCHP and Internal routing to enable client to access internet even when in Private Virtual Network. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Oracle Virtual Box</b> 
- <b>Powershell</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Install Window Server in Virtualbox : <br/>
<img src="https://i.imgur.com/pd3p9su.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
After installation, Create Log in credintialsk:  <br/>
<img src="https://i.imgur.com/V1FfuQu.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Install VM guest edition to give a better UX experience: <br/>
<img src="https://i.imgur.com/s1xLl85.png?1" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Click Adapter to view available networks:  <br/>
<img src="https://i.imgur.com/wnI3U4Y.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Open each network by right clicking icon to view status and see which network is connected to the internet. Also, rename each netowrk to easily identify internet and internal network as shown below example:  <br/>
<img src="https://i.imgur.com/Zl2l9wy.png?1" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Click right click Internal network and configure IPv4 properties; see configuration below:  <br/>
<img src="https://i.imgur.com/9MGSNOy.png?1" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Renaming Computer name helps Identify Domain Controller. Computer will restart after renaming:  <br/>
<img src="https://i.imgur.com/5Vccgeb.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />

<h2>Installing Active Directory and Domain Services:</h2>
<p align="center">
Click Add Roles and Features:  <br/>
<img src="https://i.imgur.com/lZwGdVI.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Click through the setup steps up until it reaches Server Roles:  <br/>
<img src="https://i.imgur.com/ZexlHh3.png" height="80%" width="80%" alt="Active Directory Homelab"/
<br />
<br />
Select Active Directory and Domain Services and click add features in the pop up box:  <br/>
<img src="https://i.imgur.com/RVrDLo5.png" height="80%" width="80%" alt="Active Directory Homelab"/
<br />
<br />
Installation of AD DS will start:  <br/>
<img src="https://i.imgur.com/hsZI3OU.png" height="80%" width="80%" alt="Active Directory Homelab"/
<br />
<br />
Promoting the current server into Domain Controller:  <br/>
<img src="https://i.imgur.com/D6QaQzD.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Promoting the current server into Domain Controller:  <br/>
<img src="https://i.imgur.com/sVCgNGb.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Create a Login password to use:  <br/>
<img src="https://i.imgur.com/YmPvFgU.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Click all the way to the end and click install ; no modification need. Computer will restart after installing AD DS:  <br/>
<img src="https://i.imgur.com/IQ5zzTz.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Go to tools in Server Manager and click on "Active Directory Users and Computers: <br/>
<img src=https://i.imgur.com/qnYzbn2.png" height="80%" width="80%" alt="Active Directory Homelab"

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
