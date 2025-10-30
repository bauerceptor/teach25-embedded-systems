---
layout: satellite
title: "Chapter Notes - Operating Systems"
date: 2024-01-15
author: "Course Material"
categories: [Software-I, Operating Systems]
tags: [OS, system software, application software, firmware, Linux, Windows]
---

# Chapter Notes: Operating Systems

## Learning Objectives

By the end of this chapter, students will be able to:
- Distinguish between system software and application software
- Understand the functions and abstractions of operating systems
- Explain the role of firmware in computer systems
- Navigate both Linux and Windows operating environments
- Perform basic file operations using command line interfaces
- Install and manage operating systems including virtualization
- Compare different types of software updates and upgrades

---

## 2.1 System Software vs Application Software

### What is Software?

Software is a set of instructions or programs that tell a computer to perform specific tasks. It is a generic term that describes computer programs, scripts, applications, and sets of instructions that make computers functional and useful.

Software can be classified into two main categories based on the programming language used for development and the platform required for execution:

### System Software

**Definition:** System software acts as an interface between application software and the computer system hardware.

**Key Characteristics:**
- **Development Language:** Developed using low-level programming languages that are more compatible with system hardware
- **Purpose:** Controls and manages computer hardware operations
- **Installation:** Automatically installed when the operating system is installed
- **User Interaction:** Limited or no direct user interaction due to hardware-specific nature
- **Independence:** Can run independently and provides a platform for other software

**Examples:**
- Operating systems (Windows, Linux, macOS)
- Device drivers
- Compilers and assemblers
- Debuggers
- Firmware and BIOS

### Application Software

**Definition:** Application software runs on the platform provided by system software to perform specific user-requested tasks.

**Key Characteristics:**
- **Development Language:** Developed using high-level programming languages for specific purposes
- **Purpose:** Performs specific tasks requested by users
- **Installation:** Installed according to user requirements
- **User Interaction:** Provides user-friendly interfaces for direct interaction
- **Dependency:** Cannot run independently; requires system software to function

**Examples:**
- Word processors (Microsoft Word, LibreOffice Writer)
- Web browsers (Chrome, Firefox, Safari)
- Media players (VLC, Windows Media Player)
- Games and entertainment software
- Productivity applications

### Comparison Summary

| Aspect | System Software | Application Software |
|--------|----------------|---------------------|
| **Function** | Interface between hardware and applications | Performs specific user tasks |
| **Language** | Low-level languages | High-level languages |
| **Installation** | With operating system | User-specific requirements |
| **User Interface** | Minimal or none | User-friendly interfaces |
| **Independence** | Runs independently | Depends on system software |
| **Examples** | OS, drivers, compilers | Word processors, browsers, games |

---

## 2.2 Operating System Abstractions

### Definition and Purpose

An **Operating System (OS)** is a program that acts as an interface between computer users and computer hardware. It controls the execution of all types of programs and manages system resources efficiently.

The OS provides abstractions that hide the complexity of hardware from users and applications, making computers easier to use and program.

### 2.2.1 Functions of an Operating System

Modern operating systems perform nine essential functions:

#### 1. Memory Management

**Primary Responsibilities:**
- Tracks which parts of main memory are in use and by which processes
- Decides which processes receive memory allocation in multiprogramming environments
- Allocates memory when processes request it
- Deallocates memory when processes terminate or no longer need it

**Key Concepts:**
- Main memory consists of an array of words or bytes, each with a unique address
- Programs must be loaded into main memory for execution
- Efficient memory allocation prevents system crashes and ensures optimal performance

#### 2. Processor Management (Process Scheduling)

**Core Activities:**
- Maintains status information about all processes
- Uses a traffic controller program to track processor usage
- Allocates CPU time to processes based on scheduling algorithms
- Deallocates processor resources when processes complete

**Process Scheduling:** Determines which process gets the processor, when, and for how long in multiprogramming environments.

#### 3. Device Management

**Device Control Functions:**
- Manages communication with all hardware devices through device drivers
- Maintains device status through I/O controller programs
- Allocates devices efficiently to requesting processes
- Handles device conflicts and ensures proper resource sharing
- Deallocates devices when no longer needed

#### 4. File Management

**File System Operations:**
- Organizes files into directories for easy navigation
- Tracks file information, location, usage, and status
- Controls file access permissions and security
- Manages file allocation and deallocation
- Provides file system hierarchy and organization

#### 5. Security

**Security Measures:**
- Implements password protection and authentication systems
- Prevents unauthorized access to programs and data
- Manages user accounts and permissions
- Monitors system access and logs security events
- Protects against malware and security threats

#### 6. Performance Monitoring

**System Performance:**
- Records response times between service requests and system responses
- Monitors resource utilization (CPU, memory, disk, network)
- Identifies performance bottlenecks
- Provides performance metrics and statistics
- Optimizes system efficiency

#### 7. Job Accounting

**Resource Tracking:**
- Monitors time and resources used by various jobs and users
- Tracks system usage for billing or administrative purposes
- Maintains logs of user activities
- Provides usage reports and statistics
- Manages resource quotas and limits

#### 8. Error Detection and Handling

**Error Management:**
- Produces system dumps for debugging
- Generates error traces and messages
- Provides debugging and diagnostic tools
- Handles system crashes and recovery
- Maintains system stability and reliability

#### 9. Software Coordination

**System Integration:**
- Coordinates compilers, interpreters, and assemblers
- Manages software installation and updates
- Assigns software resources to users
- Handles software compatibility issues
- Facilitates communication between different software components

### 2.2.2 Examples of Operating Systems

#### Linux Operating System

**Advantages:**
- **Free and Open Source:** No licensing costs, source code freely available
- **Customizable:** Can be modified to meet specific requirements
- **Secure:** Strong security features and regular security updates
- **Stable and Reliable:** Less prone to crashes and system failures
- **Performance:** Efficient resource utilization

**Disadvantages:**
- **Complexity:** Steeper learning curve for users without programming background
- **Software Compatibility:** Limited availability of some commercial software
- **Hardware Support:** May require additional effort for newer hardware

**Best Used For:** Servers, embedded systems, development environments, security-critical applications

#### Windows Operating System

**Advantages:**
- **User-Friendly:** Intuitive graphical interface
- **Software Compatibility:** Wide range of commercial software available
- **Hardware Support:** Excellent driver support for most hardware
- **Gaming:** Superior gaming platform with DirectX support
- **Business Integration:** Strong integration with Microsoft Office and enterprise tools

**Disadvantages:**
- **Cost:** Requires purchasing licenses
- **Security Vulnerabilities:** More frequent target for malware
- **Resource Usage:** Can be resource-intensive
- **Less Customizable:** Limited ability to modify core system components

**Best Used For:** Desktop computers, gaming, business applications, multimedia

---

## 2.3 Firmware

### Definition and Characteristics

**Firmware** is a tangible electronic component containing embedded software instructions that tell electronic devices how to operate. It serves as the lowest level of software that directly controls hardware components.

### Key Features of Firmware

#### Storage and Persistence
- Stored in **non-volatile memory** devices such as:
  - ROM (Read-Only Memory)
  - EPROM (Erasable Programmable ROM)
  - Flash memory
- Retains instructions even when power is turned off
- Permanent installation that rarely changes during device lifetime

#### Types and Functions

**Basic Firmware (BIOS Example):**
- Provides elementary basic functions for devices
- Offers services to higher-level software
- Contains minimal functionality for hardware initialization

**Complete System Firmware:**
- May be the only program running on embedded systems
- Provides all device functions and capabilities
- Common in consumer appliances, digital cameras, mobile phones

#### Firmware Updates

**Reasons for Updates:**
- Bug fixes and stability improvements
- Adding support for new hardware drivers
- Security patches and vulnerability fixes
- New feature implementation
- Performance optimizations

**Update Methods:**
- Physical ROM replacement (older systems)
- Flash memory reprogramming through special procedures
- Over-the-air (OTA) updates for modern devices

### BIOS (Basic Input/Output System)

**Historical Context:**
- First operating system was created by General Motors in 1956 for IBM computers
- IBM became the first manufacturer to develop and distribute operating systems in the 1960s

**BIOS Functionality:**
- Computer program embedded on motherboard chip
- Recognizes and controls various computer devices
- Performs hardware initialization during boot process
- Provides interface between operating system and hardware

---

## 2.4 Virtual Machines

### Definition and Purpose

A **Virtual Machine (VM)** is a software resource that uses software instead of physical computer hardware to run programs and deploy applications. Multiple virtual machines can run on a single physical host computer.

### Key Characteristics

#### Isolation and Independence
- Each VM runs its own operating system independently
- VMs function separately even when running on the same host
- Hardware resources are shared but logically separated
- Each VM appears as a complete computer system

#### Resource Management
- Host machine allocates physical resources to guest VMs
- Memory, CPU, storage, and network resources are virtualized
- Resource allocation can be adjusted based on needs
- Efficient utilization of underlying hardware

### Virtualization Benefits

**Cost Efficiency:**
- Reduces hardware requirements
- Lower power consumption
- Decreased physical space requirements
- Shared infrastructure costs

**Flexibility and Scalability:**
- Easy deployment of new systems
- Quick provisioning of resources
- Scalable infrastructure
- Simple backup and recovery

**Testing and Development:**
- Safe environment for testing software
- Multiple OS environments on single machine
- Easy system state snapshots
- Isolated development environments

---

## 2.5 Operating System Usage

Understanding how to effectively use operating systems is crucial for IoT development and system administration.

### 2.5.1 Linux Command Line Usage

Linux provides powerful command-line tools for system management and file operations.

#### Essential File Operations

**Copy Command (cp):**
```bash
cp <source> <destination>
```
- Copies files and directories
- Preserves original file
- Can copy multiple files simultaneously

**Move Command (mv):**
```bash
mv <source> <destination>
```
- Moves files and directories
- Also used for renaming files
- Original file is moved, not copied

**Rename Operation:**
```bash
mv <current_name> <new_name>
```

#### File and Directory Search

**Find Command Structure:**
```bash
find [options] [starting_path] [expression]
```

**Common Examples:**
- `find . -name "thisfile.txt"` - Search for specific file
- `find /home -name "*.jpg"` - Find all JPEG files
- `find . -type f -empty` - Locate empty files
- `find /home -user username -mtime 6 -iname "*.db"` - Complex search with multiple criteria

### 2.5.2 Windows Operating System Usage

Windows provides both graphical and command-line interfaces for system management.

#### System Customization

**Personalization Settings:**
- Right-click desktop → Select "Personalize"
- Customize wallpapers, themes, and colors
- Adjust display settings and scaling
- Configure start menu and taskbar

**Display Configuration:**
- Settings → System → Display
- Adjust text, apps, and item scaling
- Configure multiple monitor setups
- Set display resolution and orientation

#### File Management

**File Extensions:**
- Windows uses file extensions to identify file types
- Extensions determine associated applications
- Example: `.docx` files open with Microsoft Word
- Extensions can be hidden or shown in File Explorer

**Hidden Files and Folders:**
- Access through "Show hidden files and folders" option
- Hidden files use special attributes
- Can be shown or hidden through File Explorer options
- Protected system files require additional settings

#### System Management Tools

**Device Manager:**
- Central view of Windows-recognized hardware
- Manage device drivers and hardware conflicts
- Enable, disable, or update device drivers
- Troubleshoot hardware problems

**Task Manager:**
- Monitor system resource usage
- View running applications and processes
- End unresponsive programs
- Analyze system performance
- Access via Ctrl+Shift+Esc

**Command Prompt:**
- Command-line interface for Windows
- Access via Start → Run → "cmd"
- Execute system commands and utilities
- Manage files and directories from command line

---

## 2.6 Software Updates vs Upgrades

Understanding the difference between updates and upgrades is essential for system maintenance.

### Software Updates

**Definition:** Small changes to software that do not affect core structure.

**Characteristics:**
- **Size:** Usually small (kilobytes to megabytes)
- **Frequency:** Regular and frequent
- **Purpose:** Bug fixes, security patches, driver support
- **Installation Time:** Minutes to complete
- **Cost:** Typically free

**Examples:**
- Security patches
- Bug fixes
- Minor feature additions
- Driver updates
- Performance optimizations

### Software Upgrades

**Definition:** Significant and substantial changes to software including major new features.

**Characteristics:**
- **Size:** Large (can be gigabytes)
- **Frequency:** Less frequent, major releases
- **Purpose:** New features, GUI changes, major improvements
- **Installation Time:** Hours to complete
- **Cost:** May require purchase or subscription

**Examples:**
- Windows 7 to Windows 10 upgrade
- Ubuntu 16.04 to Ubuntu 18.04 upgrade
- Microsoft Office 2016 to Office 2019
- Major version releases

### Update and Upgrade Management

#### Windows Update Process
1. Settings → Update & Security → Windows Update
2. Check for available updates
3. Download and install automatically or manually
4. Restart system if required
5. Configure update settings and schedule

#### Linux Update Process (Ubuntu)
```bash
sudo apt update           # Update package lists
sudo apt upgrade          # Install available updates
sudo apt dist-upgrade     # System upgrade
sudo do-release-upgrade   # Major version upgrade
```

---

## Summary

Operating systems serve as the crucial interface between users, applications, and computer hardware. System software provides the foundation that enables application software to function effectively. Understanding the distinctions between different types of software, operating system functions, and proper system usage is essential for anyone working with computer systems, especially in IoT environments where diverse operating systems and embedded firmware play critical roles.

The knowledge of file operations, system management tools, and software maintenance practices enables efficient system administration and troubleshooting. Whether working with Linux command-line environments or Windows graphical interfaces, these fundamental concepts provide the groundwork for more advanced system administration and IoT development tasks.

Modern computing relies heavily on virtualization technologies that allow multiple operating systems to coexist on single hardware platforms, making efficient resource utilization and system testing possible. This foundation becomes particularly important when developing and deploying IoT solutions that may require various operating system environments.