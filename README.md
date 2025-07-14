# TermiTools: A GUI-Based Linux System Administration Tool

TermiTools is a lightweight, beginner-friendly GUI system administration tool designed for Linux (Ubuntu/Kali) users. Built with **Bash scripting** and **Zenity**, it helps simplify essential system monitoring and maintenance tasks — without the need to memorize or type terminal commands.

## 🎯 Project Objective

To develop a user-friendly graphical interface tool for Linux users to perform key administrative tasks easily, such as:

- Viewing logged-in users
- Checking disk usage and system uptime
- Monitoring firewall status
- Listing running services
- Performing quick network scans

All actions are logged for later reference and displayed in popup dialogs using Zenity.

---

## 🛠️ Features

- 📋 **Graphical Menu Interface** using Zenity
- 🔍 **View Logged-in Users**
- 💽 **Check Disk Usage**
- ⏳ **System Uptime Monitoring**
- 🔐 **Firewall Status (UFW)**
- ⚙️ **List Running Services (systemctl)**
- 🌐 **Quick Network Scan (Nmap)**
- 🧾 **Auto Logging** to a log file
- 🧒 **Beginner Friendly** - No CLI expertise required

---

## 🧰 Technologies Used

| Tool/Technology | Purpose |
|-----------------|---------|
| Bash (Shell Scripting) | Core logic and task execution |
| Zenity | GUI dialog boxes and menus |
| UFW | Firewall status checking |
| Nmap | Quick local network scanning |
| Systemctl | Service monitoring |
| Logger | Saves outputs to a log file |
| GNU/Linux (Ubuntu/Kali) | Compatible platforms |

---

## 📦 Installation & Setup

### 1. Install Zenity (if not already installed)
```bash
sudo apt install zenity
```

### 2. Download the Script
Clone or download the `termitool-gui.sh` script to your Linux machine.

### 3. Make the Script Executable
```bash
chmod +x termitool-gui.sh
```

### 4. Run the Tool
```bash
./termitool-gui.sh
```

A dropdown menu will appear with various system tasks you can execute via GUI.

---

## 📂 Script Overview

```bash
# Sample menu option in the script
"Disk Usage")
  df -h | tee -a "$LOGFILE" | zenity --text-info --title="Disk Usage" --width=500 --height=300
;;
```

- Uses `zenity --list` to display task options.
- Every result is:
  - Displayed in a pop-up window
  - Appended to a `.log` file (`$HOME/termitoolplus_gui.log`)

---

## 🚀 Demo

🌐 [Live GUI Web Preview](https://scintillating-pudding-b1599d.netlify.app/)

---

## 📄 Deliverables

- ✅ Bash script with Zenity GUI
- ✅ Functional system monitoring tool
- ✅ Log file generation
- ✅ Project Documentation (DOCX, PPTX)

---

## 🧠 Author & Guide

**Presented by:**  
👤 Praveen Kumar  
📚 Course: Cyber Security – Teks Academy  

**Guided by:**  
🎓 Udutha Shashidhar (Cyber Security Trainer)

---

## ✅ Conclusion

TermiTools bridges the gap between complex Linux commands and user-friendly interaction. Whether you're a student, beginner, or casual Linux user, TermiTools provides an efficient way to manage your system without touching the terminal.

---

> ✨ *"TermiTools makes Linux simple, visual, and accessible."*