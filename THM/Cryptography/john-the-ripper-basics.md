# John The Ripper - Basics

**Platform:** TryHackMe  
**Date:** 2026-03-31/2026-04-01
**Diff:** Easy

## Tools

John The Ripper, extended version Jumbo John,  hash-identifier

## What am learned

-P (Polynomial Time): Class P covers the problems whose solution can be found in polynomial time. Consider sorting a list in increasing order. The longer the list, the longer it would take to sort; however, the increase in time is not exponential.
-NP (Non-deterministic Polynomial Time): Problems in the class NP are those for which a given solution can be checked quickly, even though finding the solution itself might be hard. In fact, we don’t know if there is a fast algorithm to find the solution in the first place.

NTHash / NTLM , Word Mangling

## Commands

john [options] [file path]

john --wordlist=/usr/share/wordlists/rockyou.txt hash_to_crack.txt

python3 hash-id.py

john --format=LM --wordlist=/usr/share/wordlists/rockyou.txt ntlm.txt

unshadow [path to passwd] [path to shadow]

zip2john [options] [zip file] > [output file]

rar2john [rar file] > [output file]

ssh2john [id_rsa private key file] > [output file]
