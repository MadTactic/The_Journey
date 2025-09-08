# 🧪 Lab: 021 Configure a RADIUS Solution

## 🎯 Lab Overview

**Objective:** Implement centralized RADIUS authentication and access control for enterprise remote access infrastructure 

**Skills Practiced:**
- Deploy Network Policy Server (NPS) role for RADIUS functionality
- Configure RADIUS clients with shared secrets and vendor specifications
- Create network access policies with group-based authentication controls
- Integrate remote access servers with centralized RADIUS authentication 

**CertMaster Environment:** 13.2.10 Lab - Configure a RADIUS Solution

---
## 📝 Implementation Steps

### Step 1: Install NPS Role on CorpNPS Server

- Access **CorpNPS** server
- Add **Network Policy and Access Services** server role
- Select **Network Policy Server** role service only
- Complete role installation without unnecessary services

### Step 2: Configure RADIUS Clients in NPS

- Open **Network Policy Server** management console
- Add RADIUS clients with the following specifications:

**CorpVPN1:**

- **Friendly name:** CorpVPN1
- **IP address:** 192.168.0.20
- **Shared secret:** J51nj3T%
- **Vendor:** RADIUS Standard

**BranchVPN1:**

- **Friendly name:** BranchVPN1
- **IP address:** 192.168.20.20
- **Shared secret:** J51nj3T%
- **Vendor:** RADIUS Standard

### Step 3: Create Network Access Policy for Sales Team

- Create new network policy with configuration:
    - **Policy name:** Sales
    - **Network access server type:** Remote Access Server
    - **Condition:** User Groups membership in **Sales** group
    - **Access permission:** Grant access (override user account settings)
    - **Authentication methods:** Smart card or other certificate **only**
    - Disable all other authentication methods

### Step 4: Configure RADIUS Authentication on VPN Servers

**Configure CorpVPN1:**

- Access **Routing and Remote Access** console
- Configure **Authentication Provider:** RADIUS Authentication
- Set **RADIUS Server:** CorpNPS
- Configure **Shared secret:** J51nj3T%
- Set **Accounting Provider:** RADIUS Accounting
- Accept default accounting settings

**Configure BranchVPN1:**

- Repeat identical RADIUS configuration:
    - **Authentication Provider:** RADIUS Authentication
    - **RADIUS Server:** CorpNPS
    - **Shared secret:** J51nj3T%
    - **Accounting Provider:** RADIUS Accounting

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. RADIUS centralization eliminates the need to manage user accounts and policies separately on each remote access server, reducing administrative overhead and security risks.
    
2. Network access policies enable granular control over authentication requirements, allowing organizations to enforce different security standards based on user group membership.
    
3. Shared secrets provide secure communication channels between RADIUS clients and servers, ensuring authentication requests cannot be intercepted or tampered with.
    
4. Certificate-based authentication provides stronger security than password-based methods, supporting zero-trust architecture principles for remote access.
    

**Real-World Application:**

- Enterprise organizations deploy RADIUS solutions to centrally manage authentication across multiple VPN concentrators, wireless access points, and network devices.
    
- IT security teams use RADIUS policies to enforce role-based access controls, ensuring users only access network resources appropriate for their job functions and security clearance levels.
    
## 🖼️ Screenshots