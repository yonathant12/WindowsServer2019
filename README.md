<h1>Setting Up Windows Server 2019</h1>

<h2>Description</h2>
Setting up a Windows Server 2019 on VMware Workstation 17 Pro involves creating a new virtual machine, configuring hardware resources, installing the server OS from an ISO file, and performing initial setup tasks such as installing VMware Tools, assigning a static IP, and renaming the machine.
<br />


<h2>Application Used</h2>

- <b>Cisco Packet Tracer</b>

<h2>Lab walk-through:</h2>

<p align="center">
Click the "File" option on the top left and select "New Virtual Machine". Choose the Custom option and hit next.<br/>
<img src="https://i.imgur.com/L7q5mZ5.png" height="60%" width="60%"/>
<br />
<br />
Select the "I will install the operating system later" option and click next.<br/>
<img src="https://i.imgur.com/7Tnz4cn.png" height="60%" width="60%"/>
<br />
<br />
Select Microsoft Windows as the Guest operating system and choose Windows Server 2019 as the Version, then click next.<br/>
<img src="https://i.imgur.com/opASZYp.png" height="60%" width="60%"/>
<br />
<br />
Press next on the "Name the Virtucal Machine" screen. Select BIOS as Firmware Type and click next.<br/>
<img src="https://i.imgur.com/fhKOpZM.png" height="60%" width="60%"/>
<br />
<br />
Leave the "Processor Configuration" screen as default. Increase "Memory for the Virtual Machine" from 2GB to 4GB.<br/>
<img src="https://i.imgur.com/8sk9Rz1.png" height="60%" width="60%"/>
<br />
<br />
Choose "Use network address translation (NAT)" as the Network Type and click next.<br/>
Choose "LSI Logic SAS (Recommended)" as the I/O Controller Type and click next.<br/>
Choose "NVMe (Recommended)" as the Disk Type and click next.<br/>
Choose "Create a new virtual disk" on the Select a Disk screen and click next.<br/>
Leave "Disk Capacity" as the recommended amount which is 60GB, select "Split virtual disk into multiple files", and then click next.<br/>
Leave "Disk File" as default and click next.<br/>
Verify the following setting and click finish.<br/>
<img src="https://i.imgur.com/FIvPUDx.png" height="60%" width="60%"/>
<br />
<br />
Click "Edit virtual machine settings.<br/>
<img src="https://i.imgur.com/wUOFD0P.png" height="60%" width="60%"/>
<br />
<br />
Click the Add button.<br/>
<img src="https://i.imgur.com/7wZPhMF.png" height="60%" width="60%"/>
<br />
<br />
Select Network Adapter and click finish.<br/>
<img src="https://i.imgur.com/ZlHiEGC.png" height="60%" width="60%"/>
<br />
<br />
Select Network Adapter 2 and choose "Host-only" option.<br/>
<img src="https://i.imgur.com/fNUy57t.png" height="60%" width="60%"/>
<br />
<br />
Select CD/DVD (SATA), choose the "Use ISO image file:" and click browse. Find the Windows Server 2019 ISO and click ok.<br/>
<img src="https://i.imgur.com/Dzy6qsu.png" height="60%" width="60%"/>
<br />
<br />
Click "Power on this virtual machine"<br/>
<img src="https://i.imgur.com/spgYBww.png" height="60%" width="60%"/>
<br />
<br />
Once the Windows Setup comes on, click next and then click the Install now button.<br/>
<img src="https://i.imgur.com/ZdOkz5R.png" height="60%" width="60%"/>
<br />
<br />
Select "Windows Server 2019 Standard Evaluation (Desktop Experience)" and click next.<br/>
<img src="https://i.imgur.com/qJAe64i.png" height="60%" width="60%"/>
<br />
<br />
Accept the license terms and click next.<br/>
Select Custom for the intallation type.<br/>
<img src="https://i.imgur.com/WaqQ5bb.png" height="60%" width="60%"/>
<br />
<br />
Click next on the "Where do you want to install Windows" screen.<br/>
Wait for Windows to install.<br/>
<img src="https://i.imgur.com/64s8CIb.png" height="60%" width="60%"/>
<br />
<br />
Create a password for the administrator account and click finish.<br/>
<img src="https://i.imgur.com/3cq3s9K.png" height="60%" width="60%"/>
<br />
<br />
Click the "Send Ctrl+Alt+Del to this virtual machine" button at the top to get the login screen.<br/>
<img src="https://i.imgur.com/JrhDHHC.png" height="60%" width="60%"/>
<br />
<br />
Click Yes on the Networks pop-up.<br/>
Click the VM button at the top left and click "Install VMware Tools".<br/>
<img src="https://i.imgur.com/MxCbAYF.png" height="60%" width="60%"/>
<br />
<br />
Open up File Explorer and double click on "DVD Drive (D:) VMware Tools".<br/>
<img src="https://i.imgur.com/KejSXVz.png" height="60%" width="60%"/>
<br />
<br />
Click next on the "Welcome to the installation wizard for VMware Tools" screen.<br/>
<img src="https://i.imgur.com/10Dvy2t.png" height="60%" width="60%"/>
<br />
<br />
Select Typical as the setup type and click next.<br/>
Click install on the "Ready to intall VMware Tools" screen.<br/>
Click finish once it's completed.<br/>
Click Yes when asked to restart.<br/>
<img src="https://i.imgur.com/qp5Qslw.png" height="60%" width="60%"/>
<br />
<br />
Once the machine has restarted, log back in and open Windows Settings.<br/>
Select "Network & Internet" and then click on "Change adapter options".<br/>
Ethernet0 is NAT and Ethernet1 is Host(internal network).<br/>
Right click Ethernet1 and select properties.<br/>
<img src="https://i.imgur.com/KEtdh0G.png" height="60%" width="60%"/>
<br />
<br />
Double click on "Internet Protocol Version 4 (TCP/IPv4)".<br/>
<img src="https://i.imgur.com/2qhtM27.png" height="60%" width="60%"/>
<br />
<br />
Select "Use the following IP address:" option and enter the static IP address. Enter the Ip address as the DNS Server. No need to enter Default gateway because this machine will serve as the default gateway and the DNS Server.<br/>
<img src="https://i.imgur.com/ElBZwJy.png" height="60%" width="60%"/>
<br />
<br />
Open Windows Settings and click on System.<br/>
On the System page, select About and click on "Rename this PC".<br/>
<img src="https://i.imgur.com/Lyxx3Lr.png" height="60%" width="60%"/>
<br />
<br />
Enter a name for this machine and click next.<br/>
Click Restart now then Continue.<br/>
<img src="https://i.imgur.com/pV6dST8.png" height="60%" width="60%"/>
<br />
<br />
</p>
