
# Cyber Security Internship Task 1: Scan Local Network for Open Ports

## 🔍 Objective:
To discover open ports on devices in the local network to understand network exposure.

## 🛠 Tools Used:
- Nmap (Free)
- Wireshark (Optional)

## 🧠 IP Range Used:
- `172.20.10.0/24`

## 🔧 Command Executed:
```bash
nmap -sS 172.20.10.0/24
```

## 📄 Sample Scan Result Summary:
- Device 1: 172.20.10.1 - Open Ports: 80 (HTTP), 443 (HTTPS)
- Device 2: 172.20.10.5 - Open Ports: 22 (SSH), 139 (NetBIOS)
- Device 3: 172.20.10.8 - Open Ports: 445 (SMB)

## 🔐 Security Risk Observations:
- Port 445 can expose systems to SMB-related vulnerabilities (e.g., EternalBlue).
- Port 22 should be restricted or use key-based authentication.
- Web ports (80/443) should be monitored for outdated web servers.

## 🛡 Recommendations:
- Close unused ports using firewall rules.
- Use secure protocols (e.g., SSH, HTTPS).
- Keep systems updated and patched regularly.

## 🧾 Output File:
Results are saved in `scan_results.txt`

---

## 📘 Interview Questions Answered:
Check `Interview_Questions.txt` for well-structured answers.
