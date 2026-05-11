# Onion Reconnaissance Tool

A professional automated reconnaissance framework designed for performing passive and light active enumeration against `.onion` services through the Tor network.

Built for cybersecurity researchers, VAPT analysts, bug bounty hunters, and ethical hackers using Kali Linux.

---

## 🚀 Features

✔ Automated Tor verification  
✔ HTTP header collection  
✔ Technology fingerprinting using WhatWeb  
✔ robots.txt extraction  
✔ HTML source collection  
✔ HTML comment extraction  
✔ JavaScript file discovery  
✔ Light directory enumeration  
✔ Organized output saving  
✔ Clean terminal logging  
✔ Lightweight and fast execution  

---

## 📸 Overview

The Onion Reconnaissance Tool performs basic intelligence gathering against Tor hidden services while routing all traffic through the Tor network using `torsocks`.

The tool automatically:

- Validates `.onion` targets
- Starts Tor service
- Verifies Tor connectivity
- Collects reconnaissance artifacts
- Saves all findings into organized output folders

This tool is useful during:

- VAPT assessments
- Dark web investigations
- Threat intelligence
- Bug bounty reconnaissance
- OSINT operations
- Red team activities

---

## ⚙️ Technologies Used

- Node.js
- Tor
- Torsocks
- Curl
- WhatWeb
- Linux CLI Utilities

---

# 📂 Project Structure

```bash
Onion-Reconnaissance-Tool/
│
├── recon.js
├── README.md
│
└── output_target.onion/
    ├── headers.txt
    ├── whatweb.txt
    ├── robots.txt
    ├── index.html
    ├── html_comments.txt
    ├── javascript_files.txt
    ├── directories.txt
    └── tor_check.html
# =========================================================
# 🕵️ Onion Reconnaissance Tool - Full Installation Process
# Platform : Kali Linux
# Author   : Jagadish A
# =========================================================
INSTALLATION 
# ---------------------------------------------------------
# 1️⃣ Update System
# ---------------------------------------------------------

sudo apt update && sudo apt upgrade -y


# ---------------------------------------------------------
# 2️⃣ Install Node.js & NPM
# ---------------------------------------------------------

sudo apt install nodejs npm -y


# ---------------------------------------------------------
# 3️⃣ Verify Node.js Installation
# ---------------------------------------------------------

node -v
npm -v


# ---------------------------------------------------------
# 4️⃣ Install Required Reconnaissance Dependencies
# ---------------------------------------------------------

sudo apt install tor torsocks curl whatweb grep gawk sed -y


# ---------------------------------------------------------
# 5️⃣ Start Tor Service
# ---------------------------------------------------------

sudo systemctl start tor


# ---------------------------------------------------------
# 6️⃣ Enable Tor Service on Boot
# ---------------------------------------------------------

sudo systemctl enable tor


# ---------------------------------------------------------
# 7️⃣ Verify Tor Service Status
# ---------------------------------------------------------

sudo systemctl status tor


# ---------------------------------------------------------
# 8️⃣ Clone Repository
# ---------------------------------------------------------

git clone https://github.com/yourusername/onion-reconnaissance-tool.git


# ---------------------------------------------------------
# 9️⃣ Move Into Project Directory
# ---------------------------------------------------------

cd onion-reconnaissance-tool


# ---------------------------------------------------------
# 🔟 Verify Required Tools
# ---------------------------------------------------------

which tor
which torsocks
which curl
which whatweb
which grep
which awk
which sed


# ---------------------------------------------------------
# 1️⃣1️⃣ Run the Reconnaissance Tool
# ---------------------------------------------------------

node recon.js


# ---------------------------------------------------------
# 1️⃣2️⃣ Example Usage
# ---------------------------------------------------------

# After running:
# Enter target .onion domain:

examplehiddenservice.onion


# ---------------------------------------------------------
# 1️⃣3️⃣ Output Example
# ---------------------------------------------------------

# Results will be saved inside:

output_examplehiddenservice.onion/


# ---------------------------------------------------------
# 📂GENERATED FILES
# ---------------------------------------------------------

# headers.txt
# whatweb.txt
# robots.txt
# index.html
# html_comments.txt
# javascript_files.txt
# directories.txt
# tor_check.html


# ---------------------------------------------------------
# ⚠️ TROUBLESHOOTING
# ---------------------------------------------------------

# If Tor is not running:

sudo service tor restart


# If WhatWeb is missing:

sudo apt install whatweb -y


# If permission denied:

chmod +x recon.js


# ---------------------------------------------------------
# 🔒 Recommended Environment
# ---------------------------------------------------------

# OS        : Kali Linux
# Runtime   : Node.js 18+
# RAM       : 4GB+
# Network   : Stable Internet + Tor Connectivity


# ---------------------------------------------------------
# ✅ Tool Ready
# ---------------------------------------------------------
