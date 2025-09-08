# 🧪 Lab: 043 Use ping and tracert on Windows/Linux

## 🎯 Lab Overview

**Objective:** Diagnose and resolve network connectivity issues using command-line diagnostic tools across Windows and Linux platforms 

**Skills Practiced:**
- Execute ping and traceroute commands for network troubleshooting
- Analyze IP configuration settings to identify connectivity problems
- Apply systematic troubleshooting methodology to resolve routing issues

**CertMaster Environment:** 4.6.4 Lab (Windows) / 4.6.5 Lab (Linux)

---
## 📝 Implementation Steps

### Step 1: Test Local Network Connectivity (Windows)

- From **Exec** computer, open Admin Terminal
- Ping **CorpServer (192.168.0.10)** and **Office2 (192.168.0.31)**
- Verify local network connectivity is functional
- Document successful local communication

### Step 2: Diagnose Internet Connectivity Issues (Windows)

- Review network diagram in **Exhibits** for router IP addresses
- Use **ipconfig** to examine Exec computer network configuration
- Ping **Building A router (192.168.0.5)** to test gateway connectivity
- Use **tracert** to trace path to ISP router and identify routing problems
- Modify IP configuration to resolve connectivity issues

### Step 3: Explore Network Communication Limitations (Linux)

- From **IT-Laptop**, test connectivity using **ping -c4** commands:
    - **192.168.0.30 (Office1)** - successful (same network)
    - **199.92.0.32 (Support)** - fails (different network, no gateway)
    - **192.168.0.5 (router)** - successful (same network)
    - **163.128.78.93 (DNS)** - fails (no default gateway configured)

### Step 4: Analyze Network Configuration and Routing (Linux)

- Examine IP configuration in **/etc/sysconfig/network-scripts/ifcfg-enp2s0**
- Identify missing **GATEWAY** parameter causing external connectivity failure
- From **Office2**, use **traceroute 198.28.56.1** to trace path to internet router
- Use **traceroute 163.128.78.93** to analyze path to external DNS server

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Network diagnostic tools like ping and traceroute provide essential visibility into connectivity problems and routing paths between network segments.
    
2. Default gateway configuration is critical for inter-network communication - devices cannot reach external networks without proper gateway settings.
    
3. Cross-platform diagnostic skills (Windows/Linux) are essential as enterprise environments typically contain mixed operating system deployments.
    
4. Systematic troubleshooting methodology helps identify whether problems exist at local, gateway, or external network levels.


**Real-World Application:**

- IT support professionals use ping and traceroute daily to diagnose connectivity issues and validate network path functionality.
    
- Network administrators rely on these diagnostic tools to troubleshoot routing problems and verify network configuration changes in enterprise environments.

## 🖼️ Screenshots