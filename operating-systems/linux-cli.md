# Linux CLI Basics

We will use one common folder for all examples:

/home/ash/lab

Structure:
/home/ash/lab
├── users.txt
├── passwords.txt
└── tools/

--------------------------------

## Navigation

Go to folder
cd /home/ash/lab

Check current directory
pwd

List files
ls

List hidden files
ls -a

Check current user
whoami

Clear terminal
clear

--------------------------------

## File Creation

Create file
touch targets.txt

Create folder
mkdir scans

--------------------------------

## Delete

Delete file
rm users.txt

Delete folder
rm -r scans

--------------------------------

## Copy / Move

Copy file
cp passwords.txt backup.txt

Rename file
mv backup.txt old-passwords.txt

Move file to folder
mv old-passwords.txt tools/

--------------------------------

## Viewing Files

Show content
cat passwords.txt

Scrollable view
less passwords.txt

First lines
head passwords.txt

Last lines
tail passwords.txt

--------------------------------

## Searching

Find file
find /home/ash/lab -name passwords.txt

Find folder
find /home/ash/lab -type d -name tools

--------------------------------

## Permissions

Make executable
chmod +x script.sh

--------------------------------

## SSH

Connect to remote machine
ssh ash@10.10.10.10
