# FTP Login Brute Force & Banner Grabbing

## Challenge Title
Discover Hidden FTP Service, Extract Users from Banner, Brute Force Credentials, and Retrieve the Flag.

## Category
Assessment Methodologies – Enumeration

## Lab Link
[INE Lab](https://my.ine.com/CyberSecurity/courses/d707f31c-913d-477e-951e-74503392e9ae/assessment-methodologies-enumeration/lab/24c50c27-185b-4541-a88f-e2a12811053e)

---

## Objective

Identify hidden services using Nmap, enumerate users from FTP banner, brute force FTP credentials, and extract flag3 from the user directory.

---

## Tools Used

- `nmap` – for service enumeration
- `nc` – for FTP banner grabbing
- `hydra` – for brute-force attacks
- `ftp` – to retrieve flag manually

---

## Step-by-Step Walkthrough

### 🔹 Step 1: Nmap Scan

Initial scan shows SMB and SSH.

```bash
nmap -sV target.ine.local
