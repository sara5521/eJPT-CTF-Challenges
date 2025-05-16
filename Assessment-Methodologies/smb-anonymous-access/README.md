# SMB Enumeration: Anonymous Access

## Challenge Title
SMB Share with Anonymous Access

## Category
Assessment Methodologies – Enumeration

## Lab Link
[INE Lab](https://my.ine.com/CyberSecurity/courses/d707f31c-913d-477e-951e-74503392e9ae/assessment-methodologies-enumeration/lab/24c50c27-185b-4541-a88f-e2a12811053e)

---

## Description

The goal of this challenge is to identify an SMB share that allows **anonymous access**, enumerate its contents, and retrieve a hidden flag.

---

## Tools Used

- `smbclient`: to query SMB shares
- `bash`: to script brute-force enumeration of share names
- `nano` / `chmod`: to edit and execute the script

---

## Step-by-Step Walkthrough

### 🔹 Step 1: Initial Enumeration with `smbclient`

```bash
smbclient -L //target.ine.local -N
