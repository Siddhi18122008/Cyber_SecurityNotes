# 📅 Day_07 - Nmap Implementation, Ports, Vulnerability Tools & Exploit Search

---

## 🔎 Implementation of Nmap

> Nmap is widely used for network scanning and vulnerability assessment.

### 🔧 Basic Nmap Command Example:

```bash
nmap <target-ip>
```

### 🔬 Useful Nmap Commands for Implementation:

- Scan all ports:

```bash
nmap -p- <target-ip>
```

- Service and version detection:

```bash
nmap -sV <target-ip>
```

- OS detection:

```bash
nmap -O <target-ip>
```

- Aggressive scan (includes version detection, OS detection, and script scanning):

```bash
nmap -A <target-ip>
```

---

## 🔢 Ports & Paths for Data Transfer

- Ports are logical connection points for data transmission in networking.
- Each service listens on specific ports:

| Port Number | Service |
|-------------|---------|
| 80 | HTTP (Web Traffic) |
| 443 | HTTPS (Secure Web Traffic) |
| 8080 | Apache Tomcat (HTTP alternate) |
| 22 | SSH (Secure Shell for remote access) |

- Ports enable data to be sent/received to the right application.

---

## 🌐 Wiki: TCP vs UDP

| Protocol | Description | Features |
|----------|-------------|----------|
| TCP | Transmission Control Protocol | Connection-oriented, reliable, guarantees delivery, slower |
| UDP | User Datagram Protocol | Connectionless, faster, may lose packets, suitable for streaming |

- **Bind Port Numbers**: Ports where applications listen for incoming data.
- Example: Wikipedia typically operates on ports 80 (HTTP) and 443 (HTTPS).

---

## 🛠️ Tools & Platforms

### ✅ Jira
- A project management tool widely used for issue tracking, bug tracking, and team collaboration.
- Often used in software development and security teams.

### ✅ SSH (Secure Shell Connection)
- Allows secure remote login to Linux systems.

```bash
ssh user@hostname
```

- Uses port `22`.

### ✅ Mousepad
- Lightweight text editor in Kali Linux.
- GUI-based simple editor for quick file editing.

```bash
mousepad filename.txt
```

### ✅ Searchsploit
- Local exploit database search tool (uses Exploit-DB database).
- Helps in quickly finding known vulnerabilities and exploits for specific software.

```bash
searchsploit <software-name>
```

- Update exploit database:

```bash
searchsploit -u
```

---

## 🌐 Vulnerability Finding Platforms

### 🔍 Shodan.io
- Search engine for Internet-connected devices.
- Can discover IP leaks, exposed devices, vulnerable services.

### 🔍 ZoomEye.ai
- Similar to Shodan.
- Provides deeper scanning of global internet-connected assets.

---
