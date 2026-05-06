# Endpoint Security (EDR & XDR Concepts)

## Objective

The objective of this session is to understand how endpoint security solutions detect, analyze, and respond to cyber threats targeting systems like laptops, desktops, and servers.

By the end of this session, you will be able to:

- Understand endpoint security
- Differentiate between EDR and XDR
- Identify suspicious endpoint activities
- Analyze attack scenarios
- Apply detection logic
- Understand SOC workflows
- Suggest response strategies


## 1. Endpoint Security

Endpoint security protects devices such as:

- Laptops
- Desktops
- Servers
- Mobile devices

### Key Functions

- Monitor endpoint activity
- Detect malicious files and processes
- Prevent unauthorized access
- Respond to incidents

### Importance

- Endpoints are common attack targets
- Protects against malware and ransomware
- Prevents lateral movement
- Ensures data security


## 2. EDR (Endpoint Detection and Response)

EDR focuses on monitoring and detecting threats at the endpoint level.

### Capabilities

Monitoring:
- Tracks processes
- Monitors files
- Observes user activity

Detection:
- Identifies suspicious behavior
- Detects malware

Response:
- Kill malicious processes
- Isolate system
- Quarantine files

### Features

- Real-time monitoring
- Behavioral detection
- Investigation support
- Automated response


## 3. XDR (Extended Detection and Response)

XDR expands security by combining multiple data sources.

### Data Sources

- Endpoint logs
- Network traffic
- Email systems
- Cloud systems

### Advantages

- Centralized visibility
- Multi-source correlation
- Detects complex attacks
- Reduces false alerts


## EDR vs XDR

EDR:
- Works only on endpoints
- Limited visibility
- Detects endpoint-level threats

XDR:
- Covers endpoint, network, email, cloud
- Broad visibility
- Detects multi-stage attacks


## 4. Example Scenario

Alert:
- malware.exe running
- Connected to external IP

### Analysis

- Unknown process → Possible malware
- External connection → Possible C2 communication
- Continuous activity → Possible attack control

### Risk Level

HIGH


## 5. Detection Logic

Basic Rule:

IF unknown process is running  
AND external connection detected  
THEN alert: Possible malware activity  

Advanced Rule:

IF process not trusted  
AND external connection = true  
AND IP suspicious  
THEN HIGH alert: Endpoint compromise  


## 6. SOC Workflow

L1 Analyst:
- Monitor alerts
- Detect suspicious activity
- Escalate issues

L2 Analyst:
- Investigate logs
- Confirm threat
- Respond (kill process, isolate system)

L3 Analyst:
- Improve detection rules
- Build advanced logic
- Enhance security


## 7. Attack Scenario

Scenario: Malware Infection

Step 1: User downloads malicious file  
Step 2: malware.exe executes  
Step 3: Malware creates persistence  
Step 4: Connects to external server  
Step 5: Attacker gains control  

Impact:
- Data theft
- System compromise


## 8. Response and Mitigation

### Immediate Actions

- Kill malicious process
- Isolate system
- Block IP
- Disable account

### Investigation

- Analyze logs
- Find infection source
- Check persistence

### Containment

- Quarantine system
- Monitor other endpoints

### Eradication

- Remove malware
- Delete malicious files
- Apply patches

### Recovery

- Restore from backup
- Validate system

### Prevention

- Use EDR/XDR
- Enable MFA
- Train users
- Restrict unknown files
- Improve detection rules


## Final Summary

- EDR protects endpoints
- XDR provides wider visibility
- Together they improve detection and response

Key Takeaway:

Endpoint security is critical. Combining EDR and XDR helps detect and stop advanced cyber attacks effectively.

# Author 
Adithya Raj K R
