# 🧪 Lab: 030 Troubleshoot with Wireshark

## 🎯 Lab Overview

**Objective:** Master advanced Wireshark filtering techniques for network troubleshooting and security analysis 

**Skills Practiced:**
- Apply network-specific filters for traffic analysis
- Use host-based filtering to isolate device communications
- Implement protocol-specific filters for targeted investigation
- Analyze MAC addresses and search packet contents for security indicators 

**CertMaster Environment:** 8.5.5 Lab - Troubleshoot with Wireshark

---
## 📝 Implementation Steps

### Step 1: Configure Wireshark Packet Capture

- Launch **Wireshark** and select **enp2s0** interface
- Begin packet capture session for network monitoring
### Step 2: Apply Network-Based Filters

- Filter for **192.168.0.0 network** traffic using: `net 192.168.0.0/24`
- Document findings for Question 1
- Filter for **192.168.0.45 host** traffic using: `host 192.168.0.45`
- Document findings for Question 2
### Step 3: Implement Directional IP Filters

- Filter for **source traffic from 192.168.0.45** using: `ip.src == 192.168.0.45`
- Document findings for Question 3
- Filter for **destination traffic to 192.168.0.45** using: `ip.dst == 192.168.0.45`
- Document findings for Question 4
### Step 4: Apply Protocol and Content Filters

- Filter for **HTTP traffic on port 80** using: `http and tcp.port == 80`
- Document findings for Question 5
- Filter for **MAC addresses containing 11:12:13** using: `eth.addr contains 11:12:13`
- Document findings for Question 6
- Filter for **TCP packets containing "password"** using: `tcp contains "password"`
- Document findings for Question 7

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Wireshark filters enable precise traffic isolation for focused analysis during network troubleshooting and security investigations.
    
2. Network-based filters help identify traffic patterns and communication flows within specific subnets or between hosts.
    
3. Protocol-specific filtering allows security analysts to focus on particular services or applications during incident response.
    
4. Content-based filtering enables detection of sensitive information transmission and potential security policy violations.


**Real-World Application:**

- SOC analysts use Wireshark filtering to investigate security incidents and identify malicious network activity patterns.
    
- Network troubleshooting requires systematic filtering approaches to isolate problems and identify root causes in complex network environments.

## 🖼️ Screenshots