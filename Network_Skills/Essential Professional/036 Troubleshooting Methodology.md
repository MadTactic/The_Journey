# 🧪 Lab: 036 Troubleshooting Methodology

## 🎯 Lab Overview

**Objective:** Apply systematic troubleshooting methodology to identify and resolve network connectivity issues 

**Skills Practiced:**
- Implement structured problem identification and isolation techniques
- Compare working vs. non-working configurations to identify root causes
- Test hypotheses systematically and validate solutions 

**CertMaster Environment:** 1.4.10 Lab - Troubleshooting Methodology

---
## 📝 Implementation Steps

### Step 1: Establish Network Connectivity and Identify Problem

- Use **Create Link** tool to connect Office1 and Home-Laptop to Switch
- Test internet connectivity on **Office1** by browsing to **rmksupplies.com**
- Document connectivity failure: "This site can't be reached"
- Test **Home-Laptop** connectivity to same website - verify successful access

### Step 2: Isolate Problem Scope and Develop Theories

- Confirm internet connectivity works for Home-Laptop but fails for Office1
- Develop potential root cause theories:
    - Incorrect IP configuration on Office1
    - Faulty network cable connection
    - Defective NIC hardware
    - Bad switch port assignment

### Step 3: Compare and Analyze Configurations

- Check **Home-Laptop** network settings:
    - Navigate to Network & Internet settings > Ethernet
    - Document: Configured for **Automatic (DHCP)**
- Check **Office1** network settings:
    - Navigate to Network & Internet settings > Ethernet
    - Document: Configured with **manual IP assignment**

### Step 4: Implement and Test Solution

- Change Office1 IP configuration to match working system:
    - Select **Edit** under IP assignment
    - Change to **Automatic (DHCP)** and **Save**
- Test fix by browsing to **rmksupplies.com** from Office1
- Verify successful connectivity and problem resolution

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Systematic troubleshooting methodology prevents random fixes by using structured problem identification and hypothesis testing.
    
2. Comparing working vs. non-working systems quickly identifies configuration differences and potential root causes.
    
3. Network connectivity issues often stem from basic configuration problems rather than complex hardware failures.
    
4. Testing solutions immediately after implementation validates effectiveness and ensures problems are fully resolved.

**Real-World Application:**

- IT professionals use structured troubleshooting approaches to efficiently resolve network issues while minimizing downtime and user impact.
    
- Systematic problem-solving demonstrates professional competence and is essential for technical support, network administration, and cybersecurity incident response roles.

## 🖼️ Screenshots