# 👥 Linux Shell Scripting Challenge: User Management (10 Real-World Tasks)

This set of 10 shell scripting questions will help you master Linux user management—covering everything from basic user creation to advanced auditing using UID, GID, and expiration handling.

---

## 📌 Question 1: Create User Only If Not Exists

**Objective:**  
Write a shell script that checks if a user exists. If not, create the user.

**Requirements:**
- Accept username input
- Use `id` or `getent passwd`
- Show relevant message

---

## 📌 Question 2: Bulk User Creation & Deletion

**Objective:**  
Create and delete users in bulk using a username list file.

**Requirements:**
- Input file: `userlist.txt`
- Use `useradd` and `userdel`
- Add logging for each action

---

## 📌 Question 3: Filter Users Based on UID/GID Range

**Objective:**  
List all users whose UID and GID fall within a custom range.

**Requirements:**
- Accept UID_MIN, UID_MAX, GID_MIN, GID_MAX
- Parse `/etc/passwd` and `/etc/group`
- Show username, UID, GID, shell

---

## 📌 Question 4: Set Expiry Date for a Single User

**Objective:**  
Prompt the user for a username and expiry date, and set it using `usermod`.

**Requirements:**
- Validate username
- Use `usermod -e YYYY-MM-DD`
- Confirm changes

---

## 📌 Question 5: Set Expiry for Multiple Users (Bulk)

**Objective:**  
Use a file `users_expiry.txt` with `username:YYYY-MM-DD` format to set expirations.

**Requirements:**
- Parse file line by line
- Set using `chage` or `usermod`
- Log success/failure

---

## 📌 Question 6: List All Users with Expiration Dates

**Objective:**  
Generate a report of all users along with their account expiration dates.

**Requirements:**
- Use `chage -l`
- Filter only UID ≥ 1000
- Output format: `Username | Expiry Date`

---

## 📌 Question 7: Audit Expired and Soon-to-Expire Users

**Objective:**  
List expired accounts and accounts expiring in the next 7 days.

**Requirements:**
- Use `chage` and `date` commands
- Format output with tags:
  - `[EXPIRED]`
  - `[EXPIRING in X days]`

---

## 📌 Question 8: Lock or Unlock User Accounts

**Objective:**  
Write a script to lock or unlock a user account based on user input.

**Requirements:**
- Accept username and choice (`lock` or `unlock`)
- Use `passwd -l` and `passwd -u`
- Confirm status after action

---

## 📌 Question 9: Change Shell for a Given User

**Objective:**  
Write a script to change the login shell for a user.

**Requirements:**
- Accept username and shell path (e.g., `/bin/bash`)
- Validate if shell exists
- Use `chsh` or `usermod -s`

---

## 📌 Question 10: Backup and Restore User Info

**Objective:**  
Create a backup of a user's home directory, and restore it if needed.

**Requirements:**
- Accept the username
- Use `tar` to compress `/home/username` to `/backups/username.tar.gz`
- Provide a restore option

---



