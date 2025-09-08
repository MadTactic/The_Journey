# 🧪 Lab: 027 Configure a Perimeter Firewall

## 🎯 Lab Overview

**Objective:** Configure perimeter firewall rules to secure DMZ web services while enabling required network access 

**Skills Practiced:**
- Create firewall rules for HTTP/HTTPS traffic from WAN to DMZ
- Configure LAN-to-DMZ access policies
- Implement network security hardening on pfSense appliance 

**CertMaster Environment:** 10.5.8 Lab - Configure a Perimeter Firewall

---
## 📝 Implementation Steps

### Step 1: Access pfSense Management Console

- Login to pfSense web interface:
    - **Username:** admin
    - **Password:** P@ssw0rd
- Navigate to **Firewall > Rules** section

### Step 2: Create HTTP Traffic Rule (WAN to DMZ)

- Create new firewall rule:
    - **Source:** WAN network
    - **Destination:** Single host (172.16.1.5)
    - **Destination port:** HTTP (80)
    - **Action:** Pass
    - **Description:** HTTP from WAN to DMZ

### Step 3: Create HTTPS Traffic Rule (WAN to DMZ)

- Create new firewall rule:
    - **Source:** WAN network
    - **Destination:** Single host (172.16.1.5)
    - **Destination port:** HTTPS (443)
    - **Action:** Pass
    - **Description:** HTTPS from WAN to DMZ

### Step 4: Create LAN-to-DMZ Access Rule

- Create new firewall rule:
    - **Source:** LAN network
    - **Destination:** DMZ network
    - **Protocol:** Any
    - **Action:** Pass
    - **Description:** LAN to DMZ Any
- Save and apply all firewall rule configurations

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Perimeter firewalls control traffic between network segments, enforcing security policies at network boundaries.
    
2. Protocol-specific rules enable precise control over allowed services while blocking unnecessary traffic.
    
3. DMZ placement isolates public-facing services from internal networks while allowing controlled access.
    
4. Firewall rule ordering and specificity determine traffic flow and security enforcement effectiveness.
    

**Real-World Application:**

- Organizations use perimeter firewalls to protect web services in DMZ while maintaining strict controls between network segments.
    
- Layered security approaches combine firewall rules with network segmentation to minimize attack surface and contain potential breaches.

## 🖼️ Screenshots