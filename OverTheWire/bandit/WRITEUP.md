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

