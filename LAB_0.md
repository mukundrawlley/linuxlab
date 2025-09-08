# 🦜 Installing Parrot OS on VirtualBox

This guide will walk you through setting up **Parrot OS** inside **VirtualBox** with clear steps, places for your screenshots, and notes on common challenges you might face.  

---

## ✅ Step 1: Download Parrot OS ISO
- Visit the official [Parrot OS website](https://parrotsec.org/download/).
- Download the ISO image (choose **Parrot Security** or **Parrot Home** depending on your needs).

![alt text](IMAGES/LAB_0/a.png)

---

## ✅ Step 2: Install VirtualBox
- Head to the [VirtualBox official site](https://www.virtualbox.org/).
- Download and install VirtualBox (works on **Windows, Linux, and macOS**).

![alt text](IMAGES/LAB_0/b.png)

---

## ✅ Step 3: Create a New Virtual Machine
1. Open VirtualBox → click **New**.  
2. Fill in:
   - **Name:** Parrot OS  
   - **Type:** Linux  
   - **Version:** Debian (64-bit)  
3. Allocate resources:  
   - **RAM:** Minimum 2 GB (4 GB+ recommended)  
   - **Disk:** At least 20 GB  

![alt text](IMAGES/LAB_0/c.png)

---

## ✅ Step 4: Mount the ISO
- Open VM **Settings** → go to **Storage**.  
- Under "Controller: IDE", select **Empty** → choose the **Parrot ISO**.  
- Save settings.  


---

## ✅ Step 5: Start the VM and Install
- Launch the VM.  
- Select **Try/Install Parrot OS**.  
- Follow the installer:
  - Language, Region, Keyboard  
  - Partition disk  
  - Create username & password  
- Wait for installation → reboot.  


---

## ✅ Step 6: Post-Installation
- Remove the ISO from **Storage** (prevents boot loop).  
- Start VM again → log in and explore Parrot OS!  


---

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
---
![alt text](IMAGES/LAB_0/e.png)![alt text](IMAGES/LAB_0/f.png)![alt text](IMAGES/LAB_0/h.png)![alt text](IMAGES/LAB_0/i.png)


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

