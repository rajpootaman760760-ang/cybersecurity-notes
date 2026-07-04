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
