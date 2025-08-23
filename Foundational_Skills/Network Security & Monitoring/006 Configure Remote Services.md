# 🧪 Lab: 006 Configure Remote Services

## 🎯 Lab Overview

**Objective:** Secure remote access - critical for SOC operations and help desk support scenarios 

**Skills Practiced:**
- Configure Windows Remote Desktop Protocol (RDP) settings
- Manage user access permissions for remote connections
- Verify firewall configurations for remote services
- Navigate system remote access security settings 

**CertMaster Environment:** Simulation/Virtual lab details

---

## 📝 Implementation Steps

### Step 1: Enable Remote Desktop on Office1

- Open the **Settings** app
- Navigate to **System**
- Select **Remote Desktop**
- Turn on **Enable Remote Desktop** to allow incoming RDP connections
- Note any additional security prompts and confirm enabling the service

### Step 2: Add Tom Plask to Remote Desktop Users

- In the Remote Desktop settings, locate user management options
- Click **Advanced settings** or **Select Users** (depending on interface)
- Click **Add** to add a new user for Remote Desktop access
- Search for and select **Tom Plask** from the user directory
- Add Tom Plask to the **Remote Desktop Users** group
- Click **OK** to confirm the user addition

### Step 3: Verify Remote Desktop User Permissions

- Confirm Tom Plask appears in the list of authorized Remote Desktop users
- Verify that Tom Plask has appropriate permissions for remote connection
- Review any additional security settings or requirements

### Step 4: Check Firewall Configuration for Remote Desktop

- Navigate to **Settings** app
- Go to **Privacy & security**
- Select **Windows Security**
- Click **Firewall & network protection**
- Select **Allow an app through firewall**
- Locate **Remote Desktop** in the applications list
- Verify that Remote Desktop is enabled for appropriate network profiles
- Confirm firewall ports are opened correctly for RDP traffic (typically port 3389)

### Step 5: Answer Assessment Question

- Use the firewall configuration interface to answer the provided question about Remote Desktop port settings
- Apply knowledge gained from firewall inspection to determine correct responses

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. Remote Desktop Protocol (RDP) provides secure graphical remote access to Windows systems, enabling help desk support and system administration from remote locations.
    
2. User-based access control for RDP ensures only authorized personnel can establish remote connections, maintaining security boundaries while enabling support functions.
    
3. Firewall configuration must explicitly allow RDP traffic through appropriate network profiles, balancing accessibility with network security requirements.
    
4. Remote access services require careful security consideration, including user permissions, network profiles, and authentication mechanisms to prevent unauthorized access.
    

**Real-World Application:**

- Help desk technicians use RDP to provide remote troubleshooting and support without requiring physical access to user workstations, improving response times and operational efficiency.
    
- IT administrators configure RDP access controls as part of secure remote work policies, ensuring authorized personnel can manage systems remotely while maintaining security standards and audit trails for compliance requirements.
    

## 🖼️ Screenshots

![[Lab006_01.png]]

![[Lab006_02.png]]

![[Lab006_03.png]]

![[Lab006_04.png]]

![[Lab006_05.png]]

![[Lab006_06.png]]

![[Lab006_07.png]]