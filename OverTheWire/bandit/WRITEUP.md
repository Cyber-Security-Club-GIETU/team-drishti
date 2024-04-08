# WRITEUP
Certainly! Here's an explanation of each column in the table:

1. **Command**: name of the command
2. **Input**: input required for the command.
3. **Description**: provide a brief description of what the command does or its purpose. 
4. **Syntax**: syntax or usage of the command. 

# Leve0 

Problem Statement: Initiate bandit challenge

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |

Approach: I discovered that I need to connect to a remote server hosted by BanditLab. To establish this connection, I will use the SSH protocol, and the necessary credentials are provided here. We are all set to proceed without any hurdles. 🚀


### Commands Used
```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

# Leve0-1

Problem Statement: Read the readme file , present in home directory of level0

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cat     | file or files|  output the content of file or files | 'cat [file/files]'|

Approach: I already in the home directory (~) of Level 0.
To list all the contents of the current directory, used the 'ls' command.

Next, let’s output the content of the readme file using the 'cat' command.


The password for the next level is stored in this file. 🚀 


### Commands Used
```Bash
ls 
cat readme
```

### Password for next level
Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`


# Leve1-2

Problem Statement: Read the -(Dash) file , which content the password for level 2

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cat     | file or files|  output the content of file or files | 'cat [option] [file/files]'|

Approach: using ssh and necessary credentials(found on previous lab ), I connected to the remote server of BanditLab and entered in the home directory (~) of Level 1.
To list all the contents of the current directory, I used the 'ls' command.

Next, for output the content of the -(dash) file, I used the 'cat' command :
cat < -

The password for the next level is stored in this file. 🚀 


### Commands Used
```Bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
ls 
cat < -
```

### Password for next level
Level 2: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`



# Level2-3

Problem Statement: Read a file , which have spaces in it's file name.

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|

Approach: using ssh and necessary credentials(found on previous lab ), I connected to the remote server of BanditLab and entered in the home directory (~) of Level 2.
To list all the contents of the current directory, I used the 'ls' command. 

Next, for output the content of the file which have spaces on it's file name, I used the 'cat' command with following syntax:

cat 'file name with spaces as given'

The password for the next level is stored in this file. 🚀 


### Commands Used
```Bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
ls 
cat 'spaces in this filename'
```

### Password for next level
Level 3: `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`


# Level3-4
Problem Statement:Read a hidden file

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` | 
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cd      | directory      | change directory | 'cd [option] [directory]' |  
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|

Approach: 
Using SSH and the necessary credentials obtained from the previous lab, I connected to the remote server of BanditLab and entered the home directory (~) of Level 3. Upon listing all the contents of the current directory using the 'ls' command, I used the 'cd' command to enter the 'inhere' directory. In the inhere directory, I employed the 'ls' command with the '-a' option to identify all types of files present in this particular directory. Here, I discovered a hidden file named '.hidden'.

To retrieve the contents of the '.hidden' file, I utilized the 'cat' command.

The password for the next level is stored in this file. 🚀

### Commands Used
```Bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
cd inhere
ls -a
cat .hidden
```

### Password for next level
Level 4: `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`



# Level4-5
Problem Statement:Read a human readable file

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` | 
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cd      | directory      | change directory | 'cd [option] [directory]' |  
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|
| file    | file or files |  for recognizing the type of data contained | 'file [option] [file/files]' |

Approach: Using SSH and the necessary credentials obtained from the previous lab, I connected to the remote server of BanditLab and entered the home directory (~) of Level 4. Upon listing all the contents of the current directory using the 'ls' command, I used the 'cd' command to enter the 'inhere' directory. In the inhere directory, I employed the 'ls' command with the '-a' option to identify all types of files present in this particular directory. Here, I discovered many dash(-) files.
Then I used 'file' command with required option for finding out the type of data contained in these file. Then i found a  human readable file(contained ASCII text) '-file07' .

To retrieve the contents of the '-file07' file, I utilized the 'cat' command.

The password for the next level is stored in this file. 🚀


### Commands Used
```Bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
cd inhere
ls -a
cat ./-file07
```

### Password for next level
Level 5: `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`


# Level5-6
Problem Statement: Search and read a file , which have following properties : <br>
human-readable<br>
1033 bytes in size<br>
not executable

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` | 
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cd      | directory     | change directory | 'cd [option] [directory]' |
| find    | path          | searching for files based on diverse criteria| 'find [path] [options] [expression]'|
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|

Approach: Using SSH and the necessary credentials obtained from the previous lab, I connected to the remote server of BanditLab and entered the home directory (~) of Level 5. Upon listing all the contents of the current directory using the 'ls' command, I used the 'cd' command to enter the 'inhere' directory. In the inhere directory, I employed the 'ls' command with the '-a' option to list out all types of files present in this particular directory. Here, I discovered many some hidden files and many different type of directory .
Then I used 'find' command with required option for finding out the perticluar type of file as per the problem statement. Then i found a file with desired propertie which was present in the './maybehere07/.file2' .

To retrieve the contents of the '.file2' file, I utilized the 'cat' command.

The password for the next level is stored in this file. 🚀


### Commands Used
```Bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
cd inhere
ls
find . -type f -size 1033c ! -executable
cat ./maybehere07/.file2
```

### Password for next level
Level 6: `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU`


# Level6-7
Problem Statement: Search and read a file , which have following properties : <br>
owned by user bandit7<br>
owned by group bandit6<br>
33 bytes in size<br>

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` | 
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cd      | directory     | change directory | 'cd [option] [directory]' |
| find    | path          | searching for files based on diverse criteria| 'find [path] [options] [expression]'|
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|

Approach: Using SSH and the necessary credentials obtained from the previous lab, I connected to the remote server of BanditLab and entered the home directory (~) of Level 6. Then I used 'find' command with required option for finding out the perticluar type of file as per the problem statement. Then i found a file with desired propertie which was present in the '/var/lib/dpkg/info/bandit7.password' .

To retrieve the contents of the '.password' file, I utilized the 'cat' command.

The password for the next level is stored in this file. 🚀


### Commands Used
```Bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
cd inhere
ls
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

### Password for next level
Level 7: `z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S`


# Level7-8
Problem Statement: The password for the next level is stored in the file data.txt next to the word millionth

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` | 
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cat     | file or files |  output the content of file or files | ' cat [option] [file/files] '|
| grep    | pattern [files] | searching and manipulating text patterns within files | grep [options] pattern [files] | 


Approach: Using SSH and the necessary credentials obtained from the previous lab, I connected to the remote server of BanditLab and entered the home directory (~) of Level 7. Then I used 'ls' command and found 'data.txt is right at the home directory. Hence, we don’t have to perform cd. Then i used 'cat data.txt | grep millionth' , for geting the password.🚀


### Commands Used
```Bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
ls
cat data.txt | grep millionth
```

### Password for next level
Level 8: `TESKZC0XvTetK0S9xNwm25STk5iWrBvP`
