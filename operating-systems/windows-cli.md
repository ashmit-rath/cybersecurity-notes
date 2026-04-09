# Windows CLI Basics

We will use one common folder:

C:\Users\ash\lab

Structure:
C:\Users\ash\lab
├── users.txt
├── passwords.txt
└── tools

--------------------------------

## Navigation

Go to folder
cd C:\Users\ash\lab

Check current directory
cd

List files
dir

List hidden files
dir /a

Clear screen
cls

--------------------------------

## File Creation

Create file
type nul > targets.txt

Create folder
mkdir scans

--------------------------------

## Delete

Delete file
del users.txt

Delete folder
rmdir scans

Delete folder recursively
rmdir /s scans

--------------------------------

## Copy / Move

Copy file
copy passwords.txt backup.txt

Rename file
rename backup.txt old-passwords.txt

Move file
move old-passwords.txt tools

--------------------------------

## Viewing Files

Show content
type passwords.txt

--------------------------------

## Searching

Search file in current folder
dir passwords.txt

Search recursively
dir /s passwords.txt

Search hidden files
dir /a

--------------------------------

## User Info

Current user
whoami

Hostname
hostname
