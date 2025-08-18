# 🥼 LAB-4: Linux Advance File Commands  

Welcome to **Linux Lab 4**! 🎉  
In this lab, we’ll explore some of the **most important Linux commands** for handling files.  
Mastering these will give you strong foundations in file management.  

We’ll cover the following commands:  
👉 `touch`  
👉 `cp`  
👉 `mv`  
👉 `echo`  
👉 `cat`  

Each section includes:  
✅ Definition  
✅ Examples  
✅ Pro Tips  
✅ Output Previews  

---

## 📌 1. `touch` — Create Files or Update Timestamps  

**Definition:**  
The `touch` command is used to create an empty file or update the **last modified timestamp** of an existing file.  

💡 **Pro Tip:** You can create multiple files at once with a single command.  

```bash
# Create an empty file named file1.txt
touch file1.txt

# Create multiple files in one go
touch file2.txt file3.txt
```

🔎 **Preview:**  
```bash
$ touch file1.txt
$ ls
file1.txt
```

---

## 📌 2. `cp` — Copy Files and Directories  

**Definition:**  
The `cp` (copy) command lets you duplicate files and directories.  

💡 **Pro Tip:** Use `-r` (recursive) when copying directories, otherwise only files can be copied.  

```bash
# Copy file1.txt to backup.txt
cp file1.txt backup.txt

# Copy a file into another directory
cp file1.txt /home/user/Documents/

# Copy an entire folder (recursively)
cp -r myfolder /home/user/backup/
```

🔎 **Preview:**  
```bash
$ cp file1.txt file_copy.txt
$ ls
file1.txt  file_copy.txt
```

---

## 📌 3. `mv` — Move or Rename Files/Directories  

**Definition:**  
The `mv` (move) command moves files/directories to another location OR renames them.  

💡 **Pro Tip:** If you "move" a file within the same directory but change its name, it acts as a **rename**.  

```bash
# Rename file1.txt to file_renamed.txt
mv file1.txt file_renamed.txt

# Move a file into another directory
mv file2.txt /home/user/Desktop/
```

🔎 **Preview:**  
```bash
$ mv file1.txt newname.txt
$ ls
newname.txt
```

---

## 📌 4. `echo` — Print or Write Text to Files  

**Definition:**  
The `echo` command displays text in the terminal OR writes text into a file.  

💡 **Pro Tip:**  
- Use `>` to overwrite a file.  
- Use `>>` to append (add new content without deleting old content).  

```bash
# Print text in terminal
echo "Hello, Linux!"

# Write (overwrite) content into a file
echo "This is a test file" > test.txt

# Append content to the file
echo "Adding more content" >> test.txt
```

🔎 **Preview:**  
```bash
$ echo "Hello, Linux!"
Hello, Linux!

$ cat test.txt
This is a test file
Adding more content
```

---

## 📌 5. `cat` — View and Combine File Contents  

**Definition:**  
The `cat` (concatenate) command is used to **view file contents**, **merge multiple files**, or even **create new files**.  

💡 **Pro Tip:** Combine multiple files using `cat file1 file2 > newfile`.  

```bash
# View file contents
cat test.txt

# Combine file2.txt and file3.txt into merged.txt
cat file2.txt file3.txt > merged.txt

# Create a new file with content
cat > notes.txt
This is a note.
Press CTRL+D to save and exit.
```

🔎 **Preview:**  
```bash
$ cat test.txt
This is a test file
Adding more content
```

---

## 🖼️ Example Terminal Flow  

```bash
$ touch file1.txt
$ echo "Hello Linux" > file1.txt
$ cp file1.txt file_copy.txt
$ mv file_copy.txt renamed_file.txt
$ cat file1.txt
Hello Linux
```

---

## 📊 Quick Command Cheat Sheet  

| Command | Purpose | Example |
|---------|----------|---------|
| `touch` | Create empty files or update timestamps | `touch file.txt` |
| `cp`    | Copy files/directories | `cp file.txt /home/user/` |
| `mv`    | Move or rename files | `mv file.txt newfile.txt` |
| `echo`  | Print/write text | `echo "Hello" > file.txt` |
| `cat`   | View/merge files | `cat file1 file2 > merged.txt` |

---

## 🎯 Summary  

By the end of this lab, you can now:  
✔️ Create files with `touch`  
✔️ Copy files/folders with `cp`  
✔️ Move/Rename files with `mv`  
✔️ Write/Append text with `echo`  
✔️ View/Combine files with `cat`  

🚀 These commands are your **first step to mastering Linux file management**!  

---
## 🖼️ Screenshots
![alt text](<images/LAB 4/2.png>)
---
```
```
---
![alt text](<images/LAB 4/3.png>)
---
```
```
---
![alt text](<images/LAB 4/4.png>)
---
```
```
---
![alt text](<images/LAB 4/5.png>)
---

# ✅ **End of Lab 4**
```  
Now you’re ready to experiment with these commands in your terminal! 🖥️
```
---







