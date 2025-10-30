---
layout: satellite
title: "Exercise Solutions - Operating Systems"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, Operating Systems]
tags: [OS, system software, application software, firmware, Linux, Windows]
---

# Exercise Solutions: Operating Systems

## Part A: Multiple Choice Questions

### 1. Windows is a
**Answer: a) Operating Systems**

**Explanation:** Windows is primarily an operating system that manages computer hardware and provides services for application software. While it contains firmware-like components, its main classification is as an operating system.

### 2. VMware is a
**Answer: c) Application Software**

**Explanation:** VMware is virtualization application software that runs on top of an operating system to create and manage virtual machines. It is not an operating system itself but rather software that enables virtualization.

### 3. Which of the following OS is open source?
**Answer: a) Linux**

**Explanation:** Linux is an open-source operating system where the source code is freely available and can be modified. Windows and MS-DOS are proprietary closed-source operating systems.

### 4. cp command is used to
**Answer: b) copy files**

**Explanation:** The cp command in Linux stands for "copy" and is used to copy files and directories from one location to another while preserving the original file.

### 5. mv command is used to
**Answer: a) move files**

**Explanation:** The mv command in Linux stands for "move" and is used to move files and directories from one location to another. It can also be used for renaming files.

## Part B: Short Answer Questions

### 1. Define Software.

**Answer:** Software is a set of instructions or programs that tell a computer to perform specific tasks. It is a generic term used to describe computer programs, including scripts, applications, and sets of instructions that make computers functional and useful. Software can be classified into system software and application software based on their function and purpose.

### 2. Differentiate between applications software and system software?

**Answer:**

| Aspect | System Software | Application Software |
|--------|----------------|---------------------|
| **Definition** | Interface between application software and hardware | Software that runs as per user request |
| **Development Language** | Low-level languages compatible with hardware | High-level languages for specific purposes |
| **Usage** | Controls and operates computer hardware | Performs specific user tasks |
| **Installation** | Installed with operating system | Installed according to user requirements |
| **User Interaction** | Minimal or no direct user interaction | User-friendly interfaces for interaction |
| **Dependency** | Runs independently, provides platform for others | Depends on system software to function |
| **Examples** | OS, compilers, debuggers, drivers | Word processors, web browsers, games |

### 3. Describe functionalities of an operating system.

**Answer:** An operating system performs nine essential functions:

1. **Memory Management:** Tracks memory usage, allocates memory to processes, and deallocates when no longer needed
2. **Processor Management:** Schedules processes, allocates CPU time, and manages process execution
3. **Device Management:** Controls hardware devices through drivers and manages device allocation
4. **File Management:** Organizes files in directories, manages file access, and controls file operations
5. **Security:** Implements password protection and prevents unauthorized access to data
6. **Performance Monitoring:** Records system response times and monitors resource utilization
7. **Job Accounting:** Tracks time and resources used by various processes and users
8. **Error Detection:** Produces debugging aids, error messages, and handles system failures
9. **Software Coordination:** Manages compilers, interpreters, and assigns software resources to users

### 4. Define Firmware.

**Answer:** Firmware is a tangible electronic component containing embedded software instructions that tell electronic devices how to operate. It is stored in non-volatile memory devices such as ROM, EPROM, or flash memory. Firmware provides the control program for devices and is typically permanent, rarely changing during the device's economic lifetime. Examples include BIOS in computers, software in embedded systems like traffic lights, and control programs in consumer appliances.

### 5. Define Virtual Machine.

**Answer:** A Virtual Machine (VM) is a software resource that uses software instead of physical computer hardware to run programs and deploy applications. One or more virtual machines can run on a single physical host computer, with each VM running its own operating system independently. VMs function separately from each other even when running on the same host, allowing for efficient resource utilization and isolated computing environments.

### 6. Define Task Manager.

**Answer:** Task Manager is a powerful Windows tool that provides information about system resource usage and running processes. It displays detailed statistics about each process, monitors CPU, memory, disk, and network usage, and allows users to manage running applications. Task Manager can be used to end unresponsive programs, monitor system performance, and analyze resource consumption by different applications and services.

### 7. Describe command prompt and its usage.

**Answer:** Command Prompt is a command-line interface for Windows operating systems that allows users to interact with the system through text commands. 

**Access Methods:**
- Click Start → Search/Run → type "cmd" → press Enter
- Use keyboard shortcut Windows+R → type "cmd"

**Usage:**
- List directory contents using commands like "dir"
- Navigate directories using "cd" command
- Run application programs directly
- Perform file operations (copy, move, delete)
- Execute system utilities and administrative tasks
- Automate tasks through batch scripts

### 8. What is the purpose of Device Manager in Windows?

**Answer:** Device Manager serves several important purposes in Windows:

**Primary Functions:**
- Provides an organized, central view of all Windows-recognized hardware attached to the computer
- Lists hardware devices by categories (keyboards, hard drives, USB devices, etc.)
- Monitors device status and immediately notifies users of malfunctions
- Enables users to control devices (enable, disable, configure)
- Manages device drivers and identifies conflicts between devices

**Capabilities:**
- Update device drivers automatically or manually
- Troubleshoot hardware problems and conflicts
- View detailed device properties and specifications
- Install new hardware and remove obsolete devices
- Configure device settings and resources

### 9. Differentiate Update and Upgrade.

**Answer:**

| Aspect | Update | Upgrade |
|--------|--------|---------|
| **Definition** | Small changes that do not affect core structure | Significant and substantial changes to software |
| **Size** | Small (kilobytes to megabytes) | Large (can be gigabytes) |
| **Frequency** | Regular and frequent | Less frequent, major releases |
| **Purpose** | Bug fixes, security patches, minor improvements | New features, GUI changes, major functionality |
| **Installation Time** | Minutes to complete | Hours to complete |
| **Cost** | Usually free | May require purchase or subscription |
| **Examples** | Security patches, driver updates, bug fixes | Windows 7 to Windows 10, Office 2016 to 2019 |
| **Impact** | Maintains existing functionality with improvements | Introduces new capabilities and features |

## Part C: Practical Task Solutions

### 1. Install Windows 10 on the given PC.

**Solution Steps:**

**Preparation:**
1. Create installation media using Microsoft's Media Creation Tool
2. Download Windows 10 ISO and create bootable USB drive
3. Ensure minimum system requirements are met
4. Backup important data if upgrading existing system

**Installation Process:**
1. Insert bootable USB and restart computer
2. Access BIOS/UEFI (usually F2, F12, or Delete key)
3. Set USB as first boot device in boot order
4. Save BIOS settings and restart
5. Follow Windows installation wizard:
   - Select language and region
   - Enter product key or skip for later activation
   - Accept license terms
   - Choose installation type (custom for clean install)
   - Select hard drive partition
   - Wait for installation to complete (may restart multiple times)
6. Complete initial setup:
   - Create user account
   - Configure privacy settings
   - Connect to network
   - Install updates

### 2. Replace Windows Installation with Ubuntu Installation.

**Solution Steps:**

**Preparation:**
1. Download Ubuntu ISO from official website
2. Create bootable USB using tools like Rufus or Balena Etcher
3. Backup important Windows data to external storage
4. Note down WiFi passwords and important settings

**Installation Process:**
1. Boot from Ubuntu USB drive
2. Select "Install Ubuntu" from welcome screen
3. Choose keyboard layout and language
4. Select "Normal installation" or "Minimal installation"
5. Choose "Erase disk and install Ubuntu" to replace Windows
6. Confirm disk changes (this will delete Windows)
7. Select timezone and location
8. Create user account with strong password
9. Complete installation and restart system
10. Remove USB drive when prompted
11. Configure system after first boot:
    - Update software packages
    - Install additional drivers if needed
    - Restore backed-up data

### 3. Install Ubuntu on VMware Workstation.

**Solution Steps:**

**VMware Setup:**
1. Install VMware Workstation on host system
2. Launch VMware and select "Create a New Virtual Machine"
3. Choose "Typical (recommended)" configuration
4. Select "Installer disc image file (iso)" and browse to Ubuntu ISO
5. Configure virtual machine settings:
   - Name and location for VM
   - Disk size (minimum 20GB recommended)
   - Memory allocation (minimum 2GB recommended)
   - Network adapter settings

**Ubuntu Installation in VM:**
1. Power on virtual machine
2. Ubuntu installer will start automatically
3. Follow standard Ubuntu installation process:
   - Select language and keyboard
   - Choose "Erase disk and install Ubuntu" (safe in VM)
   - Create user account
   - Complete installation
4. Install VMware Tools for better integration:
   - VM menu → Install VMware Tools
   - Mount tools disc in Ubuntu
   - Run installation script
   - Restart virtual machine

### 4. Use Command Prompt to copy the contents of a file into another file.

**Solution Steps:**

**Method 1: Using COPY command**
```cmd
copy source_file.txt destination_file.txt
```

**Method 2: Using XCOPY command (for directories)**
```cmd
xcopy source_folder destination_folder /E /I
```

**Step-by-step Process:**
1. Open Command Prompt (Start → Run → cmd)
2. Navigate to the directory containing source file:
   ```cmd
   cd C:\path\to\source\directory
   ```
3. Use copy command to duplicate file:
   ```cmd
   copy original.txt copy_of_original.txt
   ```
4. Verify copy was successful:
   ```cmd
   dir
   ```

**Advanced Options:**
- Copy with verification: `copy /V source.txt dest.txt`
- Copy and overwrite: `copy /Y source.txt dest.txt`
- Copy multiple files: `copy *.txt backup_folder\`

### 5. Uninstall an application program from Windows using Control Panel.

**Solution Steps:**

**Method 1: Control Panel**
1. Open Control Panel:
   - Start → Control Panel
   - Or Windows+R → "appwiz.cpl"
2. Select "Programs and Features" or "Uninstall a program"
3. Find the application in the list
4. Right-click and select "Uninstall" or double-click
5. Follow uninstall wizard prompts
6. Restart computer if prompted

**Method 2: Settings App (Windows 10)**
1. Open Settings (Windows+I)
2. Go to Apps → Apps & features
3. Find the application in the list
4. Click on the app and select "Uninstall"
5. Confirm uninstallation
6. Follow any additional prompts

**Method 3: Application's Own Uninstaller**
1. Check Start Menu for application's uninstall option
2. Navigate to application installation folder
3. Look for uninstall.exe or similar file
4. Run uninstaller as administrator
5. Follow prompts to complete removal

### 6. Upgrade Windows 7 to Windows 10 and make sure to keep all programs and data.

**Solution Steps:**

**Preparation:**
1. Check system compatibility for Windows 10
2. Backup important data to external storage
3. Note down software license keys
4. Ensure stable internet connection
5. Free up disk space (minimum 16GB for 32-bit, 32GB for 64-bit)

**In-Place Upgrade Process:**
1. Download Windows 10 Media Creation Tool from Microsoft
2. Run the tool and select "Upgrade this PC now"
3. Accept license terms
4. Choose "Keep personal files and apps" option
5. Wait for download and preparation (depends on internet speed)
6. Follow installation prompts:
   - Click "Install" when ready
   - Select "Keep personal files and apps" when asked what to keep
7. Wait for upgrade process (may restart several times)
8. Complete initial Windows 10 setup:
   - Sign in with existing account
   - Configure privacy settings
   - Verify all programs and data are intact

**Post-Upgrade Verification:**
1. Check that all programs still work correctly
2. Verify personal files are accessible
3. Update device drivers if necessary
4. Run Windows Update to get latest patches
5. Activate Windows 10 (should activate automatically)

**Troubleshooting Tips:**
- If upgrade fails, check Windows Update troubleshooter
- Temporarily disable antivirus during upgrade
- Remove unnecessary programs before upgrading
- Use Windows 10 compatibility checker for older software

---

*These solutions provide comprehensive guidance for completing all practical tasks while ensuring proper system configuration and data preservation.*