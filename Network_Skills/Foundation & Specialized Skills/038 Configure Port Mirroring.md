# 🧪 Lab: 038 Configure Port Mirroring

## 🎯 Lab Overview

**Objective:** Configure switch port mirroring to enable network traffic analysis and intrusion detection monitoring 

**Skills Practiced:**
- Configure VLAN assignments for network monitoring infrastructure
- Implement port mirroring to copy traffic for security analysis
- Save switch configurations for persistent monitoring capabilities 

**CertMaster Environment:** 8.5.6 Lab - Configure Port Mirroring

---
## 📝 Implementation Steps

### Step 1: Access Switch Management Console

- Open **Google Chrome** and navigate to **192.168.0.2**
- Login with credentials (case-sensitive):
    - **Username:** cisco
    - **Password:** cisco
- Access switch port configuration interface

### Step 2: Configure Destination Port VLAN Assignment

- Assign **port GE26** to **VLAN 1**
- Verify VLAN assignment for monitoring port configuration
- Prepare destination port for mirrored traffic reception

### Step 3: Configure Port Mirroring

- Configure traffic mirroring from **source port GE28** to **destination port GE26**
- Set mirroring to capture **received traffic** from GE28
- Verify port mirroring configuration activation

### Step 4: Save Configuration for Persistence

- Save all configuration changes to **startup configuration file**
- Verify configuration persistence across switch reboots
- Confirm monitoring setup is ready for IDS integration

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Port mirroring enables passive network monitoring by copying traffic from source ports to dedicated analysis ports without affecting network performance.
    
2. VLAN assignment ensures mirrored traffic is properly segmented and routed to monitoring systems like intrusion detection systems.
    
3. Persistent configuration storage ensures network monitoring capabilities remain active through power cycles and maintenance events.
    
4. Traffic mirroring supports security operations by providing visibility into network communications for threat detection and analysis.
    

**Real-World Application:**

- Security teams use port mirroring to feed network traffic into SIEM systems and intrusion detection platforms for continuous monitoring.
    
- Network troubleshooting often requires port mirroring to analyze traffic patterns and identify performance or security issues.

## 🖼️ Screenshots