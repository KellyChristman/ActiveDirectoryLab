# **Active Directory Lab**

## ⚙️ **Languages and Utilities Used**

- **Active Directory**  
- **DHCP**  
- **DNS**  
- **PowerShell**  
- **VirtualBox**  

---

## 📄 **Project Overview**

This homelab project simulates a larger IT infrastructure, showcasing essential system administration tasks. The environment includes:  
- **Active Directory** for centralized user and resource management.  
- Automated creation of **1,000 user accounts** using a PowerShell script.  
- A **DHCP server** to handle IP address assignments.  
- **DNS** to resolve hostnames to IP addresses, enabling seamless network communication.  

The completed lab serves as a practical platform for learning IT infrastructure management and network configuration.

---

## **Windows Server 2019 Setup**  

To begin, I installed **Windows Server 2019**. Using the ISO file, I created a bootable medium and launched the installation on a virtual machine. I selected the 'Windows Server 2019 Standard' edition with Desktop Experience. After completing the installation, I set up a secure administrator password, renamed the server, and installed essential roles, including **Active Directory Domain Services**.

![Server Manager](https://i.imgur.com/t8Z8eAX.png)

---

## **Network Connections**  

I configured two network ports on the server:  
- One port for **internet access**, connecting to the external network.  
- Another port for **internal use**, intended for the DHCP server.  

For the internal network, I assigned the IP scheme **172.16.0.1**.

![Network Connections](https://imgur.com/Ld5Egds.png)

---

## **DHCP Server Configuration**  

I set up a **DHCP server** and configured an IP address scope from **172.16.0.100 to 172.16.0.200**. This ensured that devices on the internal network, such as the Client 1 virtual machine, could receive IP addresses automatically.

![DHCP](https://imgur.com/PjrttTV.png)

---

## **User Creation via PowerShell**  

Using a **PowerShell script**, I automated the creation of **1,000 user accounts**. After running the script, I verified that all user accounts were successfully added to **Active Directory**.

![Powershell Script](https://imgur.com/QbpY5aj.png)  

![User Verification](https://imgur.com/g4ah5VH.png)

---

## **Completed Virtual Machines**  

The final setup in **VirtualBox** shows both the **domain controller** and the **Client 1 virtual machine** fully configured and networked. This validates the successful integration of all components within the homelab environment.  

![Virtual Box](https://imgur.com/ggXvhxm.png)

---

This lab provides a hands-on approach to learning and refining IT administration skills, including user management, network configuration, and service deployment.  
