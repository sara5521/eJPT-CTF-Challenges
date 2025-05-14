# SMB Anonymous Access

## Description

There is a Samba share that allows anonymous access. Wonder what's in there!

This challenge demonstrates how unauthenticated users can sometimes access sensitive files through misconfigured SMB shares.

## Objectives

- Enumerate available SMB shares on the target.
- Identify which ones allow anonymous access.
- Access the anonymous share and retrieve the flag.

## Tools Used

- `nmap`
- `smbclient`
- Bash scripting

## Flag

`FLAG{56a55b23a464f5b8893fe22c6e3d611}`
