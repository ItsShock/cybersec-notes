# Windows CMD

**Platform:** TryHackMe  
**Date:** 2026-03-14  
**Diff:** Easy

## Room description
Krótko o czym był, 2-3 zdania.

## What i learned
commands:
- os info commands: set, ver, systeminfo , driverquery "'command' | more" - better to read 
- networking commands: ipconfig (info about connection), ping, tracert , nslookup, netstat
- disk management: cd (like pwd), dir (like ls) , tree, cd target, cd .., mkdir, rmdir
- working with files: type (ex. read txt file), copy , move , del or erase, * (wildcard)
- process mgmt: tasklist, taskkill
/? - help , not working always

## Tools and commands
```bash
copy *.md C:\Markdown // copy all files with .md extension to folder C:\Markdown
```

```bash
tasklist /FI "imagename eq sshd.exe"
```
