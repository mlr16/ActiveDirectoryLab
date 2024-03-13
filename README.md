<h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](URL)

<h2>Description</h2>
This Lab consists of a walkthrough on Server 2019 and Microsoft Windows 10 in a virtual machine (Virtualbox). The steps will also demonstrate installation of DCHP and Internal routing to enable clients to access internet even when in a Private Virtual Network. 
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
After installation, Create Log in credintials:  <br/>
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
<br />
<br />
It will automatically restart the computer <br/>
<img src=https://i.imgur.com/P7Wmg5Y.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Log in again with built-in admin password <br/>
<img src=https://i.imgur.com/Pplo56H.png" height="80%" width="80%" alt="Active Directory Homelab"
<br />
<br />
Go to tool and click on ad Users and Computers <br/>
<img src=https://i.imgur.com/zHWtEts.png" height="80%" width="80%" alt="Active Directory Homelab"                                                                                         <br />
<br />
Right click mydomain and go to new and click on Organizational Unit <br/>
<img src=https://i.imgur.com/K5HE6F2.png" height="80%" width="80%" alt="Active Directory Homelab"    
<br />
<br />
Create Admin and uncheck Accidental Deletion <br/>
<img src=https://i.imgur.com/GJp6Zoq.png" height="80%" width="80%" alt="Active Directory Homelab"                                                                                         <br />
<br />
Right click on Admins, click on new and click on user <br/>
<img src=https://i.imgur.com/6y1hcAq.png" height="80%" width="80%" alt="Active Directory Homelab" 
<br />
<br />
Fill in all information and create user logon name <br/>
<img src=https://i.imgur.com/XouzCG0.png" height="80%" width="80%" alt="Active Directory Homelab"    
<br />
<br />
Create password for admin user, uncheck change password at next logon<br/>
<img src=https://i.imgur.com/ZNOmrwW.png" height="80%" width="80%" alt="Active Directory Homelab" 
<br />
<br />
Right click user, go to properties, click on "member of", click "add", type "Domain admins", click check "names" and click OK <br/>
<img src=https://i.imgur.com/bQdxzqZ.png" height="80%" width="80%" alt="Active Directory Homelab"                                                                                          <br />
<br />
Sign out from current user and sign in to the created admin user <br/>
<img src=https://i.imgur.com/IyoWSqC.png" height="80%" width="80%" alt="Active Directory Homelab"         
 <br />
<br />
Type created user in "other user". Make sure it shows signing in to created directory mydomain <br/>
<img src=https://i.imgur.com/haT0yaU.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />
Follow the same process as adding AD. Go to "roles and features" and an check Remote Access {Note: Do not uncheck any of prechecked boxes} <br/>
<img src=https://i.imgur.com/r4bsX65.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />
Under Roles and Services click Routing  and click okay, will automatically check VPN RAS <br/>
<img src=https://i.imgur.com/Ij6QlVB.png" height="80%" width="80%" alt="Active Directory Homelab"                                                                                         <br />
<br />
Click Tools and Go to Routing and Remote Access <br/>
<img src=https://i.imgur.com/wwl4Y3q.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />
DC is off. Click on DC and click "Configure and Enable..." and a setting screen will appear t<br/>
<img src=https://i.imgur.com/xoVEEsu.png" height="80%" width="80%" alt="Active Directory Homelab"                                                                       <<br />
<br />
Click on "Network Address Translation" and click "next" <br/>
<img src=https://i.imgur.com/zaO4M9z.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />
Click on "_INTERNET_" and  click "next" {Note: Renaming network adapters make it easier to differentiate NIC internal and internet} <br/>
<img src=https://i.imgur.com/KSXdnlX.png" height="80%" width="80%" alt="Active Directory Homelab"  
<<br />
<br />
Next is adding DHCP. Same process as adding NAT go to roles and features. Under Servers Roles, check "DHCP Servers" and click "Add Features" <br/>
<img src=https://i.imgur.com/WOuo5Z8.png" height="80%" width="80%" alt="Active Directory Homelab"                               
<<br />
<br />
 Click on "Tools" and navigate to "DHCP" to open a window <br/>
<img src=https://i.imgur.com/EgHWF90.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />    
DHCP is currently inactive. Click on DHCP and expand "dc.mydomain.com. Right click IPv4 and and side window will open. Click on "New Scope" <br/>
<img src=https://i.imgur.com/B4bYZef.png" height="80%" width="80%" alt="Active Directory Homelab"      
 <<br />
<br />
Type IP scope range 192.169.0.100-200 in under "Name" box <br/>
<img src=https://i.imgur.com/34H58GZ.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />
Type the ranges 192.168.0.11 starting and 192.168.0.20 and length 24 and subnet mask 255.255.255.0 <br/>
<img src=https://i.imgur.com/ymq8rur.png" height="80%" width="80%" alt="Active Directory Homelab"  
<<br />
<br />
Lease duration is how long is client kept connected to same network. Click "Next" <br/>
<img src=https://i.imgur.com/oGNKC2I.png" height="80%" width="80%" alt="Active Directory Homelab"                               
<<br />
<br />
 Add the internal IP address (192.168.0.1) of the network if it is not already in the DNS box <br/>
<img src=https://i.imgur.com/6inhMAG.png" height="80%" width="80%" alt="Active Directory Homelab"         
<br />
<br />   
Right click "dc.mydomain.com" and toggle to  and click "authorize" to activate server <br/>
<img src=https://i.imgur.com/m49980Z.png" height="80%" width="80%" alt="Active Directory Homelab"                               
<<br />
<br />

<h2>Creating and Adding Client Using Powershell: </h2>
<p align="center">
Open Powershell ISE and right click to go more. Then run as admin:  <br/>
<img src="hhttps://i.imgur.com/moUdDUL.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
This is the script that generates multiple username credentials:  <br/>
<img src="https://i.imgur.com/isFhT8W.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />                                                                                                 
Type the command below and it will allow the script to run:  <br/>
<img src="https://i.imgur.com/vK7FZT7.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />                                                                                                
 
 <h2>Create Windows 10 Virtual Machine (Client): </h2>
<p align="center">
Open Virtual Box. Follow the samessteps from "Program walkthrough in isntalling Windows 10 Client  (download ISO image of Windows 10 before creating VM) <br/>
<img src="https://i.imgur.com/jnOWvfW.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
Windows will start downloading:  <br/>
<img src="https://i.imgur.com/Kv877Pk.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
 After installation, type user in the blank space (use windows 10 pro if prompted to ask which version to use) and no password needed <br/>
<img src="https://i.imgur.com/QC1INZr.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br />
 After logging in, Go to command line by clicking windows icon and typing cmd:  <br/>
<img src="https://i.imgur.com/nTt64B0.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br /> 
  Type the following command (in the red box) and it will show i the client can connect to the network. Pay attention to the Default Gateway and DNS. There should be assigned IP address on both. Use the following command to ping external and internal network to make sure CLIENT connects. <br/>
<img src="https://i.imgur.com/rhEWXIY.png height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br /> 
Go to the windows icon and right click this. Click on system and scroll down to find Rename (Advanced): <br/>
<img src="https://i.imgur.com/1ch40r2.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br /> 
Typed the following information from the screenshot. After, click OK and it will promopt to restart. CLick Restart (If no prompt, manually navigate to restart menu). This will help restart computer configurations to be added to the AD DS <br/>
<img src="https://i.imgur.com/6GoSJB4.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br /> 
Navigate back to the AD DS VM to check if Computer (Client2) is added in the Domain. Go to tools to check on DHCP and Active Directory Users and Computers: <br/>
<img src="https://i.imgur.com/QfecDSy.png" height="80%" width="80%" alt="Active Directory Homelab"/>
<br />
<br /> 
                                                                                                  
</h2>THIS CONCLUDES THE LAB INSTRUCTIONS. </h2>

credits to: Jason Madakor video demonstration where I base my understanding of this subject.  
                                                                                                 
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
