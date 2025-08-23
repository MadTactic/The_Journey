# 🧪 Lab: 017 Create User Accounts

## 🎯 Lab Overview

**Objective:** Identity and access management - fundamental security principle for organizational user provisioning 

**Skills Practiced:**
- Create Active Directory user accounts with proper organizational unit placement
- Implement corporate naming conventions and domain standards
- Configure account restrictions and time-based access controls
- Apply temporary employee security policies and account expiration
- Navigate Active Directory Users and Computers management console 

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps

### Step 1: Access Active Directory Management

- Launch the **CorpDC** virtual machine
- Open **Server Manager**
- Navigate to **Tools** > **Active Directory Users and Computers**
- Expand **CorpNet.local** to view organizational units

### Step 2: Create Juan Suarez Account

- Navigate to **Marketing\MarketingManagers** OU
- Right-click the OU and select **New** > **User**
- Enter user information:
    - **First name:** Juan
    - **Last name:** Suarez
    - **User logon name:** jsuarez@CorpNet.local
- Click **Next**
- Set password: **asdf1234$**
- Check **User must change password at next logon**
- Click **Next** and **Finish**

### Step 3: Create Susan Smith Account

- Navigate to **Sales\PermSales** OU
- Right-click the OU and select **New** > **User**
- Enter user information:
    - **First name:** Susan
    - **Last name:** Smith
    - **User logon name:** ssmith@CorpNet.local
- Set password: **asdf1234$**
- Check **User must change password at next logon**
- Complete account creation

### Step 4: Create Mark Burnes Account

- Navigate to **Sales\SalesManagers** OU
- Right-click the OU and select **New** > **User**
- Enter user information:
    - **First name:** Mark
    - **Last name:** Burnes
    - **User logon name:** mburnes@CorpNet.local
- Set password: **asdf1234$**
- Check **User must change password at next logon**
- Complete account creation

### Step 5: Create Borey Chan Account (Temporary Employee)

- Navigate to **Sales\TempSales** OU
- Right-click the OU and select **New** > **User**
- Enter user information:
    - **First name:** Borey
    - **Last name:** Chan
    - **User logon name:** bchan@CorpNet.local
- Set password: **asdf1234$**
- Check **User must change password at next logon**
- Complete account creation

### Step 6: Configure Temporary Employee Restrictions

- Right-click **Borey Chan** account and select **Properties**
- Navigate to the **Account** tab
- Configure logon hour restrictions:
    - Click **Logon Hours**
    - Set allowed hours: **Monday through Friday, 8:00 AM to 5:00 PM**
    - Deny access for all other times
    - Click **OK**
- Set account expiration:
    - Check **Account expires**
    - Set expiration date: **December 31st** of current year
- Click **OK** to apply all restrictions

### Step 7: Verify Account Creation

- Confirm all four user accounts appear in their respective OUs
- Verify naming convention compliance for all accounts
- Test logon restrictions for temporary employee if possible
- Document account creation completion

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. Active Directory organizational units enable logical grouping of user accounts based on business roles and departmental structure, facilitating efficient administration and policy application.
    
2. Standardized naming conventions ensure consistency and predictability in user account management while supporting automated processes and integration with other systems.
    
3. Temporary employee accounts require additional security controls including time-based access restrictions and automatic expiration dates to limit security exposure.
    
4. Password policies requiring initial password changes ensure users establish personal credentials while maintaining security standards from account creation.
    

**Real-World Application:**

- HR onboarding processes rely on standardized account creation procedures to ensure new employees receive appropriate access based on their roles and employment status.
    
- Identity and Access Management (IAM) systems use OU-based organization and time-based restrictions to implement principle of least privilege and automatically manage temporary access for contractors and seasonal employees.
    

## 🖼️ Screenshots

![[Lab017_01.png]]

![[Lab017_02.png]]

![[Lab017_03.png]]

![[Lab017_04.png]]

![[Lab017_05.png]]

![[Lab017_06.png]]

![[Lab017_07.png]]

![[Lab017_08.png]]

![[Lab017_09.png]]