# 🧪 Lab: 023 Configure Trunking

## 🎯 Lab Overview

**Objective:** Configure VLAN trunking and port assignments for secure network segmentation 

**Skills Practiced:**
- Configure switch port modes (Access vs Trunk)
- Assign Port VLAN IDs (PVIDs) and add VLANs to trunk ports
- Save configuration changes to startup configuration 

**CertMaster Environment:** 5.6.10 Lab - Configure Trunking

---
## 📝 Implementation Steps

### Step 1: Access Switch Management Console

- Open **Google Chrome** and navigate to **192.168.0.2**
- Login credentials:
    - **Username:** cisco
    - **Password:** cisco
- Examine default port settings and document current configuration

### Step 2: Configure Access Mode Ports

- Set ports **GE1 through GE26** to **Access Mode**
- Verify access mode configuration for all designated ports

### Step 3: Configure Trunk Ports with PVID

- Set ports **GE27** and **GE28** to:
    - **Port VLAN ID (PVID):** 2
    - Configure as trunk ports to carry multiple VLANs

### Step 4: Add VLANs to Trunk Ports

- Add the following VLANs to ports **GE27** and **GE28:**
    - **VLAN 22**
    - **VLAN 44**
    - **VLAN 67**
- Verify VLAN assignments on both trunk ports

### Step 5: Save Configuration

- Save configuration changes to **startup configuration file**
- Ensure settings persist after switch reboot

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Access ports carry traffic for a single VLAN, while trunk ports can carry multiple VLANs simultaneously using VLAN tags.
    
2. Port VLAN ID (PVID) determines which VLAN untagged traffic is assigned to when entering a trunk port.
    
3. VLAN trunking enables efficient use of physical links by allowing multiple logical networks to share the same physical infrastructure.
    
4. Saving configurations to startup files ensures network settings persist through power cycles and system reboots.

**Real-World Application:**

- Network administrators use VLAN trunking to connect switches while maintaining network segmentation for security and traffic management.
    
- Trunk configuration is essential for connecting access layer switches to distribution switches in hierarchical network designs.

## 🖼️ Screenshots