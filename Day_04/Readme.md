# Day_04 - Administrative Commands, Networking & Ethical Hacking Stages

---

## 📌 Administrative Commands in Kali Linux

| Command | Description |
|---------|-------------|
| `whoami` | Displays the current user. |
| `hostname` | Shows the system's hostname. |
| `sudo su` | Switch to superuser (root). |
| `sudo useradd <username>` | Create a new user account. |
| `sudo passwd <username>` | Set password for the user. |
| `df -h` | Shows disk space usage in human-readable format. |
| `du -sh <directory>` | Displays size of directory. |
| `htop` | Interactive system-monitor process viewer. |

---

## 📌 Kali Linux Firewall - `ufw`

- **ufw (Uncomplicated Firewall)**: Simple interface for managing firewall rules.
- Can be used to allow/deny traffic on certain ports.

---

## 📌 Google DNS & Ping

- **Google DNS**: `8.8.8.8` (Public DNS server).
- Use `ping 8.8.8.8` to check internet connectivity or latency.
- DNS servers resolve domain names into IP addresses.

---

## 📌 DNS Server Concept

- DNS server stores an index page (list) mapping domain names to their IP addresses.
- Acts like the phonebook of the internet.

---

## 📌 IP & Network Interfaces

### `ifconfig` Command

- Shows network interface configuration.
- Displays IP address, MAC address, and interface status.

### Network Adapters

- **Docker Adapter**: Virtual network for Docker containers.
- **NAT (Network Address Translation)**: Allows multiple devices to share a single public IP.

### Ethernet Adapter

- Often shown as `eth0` (or `enoX`) in Linux.
- Handles physical wired network connections.

---

## 📌 IP Versions

- **IPv4**: 32-bit address, e.g., `192.168.0.1`
- **IPv6**: 128-bit address, e.g., `2001:0db8:85a3::8a2e:0370:7334`
- **Localhost IP**:
  - IPv4: `127.0.0.1`
  - IPv6: `::1`

### Localhost Concept

- Refers to the local machine.
- Commonly used for testing servers and services locally.

---

## 📌 Flipper Zero (FlipperO)

- Multi-functional portable cybersecurity tool.
- Can interact with RFID, NFC, Bluetooth, IR, and other wireless protocols.
- Used for ethical hacking, penetration testing, and hardware research.

---

## 📌 Ethical Hacking Stages

### 1️⃣ Reconnaissance
- Information gathering about target.
- Includes passive and active scanning.

### 2️⃣ Scanning / Enumeration
- Identifying open ports, services, and vulnerabilities.
- Tools: Nmap, Nessus, etc.

### 3️⃣ Penetration Testing
- Exploiting vulnerabilities to assess security posture.

### 4️⃣ SOC (Security Operations Center)
- Monitors and manages security events 24/7.
- Detects, analyzes, and responds to cybersecurity incidents.

---

