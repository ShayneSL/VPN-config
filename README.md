![image](https://github.com/ShayneSL/VPN-config/assets/88577075/d92594e0-ad21-4f37-94da-2822bbdef201)





<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this project, I observed the impact of a virtual private network (VPN) on IP address, location, and web browsing. 
<br />
  
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
-	Remote Desktop
-	ProtonVPN (free version)


<h2>Operating System Used </h2>

- Windows 10 (21H2)

# Lab Tutorial: Setting Up VPN in an Azure Virtual Machine

## Objective
Gain a better understanding of VPNs by setting up a Virtual Private Network inside an Azure virtual machine. This lab will explore the impact of VPNs on IP addresses and locations.

## Step-by-Step Guide

1. Start by accessing the website "whatismyipaddress.com" on your actual PC. Take note of your public IP address and the corresponding city.

2. Create a virtual machine in Azure and establish a connection to it using Remote Desktop Protocol (RDP). This connection bridges your PC and the Azure virtual machine.

3. Within the Azure virtual machine, visit the website "whatismyipaddress.com" once again. This time, note down the new IP address and location. It should differ from your actual PC's IP address.

4. Sign up for the free version of ProtonVPN on your PC. Download and install the ProtonVPN client.

5. Inside the Azure virtual machine, connect to a ProtonVPN server located in Japan (or another available country). This establishes a VPN connection between the virtual machine and the chosen ProtonVPN server.

6. Access the website "whatismyipaddress.com" again from within the Azure virtual machine, with the VPN active. Take note of the new IP address and location displayed. This IP address should reflect the location of the VPN server (e.g., Tokyo, Japan).

By following these steps, you will have three entries in your text file representing different IP addresses and locations:

1. IP address and location from your actual PC without using a VPN.

![image](https://github.com/ShayneSL/VPN-config/assets/88577075/433c75ec-e80c-4b15-a0c5-00b07305487a)
[Screenshot Here: PC IP Address]

4. IP address and location from the Azure virtual machine without using a VPN.

![image](https://github.com/ShayneSL/VPN-config/assets/88577075/dfc8b3a3-4c69-4f99-950f-ee457cd3d639)

[Screenshot Here: Azure VM IP Address]

6. IP address and location from the Azure virtual machine with the VPN connected to a ProtonVPN server in Japan.

![image](https://github.com/ShayneSL/VPN-config/assets/88577075/d8685df7-7f45-4da7-8231-f317b52e0e8c)

[Screenshot Here: VPN IP Address]

## Understanding the Results

From this exercise, you can observe the following:

- When accessing the website from your actual PC without a VPN, it shows your original IP address and your city location.

- After connecting to the Azure virtual machine and accessing the website, a different IP address and the location of the virtual machine (e.g., Washington) are displayed.

- Finally, by connecting to the ProtonVPN server in Japan from within the virtual machine and accessing the website again, another IP address and the location of the VPN server (e.g., Tokyo, Japan) are shown.

This exercise demonstrates how VPNs work by encrypting and routing your internet traffic through remote servers, making it appear as if you are browsing from different locations. VPNs can enhance privacy, and security, and allow you to bypass geo-restrictions.
