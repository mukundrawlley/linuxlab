# ⚡ Intermediate & Advanced Terminal Commands  
*(Linux, macOS, Git Bash – System Admin & DevOps Essentials)* 
````markdown
Once you’re comfortable with the basics, it’s time to level up 💻.  
These commands let you **manage users, control permissions, monitor system performance, and handle networking**.  
````
## 🔹 1. Run Commands as Admin – `sudo`  

`sudo` = **SuperUser DO** → lets you run commands with **root privileges**.  

```bash
sudo command
````

Examples:

```bash
sudo apt update    # Update package list (Debian/Ubuntu)
sudo reboot        # Restart the system
```
📌 You’ll be asked for your password.

---

## 🔹 2. User Management (Linux/macOS)

### 👤 Add a New User

```bash
sudo adduser newusername
```

### 🔑 Change User Password

```bash
sudo passwd newusername
```

### 👥 Modify User (e.g., add to a group)

```bash
sudo usermod -aG groupname username
```

Example:

```bash
sudo usermod -aG sudo alice   # Give Alice admin rights
```

### ❌ Delete a User

```bash
sudo deluser username
sudo deluser --remove-home username   # Also delete home directory
```
![alt text](<../images/LAB 3/2ND/11.png>)![alt text](<../images/LAB 3/2ND/11B.png>)
---

## 🔹 3. File Permissions & Ownership

### 🔐 `chmod` – Change Permissions

```bash
chmod 755 script.sh    # Owner: rwx, Group/Others: rx
chmod +x file.sh       # Add execute permission
chmod -x file.sh       # Remove execute permission
```

### 📊 Permission Number Reference

| Number | Meaning                |
| ------ | ---------------------- |
| 7      | read + write + execute |
| 6      | read + write           |
| 5      | read + execute         |
| 4      | read only              |
| 0      | no permission          |

Example:

```bash
chmod 644 file.txt   # Owner: rw, Group: r, Others: r
```

---

### 👑 `chown` – Change Owner

```bash
sudo chown user:group file
```

Example:

```bash
sudo chown alice:alice myfile.txt
```
---
![alt text](<../images/LAB 3/2ND/12.png>)
---

## 🔹 4. Disk & System Monitoring

### 💽 Disk Usage

```bash
df -h    # Human-readable disk space
```

### 📁 Folder Size

```bash
du -sh folder_name
```

### 🖥️ Active Processes

```bash
top      # Live system monitor (q to quit)
htop     # Nicer version (needs install)
```
---
![alt text](<../images/LAB 3/2ND/13.png>)
---

## 🔹 5. Networking Tools

### 🌐 Check Connectivity

```bash
ping google.com
```

(Stop with CTRL + C)

### 📶 View IP & Network Info

```bash
ip a
```

or

```bash
ifconfig   # Might require sudo or net-tools
```

### 🔍 Show Connections

```bash
ss -tuln   # Modern, faster
netstat -tuln   # Legacy alternative
```
---
![alt text](<../images/LAB 3/2ND/14.png>)![alt text](<../images/LAB 3/2ND/14B.png>)
---

## 🔹 6. Package Management

### 📦 On Ubuntu/Debian (APT)

```bash
sudo apt update        # Refresh package index
sudo apt upgrade       # Upgrade packages
sudo apt install git   # Install
sudo apt remove git    # Uninstall
```

### 🍎 On macOS (Homebrew)

```bash
brew install git
```
---
![alt text](<../images/LAB 3/2ND/15.png>)
---

## 🔹 7. Process Management

### 🔎 See Running Processes

```bash
ps aux
```

### 🔫 Kill a Process

```bash
kill <PID>       # Normal kill
kill -9 <PID>    # Force kill
```

Example:

```bash
kill 12345
```

---

## 🔹 8. Shutdown & Reboot

```bash
sudo shutdown now       # Power off immediately
sudo shutdown -r now    # Reboot immediately
```

---

# 🎯 Pro Tip

These commands give you **control over users, files, and system health**.
👉 Always be careful with `sudo`, `rm`, and `kill` — they can change or break your system if misused.

🚀 Practice in a **VM or test environment** before using them on your main machine!

