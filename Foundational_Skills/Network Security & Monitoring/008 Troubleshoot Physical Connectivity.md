# 🧪 Lab: 008 Troubleshoot Physical Connectivity
## 🎯 Lab Overview

**Objective:** Network troubleshooting skills - needed for security incident investigation and network infrastructure maintenance

**Skills Practiced:**
- Apply systematic network troubleshooting methodologies
- Use ping command for network connectivity testing
- Analyze network device indicator lights and status information
- Identify and resolve physical layer connectivity issues
- Replace faulty network components using spare parts

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps
### Step 1: Initial Problem Assessment
- **Problem Report:** Office1 cannot communicate with Office2
- Review network topology using **Exhibits** (network diagram and wiring schematics)
- Document current symptoms and affected systems
- Plan systematic troubleshooting approach

### Step 2: Network Connectivity Testing Using Ping
- From Office1, open **Terminal (Admin)** and test connectivity:
  - **ping 192.168.0.31** (Office2 - fails, indicating problem)
  - **ping** other workstations (all succeed except Office2)
- From Office2, test outbound connectivity:
  - All pings fail except localhost (192.168.0.31)
- Document ping results to isolate problem scope

### Step 3: Physical Layer Analysis
- Check Office2 NIC port - no blinking lights (indicates no network connection)
- Verify cable connections at NIC and wall plate (properly connected)
- Test by replacing ethernet cable from Office2 to wall (problem persists)
- Check Networking Closet switch Port 4 - no activity lights
- **Root cause identified:** Faulty patch cable between switch and patch panel

### Step 4: Windows Network Status Verification
- Access **Settings** app on affected systems
- Navigate to **Network & Internet**
- Check **Network and Internet Status** page
- Review connection status, network profile, and any error messages
- Document network adapter status and configuration

### Step 5: Problem Resolution
- In Networking Closet, replace faulty patch cable:
  - Remove cable from switch Port 4 and patch panel "Off 2"
  - Install new Ethernet cable connecting switch Port 4 to Office 2 patch panel port
- Verify Port 4 now shows green/active status lights

### Step 6: Verification Testing
- Office2 NIC now shows active blinking lights
- Windows Network Status shows connection to network and internet
- From Office1: **ping Office2** now succeeds
- All network connectivity restored

---
## 📚 Key Takeaways

**Main Concepts Learned:**
1. Systematic network troubleshooting follows a structured approach from physical layer to application layer, ensuring efficient problem resolution.
    
2. The ping command provides essential connectivity testing capabilities, helping isolate whether problems exist at network, routing, or host levels.
    
3. Physical layer indicators (LED status lights) offer immediate visual feedback about connectivity, link status, and network activity patterns.
    
4. Network configuration status in Windows provides detailed information about adapter state, IP configuration, and connection health.
    
**Real-World Application:**
- Network technicians use these troubleshooting methodologies daily to resolve connectivity issues that could impact business operations or security monitoring systems.
    
- Security incident responders often need to verify network connectivity when investigating potential network-based attacks or when network issues might be masking security events, making these troubleshooting skills essential for SOC operations.

## 🖼️ Screenshots

![[Lab008_01.png]]

![[Lab008_02.png]]

![[Lab008_03.png]]

![[Lab008_04.png]]

![[Lab008_05.png]]