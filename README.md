# ActiveDirectoryLab

## ⚙️ Languages and Utilities Used

- **Active Directory** 
- **DHCP**
- **DNS**
- **Powershell** 
- **Virtual Box**

## 📄 Description

This project involves setting up a homelab environment to simulate a larger IT infrastructure. It includes using Active Directory for centralized user and resource management, creating a thousand user accounts using a PowerShell script, and configuring a DHCP server to manage IP address assignments. As well as setting up DNS to resolve hostnames to IP addresses, ensuring seamless communication within the network. This environment serves as a practical learning platform for IT administration and systems management.

---

## Windows Server 2019
I started by installing Windows Server 2019. I used the ISO file to create a bootable medium and launched the setup on my virtual machine. During the installation, I selected the 'Windows Server 2019 Standard' edition with Desktop Experience. Once the setup was complete, I configured a secure administrator password, renamed the server, and started installing services needed for the project. Such as, Active Directory Domain Services.

![Server Manager](https://i.imgur.com/t8Z8eAX.png)

---

## Network Connections
Next, I configured the two network ports on the server. One port was set up for internet access to connect to the external network, while the other was designated for internal use, intended for the future DHCP server. For the internal network, I assigned the IP scheme 172.16.0.1.

![Network Connections](https://imgur.com/Ld5Egds.png)

---

## DHCP Server
I set up the DHCP server and created an IP address scope ranging from 172.16.0.100 to 172.16.0.200. This configuration was later used to assign an IP address automatically to my Client 1 virtual machine.
![DHCP](https://imgur.com/PjrttTV.png)

---
