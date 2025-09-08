# 🧪 Lab: 026 Secure an Enterprise Wireless Network

## 🎯 Lab Overview

**Objective:** Implement comprehensive wireless security controls including credential management, MAC filtering, and device access policies 

**Skills Practiced:**
- Configure wireless controller administrative security credentials
- Implement MAC address filtering with allow lists for device control
- Create device access policies to block specific device categories 

**CertMaster Environment:** 12.3.9 Lab - Secure an Enterprise Wireless Network

---
## 📝 Implementation Steps

### Step 1: Access Ruckus ZoneDirector

- Open **Google Chrome** and navigate to **http://192.168.0.6**
- Login with default credentials:
    - **Admin Name:** admin
    - **Password:** password

### Step 2: Change Administrative Credentials

- Update administrator account security:
    - **New Admin Name:** WxAdmin
    - **New Password:** ZDAdminsOnly!$
- Save credential changes and re-authenticate with new credentials

### Step 3: Configure MAC Address Filtering

- Create L2-L7 Access Control allow list named **Allowed Devices**
- Add the following MAC addresses to whitelist:
    - **00:18:DE:01:34:67**
    - **00:18:DE:22:55:99**
    - **00:02:2D:23:56:89**
    - **00:02:2D:44:66:88**
- Apply allow list to wireless network interfaces

### Step 4: Implement Device Access Policy

- Create device access policy named **NoGames**
- Configure policy to **block gaming consoles** from wireless network
- Apply policy to appropriate wireless network segments
- Verify policy activation and enforcement

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Administrative credential security is the first line of defense for wireless infrastructure, preventing unauthorized configuration changes.
    
2. MAC address filtering provides device-level access control, though it should be combined with other security measures for comprehensive protection.
    
3. Device access policies enable granular control over network access based on device type, supporting acceptable use policies and network resource management.
    
4. Wireless controllers centralize security policy management across multiple access points, ensuring consistent security enforcement.
    

**Real-World Application:**

- Enterprise wireless deployments use multiple security layers including strong administrative controls, device filtering, and policy-based access management.
    
- Device access policies help organizations maintain productivity by restricting non-business devices while allowing necessary corporate and BYOD equipment.
    
## 🖼️ Screenshots