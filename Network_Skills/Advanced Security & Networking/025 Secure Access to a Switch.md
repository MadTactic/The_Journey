# 🧪 Lab: 025 Secure Access to a Switch

## 🎯 Lab Overview

**Objective:** Implement access control profiles to secure switch management and restrict unauthorized administrative access 

**Skills Practiced:**
- Create and configure access control profiles with deny-by-default policies
- Implement IP-based access restrictions for network device management
- Apply access profiles and save security configurations to startup files 

**CertMaster Environment:** 10.4.2 Lab - Secure Access to a Switch

---
## 📝 Implementation Steps

### Step 1: Create Base Access Profile

- Access switch management interface
- Create new access profile named **MgtAccess** with settings:
    - **Access Profile Name:** MgtAccess
    - **Rule Priority:** 1
    - **Management Method:** All
    - **Action:** Deny
    - **Applies to Interface:** All
    - **Applies to Source IP address:** All

### Step 2: Add Permitted Access Rule

- Add profile rule to **MgtAccess** profile with configuration:
    - **Rule Priority:** 2
    - **Management Method:** HTTP
    - **Action:** Permit
    - **Applies to Interface:** All
    - **Source IP Settings:**
        - **IP Version:** Version 4
        - **IP Address:** 192.168.0.10
        - **Network Mask:** 255.255.255.0

### Step 3: Activate Access Profile

- Set **MgtAccess** profile as the **active access profile**
- Verify profile activation and rule application
- Test access restrictions from authorized and unauthorized source IPs

### Step 4: Save Configuration

- Save configuration changes to **startup configuration file**
- Use default settings for configuration save operation
- **Backup credentials:** Username: ITSwitchAdmin, Password: A

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Access control profiles implement deny-by-default security policies, blocking all management access except explicitly permitted connections.
    
2. IP-based access restrictions limit switch management to authorized network segments, reducing attack surface and unauthorized access attempts.
    
3. Rule priority determines the order of policy evaluation, with lower numbers processed first in access control decisions.
    
4. Saving security configurations to startup files ensures access restrictions persist through device reboots and power cycles.
    

**Real-World Application:**

- Network security teams implement access profiles to prevent unauthorized management access to critical infrastructure devices.
    
- IP-based restrictions are standard practice for securing network device management, typically limiting access to dedicated management VLANs or jump hosts.
    
## 🖼️ Screenshots