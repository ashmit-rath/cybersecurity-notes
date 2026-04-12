# Linux Fundamentals

Basic Linux commands used in cybersecurity.

--------------------------------

# Navigation

pwd  
Print working directory

ls  
List files

ls -la  
List hidden files with details

cd folder  
Change directory

cd ..  
Go back

cd ~  
Home directory

clear  
Clear terminal

--------------------------------

# File Operations

touch file.txt  
Create file

mkdir folder  
Create directory

cp file1 file2  
Copy file

mv file1 file2  
Rename file

mv file folder/  
Move file

rm file.txt  
Delete file

rm -r folder  
Delete folder

--------------------------------

# File Viewing

cat file.txt  
Show file content

less file.txt  
Scrollable view

head file.txt  
Top lines

tail file.txt  
Last lines

--------------------------------

# User Commands

whoami  
Current user

id  
User id and groups

sudo command  
Run as admin

--------------------------------

# Permissions

ls -l  
View permissions

chmod +x file  
Execute permission

chmod 777 file  
Full permission

chown user file  
Change owner

--------------------------------

# Search

find / -name file.txt  
Search file

grep "text" file.txt  
Search inside file

grep -r "text" .  
Recursive search

--------------------------------

# Networking

ping google.com  
Check connectivity

ssh user@ip  
Remote login

scp file user@ip:/path  
Copy file to remote

--------------------------------

# Download Files

wget http://example.com/file  
Download file

curl http://example.com  
Fetch URL content

--------------------------------

# System Info

uname -a  
System info

history  
Command history

man ls  
Help manual

--------------------------------

# Hidden Files

ls -a  
Show hidden files

. hidden file indicator

--------------------------------

# Processes

ps  
Running processes

ps aux  
Detailed process list

kill PID  
Kill process

--------------------------------

# Echo

echo hello  
Print output

echo $USER  
Show variable

--------------------------------

# Python

python3 file.py  
Run python file

--------------------------------

# Operators

&  
Run in background  
example: command &

&&  
Run second command if first success  
example: ls && pwd

>  
Overwrite file  
echo hello > file.txt

>>  
Append file  
echo hello >> file.txt

|  
Pipe output  
cat file | grep hello
