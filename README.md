# Azure VM Network Analysis - Part 1 - Prerequisites and Configuration
In this tutorial, we will create a Ressource Group and configure 2 Virtual Machines which will operate in the same Virtual Network.


<p align="center">
<img src="https://i.imgur.com/v8sgAIn.png" alt="Traffic Examination"/>
</p>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)

<h3>Operating Systems Used </h3>

- Windows 10 Pro, version 22H2
- Ubuntu Server 22.04 LTS

<h2>High-Level Steps</h2>

- Step 1: Create a Resource Group
- Step 2: Create a Windows Virtual Machine
- Step 3: Create a Linux Virtual Machine
- Step 4: Verify Configuration
- Step 5: Prepare for Part 2

<h2>Actions and Observations</h2>

<h3>Step 1: Create a Resource Group</h3>
<p>
<img src="https://i.imgur.com/39rastI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Once logged in to your Azure account, type "Resource groups" in the navigation pane and create one.
</p>
<br />



<h3>Step 2: Create a Windows Virtual Machine</h3>
<p>
<img src="https://i.imgur.com/W61P5BL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Once the Resource group is created, type "Virtual machines" in the navigation pane and choose the first option under "Create".
</p>
<br />

<p>
<img src="https://i.imgur.com/7o20QHT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Associate the Windows VM to the previously created Resource Group.
  
-Create a name for the Windows virtual machine (ex: Windows-VM).
  
-Choose a Region for the virtual machine.
  
-Pick the Windows 10 Pro version 22H2 virtual machine image type.
</p>
<br />


<p>
<img src="https://i.imgur.com/0YzLocL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Select a VM size; having at least 2 vcpus and 8 GiB memory is recommended.

-Create a username and a password for the Windows VM (write them down in Notepad for futur use).
  
-Leave the other options at their default configuration and move on to the Networking section.
</p>
<br />

<p>
<img src="https://i.imgur.com/mbg3Tw9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-In the Networking section, create a new Virtual Network.

-Leave all the other options at their default configuration and click review + create. 
</p>
<br />



<h3>Step 3: Create a Linux Virtual Machine</h3>
<p>
-Use the information provided in Step 2 to create the Linux VM; ensure that the Linux VM is connected to the same Resource group and Virtual Network as the Windows VM. Additionally, pick the Ubuntu Server 22.04 LTS VM image type, and write down the credentials that you will have to create to access the Linux VM as we will need them later. 
</p>
<br />



<h3>Step 4: Verify Configuration</h3>
<p>
<img src="https://i.imgur.com/aszxCvi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Once the Linux VM is created, verify that both VMs are connected to the same Virtual Network / Subnet.  
</p>
<br />





<h3>Step 5: Prepare for Part 2</h3>
<p>
<img src="https://i.imgur.com/cQ2zp44.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Once you have verified that both VMs are correctly configured, you can decide wether to suspend the VMs temporalily by selecting them and pressing "Stop" or keeping them active and directly moving on to Part 2 - check out: Azure VM Network Analysis - Part 2 - ICMP traffic analysis in my repository.
</p>
<br />




