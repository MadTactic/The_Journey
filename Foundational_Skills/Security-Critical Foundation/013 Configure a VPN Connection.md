# 🧪 Lab: 013 Configure a VPN Connection

## 🎯 Lab Overview

**Objective:** Secure remote access configuration - demonstrates VPN deployment for mobile workforce security 

**Skills Practiced:**
- Configure Windows built-in VPN client connections
- Implement SSTP (Secure Socket Tunneling Protocol) for firewall-friendly VPN access
- Apply secure authentication protocols (EAP-MSCHAP v2) for password-based access
- Manage VPN security properties and connection parameters
- Test and verify VPN connectivity for remote workers 

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps

### Step 1: Add VPN Connection

- Open the **Settings** app
- Navigate to **Network & internet**
- Select **VPN**
- Click **Add VPN** to create new connection

### Step 2: Configure Basic VPN Settings

Enter the following VPN connection details:
- **VPN provider:** Windows (built-in)
- **Connection name:** SalesVPN
- **Server name or address:** 198.10.20.12
- **VPN type:** Secure Socket Tunneling Protocol (SSTP)
- **Type of sign-in info:** User name and password
- **Don't save authentication credentials** (uncheck remember credentials option)
- Click **Save** to create the VPN connection

### Step 3: Configure Advanced Security Properties

- Return to **Settings** app
- Navigate to **Network & internet**
- Select **Advanced network settings**
- Click **More network adapter options**
- Right-click the **SalesVPN** connection
- Select **Properties**

### Step 4: Set Security Authentication

- In the VPN Properties dialog, click the **Security** tab
- Configure security settings:
    - **VPN type:** Secure Socket Tunneling Protocol (SSTP)
    - **Authentication:** Microsoft: Secured password (EAP-MSCHAP v2) (encryption enabled)
- Click **OK** to apply security settings

### Step 5: Test VPN Connection

- Return to **Settings** > **Network & internet** > **VPN**
- Select the **SalesVPN** connection
- Click **Connect**
- Enter authentication credentials when prompted:
    - **Username:** MaryS49
    - **Password:** Sm@rt72#
- Verify successful VPN connection establishment

### Step 6: Verify Connection Status

- Confirm VPN connection shows as **Connected**
- Verify network traffic is routing through the VPN tunnel
- Test access to corporate network resources

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. SSTP (Secure Socket Tunneling Protocol) uses HTTPS port 443, making it firewall-friendly since this port is typically open for web traffic in most corporate environments.
    
2. EAP-MSCHAP v2 provides the strongest password-based authentication without requiring smart cards, offering mutual authentication and encrypted credential exchange.
    
3. VPN security configuration requires both connection-level settings and protocol-specific authentication parameters to ensure secure remote access.
    
4. Mobile workforce VPN solutions must balance security requirements with usability and network infrastructure constraints.
    

**Real-World Application:**

- Sales teams and remote workers rely on VPN connections to securely access corporate networks from various locations, requiring reliable and secure authentication methods.
    
- IT administrators choose SSTP for environments with restrictive firewalls, as it leverages standard HTTPS protocols that are less likely to be blocked by network security devices.
    

## 🖼️ Screenshots

![[Lab013_01.png]]

![[Lab013_02.png]]

![[Lab013_03.png]]

![[Lab013_04.png]]

![[Lab013_05.png]]