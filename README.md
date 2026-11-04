# 🔐 Cybersecurity Lab Environment Setup

<p align="center">
  <strong>Networkwalks Cybersecurity Internship</strong><br>
  Week 1 – Project Module 1 (WK1-PM1)
</p>

---

## 📌 Project Overview

This project involves setting up a virtual cybersecurity testing laboratory using Oracle VirtualBox and Kali Linux.

The objective is to establish a virtual environment for practicing cybersecurity concepts, ethical hacking, network security, and penetration testing.

Kali Linux is configured as the attacking machine, while Oracle VirtualBox provides the virtualization platform and NAT Network infrastructure.

## 🎯 Project Objectives

- Install and configure Oracle VirtualBox.
- Download and import Kali Linux into VirtualBox.
- Create a NAT Network using the `10.0.0.0/24` subnet.
- Configure Kali Linux with the required static IP address.
- Enable shared clipboard and drag-and-drop functionality.
- Configure a shared folder between the host and virtual machine.
- Establish internet connectivity from Kali Linux.
- Verify network configuration using Linux commands.

## 🛠️ Tools and Technologies

| Tool | Description |
|---|---|
| Oracle VirtualBox | Virtualization platform |
| Kali Linux | Penetration testing operating system |
| NAT Network | Virtual networking |
| Windows | Host operating system |

## 🏗️ Lab Architecture

The laboratory uses the following network configuration:

```text
           Host Machine (Windows)
                    |
              Oracle VirtualBox
                    |
                NAT Network
              10.0.0.0/24
                    |
               Kali Linux
              Attacking Machine
                    |
               eth0 Interface
                    |
             Internet Access
```

## ⚙️ Network Configuration

The following configuration is specified in the project requirements:

| Component | Required Configuration |
|---|---|
| Network Mode | NAT Network |
| Network Name | NatNetwork |
| IPv4 Network | `10.0.0.0/24` |
| Kali Linux IP | `10.0.0.2/24` |
| Subnet Mask | `255.255.255.0` |
| Default Gateway | `10.0.0.1` |
| DNS Server | `8.8.8.8` |
| DHCP | Enabled on NAT Network |
| Internet Access | Required |

## 🚀 Implementation

### 1. Oracle VirtualBox Installation

Installed Oracle VirtualBox to create and manage virtual machines for the cybersecurity laboratory.

### 2. Kali Linux Installation

Downloaded and imported the Kali Linux virtual machine into Oracle VirtualBox.

Successfully started Kali Linux and accessed its desktop environment.

### 3. NAT Network Configuration

Created a NAT Network in VirtualBox with the following settings:

- Network Name: `NatNetwork`
- IPv4 Prefix: `10.0.0.0/24`
- DHCP Server: Enabled

**Screenshot:**

<img width="1534" height="820" alt="01" src="https://github.com/user-attachments/assets/936dfe72-3723-42a7-82fc-0606afe91e4a" />


### 4. Kali Linux Virtual Machine

Successfully launched Kali Linux inside Oracle VirtualBox.

**Screenshot:**

<img width="1506" height="714" alt="02" src="https://github.com/user-attachments/assets/15adc9b8-3c02-4ac6-bd55-1ea90e40d6f0" />


### 5. IPv4 Network Configuration

Configured the Kali Linux network connection with the intended network parameters:

- Target IP Address: `10.0.0.2`
- Netmask: `/24`
- Gateway: `10.0.0.1`
- DNS Server: `8.8.8.8`

**Screenshot:**

<img width="1366" height="698" alt="03" src="https://github.com/user-attachments/assets/9a7a9fb4-3c4f-4add-85d0-810e9f8a445e" />


### 6. Network Connectivity Verification

Used Linux networking commands to inspect the network interface, routing table, and internet connectivity.

**Commands executed:**

Check network interfaces:

```bash
ip addr
```

Check routing table:

```bash
ip route
```

Test internet connectivity:

```bash
ping -c 4 google.com
```

**Observed Results:**

| Parameter | Observed Result |
|---|---|
| Network Interface | `eth0` |
| IPv4 Address | `10.0.0.3/24` |
| Default Gateway | `10.0.0.1` |
| Network Subnet | `10.0.0.0/24` |
| Internet Connectivity | Successful |
| Packet Loss | 0% |

**Screenshot:**

<img width="1206" height="686" alt="04" src="https://github.com/user-attachments/assets/acd52f9d-9231-4932-99b4-3b2b7a28cff3" />



## 📁 Repository Structure

```text
NETWORKWALKS-TIN-MG-SOE-B084-WK1-PM1/
│
├── README.md
│
└── screenshots/
    ├── 01-nat-network.png
    ├── 02-kali-desktop.png
    ├── 03-kali-ipv4-settings.png
    └── 04-network-connectivity-test.png
```

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Virtualization using Oracle VirtualBox.
- Kali Linux installation and configuration.
- Virtual network creation and management.
- IPv4 addressing and subnetting.
- Linux network interface configuration.
- Default gateway and DNS configuration.
- Network connectivity testing and troubleshooting.

## 🔒 Ethical Considerations

This laboratory is intended strictly for educational purposes and authorized cybersecurity testing.

All penetration testing and security assessments will be performed only within controlled lab environments or on systems for which proper authorization has been obtained.

## 👨‍💻 Author

**Tin Mg Soe**

Cybersecurity Intern  
Networkwalks IT Solutions & Training

**Project:** WK1-PM1 – Cybersecurity Lab Environment Setup

---

*Building practical cybersecurity skills through hands-on learning and experimentation.*
