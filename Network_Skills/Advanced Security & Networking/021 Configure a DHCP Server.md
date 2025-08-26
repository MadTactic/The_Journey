# 🧪 Lab: 020 Configure a DHCP Server

## 🎯 Lab Overview

**Objective:** Configure and deploy DHCP services for automated IP address management in corporate network environments 

**Skills Practiced:**
- Create and configure DHCP IPv4 scopes with specific parameters
- Set DHCP scope options for gateway and DNS server assignments
- Activate DHCP services and verify client connectivity

**CertMaster Environment:** 6.2.5 Lab - Configure a DHCP Server

---
## 📝 Implementation Steps

### Step 1: Create DHCP IPv4 Scope on CorpDHCP Server

- Access **CorpDHCP** server (guest on CorpServer)
- Open DHCP management console
- Create new IPv4 scope with the following configuration:
    - **Scope name:** Subnet1
    - **Start IP address:** 192.168.0.20
    - **End IP address:** 192.168.0.200
    - **Length:** 24
    - **Subnet mask:** 255.255.255.0
- Accept default lease duration settings
- Skip exclusions and delays configuration

### Step 2: Configure DHCP Scope Options

- Set **Router (Default Gateway)** option:
    - **Gateway IP:** 192.168.0.5
- Configure **DNS Servers** option:
    - **DNS Server IP:** 163.128.78.93
- Accept default parent domain settings
- Skip WINS server configuration

### Step 3: Activate DHCP Scope

- Right-click on **Subnet1** scope
- Select **Activate** to enable the scope
- Verify scope status shows as **Active**

### Step 4: Test DHCP Client Configuration

- Navigate to **Gst-Lap** workstation in the Lobby
- Access **Local Area Connection** network properties
- Configure network adapter to:
    - **Obtain an IP address automatically**
    - **Obtain DNS server address automatically**
- Verify successful DHCP lease acquisition

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. DHCP servers automate IP address distribution and reduce manual configuration errors in network environments with multiple clients.
    
2. DHCP scopes define the range of IP addresses available for assignment, along with associated network configuration parameters like gateways and DNS servers.
    
3. Scope options centralize network configuration management, ensuring consistent settings across all DHCP clients without individual workstation configuration.
    
4. DHCP lease duration controls how long clients retain IP addresses, balancing address pool efficiency with network stability requirements.
    

**Real-World Application:**

- Enterprise networks rely on DHCP services to manage hundreds or thousands of devices automatically, reducing administrative overhead and configuration inconsistencies.
    
- Network administrators configure DHCP reservations and scope options to ensure critical services like DNS and gateway settings are consistently deployed across corporate infrastructure.
    

## 🖼️ Screenshots

![[Lab020_01.png]]

![[Lab020_02.png]]

![[Lab020_03.png]]

![[Lab020_04.png]]

![[Lab020_05.png]]

![[Lab020_06.png]]

![[Lab020_07.png]]

![[Lab020_08.png]]

![[Lab020_09.png]]