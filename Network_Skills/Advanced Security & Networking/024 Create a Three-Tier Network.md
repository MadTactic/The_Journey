# 🧪 Lab: 024 Create a Three-Tier Network

## 🎯 Lab Overview

**Objective:** Design and implement a three-tier hierarchical network architecture with proper redundancy and connectivity 

**Skills Practiced:**
- Design hierarchical network topologies (Access, Distribution, Core layers)
- Implement redundant connections for high availability
- Configure inter-layer connectivity using proper port assignments 

**CertMaster Environment:** 5.5.4 Lab - Create a Three-Tier Network

---
## 📝 Implementation Steps

### Step 1: Create Access Layer Default Connections

- Connect **Access1 port 0** to **Dist1 enp2s0**
- Connect **Access2 port 0** to **Dist2 enp2s0**
- Connect **Access3 port 0** to **Dist3 enp2s0**
- Verify primary uplink connections from access switches to distribution routers

### Step 2: Implement Distribution Layer Redundancy

- Access **Exhibits** panel from top right toolbar
- Review interface-to-IP address mappings and network assignments
- Create redundant connections between distribution routers and access switches:
    - Connect each distribution router to the other two access switches
    - Use available open ports on switches for redundant paths
- Follow exhibit specifications for proper interface assignments

### Step 3: Configure Core Layer Connectivity

- Implement connections from **Core layer** to **Distribution layer**
- Establish high-speed backbone links between core and distribution routers
- Ensure all distribution routers have redundant paths to core layer
- Use **Hide Notes** toggle to manage display visibility as needed

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Three-tier architecture provides scalability, redundancy, and clear separation of network functions across Access, Distribution, and Core layers.
    
2. Redundant connections prevent single points of failure and ensure network availability during equipment failures or maintenance.
    
3. Hierarchical design simplifies network management by creating clear boundaries between network functions and traffic flows.
    
4. Proper port assignment and interface mapping are critical for maintaining organized, manageable network infrastructures.
    

**Real-World Application:**

- Enterprise networks use three-tier designs to support thousands of users while maintaining performance, security, and fault tolerance.
    
- Network architects implement redundant paths to meet SLA requirements and ensure business continuity during infrastructure failures.

## 🖼️ Screenshots