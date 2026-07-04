# Kali Linux Notes

## 📁 Navigation Commands

### pwd
Current working directory ka path dikhata hai.

```bash
pwd
```

Example:
```bash
pwd
# Output:
/home/kali/Documents
```

---

### ls
Current folder ke andar ki files aur folders dikhata hai.

```bash
ls
```

Example:
```bash
ls
# Output:
Desktop Documents Downloads
```

---

### ls -l
Files aur folders ki detailed information dikhata hai.

```bash
ls -l
```

Example:
```bash
ls -l
```

---

### ls -a
Hidden files aur folders dikhata hai.

```bash
ls -a
```

Example:
```bash
ls -a
```

---

### cd
Ek folder se dusre folder me jane ke liye.

```bash
cd Documents
```

Example:
```bash
cd Downloads
```

Go Back:

```bash
cd ..
```

Go Home:

```bash
cd ~
```

---

## 📂 File & Folder Operations

### mkdir
Naya folder create karta hai.

```bash
mkdir Projects
```

Example:
```bash
mkdir Notes
```

---

### touch
Nayi empty file create karta hai.

```bash
touch notes.txt
```

Example:
```bash
touch demo.py
```

---

### cp
File ya folder copy karta hai.

```bash
cp notes.txt backup.txt
```

Example:
```bash
cp report.txt Documents/
```

Folder Copy:

```bash
cp -r Notes Backup
```

---

### mv
File move ya rename karta hai.

```bash
mv notes.txt Documents/
```

Example:
```bash
mv old.txt new.txt
```

---

### rm
File ya folder delete karta hai.

```bash
rm notes.txt
```

Example:
```bash
rm demo.py
```

Folder Delete:

```bash
rm -r Notes
```

---

### rmdir
Empty folder delete karta hai.

```bash
rmdir Test
```

Example:
```bash
rmdir EmptyFolder
```

---

## 📖 Viewing File Contents

### cat
File ka pura content terminal me dikhata hai.

```bash
cat notes.txt
```

Example:
```bash
cat passwords.txt
```

---

### less
Badi file ko page by page dekhne ke liye.

```bash
less log.txt
```

Example:
```bash
less notes.txt
```

---

### head
File ki pehli 10 lines dikhata hai.

```bash
head notes.txt
```

Example:
```bash
head -5 notes.txt
```

---

### tail
File ki last 10 lines dikhata hai.

```bash
tail notes.txt
```

Example:
```bash
tail -5 notes.txt
```

---

### tail -f
File me real-time changes monitor karta hai.

```bash
tail -f server.log
```

Example:
```bash
tail -f access.log
```

---

## ✍️ Text Editors

### nano
Simple text editor.

```bash
nano notes.txt
```

Example:
```bash
nano test.py
```

---

### vim
Advanced text editor.

```bash
vim notes.txt
```

Example:
```bash
vim script.py
```
# 🔍 Searching Inside Files

Searching Inside Files is an essential Linux skill that helps you quickly find specific words or text within files and directories. The `grep` command is the most commonly used tool for this purpose. Below are the basic `grep` commands with simple Hinglish explanations and examples.

---

# 1. grep

## Command

```bash
grep "Linux" notes.txt
```

### Hinglish Explanation

`grep` command ka use file ke andar kisi specific word ya text ko search karne ke liye hota hai. Agar word mil jata hai to us line ko terminal par show karta hai.

### Example

```bash
grep "Linux" notes.txt
```

---

# 2. grep -i

## Command

```bash
grep -i "linux" notes.txt
```

### Hinglish Explanation

`-i` option uppercase aur lowercase letters ka difference ignore karta hai. Matlab `Linux`, `LINUX`, aur `linux` sabhi ko search karega.

### Example

```bash
grep -i "linux" notes.txt
```

---

# 3. grep -n

## Command

```bash
grep -n "Linux" notes.txt
```

### Hinglish Explanation

`-n` option matching line ke saath uska line number bhi show karta hai.

### Example

```bash
grep -n "Linux" notes.txt
```

---

# 4. grep -c

## Command

```bash
grep -c "Linux" notes.txt
```

### Hinglish Explanation

`-c` option batata hai ki search kiya gaya word kitni lines me mila hai.

### Example

```bash
grep -c "Linux" notes.txt
```

---

# 5. grep -v

## Command

```bash
grep -v "Linux" notes.txt
```

### Hinglish Explanation

`-v` option un lines ko show karta hai jisme search kiya gaya word nahi hota.

### Example

```bash
grep -v "Linux" notes.txt
```

---

# 6. grep -r

## Command

```bash
grep -r "Linux" .
```

### Hinglish Explanation

`-r` option current directory aur uske andar maujood sabhi folders aur files me recursively search karta hai.

### Example

```bash
grep -r "Linux" .
```
