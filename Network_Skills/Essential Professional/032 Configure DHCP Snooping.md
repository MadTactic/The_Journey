# 🧪 Lab: 032 Configure DHCP Snooping

## 🎯 Lab Overview

**Objective:** Implement DHCP snooping and dynamic ARP inspection to prevent Layer 2 security attacks 

**Skills Practiced:**
- Configure DHCP snooping globally and per-VLAN to prevent rogue DHCP servers
- Establish trusted interfaces for legitimate network services
- Enable dynamic ARP inspection for comprehensive Layer 2 protection 

**CertMaster Environment:** 9.4.7 Lab - Configure DHCP Snooping

---
## 📝 Implementation Steps

### Step 1: Enable Global DHCP Snooping

- Access **SwitchA** configuration interface
- Enable **DHCP snooping globally** on the switch
- Verify global snooping activation status

### Step 2: Configure VLAN-Specific DHCP Snooping

- Enable **DHCP snooping for VLAN 1**
- Associate snooping configuration with **Fa0/24 interface**
- Verify VLAN snooping parameters are applied

### Step 3: Configure Trusted DHCP Interface

- Set **Fa0/24** (DHCP server port) as **trusted interface**
- Configure trust settings for DHCP snooping operations
- Verify trusted interface status and configuration

### Step 4: Enable Dynamic ARP Inspection and Save Configuration

- Enable **dynamic ARP inspection for VLAN 1**
- Verify ARP inspection integration with DHCP snooping
- Save configuration changes to **startup-config file**
- Confirm persistent configuration storage

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. DHCP snooping prevents rogue DHCP server attacks by filtering DHCP messages from untrusted interfaces, maintaining network integrity.
    
2. Trusted interfaces allow legitimate network services while blocking unauthorized DHCP responses from potentially malicious sources.
    
3. Dynamic ARP inspection leverages DHCP snooping databases to validate ARP packets and prevent ARP spoofing attacks.
    
4. Layer 2 security measures work together to create comprehensive protection against common network attacks at the switching level.
    

**Real-World Application:**

- Network security teams implement DHCP snooping to prevent unauthorized network access and maintain IP address assignment integrity.
    
- Enterprise networks use dynamic ARP inspection as part of layered security strategies to protect against man-in-the-middle attacks and network reconnaissance.

## 🖼️ Screenshots