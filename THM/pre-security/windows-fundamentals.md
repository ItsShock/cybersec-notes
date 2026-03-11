# Windows Fundamentals
**Platform:** TryHackMe  
**Date:** 2026-03-11  
**Difficulty:** Easy

## Description
Room about windows fundamentals

## What i learned
MSConfig , System properties, Computer Management, UAC Settings, msinfo32, resmon, cmd, registry editor
Microsoft updates, microsoft security (defender, firewall), BitLocker, Volume Shadow Copy Service
Active Directory basics

## Tools and commands
whoami, hostname, ipconfig, /? - (like man in linux) for net i should use help, cls, netstat, net

## What was difficult
**Active Directory — trust relationships concept**  
Initially confusing why a user from Domain A can't just access  
Domain B resources by default. Key insight: domains are isolated  
by design — a trust relationship must be explicitly configured  
between them to allow cross-domain resource access.  
This is also relevant from a pentesting perspective — misconfigured  
or overly permissive trust relationships are a common attack vector  
in AD environments.
