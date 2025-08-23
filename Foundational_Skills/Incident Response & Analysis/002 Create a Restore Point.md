# 🧪 Lab: 002 Create a Restore Point

## 🎯 Lab Overview

**Objective:** System recovery for incident response - demonstrates disaster recovery skills essential for IT support 

**Skills Practiced:**
- Configure Windows System Protection
- Set disk space allocation for restore points
- Create manual system restore points
- Navigate system recovery settings

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps

### Step 1: Access System Protection Settings

- Open the **Settings** app
- Navigate to **System**
- Select **About**
- Under **Device specifications**, in the _Related links_ box, select **System protection**
- Ensure the **System Protection** tab is selected

### Step 2: Configure System Protection for C: Volume

- Select the **C:** drive from the available drives list
- Click **Configure**
- Turn on system protection for the C: volume
- Set maximum disk space usage to **5%** for restore points
- Click **OK** to apply settings

### Step 3: Configure System Protection for D: Volume

- Select the **D:** drive from the available drives list
- Click **Configure**
- Turn on system protection for the D: volume
- Set maximum disk space usage to **7%** for restore points
- Click **OK** to apply settings

### Step 4: Create a Manual Restore Point

- Click **Create** to generate a manual restore point
- Enter a descriptive name for your restore point (e.g., "Pre-Lab Configuration Backup")
- Click **Create** to finalize the restore point
- Wait for the process to complete and verify successful creation

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. System Protection creates snapshots of system files and settings, providing a rollback mechanism when system changes cause instability or performance issues.
    
2. Disk space allocation for restore points must be balanced—too little space limits recovery options, while too much can impact available storage for applications and data.
    
3. Manual restore points allow proactive system state preservation before making significant changes like software installations or system updates.
    
4. Multiple drive protection ensures comprehensive system recovery, covering both system files and user data stored on different volumes.
    

**Real-World Application:**

- IT professionals create restore points before major system changes, software deployments, or driver updates to provide quick recovery options if issues arise.
    
- System Protection is a critical component of incident response procedures, allowing rapid system recovery without full backup restoration, minimizing downtime in business environments.
    

## 🖼️ Screenshots

![[Lab002_01.png]]

![[Lab002_03.png]]

![[Lab002_04.png]]

![[Lab002_05.png]]

![[Lab002_06.png]]