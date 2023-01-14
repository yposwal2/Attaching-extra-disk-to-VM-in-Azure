<h1>Attaching extra disk to Virtual Machine in Azure Portal </h1>

<h2>Description</h2>

In this lab, I will attach the extra disk to the virtual machine on azure. 
<br />

<h2>Utilities Used</h2>

- <b>Azure</b> 
- <b>Microsoft Remote Desktop</b>

<h2>Prerequisite </h2>

- <b>Virtual Machine Deployed on Azure Portal:</b> 
In this lab, I am using the virtual machine running on Windows Server 2012 and I will try to add extra storage space to it.    

<h2>Program walk-through:</h2>

<p align="center">
This is a screenshot of the Server Manager of the Windows Server 2012 VM. As you can see, this has 127GB of storage and 4GB of RAM. Now I will add 4GB of extra storage to this VM. <br/>
<img src="https://i.imgur.com/RQ8L8h1.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Login into Azure Portal. Go to All Services-> Compute-> Virtual Machine.  Select the Virtual Machine you want to add storage to. Go to VM's Settings ->  Disk and click create and attach a new disk. <br/>
<img src="https://i.imgur.com/oGP3GLN.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Set LUN, Disk name, and Size(GB). Since I only want one storage disk I set LUN to 1, named it an extra disk, and set the size to 4GB <br/>
<img src="https://i.imgur.com/g6bNKPP.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Make sure you also change Host caching. In my case I made it to Read & Write. Once done click on save. <br/>
<img src="https://i.imgur.com/uyCK31r.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
After that, I went back to VM refreshed the server manager, and my new disk popped up there. <br/>
<img src="https://i.imgur.com/XYyYMuo.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
Next, I clicked on "To create a volume, start the New Volume Wizard" to get that storage on my VM system <br/>
<img src="https://i.imgur.com/iA9IJNx.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
I filled out the necessary details and confirmed it. <br/>
<img src="https://i.imgur.com/bhQGJ8w.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
My Virtual Machine now has the extra disk I attached to it. <br/>
<img src="https://i.imgur.com/YzpUppB.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
