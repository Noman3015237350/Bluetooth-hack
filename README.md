"""
README.md - Bluetooth Auto Jammer Tool
======================================

This script creates a comprehensive README.md file for the Bluetooth Auto Jammer tool.
"""

def generate_readme():
    readme_content = '''
# Bluetooth Auto Jammer 🔥

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Linux%2FTermux-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/Version-2.0-red.svg)

**A powerful Bluetooth denial-of-service attack tool for educational and testing purposes**

</div>

## 📖 Description

Bluetooth Auto Jammer is an advanced penetration testing tool designed to demonstrate Bluetooth security vulnerabilities. It can perform L2ping flood attacks on nearby Bluetooth devices, effectively disrupting their connectivity for security assessment purposes.

## ⚠️ Disclaimer

> **WARNING**: This tool is for **EDUCATIONAL PURPOSES ONLY**. 
> - Only use on devices you own or have explicit permission to test
> - Unauthorized use may be illegal in your country
> - The developers are not responsible for any misuse
> - Use responsibly and ethically

## 🛠️ Installation

### Prerequisites
- Python 3.8+
- Bluetooth adapter
- Linux or Termux (Android)

### Termux Installation
```bash
# Update packages
pkg update && pkg upgrade

# Install required tools
pkg install python
pkg install bluez-tools

# Clone repository (if available)
git clone https://github.com/Thakur2309/bluetooth-jammer.git
cd bluetooth-jammer

# Run the tool
python bluetooth_jammer.py
```

Linux Installation

```bash
# Install dependencies
sudo apt update
sudo apt install python3 bluez bluez-tools

# Run the tool
python3 bluetooth_jammer.py
```

🎯 Features

· ✅ Auto Device Scanning - Automatically discovers nearby Bluetooth devices
· ✅ L2ping Flood Attacks - Executes denial-of-service attacks
· ✅ Multi-Device Targeting - Can attack multiple devices simultaneously
· ✅ Single Target Mode - Focus on specific MAC addresses
· ✅ Admin Authentication - Secure access with admin key protection
· ✅ Cross-Platform - Works on Linux and Android Termux

📷 Screenshots

```
 _   _  ____  __  __    _    _   _  
| \\ | |/ __ \\|  \\/  |  / \\  | \\ | | 
|  \\| | |  | | \\  / | / _ \\ |  \\| | 
| . ` | |  | | |\\/| |/ ___ \\| . ` |
|_|\\_| \\____/|_|  |_/_/   \\_\\_|\\_|

                    NOMAN-ETHICAL-HACKER
```

🚀 Usage

1. Start the tool:
   ```bash
   python bluetooth_jammer.py
   ```
2. Admin Authentication:
   · Enter the admin key when prompted
   · Default key: NOMAN1
3. Scan for devices:
   · Tool will automatically scan for nearby Bluetooth devices
4. Choose attack mode:
   · Attack all discovered devices
   · Or target specific device by MAC address

🔧 Technical Details

Requirements

· hciconfig - Bluetooth configuration tool
· hcitool - Bluetooth scanning utility
· l2ping - L2CAP ping implementation
· Root access (for some operations)

Attack Method

The tool uses L2ping flood attacks:

```bash
l2ping -i hci0 -s 600 -f [MAC_ADDRESS]
```

👨‍💻 Admin Information

Admin Key: NOMAN1

Social Media Links:

· 📘 Facebook: https://www.facebook.com/md.norman.988
· 💬 WhatsApp Group: https://chat.whatsapp.com/L0Y71TSqNd55sFkwpIOMyH
· 📢 WhatsApp Channel: https://whatsapp.com/channel/0029VbAkW0SATRSeAAYjNv1Z

❓ Troubleshooting

Common Issues:

1. "hciconfig not found"
   ```bash
   pkg install bluez-tools  # Termux
   sudo apt install bluez   # Linux
   ```
2. "No Bluetooth devices found"
   · Ensure Bluetooth is enabled
   · Check if devices are in discoverable mode
   · Verify Bluetooth adapter is working
3. "Permission denied"
   ```bash
   # Grant necessary permissions
   sudo setcap cap_net_raw+eip $(which hciconfig)
   sudo setcap cap_net_raw+eip $(which hcitool)
   ```

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

🤝 Contributing

1. Fork the project
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

📞 Contact

Developer: Md Noman
YouTube: Movie world 
Email: [md3173505@gmail.com]

🙏 Acknowledgments

· Thanks to the open-source community
· Bluetooth protocol researchers
· Ethical hacking community

---

<div align="center">

⭐ Don't forget to star this repository if you find it useful!

🔔 Subscribe to our YouTube channel for more tutorials!

</div>
'''

def save_readme(filename="README.md"):
"""Save the README content to a file"""
content = generate_readme()
with open(filename, 'w', encoding='utf-8') as file:
file.write(content)
print(f"✅ README.md file generated successfully as '{filename}'")

def display_readme_preview():
"""Display a preview of the README content"""
content = generate_readme()
print("📋 README.md Preview:")
print("=" * 50)
lines = content.split('\n')
for i, line in enumerate(lines[:30]):  # Show first 30 lines as preview
print(line)
print("... [content truncated] ...")
print("=" * 50)

if name == "main":
# Display preview
display_readme_preview()

```

And here's a simpler version if you just want to create the file directly:

```python
# Simple README.md generator
def create_readme():
    content = '''# Bluetooth Auto Jammer 🔥

## Description
Advanced Bluetooth security testing tool for educational purposes only.

## Features
- Auto device scanning
- L2ping flood attacks  
- Multi-device targeting
- Admin authentication

## Installation
```bash
# Termux
pkg install python bluez-tools
python bluetooth_jammer.py

# Linux
sudo apt install python3 bluez bluez-tools
python3 bluetooth_jammer.py
```

Admin Info

Facebook: https://www.facebook.com/md.norman.988

Disclaimer

For educational purposes only. Use responsibly.
'''

Run to create README

create_readme()

```

**To use this code:**

1. **Save as Python file**: Save either code as `create_readme.py`
2. **Run the script**: 
   ```bash
   python create_readme.py
```

1. Customize: Edit the generated README.md file as needed

The README includes:

· Professional badges and header
· Detailed installation instructions
· Feature list
· Usage guide
· Admin information
· Troubleshooting section
· Legal disclaimer
· Social media links
