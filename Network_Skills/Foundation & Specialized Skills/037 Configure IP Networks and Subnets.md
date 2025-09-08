# 🧪 Lab: 037 Configure IP Networks and Subnets

## 🎯 Lab Overview

**Objective:** Analyze IP subnet configurations and test inter-VLAN connectivity through routing infrastructure 

**Skills Practiced:**
- Gather and analyze IP configuration information using ipconfig commands
- Test network connectivity between different subnets and VLANs
- Configure router interfaces to enable inter-subnet communication 

**CertMaster Environment:** 4.3.7 Lab - Configure IP Networks and Subnets

---
## 📝 Implementation Steps

### Step 1: Analyze Host IP Configurations

- Use **ipconfig** command on **Account2**, **Marketing2**, and **Sales2**
- Document IP addresses, subnet masks, and network assignments
- Complete assessment questions 1-6 based on gathered information
- Use **Hide Notes** toggle to manage display visibility as needed

### Step 2: Test Layer 2 Connectivity

- Create direct link between **Switch1** and **Switch2**
- Test connectivity from **Marketing2** to **Sales2** using ping
- Test connectivity from **Sales1** to both **Sales2** and **Marketing2**
- Gather **Sales1** IP configuration using **ipconfig**
- Complete assessment questions 7-11 based on connectivity results

### Step 3: Implement Layer 3 Routing

- Remove direct switch-to-switch connection
- Connect **Router1** interfaces to switches:
    - **enp2s0** → **Switch1**
    - **enp2s1** → **Switch2**
    - **enp2s2** → **Switch3**

### Step 4: Verify Inter-Subnet Routing

- Test connectivity from **Account2**:
    - Ping **Sales2** IP address
    - Ping **Marketing2** IP address
- Complete assessment question 12 based on routing test results
- Document successful inter-subnet communication through router

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Layer 2 switching enables communication within the same subnet but cannot route traffic between different network segments.
    
2. Routers provide Layer 3 functionality necessary for inter-subnet communication by forwarding packets between different network segments.
    
3. IP subnet analysis requires understanding of network addresses, host ranges, and subnet mask configurations.
    
4. Network connectivity testing validates proper routing configuration and helps identify communication barriers between subnets.


**Real-World Application:**

- Network administrators use subnet analysis to design efficient IP addressing schemes and troubleshoot connectivity issues.
    
- Inter-VLAN routing is essential for enterprise networks where different departments require network segmentation while maintaining controlled communication paths.

## 🖼️ Screenshots
