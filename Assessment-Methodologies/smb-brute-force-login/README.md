# SMB Login Brute Force with Metasploit

## Challenge Title
Brute Force SMB Credentials and Extract a Flag

## Category
Assessment Methodologies – Enumeration

## Lab Link
[INE Lab](https://my.ine.com/CyberSecurity/courses/d707f31c-913d-477e-951e-74503392e9ae/assessment-methodologies-enumeration/lab/24c50c27-185b-4541-a88f-e2a12811053e)

---

## Objective

Use Metasploit to brute force SMB credentials using user and password wordlists. Once valid credentials are found, access the SMB share and retrieve the flag.

---

## Tools Used

- Metasploit (`msfconsole`)
- Wordlists (`users.txt` and `unix_passwords.txt`)
- `smbclient` to access shares after cracking

---

## Step-by-Step Walkthrough

### 🔹 Step 1: Launch Metasploit and Load SMB Login Module

```bash
msfconsole -q
use auxiliary/scanner/smb/smb_login
set RHOSTS target.ine.local
