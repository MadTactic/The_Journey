# 🧪 Lab: 029 Poison ARP and Analyze with Wireshark
## 🎯 Lab Overview
**Objective:** Detect and analyze ARP poisoning attacks using network forensics and packet analysis techniques

**Skills Practiced:**
- Perform network packet capture using Wireshark
- Analyze ARP traffic patterns to identify malicious activity
- Distinguish between legitimate and suspicious network behavior

**CertMaster Environment:** 9.3.7 Lab - Poison ARP and Analyze with Wireshark

---
## 📝 Implementation Steps
### Step 1: Configure Wireshark Packet Capture
- Launch **Wireshark** application
- Select **enp2s0** network interface for monitoring
- Configure capture duration for **5 seconds**
- Begin packet capture session

### Step 2: Perform Network Traffic Analysis
- Allow capture to run for specified timeframe
- Stop packet capture after 5-second duration
- Review captured network traffic for analysis

### Step 3: Analyze ARP Traffic for Poisoning Indicators
- Filter captured packets for **ARP protocol** traffic
- Examine ARP requests and responses involving **192.168.0.2**
- Look for suspicious patterns:
    - Multiple MAC addresses claiming same IP
    - Frequent gratuitous ARP announcements
    - Unusual ARP response timing

### Step 4: Document Findings and Assessment
- Identify evidence of ARP poisoning activity
- Document suspicious MAC-to-IP mappings
- Complete lab assessment questions based on analysis
---
## 📚 Key Takeaways
**Main Concepts Learned:**
1. ARP poisoning attacks exploit the trustful nature of ARP protocol by sending falsified ARP messages to associate attacker MAC addresses with legitimate IP addresses.
    
2. Wireshark packet analysis enables detection of network attacks by revealing abnormal traffic patterns and protocol violations.
    
3. Network forensics requires understanding of normal protocol behavior to identify deviations that indicate malicious activity.
    
4. ARP cache poisoning can enable man-in-the-middle attacks, allowing attackers to intercept and modify network communications.
    
**Real-World Application:**
- Security analysts use packet capture and analysis to investigate network intrusions and identify attack vectors during incident response.
    
- Network forensics skills are essential for CySA+ certification and security analyst roles, enabling detection of sophisticated attack techniques.
    
## 🖼️ Screenshots