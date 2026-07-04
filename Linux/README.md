# Kali Linux Commands

## 1. pwd

**Explanation:**  
Current directory ka path dikhata hai. Matlab abhi terminal me tum kis folder ke andar ho, ye batata hai.

**Syntax**
```bash
pwd
```

**Example**
```bash
pwd
```

**Output**
```bash
/home/kali/Documents
```

---

## 2. ls

**Explanation:**  
Current folder ke andar jitni files aur folders hain, unki list dikhata hai.

**Syntax**
```bash
ls
```

**Example**
```bash
ls
```

**Output**
```bash
Desktop  Documents  Downloads  notes.txt
```

---

## 3. ls -l

**Explanation:**  
Files aur folders ki detailed information dikhata hai jaise permissions, owner, size aur date.

**Syntax**
```bash
ls -l
```

**Example**
```bash
ls -l
```

---

## 4. ls -a

**Explanation:**  
Hidden files aur folders bhi dikhata hai (jo dot `.` se start hote hain).

**Syntax**
```bash
ls -a
```

**Example**
```bash
ls -a
```

---

## 5. cd

**Explanation:**  
Ek folder se dusre folder me jane ke liye use hota hai.

**Syntax**
```bash
cd folder_name
```

**Example**
```bash
cd Documents
```

Pichle folder me jane ke liye

```bash
cd ..
```

Home directory me jane ke liye

```bash
cd ~
```

---

## 6. mkdir

**Explanation:**  
Naya folder banane ke liye use hota hai.

**Syntax**
```bash
mkdir folder_name
```

**Example**
```bash
mkdir Projects
```

---

## 7. touch

**Explanation:**  
Nayi empty file create karne ke liye use hota hai.

**Syntax**
```bash
touch file_name
```

**Example**
```bash
touch notes.txt
```

---

## 8. cp

**Explanation:**  
File ya folder ki copy banane ke liye use hota hai.

**Syntax**
```bash
cp source destination
```

**Example**
```bash
cp notes.txt backup.txt
```

Folder copy karne ke liye

```bash
cp -r Notes Backup
```

---

## 9. mv

**Explanation:**  
File ko move ya rename karne ke liye use hota hai.

**Syntax**
```bash
mv source destination
```

**Example (Rename)**
```bash
mv notes.txt linux_notes.txt
```

**Example (Move)**
```bash
mv linux_notes.txt Documents/
```

---

## 10. rm

**Explanation:**  
File ya folder delete karne ke liye use hota hai.

**Syntax**
```bash
rm file_name
```

**Example**
```bash
rm notes.txt
```

Folder delete karne ke liye

```bash
rm -r Notes
```

---

## 11. rmdir

**Explanation:**  
Sirf empty folder delete karta hai.

**Syntax**
```bash
rmdir folder_name
```

**Example**
```bash
rmdir Test
```

---

## 12. cat

**Explanation:**  
File ke andar ka content terminal me dikhata hai.

**Syntax**
```bash
cat file_name
```

**Example**
```bash
cat notes.txt
```

---

## 13. less

**Explanation:**  
Badi file ko page by page dekhne ke liye use hota hai.

**Syntax**
```bash
less file_name
```

**Example**
```bash
less log.txt
```

---

## 14. more

**Explanation:**  
File ko ek-ek page me dekhne ke liye use hota hai.

**Syntax**
```bash
more file_name
```

**Example**
```bash
more notes.txt
```
