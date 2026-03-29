# Nmap basics

**Platform:** TryHackMe  
**Date:** 2026-03-26  
**Diff:** Easy

## Description


## What am learned

IP range using: -
IP subnet using: /

-PS[portlist], -PA[portlist], -PU[portlist]

Option ; Explanation
-sT	; TCP connect scan – complete three-way handshake
-sS	; TCP SYN – only first step of the three-way handshake
-sU	; UDP scan
-F	; Fast mode – scans the 100 most common ports
-p[range]	; Specifies a range of port numbers – -p- scans all the ports

## Commands 

nmap -sS -Pn -p- {ip} | grep "/tcp" | grep "open" | wc -l

nmap -sV -Pn {ip}

T0 (paranoid)	9.8 hours
T1 (sneaky)	27.53 minutes
T2 (polite)	40.56 seconds
T3 (normal)	0.15 seconds
T4 (aggressive)	0.13 seconds

-oN <filename> - Normal output
-oX <filename> - XML output
-oG <filename> - grep-able output (useful for grep and awk)
-oA <basename> - Output in all major formats
