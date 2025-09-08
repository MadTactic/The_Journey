# 🧪 Lab: 031 Configure a Remote Access VPN

## 🎯 Lab Overview

**Objective:** Deploy OpenVPN remote access solution for secure remote connectivity to corporate resources 

**Skills Practiced:**
- Configure certificate authority and server certificates for VPN authentication
- Implement OpenVPN server with user authentication and network access controls
- Create firewall rules and user accounts for remote access managemen

**CertMaster Environment:** 13.2.8 Lab - Configure a Remote Access VPN

---
## 📝 Implementation Steps

### Step 1: Access pfSense and Create Certificate Authority

- Login to pfSense:
    - **Username:** admin
    - **Password:** P@ssw0rd
- Create certificate authority with settings:
    - **Name:** CorpNet-CA
    - **Country Code:** GB
    - **State:** Cambridgeshire
    - **City:** Woodwalton
    - **Organization:** CorpNet

### Step 2: Generate Server Certificate

- Create server certificate:
    - **Name:** CorpNet
    - **Country Code:** GB
    - **State:** Cambridgeshire
    - **City:** Woodwalton
- Associate certificate with CorpNet-CA authority

### Step 3: Configure OpenVPN Server Settings

- Configure VPN server parameters:
    - **Interface:** WAN
    - **Protocol:** UDP on IPv4 only
    - **Description:** CorpNet-VPN
    - **Tunnel network:** 198.28.20.0/24
    - **Local network:** 198.28.56.18/24
    - **Concurrent connections:** 4
    - **DNS Server 1:** 198.28.56.1

### Step 4: Configure Access Controls and User Accounts

- Create firewall rule for VPN traffic
- Configure OpenVPN rule for remote access
- Set OpenVPN mode to **Remote Access (User Auth)**
- Create VPN user accounts:
    - **blindley** / L3tM31nNow / Brian Lindley
    - **jphillips** / L3tM31nToo / Jacob Phillips

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Certificate-based authentication provides strong security for VPN connections by validating both server and client identities.
    
2. Network segmentation through tunnel addressing isolates VPN traffic while providing controlled access to internal resources.
    
3. User authentication mechanisms ensure only authorized personnel can establish remote connections to corporate networks.
    
4. Firewall integration with VPN services enables granular access control and traffic monitoring for remote connections.
    

**Real-World Application:**

- Organizations deploy remote access VPNs to support secure work-from-home capabilities while maintaining network security boundaries.
    
- VPN solutions are essential for modern business continuity, enabling secure access to corporate resources from any location with internet connectivity.

## 🖼️ Screenshots