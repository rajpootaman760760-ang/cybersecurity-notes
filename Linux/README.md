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
# ⌨️ Terminal Shortcuts

Terminal shortcuts help you work faster and more efficiently in Kali Linux. Instead of typing extra commands, you can use keyboard shortcuts to complete commands, stop running processes, clear the terminal, access previous commands, and view command documentation.

---

# 1. Tab

## Shortcut

```text
Tab
```

### Hinglish Explanation

`Tab` key ka use command ya file/folder ka naam automatically complete (Auto-complete) karne ke liye hota hai. Isse typing fast hoti hai aur spelling mistakes bhi kam hoti hain.

### Example

```bash
cd Doc
```

Press **Tab**

```bash
cd Documents/
```

---

# 2. Ctrl + C

## Shortcut

```text
Ctrl + C
```

### Hinglish Explanation

`Ctrl + C` ka use terminal me chal rahi command ya process ko turant stop (Interrupt) karne ke liye hota hai.

### Example

```bash
ping google.com
```

Press **Ctrl + C** to stop the command.

---

# 3. Ctrl + L

## Shortcut

```text
Ctrl + L
```

### Hinglish Explanation

`Ctrl + L` terminal screen ko clear kar deta hai. Ye `clear` command ke jaisa hi kaam karta hai.

### Example

```text
Press Ctrl + L
```

Terminal screen clean ho jayegi.

---

# 4. Up Arrow (↑)

## Shortcut

```text
↑ (Up Arrow)
```

### Hinglish Explanation

`Up Arrow` key ka use pehle chalayi gayi commands ko dobara dekhne aur use karne ke liye hota hai.

### Example

```bash
ls
pwd
date
```

Press **↑** to display the previous commands.

---

# 5. man

## Command

```bash
man command
```

### Hinglish Explanation

`man` (Manual) command kisi bhi Linux command ki complete documentation aur usage dikhata hai.

### Example

```bash
man ls
```

Ya

```bash
man grep
```

Exit karne ke liye **q** press karein.

# 👤 Users in Linux

Linux is a multi-user operating system, which means multiple users can use the same system. Every user has a unique identity called a **User ID (UID)**. Linux uses UIDs to identify users and control permissions.

---

# 1. User ID (UID)

## Concept

Every user in Linux has a unique **User ID (UID)**.

### Hinglish Explanation

UID (User ID) ek unique number hota hai jo Linux har user ko assign karta hai. Linux user ko uske naam se nahi, balki uske UID se identify karta hai.

### Example

```bash
id
```

Output:

```text
uid=1000(aman) gid=1000(aman) groups=1000(aman)
```

---

# 2. Root User (UID = 0)

## Concept

The **root user** always has **UID 0**.

### Hinglish Explanation

Root Linux ka Superuser hota hai. Iske paas system ki sabhi files aur settings ko access aur modify karne ki permission hoti hai.

### Example

```bash
id root
```

Output:

```text
uid=0(root) gid=0(root)
```

---

# 3. Regular Users (UID 1000+)

## Concept

Regular users usually have **UID 1000 or higher**.

### Hinglish Explanation

Jab naya normal user create hota hai, Linux usko 1000 ya usse bada UID assign karta hai. Ye users limited permissions ke saath kaam karte hain.

### Example

```bash
id aman
```

Output:

```text
uid=1000(aman)
```

---

# 4. /etc/passwd

## Command

```bash
cat /etc/passwd
```

### Hinglish Explanation

`/etc/passwd` file system ke sabhi users ki basic information store karti hai, jaise:

- Username
- UID
- GID
- Home Directory
- Default Shell

⚠️ Is file me actual password store nahi hota.

### Example

```bash
cat /etc/passwd
```

Output:

```text
aman:x:1000:1000::/home/aman:/bin/bash
```

---

# 5. /etc/shadow

## Command

```bash
sudo cat /etc/shadow
```

### Hinglish Explanation

`/etc/shadow` file users ke encrypted (hashed) passwords aur password-related information store karti hai. Is file ko sirf root user ya sudo permission ke saath hi dekha ja sakta hai.

### Example

```bash
sudo cat /etc/shadow
```

Output:

```text
aman:$y$j9T$abc123xyz...:20320:0:99999:7:::
```

---

# Useful Commands

### Check current user

```bash
whoami
```

### Check user information

```bash
id
```

### Check all users

```bash
cat /etc/passwd
```

### Check password hashes (Root only)

```bash
sudo cat /etc/shadow
```
# 👤 Key User Commands

Linux provides several user management commands to identify users, switch users, run administrative tasks, and manage passwords. Below are the most commonly used user commands with simple Hinglish explanations and examples.

---

# 1. whoami

## Command

```bash
whoami
```

### Hinglish Explanation

`whoami` command current logged-in user ka username dikhati hai.

### Example

```bash
whoami
```

Output:

```text
aman
```

---

# 2. id

## Command

```bash
id
```

### Hinglish Explanation

`id` command current user ka User ID (UID), Group ID (GID), aur jis groups ka user member hai, unki information dikhati hai.

### Example

```bash
id
```

Output:

```text
uid=1000(aman) gid=1000(aman) groups=1000(aman),27(sudo)
```

---

# 3. sudo

## Command

```bash
sudo command
```

### Hinglish Explanation

`sudo` command kisi bhi command ko Root (Administrator) permission ke saath run karne ke liye use hoti hai.

### Example

```bash
sudo apt update
```

---

# 4. su

## Command

```bash
su username
```

### Hinglish Explanation

`su` (Switch User) command ek user se dusre user par switch karne ke liye use hoti hai. Root user par switch karne ke liye `su root` ya `sudo su` use kiya jata hai.

### Example

```bash
su root
```

Ya

```bash
sudo su
```

---

# 5. passwd

## Command

```bash
passwd
```

### Hinglish Explanation

`passwd` command current user ka password change karne ke liye use hoti hai. Agar kisi dusre user ka password change karna ho to Root permission ki zarurat hoti hai.

### Example

Current user ka password change karna:

```bash
passwd
```

Kisi dusre user ka password change karna:

```bash
sudo passwd aman
```
