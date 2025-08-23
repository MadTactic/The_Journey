# 🧪 Lab: 016 Configure NTFS Permissions

## 🎯 Lab Overview

**Objective:** Access control implementation - core security administration for data segregation and group-based access management 

**Skills Practiced:**
- Configure NTFS file system permissions and access control lists (ACLs)
- Disable permissions inheritance and convert to explicit permissions
- Manage group-based access control for data segregationdsawdsawdsawdsawdsawdsaw
- Apply principle of least privilege through selective permission assignment

**CertMaster Environment:** Simulation/Virtual lab details

---
## 📝 Implementation Steps

### Step 1: Configure D:\Day Data Folder Permissions

#### Access Folder Security Properties

- Open **File Explorer** and navigate to **D:\Day Data** folder
- Right-click the **D:\Day Data** folder
- Select **Properties**
- Click the **Security** tab

#### Disable Permissions Inheritance

- Click **Advanced** to open Advanced Security Settings
- Click **Disable inheritance**
- Select **Convert inherited permissions into explicit permissions on this object**
- Click **Apply** and **OK** to confirm conversion

#### Remove Users Group

- In the Security tab, select **Users** group from the permissions list
- Click **Remove** to delete the Users group from the ACL
- Confirm removal when prompted

#### Add DayGroup with Full Control

- Click **Add** to add a new group
- Click **Select a principal**
- Type **DayGroup** and click **Check Names**
- Click **OK** to select DayGroup
- In permissions, check **Full control**
- Click **OK** to apply permissions

### Step 2: Configure D:\Night Data Folder Permissions

#### Access Folder Security Properties

- Navigate to **D:\Night Data** folder in File Explorer
- Right-click the **D:\Night Data** folder
- Select **Properties**
- Click the **Security** tab

#### Disable Permissions Inheritance

- Click **Advanced** to open Advanced Security Settings
- Click **Disable inheritance**
- Select **Convert inherited permissions into explicit permissions on this object**
- Click **Apply** and **OK** to confirm conversion

#### Remove Users Group

- In the Security tab, select **Users** group from the permissions list
- Click **Remove** to delete the Users group from the ACL
- Confirm removal when prompted

#### Add NightGroup with Full Control

- Click **Add** to add a new group
- Click **Select a principal**
- Type **NightGroup** and click **Check Names**
- Click **OK** to select NightGroup
- In permissions, check **Full control**
- Click **OK** to apply permissions

### Step 3: Verify Permission Configuration

- Confirm **D:\Day Data** shows DayGroup with Full Control permissions
- Confirm **D:\Night Data** shows NightGroup with Full Control permissions
- Verify Users group has been removed from both folders
- Ensure other existing permissions remain unchanged
- Test access with appropriate group members if possible

---

## 📚 Key Takeaways

**Main Concepts Learned:**

1. NTFS permissions inheritance can be disabled to create explicit, customized access control lists that don't automatically inherit parent directory permissions.
    
2. Converting inherited permissions to explicit permissions preserves existing access while allowing granular modification of specific user and group permissions.
    
3. Group-based access control enables efficient data segregation by assigning permissions to groups rather than individual users, simplifying administration and scaling.
    
4. The principle of least privilege is implemented by removing broad access (Users group) and granting specific access only to appropriate groups (DayGroup, NightGroup).
    

**Real-World Application:**

- IT administrators use NTFS permissions to implement data classification and access control policies, ensuring sensitive information is only accessible to authorized personnel based on business roles.
    
- Group-based permission management scales efficiently in enterprise environments, allowing role changes through group membership modifications rather than individual permission updates across multiple resources.
    

## 🖼️ Screenshots

![[Lab016_01.png]]

![[Lab016_02.png]]

![[Lab016_03.png]]

![[Lab016_04.png]]

![[Lab016_05.png]]

![[Lab016_06.png]]

![[Lab016_07.png]]

![[Lab016_08.png]]
