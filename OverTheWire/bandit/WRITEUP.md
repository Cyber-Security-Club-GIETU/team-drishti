# WRITEUP Format

# Level number

Problem Statement: Details

Certainly! Here's an explanation of each column in the table:

1. **Command**: name of the command
2. **Input**: input required for the command.
3. **Description**: provide a brief description of what the command does or its purpose. 
4. **Syntax**: syntax or usage of the command. 

### Example
| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files | output content of a file or files | `cat $FILE` |


Approach: Your solution


### Commands Used
```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
cat *
```

### Password for next level
Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

# Lets Start the Game !

# Leve0 

Problem Statement: Log in to the game using ssh 

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |

Approach: I've found that I'll need to link up with a remote server managed by BanditLab. To make this connection, I'll be utilizing the SSH protocol, and I've got all the required credentials right here. Everything's in place, so we're ready to move forward smoothly without any obstacles. 🚀


### Commands Used
```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

# Leve0-1

Problem Statement: Locate and find the password present in the readme file , present in home directory of level 0

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ls      | directory(Optional) |  lists directory contents  | 'ls [file/directory]' |
| cat     | file or files|  gives the content of the file or files | 'cat [file/files]'|

Approach: I'm currently in the home directory (~) of Level 0.
To see what's in this directory, I'll use the 'ls' command.
Now, let's display the contents of the readme file by using the 'cat' command.
The password for the next level is kept in this file. 


### Commands Used
```Bash
ls 
cat readme
```
### Password for next level
Level 1:  `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

# Leve1-2

Problem Statement: Read the -(Dash) file , which content the password for level 2

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| ls      | directory(Optional) |  lists directory contents  | 'ls [option] [file/directory]' |
| cat     | file or files|  output the content of file or files | 'cat [option] [file/files]'|

Approach: I logged into the BanditLab1 server using SSH and the provided credentials, then navigated to Level 1's home directory. To see what's in the directory, I typed 'ls'.

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
