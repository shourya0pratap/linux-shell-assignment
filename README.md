# 🐧 Linux Shell Assignment

## 📘 Project Overview
This repository contains three functional **Bash scripts** that demonstrate essential Linux automation tasks.  
Each script follows good scripting practices, including:
- Clear comments and meaningful variable names  
- Proper logging and timestamping  
- Error handling for robustness  

These scripts were developed as part of **Task 3 – Shell Script Development**.

---

## 📂 Repository Contents

| File / Folder | Description |
|----------------|-------------|
| `/scripts/` | Folder containing all executable Bash scripts. |
| `backup.sh` | Creates a timestamped backup of a specified directory and logs the operation. |
| `monitoring.sh` | Monitors and logs CPU and memory usage at regular intervals. |
| `download.sh` | Downloads a file from the internet and stores it in a predefined directory. |
| `README.md` | Project documentation and usage instructions. |
| `/screenshots/` | Folder containing screenshots of the scripts being executed. |

---

## ⚙️ How to Run the Scripts

### 🧩 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/linux-shell-assignment.git
cd linux-shell-assignment
```

---

### 📝 2. Configure Paths
Each script uses specific directories (like `/home/shourya/backup` or `/home/shourya/downloads`).  
Before running, **update these paths** in the scripts to match your own username or desired directories.

Example:
```bash
download_dir="/home/<your-username>/downloads"
```

---

### 🧾 3. Make Scripts Executable
```bash
chmod +x scripts/backup.sh scripts/monitoring.sh scripts/download.sh
```

---

## 🚀 Script Descriptions

### 📦 a) Backup Script (`backup.sh`)
**Purpose:**  
Creates a timestamped backup of a specified directory and logs the result.

**Usage:**
```bash
./scripts/backup.sh <target_directory>
```

**Example:**
```bash
./scripts/backup.sh /home/shourya/documents
```

**Log Location:**  
`/home/<your-username>/backup/logs/log.txt`

---

### 💻 b) System Monitoring Script (`monitoring.sh`)
**Purpose:**  
Logs CPU and memory usage at regular intervals into a log file.

**Usage:**
```bash
./scripts/monitoring.sh
```

**Log Location:**  
`/home/<your-username>/monitoring_logs/sys_monitoring.log`

**Default Interval:** 5 seconds  
Press `Ctrl + C` to stop logging.

---

### 🌐 c) Automated Download Script (`download.sh`)
**Purpose:**  
Downloads a file from a given URL and stores it in a predefined directory.

**Usage:**
```bash
./scripts/download.sh <file_url>
```

**Example:**
```bash
./scripts/download.sh https://example.com/file.zip
```

**Download Location:**  
`/home/<your-username>/downloads`

**Log File:**  
`/home/<your-username>/downloads/download_log.txt`

---

## 🖼️ Screenshots

Includes screenshots of each script running successfully in the `/screenshots/` folder.

---

## 📁 Folder structure:
```
linux-shell-assignment/
├── scripts/
│   ├── backup.sh
│   ├── monitoring.sh
│   └── download.sh
├── screenshots/
│   ├── backup_output.png
│   ├── monitoring_output.png
│   └── download_output.png
└── README.md
```
## 🧠 Notes
- Make sure `wget`, `curl`, and `top` commands are installed.  
- Adjust directory paths before execution.  
- Tested successfully on Ubuntu 22.04.  

## 👨‍💻 Author
Name: Shourya Pratap  
Date: 11 November 2025  
Course/Task: Linux Shell Scripting Assignment – Task 3