# NETWORKWALKS-OLANITE B084-WEEK-1-CYBERSECURITY-LAB-SETUP

**NetworkWalks Cybersecurity Training — Week 1 Assignment**

**Project:** Cybersecurity Lab Setup Using Kali Linux and Oracle VirtualBox

## 📌 Project Overview

This project focuses on setting up a **virtual cybersecurity laboratory setup** using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

---

## 🎯 Objectives

The main objectives of this project are to:

- Install and configure VirtualBox.
- Install/import Kali Linux as a virtual machine.
- Create a private **NAT Network** for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.


---

## ⚙️ Lab Configuration

| 🧩 Component       | ⚙️ Configuration   |
| ------------------ | ------------------  |
| 🖥️ Host OS         | Windows 11 Pro         |
| 🧠 Host RAM        | 16 GB               |
| ⚡ Processor       | Intel Core i5      |
| 🧰 Hypervisor      | VirtualBox 7.2  |
| 🐉 Security OS     | Kali Linux 2026.2  |
| 🧠 Kali RAM        | 2048 MB            |
| 🌐 Virtual Network | NAT Network        |
| 📡 Network Address | 10.0.0.0/24        |
| 🐧 Kali IP Address | 10.0.0.2/24        |
| 🚪 Default Gateway | 10.0.0.1           |
| 🌍 DNS Server      | 1.1.1.1            |
|    Shared Folder   | /download

---

# 🪜 Lab Setup Procedure

**Step 1: Oracle VirtualBox Installation**

Installed Oracle VirtualBox on the Windows host computer.

**Step 2: Kali Linux Installation**

Downloaded the preconfigured Kali Linux 2026.3 VirtualBox image, extracted the files, and registered the virtual machine in VirtualBox Manager.

**Step 3: NAT Network Configuration**

Created a NAT Network named CyberLab-NAT using subnet 10.0.0.0/24, with DHCP disabled.

**Step 4: Static IP Configuration**

Configured Kali Linux with static IP address 10.0.0.2/24, default gateway 10.0.0.1, and DNS servers.

**Step 5: Internet Connectivity Verification**

Successfully tested connectivity using ping commands to 1.1.1.1 and google.com.

**Step 6: Shared Folder Configuration**

Configured the Windows folder C:\CyberLab\Downloads to be accessible within Kali Linux at /downloads.

Successfully verified file transfer in both directions.

**Step 7: Clipboard and Drag-and-Drop**

Enabled bidirectional clipboard and drag-and-drop in VirtualBox.

Bidirectional clipboard functionality was successfully verified.

Windows-to-Kali drag-and-drop worked, but Kali-to-Windows drag-and-drop remained unsuccessful despite troubleshooting.

**Step 8: Recovery Snapshot**

Created a VirtualBox snapshot to preserve the working lab configuration before updating Guest Additions.

## 4. Challenges Encountered

Read-Only Filesystem Issue

During static IP configuration, Kali Linux returned a read-only filesystem error that prevented NetworkManager from saving the configuration.

The filesystem was successfully restored to read/write mode, allowing the network configuration to be completed.

VirtualBox Drag-and-Drop Issue

Guest-to-host drag-and-drop failed with VERR_TIMEOUT and VERR_IPE_UNINITIALIZED_STATUS errors.

Troubleshooting included updating Guest Additions, restarting VBoxClient, verifying the X11/XFCE session, and checking kernel modules.

The issue remains unresolved. However, bidirectional file transfer through the shared folder works successfully.

## 5. Verification Results

**Requirement & Result**

VirtualBox installation - Passed
Kali Linux installation - Passed
NAT Network configuration - Passed
Static IP configuration - Passed
Internet connectivity - Passed
Shared folder access - Passed
Bidirectional file transfer - Passed
Bidirectional clipboard - Passed
Windows-to-Kali drag-and-drop - Passed
Kali-to-Windows drag-and-drop - Unresolved

## 6. Lessons Learned

This assignment strengthened my practical understanding of:

- Virtualization using Oracle VirtualBox.
- Kali Linux installation and administration.
- NAT networking and static IP configuration.
- Linux filesystem troubleshooting.
- VirtualBox Guest Additions.
- Shared-folder configuration and file transfers.
- Troubleshooting virtualization integration issues.

---

# 🔗 Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)

---

# 👤 Author

**Waqas Karim**\
Cybersecurity Professional B082

LinkedIn: [https://www.linkedin.com/in/waqaskarim/](https://www.linkedin.com/in/waqaskarim/)

---

## 📌 Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 01 | **Project:** Cybersecurity & Pentesting Lab Setup | **Repository:** GitHub
