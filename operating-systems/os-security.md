# Operating System Security

We will use example machine:

User: ash  
IP: 10.10.10.5  

--------------------------------

## SSH

Connect to remote system
ssh ash@10.10.10.5

Connect with port
ssh ash@10.10.10.5 -p 2222

--------------------------------

## Check User

Current user
whoami

User ID
id

Groups
groups

--------------------------------

## Privileges

Check sudo permissions
sudo -l

Switch user
su root

--------------------------------

## Password

Change password
passwd

--------------------------------

## System Info

Hostname
hostname

OS info
uname -a

--------------------------------

## Important for Pentesting

whoami
id
sudo -l
uname -a
hostname
