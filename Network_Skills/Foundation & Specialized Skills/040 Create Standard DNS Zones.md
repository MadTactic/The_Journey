# 🧪 Lab: 040 Create Standard DNS Zones

## 🎯 Lab Overview

**Objective:** Configure primary and secondary DNS zones to support name resolution for new payroll system infrastructure

**Skills Practiced:**
- Create primary forward lookup zones with custom configuration parameters
- Implement secondary DNS zones for redundancy and load distribution
- Configure zone transfer policies for DNS replication 

**CertMaster Environment:** 6.5.12 Lab - Create Standard DNS Zones

---
## 📝 Implementation Steps

### Step 1: Create Primary Forward Lookup Zone on CorpDC

- Access DNS Management console on **CorpDC** server
- Create new forward lookup zone with configuration:
    - **Zone storage:** Deselect "Store the zone in Active Directory"
    - **Zone name:** acct.CorpNet.local
    - **Zone file:** Use default naming convention
    - **Dynamic updates:** Disabled

### Step 2: Configure Zone Transfer Settings

- Configure zone transfer policy to **allow transfers to any server**
- Verify zone transfer settings for replication capability
- Test primary zone functionality and record creation

### Step 3: Create Secondary Forward Lookup Zone on CorpDC3

- Access DNS Management console on **CorpDC3** server
- Create secondary forward lookup zone:
    - **Zone name:** acct.CorpNet.local
    - **Master DNS server:** 192.168.0.11 or CorpDC.CorpNet.Local

### Step 4: Verify DNS Zone Replication

- Confirm secondary zone creation and synchronization
- Test zone transfer from primary to secondary server
- Verify name resolution functionality across both DNS servers

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Primary DNS zones contain authoritative records and allow modifications, while secondary zones provide read-only copies for redundancy and load distribution.
    
2. Zone transfer configuration enables DNS replication between servers, ensuring consistent name resolution across multiple locations.
    
3. File-based DNS zones offer simplified management for specific applications while Active Directory integration provides centralized administration for enterprise environments.
    
4. Secondary DNS zones improve fault tolerance and reduce query response times by distributing name resolution workload across multiple servers.
    

**Real-World Application:**

- Organizations deploy secondary DNS zones to ensure name resolution services remain available during primary server maintenance or failures.
    
- DNS zone segmentation allows different departments to manage their own namespace while maintaining integration with corporate DNS infrastructure.
## 🖼️ Screenshots