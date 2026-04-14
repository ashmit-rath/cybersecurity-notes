# Windows PowerShell

PowerShell is advanced CLI for Windows using cmdlets.

Format:
Verb-Noun

Example:
Get-Process
Get-Service

---

# Basic Commands

## ps
Shows processes

Example:
ps

---

## Get-Content
Read file content

Example:
Get-Content file.txt

---

## Set-Location
Change directory

Example:
Set-Location Desktop

Alias:
cd

---

## Get-Command
Lists commands

Example:
Get-Command

## Get-Command -CommandType Function
List functions

Example:
Get-Command -CommandType Function

---

## Get-Help
Shows help

Example:
Get-Help Get-Process

---

# Modules

## Find-Module
Search modules

Example:
Find-Module

---

## Install-Module

Example:
Install-Module -Name PowerShellGet

---

# Users

## Get-LocalUser
List users

Example:
Get-LocalUser

---

# Creating Items

## New-Item
Create file/folder

Example:
New-Item test.txt

---

# Pipeline

Uses |

Example:
Get-Process | Select-Object Name
