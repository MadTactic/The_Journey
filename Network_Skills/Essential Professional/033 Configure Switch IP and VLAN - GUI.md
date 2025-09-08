# 🧪 Lab: 033 Configure Switch IP and VLAN - GUI

## 🎯 Lab Overview

**Objective:** Configure static IP addressing and modify default VLAN settings for network segmentation and management 

**Skills Practiced:**
- Assign static IP addresses to switch management interfaces
- Modify default VLAN configurations for security hardening
- Save configuration changes and perform system reboots

**CertMaster Environment:** 5.6.8 - Configure Switch IP and VLAN - GUI

---
## 📝 Implementation Steps

### Step 1: Access Switch Management Interface

- Open **Google Chrome** and navigate to **192.168.0.2**
- Login with credentials:
    - **Username:** cisco
    - **Password:** cisco (case-sensitive)

### Step 2: Configure Static IP Address for VLAN 1

- Navigate to VLAN 1 configuration settings
- Configure static IPv4 parameters:
    - **IP address:** 192.168.45.72
    - **Network mask:** 255.255.255.0
    - **Default gateway:** 192.168.45.1
- Apply IP configuration changes

### Step 3: Modify Default VLAN Settings

- Access VLAN configuration section
- Change **default VLAN ID** from 1 to **16**
- Verify VLAN ID modification is applied

### Step 4: Save Configuration and Reboot

- Save configuration changes to **startup configuration file**
- Verify configuration persistence settings
- Perform **system reboot** to apply all changes
- Confirm switch restarts with new configuration

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Static IP configuration ensures consistent management connectivity and eliminates dependency on DHCP services for network infrastructure.
    
2. Changing default VLAN settings improves security by moving away from commonly known default configurations that attackers may exploit.
    
3. Configuration persistence through startup files ensures network settings survive power cycles and system reboots.
    
4. Systematic configuration changes require proper saving and verification procedures to maintain network stability and accessibility.
    

**Real-World Application:**

- Network administrators configure static management IPs to ensure reliable access to network devices even during DHCP service failures.
    
- Security hardening practices include changing default VLANs and settings to reduce attack surface and improve network segmentation controls.

## 🖼️ Screenshots