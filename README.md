# L0ue Security & Pentesting Toolkit 🔓🛡️

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Termux](https://img.shields.io/badge/platform-Termux-black)
![Version](https://img.shields.io/badge/version-2.0-blue)

Professional security testing & penetration toolkit optimized for **Termux on Android**.

**Author:** L0ue James  
**Platform:** Termux (Android)  
**Last Updated:** 2026-05-02

---

## 🎯 Features

✅ **Network Security**
- Advanced nmap scanning & enumeration
- WiFi penetration testing (aircrack-ng)
- Network packet analysis (tcpdump, Wireshark)
- DNS enumeration & subdomain discovery

✅ **Web Application Security**
- SQLi/XSS vulnerability testing (sqlmap)
- Burp Suite integration
- Web server fingerprinting
- JavaScript deobfuscation tools

✅ **Password & Cryptography**
- Dictionary attacks (Hydra, John the Ripper)
- Hash cracking & identification
- Password generation & analysis
- Wordlist management

✅ **Exploitation & Post-Exploitation**
- Metasploit Framework
- Payload generation
- Reverse shell handlers
- Privilege escalation tools

✅ **Reconnaissance**
- OSINT automation
- Shodan API integration
- Google dorking templates
- Email verification tools

✅ **Custom Tools**
- L0ue ASCII menu system
- Automated scanning scripts
- Custom payloads database
- Logging & reporting system

---

## 📁 Project Structure

```
L0ue-Security-Toolkit/
├── README.md                    # This file
├── INSTALL.md                   # Installation guide
├── QUICKSTART.md                # Quick start guide
├── LICENSE                      # MIT License
│
├── toolkit/                      # Main toolkit directory
│   ├── menu.sh                  # L0ue interactive menu
│   ├── setup.sh                 # Auto-setup script
│   ├── config.sh                # Configuration settings
│   └── utils.sh                 # Utility functions
│
├── modules/                      # Organized security modules
│   ├── networking/              # Network tools
│   │   ├── nmap-scanner.sh
│   │   ├── wifi-pentesting.sh
│   │   ├── packet-sniffer.sh
│   │   ├── port-enumeration.sh
│   │   └── README.md
│   │
│   ├── web-app/                 # Web application testing
│   │   ├── sqlmap-automate.sh
│   │   ├── burp-proxy.sh
│   │   ├── http-scanner.sh
│   │   ├── ssl-tester.sh
│   │   └── README.md
│   │
│   ├── password-cracking/       # Password & hash tools
│   │   ├── hydra-launcher.sh
│   │   ├── john-cracker.sh
│   │   ├── hash-identifier.sh
│   │   ├── wordlist-manager.sh
│   │   └── README.md
│   │
│   ├── exploitation/            # Exploit & post-exploit
│   │   ├── metasploit-handler.sh
│   │   ├── payload-generator.sh
│   │   ├── revshell-builder.sh
│   │   ├── privilege-escalation.sh
│   │   └── README.md
│   │
│   ├── reconnaissance/          # OSINT & recon
│   │   ├── osint-automator.sh
│   │   ├── subdomain-finder.sh
│   │   ├── email-verification.sh
│   │   ├── shodan-search.sh
│   │   └── README.md
│   │
│   └── utilities/               # Helper utilities
│       ├── port-translator.sh
│       ├── ip-calculator.sh
│       ├── base64-encoder.sh
│       └── README.md
│
├── wordlists/                   # Password dictionaries & payloads
│   ├── common-passwords.txt
│   ├── sql-payloads.txt
│   ├── xss-payloads.txt
│   ├── command-injection.txt
│   ├── lfi-payloads.txt
│   └── README.md
│
├── templates/                   # Command & script templates
│   ├── nmap-templates.sh
│   ├── sqlmap-templates.sh
│   ├── hydra-templates.sh
│   ├── metasploit-templates.sh
│   └── README.md
│
├── payloads/                    # Custom exploit payloads
│   ├── reverse-shells/
│   ├── webshells/
│   ├── dropper-scripts/
│   └── README.md
│
├── reports/                     # Scan reports & findings
│   ├── .gitkeep
│   └── README.md
│
└── docs/                        # Documentation
    ├── INSTALL.md               # Installation instructions
    ├── QUICKSTART.md            # Quick start guide
    ├── TOOLS-GUIDE.md           # Individual tool guides
    ├── SCANNING-TECHNIQUES.md   # Methodology docs
    ├── WIFI-PENTESTING.md       # WiFi testing guide
    └── TROUBLESHOOTING.md       # Common issues & fixes
```

---

## 🚀 Quick Start

### **1. Install Toolkit**
```bash
git clone https://github.com/louejames/L0ue-Security-Toolkit.git
cd L0ue-Security-Toolkit
chmod +x toolkit/*.sh
bash toolkit/setup.sh
```

### **2. Run Main Menu**
```bash
bash toolkit/menu.sh
```

### **3. Select Module**
```
╔════════════════════════════════════════╗
║   L0ue Security & Pentesting Toolkit   ║
║              v2.0                      ║
╠════════════════════════════════════════╣
║ 1) 🌐 Network Scanning                 ║
║ 2) 🕸️  Web Application Testing          ║
║ 3) 🔑 Password Cracking                ║
║ 4) 💣 Exploitation Tools               ║
║ 5) 🔍 OSINT & Reconnaissance           ║
║ 6) ⚙️  Utilities & Helpers              ║
║ 7) 📊 Scan Reports                     ║
║ 0) ❌ Exit                              ║
╚════════════════════════════════════════╝
```

---

## 📦 Required Tools

**Auto-installed by `setup.sh`:**

```bash
# Networking
nmap, netcat, tcpdump, aircrack-ng, mdk3

# Web Application
sqlmap, nikto, whatweb, curl, wget

# Password Cracking
hydra, john, hashcat, hashid

# Exploitation
metasploit-framework, msfconsole, msfvenom

# OSINT
whois, dig, nslookup, curl, jq

# Utilities
git, vim, htop, tree, zip, unzip
```

---

## 🔐 Security Features

✅ **Input Validation** - All scripts validate user input  
✅ **Logging** - Full activity logging to `/logs/` directory  
✅ **Error Handling** - Graceful error messages & recovery  
✅ **Help System** - Built-in help for every command  
✅ **Configuration** - Customizable settings in `config.sh`  

---

## 📋 Usage Examples

### **Network Scanning**
```bash
bash modules/networking/nmap-scanner.sh 192.168.1.0/24
```

### **WiFi Penetration Testing**
```bash
bash modules/networking/wifi-pentesting.sh
```

### **SQL Injection Testing**
```bash
bash modules/web-app/sqlmap-automate.sh "http://target.com"
```

### **Password Cracking**
```bash
bash modules/password-cracking/hydra-launcher.sh
# Interactive menu for target selection
```

### **Generate Reverse Shell**
```bash
bash modules/exploitation/revshell-builder.sh
# Choose payload type & LHOST:LPORT
```

### **OSINT Automation**
```bash
bash modules/reconnaissance/osint-automator.sh example.com
```

---

## 🔧 Configuration

Edit `toolkit/config.sh` to customize:

```bash
# Colors & styling
COLOR_PRIMARY="#00ffff"
COLOR_SUCCESS="#00ff00"
COLOR_ERROR="#ff006e"

# Default paths
WORDLIST_PATH="$HOME/.config/wordlists"
PAYLOADS_PATH="$HOME/.config/payloads"
LOGS_PATH="$HOME/.logs"

# Tool options
NMAP_ARGS="-sV -sC -O"
HYDRA_THREADS=16
METASPLOIT_HANDLER_LHOST="192.168.1.x"
```

---

## 📚 Documentation

- **[INSTALL.md](docs/INSTALL.md)** - Detailed installation guide
- **[QUICKSTART.md](docs/QUICKSTART.md)** - Beginner's guide
- **[TOOLS-GUIDE.md](docs/TOOLS-GUIDE.md)** - Individual tool documentation
- **[SCANNING-TECHNIQUES.md](docs/SCANNING-TECHNIQUES.md)** - Methodology & best practices
- **[WIFI-PENTESTING.md](docs/WIFI-PENTESTING.md)** - WiFi hacking guide
- **[TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md)** - Common issues & fixes

---

## ⚠️ Legal Disclaimer

**THIS TOOLKIT IS FOR AUTHORIZED SECURITY TESTING ONLY!**

- ✅ Use only on systems you own or have explicit written permission to test
- ✅ Unauthorized access to computer systems is ILLEGAL
- ✅ Follow local, state, and federal laws
- ✅ The author assumes no liability for misuse

---

## 🤝 Contributing

Found a bug or have a tool suggestion?

1. Fork this repository
2. Create a feature branch: `git checkout -b feature/new-tool`
3. Commit changes: `git commit -m 'Add new tool'`
4. Push to branch: `git push origin feature/new-tool`
5. Open a Pull Request

---

## 📝 Changelog

### v2.0 (2026-05-02)
- ✨ Major refactor with modular structure
- 🎨 New L0ue ASCII menu system
- 📚 Comprehensive documentation
- 🔧 Auto-setup script
- 🚀 30+ security tools integrated

### v1.0 (2025-2026)
- Initial toolkit release
- Basic WiFi & network tools
- Metasploit integration

---

## 📞 Support & Contact

**Issues & Questions:** Open GitHub Issues  
**Twitter/X:** [@louejames](https://twitter.com/louejames)  
**Email:** contact@louejames.dev

---

## 📄 License

MIT License - See [LICENSE](LICENSE) file for details

```
Permission is hereby granted, free of charge, to any person obtaining
a copy of this software for authorized security testing purposes.
```

---

## 🙏 Acknowledgments

Built with ❤️ for the security research community.

Powered by:
- Termux development team
- Kali Linux foundation
- Open-source security tools authors

---

**🔥 L0ue Security Toolkit - Stay Secure, Stay Ethical! 🔒**
