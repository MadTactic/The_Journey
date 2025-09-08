# 🧪 Lab: 028 Configure Logging in pfSense

## 🎯 Lab Overview

**Objective:** Configure comprehensive logging and remote syslog forwarding for security monitoring and incident response 

**Skills Practiced:**
- Configure system log display and storage parameters
- Enable remote syslog forwarding to centralized log servers
- Filter log categories for focused security event monitoring 

**CertMaster Environment:** 8.4.6 Lab - Configure Logging in pfSense

---
## 📝 Implementation Steps

### Step 1: Access pfSense Management Interface

- Open **Chrome** and navigate to **198.28.56.22**
- Login credentials:
    - **Username:** admin
    - **Password:** P@ssw0rd
- Navigate to **Status > System Logs** section

### Step 2: Configure General System Log Settings

- Modify log display parameters:
    - **Logs to show:** 25 entries per page
    - **Maximum log file size:** 250000 bytes
- Apply general logging configuration changes

### Step 3: Enable Remote System Logging

- Navigate to **System > Advanced > Logging** settings
- Configure remote syslog forwarding:
    - **Remote log server:** 192.168.0.10 (CorpServer)
    - **Enable remote logging:** Yes
    - **Log categories to forward:**
        - System events
        - Firewall events
- Save remote logging configuration

### Step 4: Verify Logging Configuration

- Test log forwarding functionality
- Verify log file size limits are enforced
- Complete lab assessment questions

---
## 📚 Key Takeaways

**Main Concepts Learned:**

1. Centralized logging enables comprehensive security monitoring and provides audit trails for incident investigation.
    
2. Log file size limits prevent storage exhaustion while maintaining sufficient historical data for analysis.
    
3. Selective log forwarding reduces network overhead and focuses monitoring on critical security events.
    
4. Remote syslog forwarding supports compliance requirements and enables integration with SIEM platforms.
    

**Real-World Application:**

- Security operations teams use centralized logging to correlate events across multiple network devices for threat detection.
    
- Log management is fundamental to SIEM operations, providing the data foundation for security analytics and incident response procedures.
    
## 🖼️ Screenshots