# 🚀LEARNING LINUX 

````markdown
# 🐧 Linux Basics: Essential Commands

This guide introduces some **fundamental Linux commands** with definitions and examples.  
They are the building blocks for navigating and managing your files.  

````
## 📍 1. `pwd` — *Print Working Directory*

**Definition:**  
Displays the **full path** of the directory you are currently in.  

**Examples:**
```bash
pwd
# Output: /home/username
````

👉 Useful for checking your current location in the filesystem.

---

## 📂 2. `ls` — *List Files*

**Definition:**
Lists the files and directories inside the current folder.

**Examples:**

```bash
ls
# Output: file1.txt  file2.txt  Documents  Pictures

ls -l
# Detailed view with permissions, size, and modified date

ls -a
# Shows hidden files (those starting with . like .bashrc)
```

👉 Helps you see what’s inside a directory.

---

## 🚪 3. `cd` — *Change Directory*

**Definition:**
Used to **move between directories**.

**Examples:**

```bash
cd Documents
# Moves into the Documents folder

cd ..
# Moves back one level (parent directory)

cd ~
# Takes you directly to your Home directory
```
---

## 📍5. `mkdir` — *Make Directory*

**Definition:**  Creates one or more new directories in the filesystem.  

**Examples:**

```bash
mkdir Projects
# Creates a directory named "Projects" in the current location


mkdir folder1 folder2
# Creates multiple directories at once (folder1 and folder2)


mkdir -p Work/2025/Assignments
# Creates a nested directory structure (Work → 2025 → Assignments)  
# The `-p` option ensures parent folders are created if they don’t exist


mkdir ~/Downloads/NewFolder
# Creates "NewFolder" inside the Downloads directory
```

---



## 📄 4. `touch` — *Create Empty File*

**Definition:**
Creates a new **empty file** or updates the timestamp of an existing file.

**Examples:**

```bash
touch notes.txt
# Creates an empty file named notes.txt

touch file1.txt file2.txt
# Creates multiple files at once
```

👉 Ideal for quickly making new files before editing them.

---

# ✨ Quick Recap

| Command | Definition                   | Example                    |
| ------- | ---------------------------- | -------------------------- |
| `pwd`   | Shows current directory path | `pwd → /home/username`     |
| `ls`    | Lists files & folders        | `ls -a` shows hidden files |
| `cd`    | Changes directory            | `cd Documents`             |
| `mkdir` | Creates directory            | `mkdir linux`              |
| `touch` | Creates empty files          | `touch new.txt`            |

---

💡 With these four commands, you can **navigate, explore, and create files** in Linux easily!

---
---
![alt text](IMAGES/LAB_1/6.png)



