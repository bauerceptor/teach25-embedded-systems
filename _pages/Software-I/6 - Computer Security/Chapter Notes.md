---
layout: satellite
title: "Chapter Notes - Computer Security"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, Computer Security]
tags: [computer security, cybersecurity, information systems, firewall, antivirus, encryption, backup]
---

# Chapter Notes: Computer Security

## 6.1 Computer Security and Cyber Security

### Computer Security vs Cyber Security

**Computer Security:**
- Focuses on protecting standalone computers and individual systems
- Covers protection of software, hardware, and data on single machines
- Deals with local threats and vulnerabilities

**Cyber Security:**
- Focuses on protecting networked systems and interconnected devices
- Covers protection of intercommunication between systems
- Deals with network-based threats and distributed attacks

### Common Security Threats

**Viruses:**
- Malicious programs that replicate themselves
- Attach to other files and spread when files are shared
- Can corrupt, delete, or steal data

**Worms:**
- Self-replicating malware that spreads across networks
- Don't need to attach to other files
- Can consume network bandwidth and system resources

**Keylogger:**
- Software or hardware that records keystrokes
- Can capture passwords, credit card numbers, and sensitive information
- Often used for identity theft

**Botnet:**
- Network of infected computers controlled remotely
- Used for coordinated attacks, spam distribution, or data theft
- Infected computers called "zombies" or "bots"

**Phishing:**
- Fraudulent attempts to obtain sensitive information
- Uses fake emails, websites, or messages
- Tricks users into revealing passwords or personal data

## 6.2 Information Systems

### Types of Information Systems

**Data Warehouses:**
- Large repositories of data from multiple sources
- Used for analytical processing and business intelligence
- Support decision-making through data analysis

**Enterprise Systems:**
- Integrated software applications for entire organizations
- Include ERP (Enterprise Resource Planning) systems
- Coordinate business processes across departments

**Expert Systems:**
- Computer programs that mimic human expert knowledge
- Use artificial intelligence to solve complex problems
- Provide recommendations based on rules and knowledge base

**Geographic Information Systems (GIS):**
- Systems for capturing, storing, and analyzing spatial data
- Used for mapping, location analysis, and geographic planning
- Important for urban planning, environmental monitoring

**Office Automation Systems:**
- Software tools for common office tasks
- Include word processing, spreadsheets, email, calendaring
- Improve productivity and communication in organizations

### 6.2.1 Components of Information Systems

**Hardware:**
- Physical components of computer systems
- Includes processors, memory, storage devices, input/output devices
- Foundation for running software and processing data

**Software:**
- Programs and applications that run on hardware
- Includes operating systems, applications, and utilities
- Provides functionality and user interfaces

**Telecommunications:**
- Networks and communication infrastructure
- Enables data transmission between systems
- Includes internet, LANs, WANs, wireless networks

**Data:**
- Raw facts, figures, and information
- Must be organized, stored, and protected
- Core asset of information systems

**Human Resources:**
- People who use, manage, and maintain systems
- Includes end users, system administrators, developers
- Critical for system success and security

## 6.3 Importance of Computer Security

### Attack Vector
An **attack vector** is a path or method used by attackers to gain unauthorized access to a computer or network. Common attack vectors include:
- Email attachments
- Malicious websites
- USB devices
- Network vulnerabilities
- Social engineering

## 6.4 Losses in case of Security Attacks

**Productivity Loss:**
- Downtime when systems are compromised
- Employee time spent dealing with security incidents
- Reduced efficiency during recovery

**Response Loss:**
- Costs of investigating security breaches
- Expenses for hiring security experts
- Resources spent on damage assessment

**Replacement Loss:**
- Cost of replacing damaged or compromised systems
- Expense of rebuilding corrupted data
- Investment in new security measures

**Fines and Judgments:**
- Legal penalties for data breaches
- Regulatory fines for non-compliance
- Lawsuit settlements with affected parties

**Reputation Damage:**
- Loss of customer trust and confidence
- Negative media coverage
- Long-term impact on business relationships

## 6.5 Difference between Hacker and Cracker

### Hacker
- **Definition:** Security professional who uses skills ethically
- **Purpose:** Improve security, find vulnerabilities, protect systems
- **Methods:** Authorized penetration testing, security research
- **Motivation:** Knowledge, improvement, protection
- **Legality:** Works within legal boundaries

### Cracker
- **Definition:** Individual who breaks into systems maliciously
- **Purpose:** Steal data, cause damage, financial gain
- **Methods:** Unauthorized access, exploitation, destruction
- **Motivation:** Personal gain, malicious intent
- **Legality:** Criminal activity, illegal actions

## 6.6 Features of a Secure System

### Risk vs Threat vs Vulnerability

**Risk:**
- Potential for loss or damage
- Combination of threat likelihood and impact
- Measured and managed through security controls

**Threat:**
- Potential danger or harmful event
- Can be natural disasters, human actions, or technical failures
- External factors that could cause harm

**Vulnerability:**
- Weakness or flaw in a system
- Can be exploited by threats
- Internal factors that create security gaps

### Security Principles

**Confidentiality:**
- Ensures information is accessible only to authorized individuals
- Protects sensitive data from unauthorized disclosure
- Implemented through encryption, access controls

**Integrity:**
- Ensures information remains accurate and unaltered
- Protects against unauthorized modification
- Maintained through checksums, digital signatures

**Availability:**
- Ensures systems and data are accessible when needed
- Protects against service disruptions
- Maintained through redundancy, backups

**Authentication:**
- Verifies the identity of users or systems
- Ensures only legitimate users gain access
- Implemented through passwords, biometrics, certificates

**Non-repudiation:**
- Prevents denial of actions or transactions
- Provides proof of origin and delivery
- Implemented through digital signatures, audit logs

**Accountability:**
- Tracks and records user actions
- Enables attribution of activities to specific individuals
- Maintained through logging, monitoring

## 6.7 Computer Protection

### Basic Protection Steps

1. **Install and Update Operating System**
   - Keep OS current with security patches
   - Enable automatic updates when possible

2. **Install Antimalware Software**
   - Choose reputable antivirus/anti-malware programs
   - Configure real-time protection

3. **Configure Firewall**
   - Enable built-in or install third-party firewall
   - Configure appropriate rules and policies

4. **Regular Backups**
   - Create copies of important data
   - Store backups in secure, separate locations

5. **User Education**
   - Train users on security best practices
   - Promote awareness of threats and risks

### 6.7.1 Antimalware vs Firewall

**Antimalware:**
- **Purpose:** Detects and removes malicious software
- **Function:** Scans files, monitors system behavior
- **Protection:** Against viruses, worms, trojans, spyware
- **Operation:** Reactive and proactive scanning

**Firewall:**
- **Purpose:** Controls network traffic in and out of system
- **Function:** Filters packets based on rules
- **Protection:** Against unauthorized network access
- **Operation:** Real-time traffic monitoring

**Selection Criteria:**
- Both are essential for comprehensive protection
- Antimalware for file-based threats
- Firewall for network-based threats
- Consider compatibility and resource usage

### 6.7.2 Installing an Antivirus Program

**Installation Process:**
1. **Download** reputable antivirus software from official website
2. **Run installer** with administrator privileges
3. **Follow setup wizard** and accept license terms
4. **Configure settings** for real-time protection
5. **Complete installation** and restart if required

**Updating the Antivirus Program:**
- Enable automatic updates for virus definitions
- Check for program updates regularly
- Ensure internet connection for update downloads
- Verify update success through program interface

**Performing a Scan:**
- **Quick Scan:** Checks commonly infected areas
- **Full Scan:** Examines entire system thoroughly
- **Custom Scan:** User-selected files and folders
- **Scheduled Scans:** Automatic regular scanning

## 6.8 Firewalls

### Top 10 Firewall Software
1. ZoneAlarm
2. Comodo Firewall
3. Windows Defender Firewall
4. Norton Smart Firewall
5. McAfee Firewall
6. Bitdefender Firewall
7. Kaspersky Internet Security
8. AVG Internet Security
9. Avast Firewall
10. ESET Internet Security

### Configuring a Firewall (5 Steps)

1. **Access Firewall Settings**
   - Open Control Panel or Settings
   - Navigate to Windows Defender Firewall

2. **Enable/Disable Firewall**
   - Turn on for different network profiles
   - Configure for domain, private, public networks

3. **Configure Rules**
   - Allow or block specific applications
   - Set port and protocol rules

4. **Set Notifications**
   - Configure alerts for blocked programs
   - Choose notification preferences

5. **Test Configuration**
   - Verify firewall is working properly
   - Test with network scanning tools

### Logging Services in Firewall

**Log Types:**
- Dropped packets (blocked connections)
- Successful connections (allowed traffic)
- Error events and system messages

**Log Configuration:**
- Enable logging for security monitoring
- Set log file location and size limits
- Configure log rotation policies

**Log Analysis:**
- Review logs regularly for suspicious activity
- Use log analysis tools for pattern detection
- Investigate unusual connection attempts

### Uses of Firewall

- **Network Traffic Control:** Filter incoming and outgoing traffic
- **Access Control:** Block unauthorized access attempts
- **Application Control:** Manage which programs can access network
- **Port Management:** Control which network ports are open
- **Intrusion Prevention:** Detect and block attack attempts

## 6.9 Encryption and Decryption

### Encryption Concepts

**Encryption:**
- Process of converting readable data into unreadable format
- Uses algorithms and keys to scramble information
- Protects confidentiality of sensitive data

**Decryption:**
- Process of converting encrypted data back to readable format
- Requires proper key and algorithm
- Restores access to original information

### Encrypting a File in Windows 10

**Using Built-in Encryption:**
1. **Right-click** on file or folder
2. **Select Properties** from context menu
3. **Click Advanced** button in Attributes section
4. **Check** "Encrypt contents to secure data"
5. **Apply changes** and confirm encryption

**Encryption Features:**
- Uses EFS (Encrypting File System)
- Tied to user account credentials
- Automatic encryption/decryption during use
- Green color indicator for encrypted files

## 6.10 Backup and Restoration

### Creating Backup of Windows

**Backup Methods:**
- **File History:** Automatic backup of user files
- **System Image:** Complete system backup
- **OneDrive Sync:** Cloud-based file backup

**Backup Process:**
1. **Open Settings** → Update & Security → Backup
2. **Add a drive** for backup storage
3. **Configure backup options** and frequency
4. **Start backup process**
5. **Verify backup completion**

### Restore Files with File History

**Restoration Process:**
1. **Open File History** from Control Panel
2. **Browse** through backup versions
3. **Select files** or folders to restore
4. **Choose restore location** (original or new)
5. **Complete restoration** process

**File History Features:**
- Automatic regular backups
- Version history maintenance
- Easy file recovery interface
- Integration with Windows Explorer

## Key Security Best Practices

### For Organizations
1. **Implement layered security** (defense in depth)
2. **Regular security training** for all employees
3. **Maintain updated inventory** of assets and systems
4. **Conduct regular security assessments**
5. **Develop incident response procedures**

### For Individual Users
1. **Use strong, unique passwords** for all accounts
2. **Enable two-factor authentication** where available
3. **Keep software updated** with latest patches
4. **Be cautious** with email attachments and links
5. **Regular backup** of important data

---

*This chapter provides fundamental knowledge of computer security principles and practical skills for implementing basic security measures in Windows environments.*