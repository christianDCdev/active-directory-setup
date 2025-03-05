<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Setup for Active Directory Infrastructure</h1>
Welcome!  This project serves as the first step to Active Directory implementation.  The objective of this project is to simulate an environment in Azure that allows the implementation of on-premises Active Directory.  We will be connecting two virtual machines that each serve their own purpose.  The first virtual machine will be the Domain Controller, and it will act as a server for the second virtual machine, the Client, to connect to.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Objectives</h2>

- Create and configure Domain Controller virtual machine
- Create Client virtual machine
- Establish a connection between the Domain Controller and Client virtual machines
- Ensure connectivity between the two virtual machines by inspecting network traffic

<h2>Configuration Steps</h2>

<h3>&#9312; Create Resource Group and Virtual Network</h3>
<p>

- Within Azure, create a resource group
- Create a virtual network and select the resource group you just created
<img src="https://i.imgur.com/dUowvkj.png" height="80%" width="80%" alt="Virtual network creation"/>
  
</p>

<h3>&#9313; Create Domain Controller</h3>

<p>

- Create a virtual machine and name it "DC-1"
- Under "Image", select Windows Server 2022 Datacenter: Azure Edition


- Under "Size", select option with at least 2 vcpus
- Choose and confirm "Username" and "Password" under "Administrator Account" section
- Confirm licensing
<img src="https://i.imgur.com/2yLaJgw.png" height="80%" width="80%" alt="VM licensing"/>

- Navigate to "Networking" tab
- Under "Virtual Network", select the virtual network you created in the previous step
<img src="https://i.imgur.com/GmLc5OP.png" height="80%" width="80%" alt="Virtual network selection"/>

- Review + create your VM

</p>
<br />
<h3>&#9314; Create Client VM</h3>

<p>

- Create a virtual machine and name it "Client-1"
- Under "Image", select Windows 10 Pro
<img src="https://i.imgur.com/IcWRnUO.png" height="80%" width="80%" alt="Client image"/>

- Under "Size", select option with at least 2 vcpus
- Choose and confirm "Username" and "Password" under "Administrator Account" section
- Confirm licensing
- Navigate to "Networking" tab
- Under "Virtual Network", select the same virtual network you did in the previous step
<img src="https://i.imgur.com/GmLc5OP.png" height="80%" width="80%" alt="Virtual network selection"/>

- Review + create your VM
  
</p>
<br />
<h3>&#9315; Set Domain Controller's Private IP Address to "Static"</h3>

<p>

- 
  
</p>
