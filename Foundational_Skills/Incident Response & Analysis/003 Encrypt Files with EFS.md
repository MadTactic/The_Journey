# 🧪 Lab: 003 Encrypt Files with EFS

## 🎯 Lab Overview

**Objective:** Data protection at file level - demonstrates encryption understanding for securing sensitive business data 

**Skills Practiced:**
- Configure Windows Encrypting File System (EFS)
- Implement folder-level encryption with inheritance
- Manage encryption certificates for shared access
- Navigate file security properties and permissions 

**CertMaster Environment:** Simulation/Virtual lab details

---

## 📝 Implementation Steps

### Step 1: Navigate to the Target Folder

- Open **Windows Explorer**
- Browse to *_D:*_
- Locate the **Finances** folder

### Step 2: Encrypt the Finances Folder and Contents

- Right-click on the **D:\Finances** folder
- Select **Properties**
- In the Properties dialog, click **Advanced**
- Check the box for **Encrypt contents to secure data**
- Click **OK** to close Advanced Attributes
- Click **OK** to close Properties
- When prompted, select **Apply changes to this folder, subfolders and files**
- Click **OK** to confirm encryption of all contents

### Step 3: Grant John Access to Specific Encrypted File

- Navigate into the **D:\Finances** folder
- Right-click on **2023report.xlsx**
- Select **Properties**
- Click **Advanced**
- Click **Details** (next to the encryption checkbox)
- Click **Add** to add a new user
- Select **John** from the user list (or browse for John's certificate)
- Click **OK** to add John's encryption certificate
- Click **OK** to close Certificate Details
- Click **OK** to close Advanced Attributes
- Click **OK** to close Properties

### Step 4: Verify Encryption Status

- Confirm that the **Finances** folder and its contents display with green coloring (indicating EFS encryption)
- Verify that **2023report.xlsx** shows encryption status and John has been granted access

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. EFS (Encrypting File System) provides transparent file-level encryption that protects data even if unauthorized users gain physical access to the storage device.
    
2. Folder-level encryption with inheritance ensures all current and future files placed in the encrypted folder are automatically protected without additional configuration.
    
3. Certificate-based access control allows selective sharing of encrypted files with specific users while maintaining security against unauthorized access.
    
4. EFS encryption is user-specific and tied to user accounts, making it ideal for shared computer environments where data segregation is critical.
    

**Real-World Application:**

- Financial departments and sensitive data handlers use EFS to protect confidential documents on shared workstations, ensuring compliance with data protection regulations.
    
- IT administrators implement EFS as part of data loss prevention (DLP) strategies, particularly for laptops and mobile devices that may be lost or stolen, providing an additional security layer beyond standard access controls.
    

## 🖼️ Screenshots

![[Lab003_01.png]]

![[Lab003_02.png]]

![[Lab003_03.png]]

![[Lab003_04.png]]

![[Lab003_05.png]]

![[Lab003_06.png]]

![[Lab003_07.png]]