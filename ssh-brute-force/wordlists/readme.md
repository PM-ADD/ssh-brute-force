
# 📁 Wordlists for SSH Brute Force Tool

This folder contains **username** and **password** lists used by the SSH brute force script. These lists are essential for testing combinations during an authorized penetration test.

---

## 📂 Contents

- `users.txt` – A list of usernames to try. Each username goes on a new line.
- `passwords.txt` – A list of passwords to try. Each password should also be on a new line.

### 🔤 Example: `users.txt`
```
root
admin
user
test
```

### 🔐 Example: `passwords.txt`
```
123456
admin123
password
letmein
```

---

## ✏️ Editing Wordlists

You can easily add or remove entries using any text editor:

### 🧑‍💻 Using a Text Editor:
- **Windows**: Open with Notepad or Notepad++
- **Linux/macOS**: Use editors like `nano`, `vim`, or a GUI editor (e.g., VS Code)

### 📌 Instructions:
1. Open `users.txt` or `passwords.txt`.
2. Add one entry per line.
3. Save the file as plain text.
4. Avoid extra spaces, empty lines, or duplicates.

#### ✅ Example (`passwords.txt`):
```
newpass123
welcome1
pa$$w0rd
```

> 💡 Tip: You can also generate/edit wordlists using scripting (e.g., Bash, Python) or tools like `crunch`.

---

## 💻 How to Use These Wordlists

These files are passed to the script using command-line arguments.

### ✅ Linux / Kali
```bash
python brute_ssh.py 192.168.1.100 -U wordlists/users.txt -P wordlists/passwords.txt --threads 5
```

### ✅ Windows (PowerShell)
```powershell
python brute_ssh.py 192.168.1.100 -U wordlists\users.txt -P wordlists\passwords.txt --threads 5
```

### ✅ macOS
```bash
python3 brute_ssh.py 192.168.1.100 -U wordlists/users.txt -P wordlists/passwords.txt --threads 5
```

---

## 🛠 Tips for Custom Wordlists

- Use **short, targeted lists** for faster testing.
- Combine with tools like:
  - `crunch` for generating passwords
  - `cewl` for custom wordlists based on a target's website
- Avoid duplicates and empty lines.

---

## ⚠️ Ethical Use Only

These wordlists should only be used in legal and authorized penetration testing environments.  
**Do not use on systems without permission. Misuse is illegal.**
