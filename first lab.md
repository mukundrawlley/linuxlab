Here’s a simple **Markdown (.md)** file that explains the `rm`, `cp`, `touch`, and `mv` commands in Ubuntu, along with examples — including moving one file to another.

---

### 📄 Contents of the `.md` file:

````markdown
# Basic Linux File Commands

This document explains four common file commands in Linux: `touch`, `cp`, `rm`, and `mv`, along with simple examples.

---

## 📁 1. `touch`

**Purpose:** Create a new empty file or update the timestamp of an existing one.

```bash
touch file.txt
````

✅ Creates an empty file named `file.txt` in the current directory.

---

## 📁 2. `cp`

**Purpose:** Copy files or directories.

```bash
cp file.txt copy.txt
```

✅ Creates a copy of `file.txt` named `copy.txt` in the same directory.

To copy into a different folder:

```bash
cp file.txt /home/user/Documents/
```

---

## 🗑️ 3. `rm`

**Purpose:** Remove (delete) files or directories.

```bash
rm file.txt
```

⚠️ This permanently deletes `file.txt`.

To delete a folder and its contents:

```bash
rm -r my_folder/
```

---

## 🚚 4. `mv`

**Purpose:** Move or rename files and directories.

```bash
mv file.txt /home/user/Documents/
```

✅ Moves `file.txt` into the Documents folder.

To rename a file:

```bash
mv oldname.txt newname.txt
```

---

## 🛠️ Example: Move a File from One Folder to Another

```bash
mkdir folder1 folder2
touch folder1/sample.txt
mv folder1/sample.txt folder2/
```

✅ This creates two folders, a file inside `folder1`, and moves `sample.txt` to `folder2`.

---

```

Would you like me to save this as an actual `.md` file for download?
```
![alt text](image-3.png)![alt text](image-4.png)
![alt text](image-5.png)
