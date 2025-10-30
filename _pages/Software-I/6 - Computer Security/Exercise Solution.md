---
layout: satellite
title: "Exercise Solutions - Computer Security"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, Computer Security]
tags: [computer security, exercise solutions, cybersecurity practice, information systems]
---

# Exercise Solutions: Computer Security

## Multiple Choice Questions

### 1. Which of the following is NOT a component of Information Systems?
a) Hardware
b) Software
c) Telecommunications
d) Entertainment

**Answer: d) Entertainment**

**Explanation:** The five components of Information Systems are Hardware, Software, Telecommunications, Data, and Human Resources. Entertainment is not considered a core component of information systems.

### 2. A person who uses their computer skills to gain unauthorized access to systems for malicious purposes is called:
a) Hacker
b) Cracker
c) Security Expert
d) System Administrator

**Answer: b) Cracker**

**Explanation:** A cracker is someone who breaks into computer systems with malicious intent, while a hacker typically refers to someone who uses their skills ethically to improve security.

### 3. A weakness or flaw in a system that can be exploited by threats is called:
a) Risk
b) Attack Vector
c) Vulnerability
d) Threat

**Answer: c) Vulnerability**

**Explanation:** A vulnerability is a weakness or flaw in a system that can be exploited. Risk is the potential for loss, threat is a potential danger, and attack vector is the method used to exploit vulnerabilities.

### 4. Which security tool is primarily used to control network traffic in and out of a system?
a) Antivirus
b) Firewall
c) Encryption
d) Backup

**Answer: b) Firewall**

**Explanation:** A firewall is specifically designed to control and filter network traffic based on predetermined security rules, while antivirus deals with malicious software detection.

### 5. The process of creating copies of data for protection against loss is called:
a) Encryption
b) Authentication
c) Backup
d) Decryption

**Answer: c) Backup**

**Explanation:** Backup is the process of creating copies of data to protect against loss due to hardware failure, corruption, or security incidents.

## Short Answer Questions

### 1. Define Computer Security.

**Answer:**
Computer Security refers to the protection of standalone computers and individual systems. It focuses on safeguarding software, hardware, and data on single machines from various threats including malware, unauthorized access, and physical damage. Computer security deals primarily with local threats and vulnerabilities that affect individual computing devices.

### 2. Differentiate between Computer Security and Cyber Security.

**Answer:**

| Aspect | Computer Security | Cyber Security |
|--------|------------------|----------------|
| **Scope** | Standalone computers and individual systems | Networked systems and interconnected devices |
| **Focus** | Protection of software, hardware, and data on single machines | Protection of intercommunication between systems |
| **Threats** | Local threats and vulnerabilities | Network-based threats and distributed attacks |
| **Protection** | Individual system protection | Network and distributed system protection |

### 3. Define threats, attack vectors, and vulnerability.

**Answer:**

**Threat:** A potential danger or harmful event that could cause damage to a system. Threats can be natural disasters, human actions, or technical failures. They are external factors that could cause harm to information systems.

**Attack Vector:** A path or method used by attackers to gain unauthorized access to a computer or network. Common attack vectors include email attachments, malicious websites, USB devices, network vulnerabilities, and social engineering.

**Vulnerability:** A weakness or flaw in a system that can be exploited by threats. Vulnerabilities are internal factors that create security gaps and can include software bugs, configuration errors, or design flaws.

### 4. What are Information Systems?

**Answer:**
Information Systems are integrated combinations of hardware, software, networks, and people that organizations use to collect, filter, process, create, and distribute information. They include various types such as:

- **Data Warehouses:** Large repositories for analytical processing
- **Enterprise Systems:** Integrated organizational software applications
- **Expert Systems:** AI-based decision support systems
- **Geographic Information Systems (GIS):** Spatial data management systems
- **Office Automation Systems:** Software tools for common office tasks

### 5. Describe Information System Assets.

**Answer:**
Information System assets are the five core components that make up any information system:

1. **Hardware:** Physical components including processors, memory, storage devices, and input/output devices
2. **Software:** Programs and applications including operating systems, applications, and utilities
3. **Telecommunications:** Networks and communication infrastructure enabling data transmission
4. **Data:** Raw facts, figures, and information that must be organized, stored, and protected
5. **Human Resources:** People who use, manage, and maintain the systems including end users, administrators, and developers

### 6. Define hacker, cracker, and security expert.

**Answer:**

**Hacker:** A security professional who uses their technical skills ethically to improve security, find vulnerabilities, and protect systems. Hackers work within legal boundaries, often performing authorized penetration testing and security research.

**Cracker:** An individual who breaks into computer systems maliciously with the intent to steal data, cause damage, or gain unauthorized access for personal gain. Crackers engage in illegal activities and criminal behavior.

**Security Expert:** A trained professional specializing in information security who designs, implements, and maintains security measures. Security experts have formal education, certifications, and work legitimately to protect organizational assets.

## Extended Questions

### 7. Define confidentiality, integrity, and authenticity.

**Answer:**

**Confidentiality:**
- Ensures information is accessible only to authorized individuals
- Protects sensitive data from unauthorized disclosure
- Implemented through encryption, access controls, and data classification
- Prevents unauthorized viewing or copying of sensitive information

**Integrity:**
- Ensures information remains accurate, complete, and unaltered
- Protects against unauthorized modification or corruption
- Maintained through checksums, digital signatures, and version control
- Guarantees data has not been tampered with during storage or transmission

**Authenticity (Authentication):**
- Verifies the identity of users, devices, or systems
- Ensures only legitimate entities gain access to resources
- Implemented through passwords, biometrics, certificates, and multi-factor authentication
- Confirms that users are who they claim to be before granting access

### 8. Describe Encryption and Decryption.

**Answer:**

**Encryption:**
- The process of converting readable data (plaintext) into an unreadable format (ciphertext)
- Uses mathematical algorithms and encryption keys to scramble information
- Protects confidentiality of sensitive data during storage and transmission
- Makes data unintelligible to unauthorized individuals
- Common algorithms include AES, RSA, and DES

**Decryption:**
- The process of converting encrypted data (ciphertext) back to readable format (plaintext)
- Requires the proper decryption key and algorithm
- Restores access to original information for authorized users
- Must be performed by legitimate recipients with correct credentials

**Practical Implementation:**
- Windows 10 provides built-in encryption through EFS (Encrypting File System)
- Files can be encrypted by selecting Properties → Advanced → "Encrypt contents to secure data"
- Encrypted files are automatically decrypted when accessed by the authorized user
- Green color indicator shows encrypted files in Windows Explorer

### 9. Describe Malware.

**Answer:**

Malware (malicious software) refers to any software designed to harm, exploit, or gain unauthorized access to computer systems. Common types include:

**Viruses:**
- Malicious programs that replicate themselves by attaching to other files
- Spread when infected files are shared or executed
- Can corrupt, delete, or steal data from infected systems

**Worms:**
- Self-replicating malware that spreads across networks automatically
- Don't need to attach to other files to propagate
- Can consume network bandwidth and system resources

**Keyloggers:**
- Software or hardware that secretly records keystrokes
- Can capture passwords, credit card numbers, and sensitive information
- Often used for identity theft and unauthorized access

**Botnets:**
- Networks of infected computers controlled remotely by attackers
- Infected machines called "zombies" or "bots"
- Used for coordinated attacks, spam distribution, or cryptocurrency mining

**Trojans:**
- Malware disguised as legitimate software
- Create backdoors for unauthorized access
- Often used to steal personal information or install additional malware

### 10. Differentiate between Firewall and Anti-virus.

**Answer:**

| Aspect | Firewall | Anti-virus |
|--------|----------|------------|
| **Primary Purpose** | Controls network traffic in and out of system | Detects and removes malicious software |
| **Protection Type** | Network-based protection | File-based protection |
| **Function** | Filters packets based on predetermined rules | Scans files and monitors system behavior |
| **Threats Addressed** | Unauthorized network access, intrusion attempts | Viruses, worms, trojans, spyware, malware |
| **Operation Mode** | Real-time traffic monitoring and filtering | Reactive and proactive scanning |
| **Implementation** | Network perimeter or host-based | Endpoint protection on individual systems |
| **Configuration** | Rules for ports, protocols, applications | Scanning schedules, quarantine settings |
| **Focus Area** | Network communication security | File and system integrity |

**Complementary Protection:**
- Both are essential for comprehensive security
- Firewall provides first line of defense against network threats
- Anti-virus provides protection against file-based malware
- Together they create layered security architecture

## Practical Tasks

### 1. Install Antimalware Software on Windows

**Step-by-Step Process:**

1. **Download Software:**
   - Visit official website of reputable antimalware vendor
   - Download latest version compatible with your Windows version
   - Verify download integrity using checksums if provided

2. **Prepare for Installation:**
   - Close all running applications
   - Disable any existing antimalware temporarily
   - Ensure administrator privileges

3. **Run Installation:**
   - Right-click installer and select "Run as administrator"
   - Follow setup wizard instructions
   - Accept license agreement terms

4. **Configure Settings:**
   - Enable real-time protection
   - Configure automatic updates
   - Set scanning preferences
   - Choose notification settings

5. **Complete Setup:**
   - Restart computer if prompted
   - Verify installation success
   - Perform initial system scan

### 2. Perform Malware Scan on Windows

**Scanning Process:**

1. **Access Antimalware Program:**
   - Open installed antimalware software
   - Navigate to scanning options

2. **Choose Scan Type:**
   - **Quick Scan:** Checks commonly infected areas (faster)
   - **Full Scan:** Examines entire system thoroughly (comprehensive)
   - **Custom Scan:** User-selected files and folders (targeted)

3. **Initiate Scan:**
   - Click scan button to start process
   - Monitor progress and status
   - Allow scan to complete without interruption

4. **Review Results:**
   - Check scan summary for threats found
   - Review quarantined items
   - Take recommended actions

5. **Post-Scan Actions:**
   - Remove or quarantine detected threats
   - Update virus definitions
   - Schedule regular automated scans

### 3. Install and Configure Firewall on Windows

**Installation and Configuration:**

1. **Access Firewall Settings:**
   - Open Control Panel → System and Security
   - Click "Windows Defender Firewall"
   - Or Settings → Update & Security → Windows Security → Firewall

2. **Enable Firewall:**
   - Turn on firewall for different network profiles:
     - Domain networks (workplace)
     - Private networks (home)
     - Public networks (public Wi-Fi)

3. **Configure Advanced Settings:**
   - Click "Advanced settings" for detailed configuration
   - Set inbound and outbound rules
   - Configure notifications and logging

4. **Create Custom Rules:**
   - Add specific application rules
   - Configure port exceptions
   - Set protocol restrictions

5. **Test Configuration:**
   - Use online port scanners to verify protection
   - Test application connectivity
   - Verify rules are working correctly

### 4. Configure Firewall to Create Log Files

**Logging Configuration:**

1. **Access Advanced Firewall Settings:**
   - Open Windows Defender Firewall with Advanced Security
   - Right-click "Windows Defender Firewall" in left pane

2. **Configure Logging:**
   - Select "Properties" from context menu
   - Click on each profile tab (Domain, Private, Public)
   - Click "Customize" in Logging section

3. **Set Log Parameters:**
   - **Log file location:** Choose secure directory
   - **Maximum file size:** Set appropriate limit (default 4096 KB)
   - **Log dropped packets:** Enable for security monitoring
   - **Log successful connections:** Enable for audit trail

4. **Apply Settings:**
   - Click OK to save logging configuration
   - Verify log file creation in specified location

5. **Monitor Logs:**
   - Regularly review log files for suspicious activity
   - Use log analysis tools for pattern detection
   - Investigate unusual connection attempts

### 5. Perform System Restore on Windows

**System Restore Process:**

1. **Access System Restore:**
   - Type "Create a restore point" in Start menu search
   - Click "System Protection" tab
   - Click "System Restore" button

2. **Choose Restore Point:**
   - Select "Recommended restore" for most recent
   - Or "Choose a different restore point" for specific date
   - Review restore point description and date

3. **Confirm Restore:**
   - Review programs and drivers that will be affected
   - Ensure important data is backed up
   - Click "Finish" to start restore process

4. **Complete Restoration:**
   - System will restart automatically
   - Restoration process may take 15-30 minutes
   - Do not interrupt the process

5. **Verify Restoration:**
   - Check that system issues are resolved
   - Verify critical applications still function
   - Re-install any programs if necessary

---

*These exercise solutions provide practical knowledge for implementing basic computer security measures in Windows environments.*