# SOHO Network Prototype

This project involved designing and implementing a virtualized Small Office/Home Office (SOHO) network using Oracle VirtualBox. The setup includes a centralized Print Server and two client machines, demonstrating core networking concepts such as static IP addressing, network service sharing, and address resolution.

## 🚀 Project Overview

- **Scenario:** Eduvos needed a prototype to enhance its campus IT support, specifically for printing services.
- **Objective:** Build a functional, small-scale office network in a virtual environment to simulate real-world administration tasks.
- **Key Skills Demonstrated:** Virtualization, Static IP Configuration, Network Service Setup (Print Server), Client-Server Connectivity, ARP Management.

## 🛠️ Technologies Used

- **Virtualization:** Oracle VirtualBox
- **Operating Systems:** Windows 7, Windows 8, Windows 10
- **Networking:** TCP/IP, Static IP Assignment, ARP, ICMP (Ping)
- **Tools:** Command Prompt, Windows Server Features

## 📋 Project Implementation

### 1: SOHO Network Configuration

#### 1.1 Virtual Machine Setup
Created three virtual machines with password-protected user accounts:

**WIN7-CLIENT User Account**
![Username "Malao" password-protected](./hsqoczic.png)

**WIN8-CLIENT User Account**  
![Username "Lwazi" password-protected](./ftfagsfd.png)

**PRINT-SERVER User Account**
![Username "PrintServ" password-protected](./wzphpeqh.png)

#### 1.2 Network Configuration
All VMs connected to the internal network "EduvosNet" with static IP addressing:

**PRINT-SERVER Network Setup**
![PRINT-SERVER on EduvosNet](./tydnt2et.png)

**PRINT-SERVER Static IP Configuration**
![PRINT-SERVER static IP](./waeqkxho.png)

**WIN7-CLIENT Network Setup**
![WIN7-CLIENT on EduvosNet](./b0xagtuy.png)

**WIN7-CLIENT Static IP Configuration**
![WIN7-CLIENT static IP](./tmj5ecuo.png)

**WIN8-CLIENT Network Setup**
![WIN8-CLIENT on EduvosNet](./thj1b1ep.png)

**WIN8-CLIENT Static IP Configuration**
![WIN8-CLIENT static IP](./zjsyyqbp.png)

#### 1.3 Print Server Configuration
Installed and configured network printing services:

**Enable Print and Document Services**
![Enabled Print Services](./ri45r1ko.png)

**Install Generic Text Printer**
![Added Generic Text Printer](./ewpkjglk.png)

**Share Printer as 'SharedPrinter'**
![Shared Printer Configuration](./ogaw4ix1.png)

#### 1.4 Client Connectivity and Verification
Connected clients to shared printer and verified network connectivity:

**WIN7-CLIENT Printer Connection**
![WIN7 connected to SharedPrinter](./4x0ygmui.png)

**WIN8-CLIENT Printer Connection**
![WIN8 connected to SharedPrinter](./iehrrgzz.png)

**WIN7-CLIENT Test Page**
![WIN7 test page printed](./mbsuqjgg.png)

**WIN8-CLIENT Test Page**
![WIN8 test page printed](./snh5nzkt.png)

**Network Connectivity Verification**
![Ping results](./pyeoebkl.png)

**File Explorer Access**
![Access via \\\\PRINT-SERVER](./j4gpql0v.png)

###2: Address Resolution Protocol (ARP) Management

#### 2.1a Static ARP Entry Configuration

**WIN8-CLIENT MAC Address Retrieval**
![ipconfig /all results](./agzji3cj.png)

**Static ARP Entry Creation**
![arp -s command execution](./ye5l0bwx.png)

**Command Used:**
```cmd
arp -s 192.168.60.3 08-00-27-92-A9-DD
