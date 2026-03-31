# Hashing basics

**Platform:** TryHackMe  
**Date:** 2026-03-31
**Diff:** Easy

## Tools

crackstation.net, https://hashes.com , https://hashcat.net/wiki/doku.php?id=example_hashes

HashCat, John the Ripper

## What am learned

Hash, Hash Collision, pigeonhole effect, RockYou list, Rainbow Table, adding salt to hash

$prefix$options$salt$hash

On MS Windows, password hashes are stored in the SAM (Security Accounts Manager)

HMAC (Keyed-Hash Message Authentication Code)

HMAC(K,M) = H((K⊕opad)||H((K⊕ipad)||M))

## Commands

hexdump -C file1.txt 
md5sum *.txt
sha256sum *.txt

 hashcat -m <hash_type> -a <attack_mode> hashfile wordlist
