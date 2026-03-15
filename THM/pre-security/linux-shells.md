# Linux Shells

**Platform:** TryHackMe  
**Date:** 2026-03-15  
**Diff:** Easy

## Description
working with bash shell

## What am learned
-Working on dict: pwd, cd, ls , cat, grep, zsh (change shell?)

-Shells types: Friendly Interactive Shell, z shell

-Scripting: .sh (extension) , variables (read name), loops, conditional statements
## Tools and commands
```bash
nano first_script.sh
```
```bash
#!/bin/bash
echo "Hey, what’s your name?"
read name
echo "Welcome, $name"
```
```bash
chmod +x first_script.sh # execution permission to script
```
```bash
#!/bin/bash
for i in {1..10};
do
echo $i
done
```
```bash
#!/bin/bash
echo "Please enter your name first:"
read name
if [ "$name" = "Stewart" ]; then
        echo "Welcome Stewart! Here is the secret: THM_Script"
else
        echo "Sorry! You are not authorized to access the secret."
fi
```
