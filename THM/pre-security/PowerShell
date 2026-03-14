# PowerShell
**Platform:** TryHackMe  
**Date:** 2026-03-14 
**Difficulty:** Easy

## Description
Room about powershell fundamentals

## What am learned
Get-Command, Get-Help, Get-Alias
-Navigating files: dir (like ls), Set-Location (like cd) , New-Item (like mkdir), Remove-Item (like rmdir), Copy-Item (like cp) , Move-Item (like mv), Get-Content (like cat)

Piping ("|"), Where-Object, Select-Object , Select-String (like grep in linux/unix or findstr in cmd) 
###Properties:
-ne: "not equal". This operator can be used to exclude objects from the results based on specified criteria.
-gt: "greater than". This operator will filter only objects which exceed a specified value. It is important to note that this is a strict comparison, meaning that objects that are equal to the specified value will be excluded from the results.
-ge: "greater than or equal to". This is the non-strict version of the previous operator. A combination of -gt and -eq.
-lt: "less than". Like its counterpart, "greater than", this is a strict operator. It will include only objects which are strictly below a certain value.
-le: "less than or equal to". Just like its counterpart -ge, this is the non-strict version of the previous operator. A combination of -lt and -eq.

--System: Get-ComputerInfo, Get-LocalUser, Get-NetIPConfiguration, Get-NetIPAddress
-Others: Get-Process, Get-Service, Get-NetTCPConnection
-Scripting: Invoke-Command, 

## Tools and commands
Get-Command -CommandType "Function"
Install-Module -Name "PowerShellGet"
Get-Help New-LocalUser -examples

Set-Location -Path ".\Documents"
New-Item -Path ".\captain-cabin\captain-wardrobe" -ItemType "Directory"

Get-ChildItem | Sort-Object Length 
Get-ChildItem | Where-Object -Property "Extension" -eq ".txt"

Get-FileHash -Path

## What was difficult
Get-ChildItem | Sort-Object Length -Descending | Select-Object -First 1

Invoke-Command -ComputerName RoyalFortune -ScriptBlock {Get-Service}
