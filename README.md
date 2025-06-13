# 🔐 SSH Brute Force Tool

A multithreaded SSH brute force script built in Python. Designed for authorized penetration testing and ethical hacking only.

> ⚠️ **Warning:** This tool is intended for legal and educational purposes only. Do not use against systems without explicit permission.

---

## 📦 Features

- 🚀 Multithreaded for faster brute-force attempts
- 🔄 Retries SSH errors (timeouts, exceptions)
- 📂 Supports:
  - Single user or user list
  - Password list or on-the-fly password generation
- ✅ Saves valid credentials to `credentials.txt`
- 📊 Clear terminal output with color-coded results

---

## 🛠 Requirements

Install dependencies in a virtual environment:

```bash
sudo apt install python3-venv -y
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
bash'''

##  Or, for global install (not recommended on Kali):
'''bash
pip install --break-system-packages -r requirements.txt
'''
