# LAB 4 COMMANDS 

---

````markdown
# Linux Lab: Basic File Commands

This guide demonstrates some basic file commands in Linux: `touch`, `cp`, `mv`, `echo`, and `cat`dfdf.

---

## 1. `touch` Command
**Purpose:** Create an empty file or update the timestamp of an existing file.

**Example:**
```bash
# Create an empty file named file1.txt
touch file1.txt

# Create multiple files at once
touch file2.txt file3.txt
````

---

## 2. `cp` Command

**Purpose:** Copy files or directories.

**Example:**

```bash
# Copy file1.txt to backup.txt
cp file1.txt backup.txt

# Copy a file to another directory
cp file1.txt /home/user/Documents/

# Copy a directory and its contents
cp -r myfolder /home/user/backup/
```

---

## 3. `mv` Command

**Purpose:** Move or rename files/directories.

**Example:**

```bash
# Rename file1.txt to file_renamed.txt
mv file1.txt file_renamed.txt

# Move file to another directory
mv file2.txt /home/user/Desktop/
```

---

## 4. `echo` Command

**Purpose:** Display text or write it to a file.

**Example:**

```bash
# Print a message
echo "Hello, Linux!"

# Write text to a file (overwrite)
echo "This is a test file" > test.txt

# Append text to a file
echo "Adding more content" >> test.txt
```

---

## 5. `cat` Command

**Purpose:** View contents of a file, concatenate files, or create files.

**Example:**

```bash
# View file contents
cat test.txt

# Concatenate multiple files into one
cat file2.txt file3.txt > merged.txt

# Create a file with content using cat
cat > notes.txt
This is a note.
Press CTRL+D to save and exit.
```

```

---

Do you want me to **save this into a downloadable `.md` file** so you can directly use it in your Linux lab?
```
