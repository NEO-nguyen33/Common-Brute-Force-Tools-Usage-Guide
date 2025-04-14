# Common-Brute-Force-Tools-Usage-Guide

> ⚠️ **DISCLAIMER:** This guide is for ethical hacking and educational purposes only.  
> Use these tools only in authorized environments.

---

## 🧰 Top Brute-Force Tools

| Tool      | Protocols Supported              | Use Case                            |
|-----------|----------------------------------|--------------------------------------|
| **Hydra** | FTP, SSH, HTTP, SMB, Telnet, etc | Fast multi-protocol brute-forcing   |
| **Medusa**| FTP, SSH, RDP, VNC, SMB, etc     | High-performance parallel brute-force |
| **Ncrack**| SSH, RDP, VNC, FTP, etc          | Built by Nmap team for reliability   |
| **John the Ripper** | Offline password cracking | Hashes from /etc/shadow, dumped DBs |
| **Hashcat**| GPU-accelerated hash cracking   | Very fast with dictionaries/rules    |

---

## 🐍 1. Hydra (Very Popular)

### 🔑 Brute-force SSH:

```bash
hydra -l root -P /usr/share/wordlists/rockyou.txt ssh://192.168.1.105
