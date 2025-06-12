# 📅 Day_08 - Shodan, MaxMind Database, Vulnerability Scanning & Discord

---

## 🌐 Shodan - The Search Engine for Hackers

### 🔎 What is Shodan?
- Shodan is a search engine for Internet-connected devices.
- It scans and indexes open devices & services exposed on the internet.
- Often called: **Google for Hackers**.
- Can discover:
  - IP addresses
  - Ports
  - Running services
  - Vulnerabilities
  - Metadata of connected devices

### 🔑 Login Process
- Create an account at: [shodan.io](https://www.shodan.io/)
- Free and premium subscription available.
- Login gives extended scanning, advanced filters, API access.

### ⚠️ Vulnerabilities & Services

- Shodan lists exposed vulnerabilities (CVEs) on identified systems.
- Shows which services & ports are open.
- Examples:
  - HTTP (Port 80)
  - HTTPS (Port 443)
  - SSH (Port 22)
  - Apache Tomcat (Port 8080)
  - Hikvision cameras, IoT devices, servers, etc.

### 🎯 Working With Random IP Addresses
- Random IPs can be searched to analyze:
  - Services running
  - Vulnerabilities present
  - Multiple vulnerabilities across multiple open ports

### 🔍 Port Scanning

- Shodan performs global port scanning to gather service data.
- Port scanning helps identify:
  - Open ports
  - Service versions
  - Vulnerabilities mapped to specific ports

### 🐝 What is Honey Port?
- A **Honey Port** is a decoy port used in honeypots.
- When attackers connect to this port, it triggers alerts and logs their activity.
- Used to detect malicious scanning and attacks.

### 📸 What is Hikvision?
- Hikvision is a popular manufacturer of IP security cameras.
- Often exposed on the internet due to weak configurations.
- Common target for attackers searching for unsecured CCTV cameras.

---

## 🌍 MaxMind Geolocation Database

### 🔑 MaxMind Login & Account Summary

- Go to: [maxmind.com](https://www.maxmind.com/)
- Login → Navigate to **Account Summary** → **Download Database**

### 📥 Download Available Databases

- **GeoLite2 City**
- **GeoLite2 ASN (Autonomous System Numbers)**
- **GeoLite2 Country**

---

## 💻 Working With MaxMind Database Files in Kali Linux

### Step 1️⃣ : Identify File Type

- Downloaded files are compressed archives:
```bash
Geolite2.*.tar.gz
```

### Step 2️⃣ : Decompress using gunzip

```bash
gunzip Geolite2.*.tar.gz
```
- Output: `.tar` file

### Step 3️⃣ : Extract using tar

```bash
tar -xvf Geolite2.*.tar
```

- Extracts into directories containing `.mmdb` database files.

### Step 4️⃣ : View Directory Structure

```bash
tree
```

- Output will look something like:

```bash
.
├── GeoLite2-City_YYYYMMDD
│   ├── LICENSE.txt
│   ├── GeoLite2-City.mmdb
│   └── README.txt
├── GeoLite2-ASN_YYYYMMDD
│   ├── LICENSE.txt
│   ├── GeoLite2-ASN.mmdb
│   └── README.txt
├── GeoLite2-Country_YYYYMMDD
│   ├── LICENSE.txt
│   ├── GeoLite2-Country.mmdb
│   └── README.txt
```

(*Note: YYYYMMDD represents the date of the database release.*)

---

## 🔬 Vulnerability Scanning (Introduction)

- They demonstrated basic scanning using the downloaded MaxMind databases and scanning tools.

---

## 💬 Discord Invite

- An invite link was provided for the Discord server.
- Discord app was downloaded for communication and community discussions.

---

