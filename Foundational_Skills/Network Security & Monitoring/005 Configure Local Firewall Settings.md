# 🧪 Lab: 005 Configure Local Firewall Settings

## 🎯 Lab Overview

**Objective:** Network perimeter defense - essential security control for protecting systems against network-based threats 

**Skills Practiced:**
- Configure Windows Firewall for different network profiles
- Enable selective firewall protection for public networks
- Manage application and service exceptions through firewall rules
- Navigate Windows Security settings for network protection 

**CertMaster Environment:** Simulation/Virtual lab details

---

## 📝 Implementation Steps

### Step 1: Access Windows Firewall Settings

- Open the **Settings** app
- Navigate to **Privacy & security**
- Select **Windows Security**
- Click **Firewall & network protection**

### Step 2: Enable Windows Firewall for Public Network Profile

- In the Firewall & network protection window, locate the **Public network** profile
- Click on the **Public network** section
- Turn the firewall **On** for the Public network profile only
- Leave Domain and Private network profiles unchanged (as specified in scenario)

### Step 3: Configure Application Exceptions for Public Network

- Return to the main **Firewall & network protection** screen
- Select **Allow an app through firewall**
- Click **Change settings** to enable modifications

### Step 4: Add Specific Services to Public Network Exceptions

- In the allowed apps list, locate and configure the following services for **Public network only**:
    - **Key Management Service** - Check the Public column box
    - **Cloud Identity** - Check the Public column box
    - **File and Printer Sharing** - Check the Public column box
- Ensure these services are **NOT** enabled for Domain or Private networks (maintain security boundaries)
- Click **OK** to save the firewall exception settings

### Step 5: Verify Firewall Configuration

- Confirm Public network firewall is enabled
- Verify the three specified services are allowed through Public network firewall only
- Test connectivity to ensure proper functionality

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. Windows Firewall uses network profiles (Domain, Private, Public) to apply different security policies based on network trust levels and connection types.
    
2. Public network profiles require the most restrictive firewall settings due to increased security risks from untrusted network environments like airport Wi-Fi.
    
3. Selective service exceptions allow necessary business functions while maintaining security boundaries appropriate to each network environment.
    
4. Proper firewall configuration balances security requirements with operational needs, ensuring protection without disrupting legitimate network communications.
    

**Real-World Application:**

- Mobile workforce security requires dynamic firewall policies that automatically adjust protection levels based on network location and trust level.
    
- IT administrators configure firewall profiles to ensure corporate laptops maintain security standards when connecting to public networks, while allowing necessary business services to function properly for remote work scenarios.
    

## 🖼️ Screenshots

![[Lab005_01 3.png]]

![[Lab005_02 2.png]]

![[Lab005_03 2.png]]

![[Lab005_04 2.png]]

![[Lab005_05 2.png]]

![[Lab005_06 2.png]]
