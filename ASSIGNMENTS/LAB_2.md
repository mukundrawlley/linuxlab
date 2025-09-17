# 🐚 BASICS OF SHELL SCRIPTING
## 📝 Assignment 2 – Script Execution & Explanation

**Objective:** Understand how existing scripts in the `Scripts/` folder work.  
We’ll analyze two sample Bash scripts, explain them line by line, and show example runs.  

---

## 📌 Script 1: `print_numbers.sh`

### 🎯 Purpose
Prints numbers from 1 to a specified limit using a loop.

---

### 📜 Script Code
```bash
#!/bin/bash
# print_numbers.sh

for i in {1..5}
do
  echo "Number: $i"
done
```
### 🔎 Line-by-Line Explanation

- `#!/bin/bash` → tells the system to use the **Bash shell** to run this script.  
- `for i in {1..5}` → loops through numbers **1** to **5**.  
- `do` → starts the loop block.  
- `echo "Number: $i"` → prints each number with the label **Number:**.  
- `done` → ends the loop.
----
### ▶️ Example Run

**Command:**
```bash
chmod 777 print_numbers.sh
./print_numbers.sh
```
**Output:**
```bash
Number: 1
Number: 2
Number: 3
Number: 4
Number: 5
```
![alt text](../IMAGES/LAB_2/1.png)![alt text](../IMAGES/LAB_2/2.png)
---

## 📌 Script 2: `array_loop.sh`

### 🎯 Purpose
Demonstrates looping through an array of items in Bash.

---

### 📜 Script Code
```bash
#!/bin/bash
# array_loop.sh

fruits=("apple" "banana" "cherry")

for fruit in "${fruits[@]}"
do
  echo "Fruit: $fruit"
done
```
### 🔎 Line-by-Line Explanation

- `#!/bin/bash` → ensures the script runs with the **Bash interpreter**.  
- `fruits=("apple" "banana" "cherry")` → defines an array named **fruits**.  
- `for fruit in "${fruits[@]}"` → loops through all items in the array.  
- `do` → begins the loop block.  
- `echo "Fruit: $fruit"` → prints each fruit with the label **Fruit:**.  
- `done` → ends the loop.  
----
### ▶️ Example Run

**Command:**
```bash
./array_loop.sh
```
**Output:**
```bash
Fruit: apple
Fruit: banana
Fruit: cherry
```
![alt text](../IMAGES/LAB_2/3.png)![alt text](../IMAGES/LAB_2/4.png)
---
# ❓ Extra Questions

### Q1: What is the purpose of `#!/bin/bash` at the top of a script?
It is called a **shebang**. It tells the system which interpreter to use for the script (in this case, **Bash**).  
Without it, the script might not run properly or could use the wrong shell.  

---

### Q2: How do you make a script executable?
Use the `chmod` command to give it execute permissions:  
```bash
chmod +x scriptname.sh
```
Then run it with:
```bash
./scriptname.sh
```