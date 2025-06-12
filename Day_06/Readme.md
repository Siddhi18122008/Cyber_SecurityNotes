# 📅 Day_06 - Docker, Nmap, IP Tracking & Tools

---

## 🐳 Introduction to Docker

- Docker is a containerization platform that allows you to package applications along with all dependencies into isolated containers.
- Provides lightweight, portable, and consistent environments across multiple systems.
- Widely used in cybersecurity labs to deploy vulnerable environments for practice.

### 🔧 Install Docker in Kali Linux

```bash
sudo apt update
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker
docker --version
```

### 🗑️ Remove Docker Image

```bash
docker rmi <image_id>
```

- Used to delete Docker images.

### ⚠️ Docker Vulnerable Versions

- Older or intentionally vulnerable Docker images are often used in ethical hacking labs to practice exploiting weaknesses.

---

## 🖥️ Virtualization Stack Setup

| Level | Component |
|-------|-----------|
| Physical Host | Windows OS |
| Virtualization Software | VirtualBox / VMware Workstation |
| Virtual Machine | Kali Linux |
| Inside Kali Linux | Docker Containers |

---

## 🔎 Nmap - Network Scanner

> Nmap is a powerful tool used for network discovery, security auditing, and vulnerability scanning.

### 📖 Basic Syntax

```bash
nmap [Scan Type(s)] [Options] {target specification}
```

### 🎯 Target Specification Examples

- Single IP: `192.168.0.1`
- IP Range: `10.0.0.0-255.1-254`
- Domain: `scanme.nmap.org`
- Input file: `-iL <filename>`

### 🚀 Host Discovery

| Option | Description |
|--------|-------------|
| -sL | List Scan - list targets |
| -sn | Ping Scan - no port scan |
| -Pn | Skip host discovery |

### 🛠️ Scan Techniques

| Option | Description |
|--------|-------------|
| -sS | TCP SYN Scan |
| -sT | TCP Connect Scan |
| -sU | UDP Scan |
| -sA | ACK Scan |
| -sW | Window Scan |

### 🎯 Port Scanning Options

```bash
-p <ports>  # Specific ports
-p-         # All ports
--exclude-ports <range>  # Exclude ports
```

### 🔍 Service & Version Detection

```bash
-sV
```

- Probe open ports to determine service/version info.

### 🕵️ Script Scanning

```bash
--script=default
--script=<script-name>
--script-args
```

### ⏱️ Timing and Performance

```bash
-T<0-5>  # Set timing template (5 is fastest)
```

### 📄 Output Formats

| Option | Description |
|--------|-------------|
| -oN | Normal output |
| -oX | XML output |
| -oG | Grepable output |

### 🎯 Miscellaneous

- `-O` : OS detection.
- `-A` : Aggressive scan (OS detection, version detection, script scanning, and traceroute).

---

## 🌍 MaxMind Installation & IP Tracking

> MaxMind is used for IP Geolocation — tracking approximate physical locations of IP addresses.

### 🔐 MaxMind Setup

1️⃣ Register on [MaxMind.com](https://www.maxmind.com/).  
2️⃣ Get a license key.  
3️⃣ Install GeoIP tools on Kali:

```bash
sudo apt install geoipupdate
```

4️⃣ Update geolocation database using your license key.

### 📍 MaxMind Usage

- Determine:
  - Country
  - City
  - ISP
  - ASN (Autonomous System Number)
  - Organization
- Helps in cyber investigations, log analysis, and attacker attribution.

---

## 💬 Discord Download

- Used for:
  - Joining cybersecurity communities.
  - Interacting with fellow ethical hackers.
  - Sharing knowledge, queries, and tools.

---
