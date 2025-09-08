# 🧪 Lab: 022 Configure NAT

## 🎯 Lab Overview

**Objective:** Implement Network Address Translation with port forwarding rules for secure remote management of DMZ resources 

**Skills Practiced:**
- Configure NAT port forwarding rules on pfSense firewall
- Establish secure communication paths between network segments
- Implement protocol-specific forwarding for RDP and SSH services
- Manage custom port mappings for enhanced security 

**CertMaster Environment:** 5.3.4 Lab - Configure NAT

---
## 📝 Implementation Steps

### Step 1: Access pfSense Management Console

- Navigate to pfSense web interface
- Login credentials:
    - **Username:** admin
    - **Password:** P@ssw0rd
- Access **Firewall > NAT** configuration section

### Step 2: Configure RDP Port Forwarding to PC1

- Create new NAT port forwarding rule:
    - **Protocol:** TCP
    - **Destination:** RDP (Port 3389)
    - **Target IP:** 172.16.1.100
    - **Source:** LAN network
    - **Description:** RDP from LAN to PC1
- Save and apply configuration changes

### Step 3: Configure SSH Port Forwarding to Kali Linux Server

- Create new NAT port forwarding rule:
    - **Protocol:** TCP
    - **Destination:** SSH (Port 22)
    - **Target IP:** 172.16.1.6
    - **Source:** LAN network
    - **Description:** SSH from LAN to Kali
- Save and apply configuration changes

### Step 4: Configure Custom RDP Port Forwarding to Web Server

- Create new NAT port forwarding rule:
    - **Protocol:** TCP
    - **Destination port:** 5151
    - **Redirect target port:** 3389 (RDP)
    - **Target IP:** 172.16.1.5
    - **Source:** LAN network
    - **Description:** RDP from LAN to web server using custom port
- Save and apply all NAT configuration changes

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. NAT port forwarding enables secure remote management of DMZ resources while maintaining network segmentation and security boundaries.
    
2. Custom port mappings enhance security by obscuring standard service ports, making it more difficult for attackers to identify running services.
    
3. Protocol-specific forwarding rules allow granular control over which services are accessible across network segments, supporting least-privilege access principles.
    
4. pfSense firewalls provide enterprise-grade NAT capabilities that support complex network topologies with multiple security zones and access requirements.
    

**Real-World Application:**

- Network administrators use NAT port forwarding to enable secure remote administration of servers in DMZ environments without exposing direct network paths.
    
- Custom port configurations are standard security practices in enterprise environments, helping to reduce attack surface while maintaining necessary administrative access to critical infrastructure.
    
## 🖼️ Screenshots