# 🚀 EXPERIMENTING WITH SHELL SCRIPT
## 📝 Assignment 3 – Modify an Existing Script

**Objective:** Enhance and customize a script by adding user input and validation.

---

## 📌 Task 1: Original Script (`print_numbers.sh`)

### 🎯 Purpose
The original script simply prints numbers from **1 to 5** in sequence.

---

### 📜 Original Script Code
```bash
#!/bin/bash
# print_numbers.sh

for i in {1..5}
do
  echo "Number: $i"
done
```
---
### ▶️ Original Behavior

- Always prints numbers from **1 to 5**.  
- No user input, no flexibility.  

**Example Run:**
```bash
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

## 📌 Task 2: Enhanced Script (`enhanced_numbers.sh`)

### 🎯 Purpose
Enhance the script so the user provides `start`, `end`, and `step values`.
The script validates inputs (step must be positive).

---

### 📜 Enhanced Script Code
```bash
#!/bin/bash
# enhanced_numbers.sh

# Check if 3 arguments are provided
if [ $# -ne 3 ]; then
  echo "Usage: $0 <start> <end> <step>"
  exit 1
fi

start=$1
end=$2
step=$3

# Validate step
if [ $step -le 0 ]; then
  echo "Error: Step must be a positive number."
  exit 1
fi

# Loop through the range
for ((i=start; i<=end; i+=step))
do
  echo "Number: $i"
done
```
---
![alt text](../IMAGES/LAB_3/1.png)
---
**Example Run:**

` Run 1: Normal case`
```bash
./enhanced_numbers.sh 1 10 2
```
**Output:**
```bash
Number: 1
Number: 3
Number: 5
Number: 7
Number: 9
```
![alt text](../IMAGES/LAB_3/2.png)
---
`Run 2: Invalid step`
```bash
./enhanced_numbers.sh 1 10 0
```
**Output:**
```bash
Error: Step must be a positive number.
```
![alt text](../IMAGES/LAB_3/3.png)
---
# ❓ Extra Questions

### Q1: Difference between `$1`, `$@`, and `$#` in Bash?
- **`$1`** → the first argument passed to the script.  
- **`$@`** → all arguments as a list (`"$1" "$2" "$3"...`).  
- **`$#`** → the number of arguments passed to the script.  

---

### Q2: What does `exit 1` mean in a script?
- `exit` ends the script immediately.  
- `exit 0` means **successful execution**.  
- `exit 1` means the script **failed** (an error occurred).  
- Other numbers can also be used for different **error codes**.  
