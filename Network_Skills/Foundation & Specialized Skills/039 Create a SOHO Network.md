# 🧪 Lab: 039 Create a SOHO Network

## 🎯 Lab Overview

**Objective:** Design and implement complete small office/home office network infrastructure from ground up 

**Skills Practiced:**
- Deploy network devices using network modeling tools
- Configure device connectivity and verify DHCP functionality
- Test network connectivity through gateway ping verification 

**CertMaster Environment:** 1.3.10 Lab - Create a SOHO Network

---
## 📝 Implementation Steps

### Step 1: Deploy Network Infrastructure Components

- Access **End Devices** from tools tray and drag **three computers** to modeler canvas
- Select **Switches** tool and add **switch** to canvas
- Select **Routers** tool and add **router** to canvas

### Step 2: Establish Core Infrastructure Connectivity

- Use **Create Link** tool to connect **Router Port 0** to **Switch** open port
- Verify router-to-switch uplink connection establishment

### Step 3: Connect End Devices to Network Infrastructure

- Connect **Home-PC1 Ethernet port** to **Switch** open port
- Connect **Home-PC2 Ethernet port** to **Switch** open port
- Connect **Home-Laptop Ethernet port** to **Switch** open port
- Select **Create Link** to complete all connections

### Step 4: Verify Network Configuration and Connectivity

- Launch Windows on **Home-PC1** and access **Network & Internet Settings**
- Navigate to **Ethernet** section and verify **DHCP IP assignment**
- Complete assessment questions based on network configuration
- Test gateway connectivity by pinging **192.168.1.1** from Terminal (Admin)

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. SOHO networks require systematic device placement and connectivity planning to ensure proper network topology and performance.
    
2. DHCP automation simplifies network configuration by automatically assigning IP addresses and network parameters to connected devices.
    
3. Gateway connectivity testing validates that devices can communicate with network infrastructure and reach external networks.
    
4. Network modeling tools enable visualization and planning of network designs before physical implementation, reducing deployment errors.
    

**Real-World Application:**

- Small business owners and IT consultants design SOHO networks to provide reliable connectivity for remote work and small office environments.
    
- End-to-end network implementation skills demonstrate competency in complete network deployment from initial design through connectivity verification.
## 🖼️ Screenshots