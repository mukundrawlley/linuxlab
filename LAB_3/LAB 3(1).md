# 🐧 Terminal Basics – Essential Commands  

````markdown
Learning the terminal is a **superpower for developers** ⚡.  
These commands will help you **navigate, manage files, and work faster** when coding or using Git/VS Code.  

````
## 🔹 1. Navigation Commands  

### 📍 `pwd` – *Print Working Directory*  
Shows the **current folder path** you’re in.  

```bash
pwd


📌 Example Output:
/Users/yourname/projects
```

---

### 📂 `ls` – *List Directory Contents*

Displays files and directories.

```bash
ls
```

Common options:

* `ls -l` → Long format (permissions, size, date)
* `ls -a` → Includes hidden files
* `ls -la` → Combine both

---

### 🚪 `cd` – *Change Directory*

Move between folders.

```bash
cd folder_name
```

Examples:

```bash
cd Documents    # Go into Documents  
cd ..           # Go back one level  
cd /            # Jump to root directory  
cd ~            # Jump to home directory  
```
![alt text](<../images/LAB 3/1ST/6 edited.png>)
---

## 🔹 2. File & Directory Management

### 📁 `mkdir` – *Make Directory*

Create a new folder.

```bash
mkdir new_folder
```

---

### 📄 `touch` – *Create File*

Make an empty file.

```bash
touch file.txt
```

---

### 📑 `cp` – *Copy Files/Directories*

```bash
cp file1.txt backup.txt
cp -r folder1 folder2   # Copy entire folder
```

---

### ✂️ `mv` – *Move / Rename Files*

```bash
mv old.txt new.txt          # Rename  
mv file.txt ~/Documents/    # Move to Documents  
```

---

### 🗑️ `rm` – *Remove Files/Directories*

```bash
rm file.txt       # Delete a file  
rm -r folder      # Delete a folder (recursive)  
```
⚠️ **Caution:** No recycle bin → deleted means gone!
---
![alt text](<../images/LAB 3/1ST/7.png>)
---

## 🔹 3. File Viewing & Editing

### 📜 `cat` – *View File Contents*

```bash
cat notes.txt
```

---

### ✍️ `nano` – *Edit Files Inside Terminal*

```bash
nano file.txt
```

* Use arrow keys to navigate
* `CTRL + O` → Save
* `CTRL + X` → Exit

---

### 🧹 `clear` – *Clear the Screen*

```bash
clear
```
Shortcut: `CTRL + L`
---
![alt text](<../images/LAB 3/1ST/8a.png>)![alt text](<../images/LAB 3/1ST/8b.png>)
---

## 🔹 4. System Commands

### 🗣️ `echo` – *Print Text*

```bash
echo "Hello, World!"
```

---

### 👤 `whoami` – *Current User*

```bash
whoami
```

---

### 📖 `man` – *Show Command Manual*

```bash
man ls
```
Press `q` to quit the manual.
---
![alt text](<../images/LAB 3/1ST/9 a.png>)
---

## 🔹 5. Search & Find

### 🔍 `find` – *Locate Files*

```bash
find . -name "*.txt"
```

Finds all `.txt` files in current and subfolders.

---

### 🔎 `grep` – *Search Inside Files*

```bash
grep "hello" file.txt
```
Searches for the word `hello` in `file.txt`.
---
![alt text](<../images/LAB 3/1ST/10.png>)
---

## 🔹 6. Handy Shortcuts

| Shortcut   | Action                     |
| ---------- | -------------------------- |
| `Tab`      | Auto-complete path/command |
| `↑ / ↓`    | Browse command history     |
| `CTRL + C` | Stop a running process     |
| `CTRL + L` | Clear the terminal         |

---

## 🔹 7. Bonus: Chaining Commands

Run multiple commands together:

```bash
mkdir test && cd test && touch hello.txt
```

* `&&` → Run next command **only if previous succeeds**
* `;`  → Run next command **regardless of success**

---

# 🎯 Final Note

Mastering these commands will make you:
✅ Faster at coding
✅ Better at using Git/VS Code
✅ More comfortable in Linux/macOS/Windows Dev Environments

🚀 Start practicing — the terminal is your **developer toolkit**!


