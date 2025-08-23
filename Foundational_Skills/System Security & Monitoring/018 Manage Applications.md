# 🧪 Lab: 018 Manage Applications

## 🎯 Lab Overview

**Objective:** Process monitoring and management - essential for threat detection and system optimization 

**Skills Practiced:**
- Configure Windows startup application management using Task Manager
- Disable unnecessary startup programs to improve system performance and security
- Apply application compatibility settings for legacy software integration
- Implement administrative privileges for specific application requirements 

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps

### Step 1: Access Task Manager Startup Management

- Right-click **Start** button
- Select **Task Manager**
- Navigate to **Startup apps** tab (fourth icon from the bottom left)
- Review list of applications configured to start at system startup

### Step 2: Disable Unnecessary Startup Applications

Disable the following applications from startup:

#### Disable Compy DVD Apps

- Locate **Compy DVD Apps** in the startup list
- Select the application
- Click **Disable**
- Verify status changes to "Disabled"

#### Disable DIRE Event Monitor

- Locate **DIRE Event Monitor** in the startup list
- Select the application
- Click **Disable**
- Verify status changes to "Disabled"

#### Disable inTune

- Locate **inTune** in the startup list
- Select the application
- Click **Disable**
- Verify status changes to "Disabled"

#### Disable SM66 Win32 Utility

- Locate **SM66 Win32 Utility** in the startup list
- Select the application
- Click **Disable**
- Verify status changes to "Disabled"

### Step 3: Close Task Manager

- Close Task Manager after completing startup application modifications
- Changes will take effect on next system restart

### Step 4: Configure Application Compatibility Settings

- Open **File Explorer**
- Navigate to *_C:\Program Files (x86)\AccountWizard*_
- Locate **AccountWizard.exe** file

### Step 5: Access Compatibility Properties

- Right-click **AccountWizard.exe**
- Select **Properties**
- Click the **Compatibility** tab

### Step 6: Configure Compatibility Mode Settings

Apply the following compatibility settings:

#### Set Windows 8 Compatibility Mode

- Check **Run this program in compatibility mode for:**
- Select **Windows 8** from the dropdown menu

#### Configure Display Settings

- Check **Run in 640 x 480 screen resolution**
- This ensures proper display for legacy applications

#### Set Administrative Privileges

- Check **Run this program as an administrator**
- This provides elevated privileges for proper application functionality

### Step 7: Apply and Verify Settings

- Click **OK** to save all compatibility settings
- Verify settings are properly configured by reopening Properties if needed
- Test application launch if required to confirm compatibility settings work

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. Startup application management directly impacts system performance, security, and boot times by controlling which processes automatically launch with the operating system.
    
2. Disabling unnecessary startup programs reduces attack surface area and system resource consumption while maintaining only essential services and applications.
    
3. Compatibility mode settings enable legacy applications to function properly on modern operating systems by emulating older system behaviors and display requirements.
    
4. Administrative privilege configuration ensures applications requiring elevated permissions can function correctly while maintaining security boundaries.
    

**Real-World Application:**

- IT administrators regularly audit and optimize startup programs across enterprise systems to maintain performance standards and reduce security exposure from unnecessary running processes.
    
- Legacy application support through compatibility modes enables organizations to continue using business-critical software while transitioning to newer operating systems, balancing operational continuity with security modernization requirements.
    

## 🖼️ Screenshots

![[Lab018_01.png]]

![[Lab018_02.png]]

![[Lab018_03.png]]

![[Lab018_04.png]]