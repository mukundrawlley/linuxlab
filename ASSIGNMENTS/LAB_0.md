# 🐧 Installing Ubuntu on VirtualBox

This guide will walk you through setting up **Ubuntu Linux** inside **VirtualBox** . 

---

## ✅ Step 1: Download Ubuntu ISO
- Visit the official [Ubuntu Downloads page](https://ubuntu.com/download/desktop).
- Download the latest LTS (Long Term Support) version for stability.

![alt text](IMAGES/LAB_0/ubuntu.png)

---

## ✅ Step 2: Install VirtualBox
- Go to the [VirtualBox official site](https://www.virtualbox.org/).
- Download and install VirtualBox (works on **Windows, Linux, and macOS**).

![alt text](IMAGES/LAB_0/vm.png)![alt text](IMAGES/LAB_0/b.png)

---

## ✅ Step 3: Create a New Virtual Machine
1. Open VirtualBox → click **New**.  
2. Fill in:
   - **Name:** Ubuntu  
   - **Type:** Linux  
   - **Version:** Ubuntu (64-bit)  
3. Allocate resources:  
   - **RAM:** At least 2 GB (4 GB+ recommended).  
   - **Disk:** At least 25 GB.  

![alt text](IMAGES/LAB_0/vm2.png)

---

## ✅ Step 4: Mount the ISO
- Open VM **Settings** → go to **Storage**.  
- Under "Controller: IDE", select **Empty** → choose the **Ubuntu ISO** you downloaded.  
- Save settings.  

![alt text](IMAGES/LAB_0/iso.png)

---

## ✅ Step 5: Start the VM and Install Ubuntu
- Launch the VM.  
- Select **Install Ubuntu**.  
- Follow the installer:
  - Choose **Language & Keyboard layout**.  
  - Connect to **Wi-Fi (optional)**.  
  - Choose **Normal Installation**.  
  - Partition disk (use defaults for VM).  
  - Create a **username and password**.  
- Wait for installation → reboot when done.  
![alt text](IMAGES/LAB_0/install1.png)![alt text](<IMAGES/LAB_0/install 2.png>)

---

## ✅ Step 6: Post-Installation Setup
- Remove the ISO from **Storage** to avoid boot loops.  
- Start VM again → log in to Ubuntu.  
- Update system:  
  ```bash
  sudo apt update && sudo apt upgrade -y

# 🖥️ Useful Commands After Installation

Once Parrot OS is installed, open a terminal and try these commands:

```bash
# Show OS release information
lsb_release -a

# Show kernel version and system architecture
uname -a

# Show disk usage in human-readable format
df -h

# Show free and used memory in MB
free -m
```
![alt text](IMAGES/LAB_0/e.png)![alt text](IMAGES/LAB_0/f.png)![alt text](IMAGES/LAB_0/h.png)![alt text](IMAGES/LAB_0/i.png)
---

# ⚡ Common Challenges & Fixes

| Challenge | Cause | Quick Fix |
|-----------|-------|-----------|
| Slow performance | Too little RAM/CPU | Increase VM resources |
| ISO not detected | Incorrect mount | Recheck storage settings |
| Black screen / boot error | Missing Guest Additions | Enable EFI or reinstall Guest Additions |
| No internet | Network adapter issues | Switch to "Bridged Adapter" or "NAT" |

---

# ❓ Questions & Answers

## Q1: What are 2 advantages of installing Parrot OS in a VM?
1. 🔒 **Safety:** Experiment freely without harming your main OS.  
2. 🌀 **Flexibility:** Snapshots, rollbacks, and easy removal make it beginner-friendly.  

---
## Q2: What are 2 advantages of dual booting instead of using a VM?
1. ⚡ **Performance:** Full access to CPU, RAM, and GPU → smoother and faster.  
2. 🔧 **Hardware Access:** Better compatibility with Wi-Fi adapters, GPUs, and external devices.  

---
