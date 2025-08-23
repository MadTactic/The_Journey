# 🧪 Lab: 007 Configure TCP/IP Settings

## 🎯 Lab Overview

**Objective:** Network configuration for security monitoring and incident response - demonstrates static IP configuration across Windows platforms 

**Skills Practiced:**
- Configure IPv4 static addressing on multiple network adapters
- Set up dual network interfaces for segmented environments
- Navigate Windows network settings across different OS versions
- Implement DNS configuration for network connectivity 

**CertMaster Environment:** Simulation/Virtual lab details

---

## 📝 Implementation Steps

### Part A: Windows 10 Configuration (Marketing6)

#### Step 1: Access Network Adapter Settings (Windows 10)

- Open the **Settings** app
- Navigate to **Network & Internet**
- Select **Change adapter options**

#### Step 2: Configure Primary Ethernet Adapter

- Right-click **Ethernet** connection
- Select **Properties**
- Select **Internet Protocol Version 4 (TCP/IPv4)**
- Click **Properties**
- Configure with the following settings:
    - **IP address:** 192.168.0.254
    - **Subnet mask:** 255.255.255.0
    - **Default gateway:** 192.168.0.5
    - **Preferred DNS server:** 163.128.78.93
    - **Alternate DNS server:** 163.128.80.93
- Click **OK** to apply settings

#### Step 3: Configure Secondary Ethernet Adapter (Testing Network)

- Right-click **Ethernet 2** connection
- Select **Properties**
- Select **Internet Protocol Version 4 (TCP/IPv4)**
- Click **Properties**
- Configure with the following settings:
    - **IP address:** 10.0.255.254
    - **Subnet mask:** 255.255.0.0
    - **Default gateway:** (leave blank)
    - **DNS servers:** (leave blank)
- Click **OK** to apply settings

### Part B: Windows 11 Configuration (Office1)

#### Step 1: Access Network Adapter Settings (Windows 11)

- Open the **Settings** app
- Navigate to **Network & internet**
- Select **Advanced network settings**
- Click **More network adapter options**

#### Step 2: Configure Ethernet Adapter

- Right-click **Ethernet** connection
- Select **Properties**
- Select **Internet Protocol Version 4 (TCP/IPv4)**
- Click **Properties**
- Configure with the following settings:
    - **IP address:** 192.168.0.253
    - **Subnet mask:** 255.255.255.0
    - **Default gateway:** 192.168.0.5
    - **Preferred DNS server:** 163.128.78.93
    - **Alternate DNS server:** 163.128.80.93
- Click **OK** to apply settings

### Step 3: Verify Network Connectivity

- Test connectivity to local network and internet
- Verify proper IP configuration using **ipconfig** command
- Confirm DNS resolution functionality

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Static IP addressing provides consistent network identification essential for server roles, network monitoring systems, and security appliances that require predictable addressing.
    
2. Multi-homed systems with multiple network adapters enable network segmentation, allowing systems to participate in both production and testing environments simultaneously.
    
3. DNS configuration is critical for proper network functionality, enabling domain name resolution for both internal resources and internet connectivity.
    
4. Windows network configuration interfaces vary between versions, but core TCP/IP principles remain consistent across platforms.
    

**Real-World Application:**

- Network administrators configure static IP addresses for servers, security monitoring systems, and critical infrastructure that must maintain consistent network identity.
    
- Dual-network configurations are common in security environments where systems need access to both production networks and isolated testing/analysis networks for incident response and forensic activities.
    

## 🖼️ Screenshots

![[Lab007_01.png]]

![[Lab007_02.png]]

![[Lab007_03.png]]

![[Lab007_04.png]]

![[Lab007_05.png]]

![[Lab007_06.png]]

![[Lab007_07.png]]
