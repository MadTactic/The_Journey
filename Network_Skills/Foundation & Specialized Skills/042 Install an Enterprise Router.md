# 🧪 Lab: 042 Install an Enterprise Router

## 🎯 Lab Overview

**Objective:** Perform physical installation and connectivity of enterprise router with fiber optic infrastructure 

**Skills Practiced:**
- Install enterprise networking equipment in rack-mount environments
- Configure SFP transceivers for copper and fiber connections
- Implement proper fiber optic cable management with Tx/Rx polarity 

**CertMaster Environment:** 5.1.9 Lab - Install an Enterprise Router

---
## 📝 Implementation Steps

### Step 1: Install Router in Rack Infrastructure

- Mount **CorpNet router** in designated rack position near top
- Secure router using appropriate rack mounting hardware
- Verify proper rack positioning and airflow clearance

### Step 2: Install SFP Transceiver Adapters

- Install **SFP Transceiver (RJ45)** in router **WAN port**
- Install **SFP Transceiver (LC)** modules in **LAN 1-4 ports**
- Verify proper SFP seating and connection security

### Step 3: Connect Power Infrastructure

- Use **AC power cable with C14 connector**
- Connect router to **critical load bank outlet** on UPS
- Verify power connection and UPS protection status

### Step 4: Configure Fiber Optic Connections

- Connect fiber cables using proper Tx/Rx polarity:
    - **Connector A (white/red) = Tx**
    - **Connector B (black) = Rx**
- Make fiber patch panel connections:
    - **LAN 1** → **Ports 1 and 2** (Tx to odd, Rx to even)
    - **LAN 2** → **Ports 3 and 4**
    - **LAN 3** → **Ports 5 and 6**
    - **LAN 4** → **Ports 7 and 8**

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Enterprise router installation requires understanding of rack mounting, power management, and structured cabling systems.
    
2. SFP transceivers provide flexibility for connecting different media types while maintaining consistent router interface configurations.
    
3. Fiber optic connections require proper Tx/Rx polarity to ensure bidirectional communication between network devices.
    
4. UPS integration ensures network infrastructure remains operational during power outages, supporting business continuity requirements.
    

**Real-World Application:**

- Network engineers perform hardware installations as part of infrastructure expansion projects and equipment upgrades.
    
- Proper fiber optic installation and documentation are critical for maintaining high-speed enterprise network performance and troubleshooting capabilities.

## 🖼️ Screenshots