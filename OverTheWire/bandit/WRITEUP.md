# Level 0

Problem Statement: Initiate bandit challenge

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files | output content of a file or files | `cat $FILE` |


Approach: Connect to the remote system via ssh using the given credentials. Print all the contents in this directory. 

```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
cat *
```
Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

# Level 0-1

Problem Statement: Read dash files

| Command | Input | Description | Syntax |
| ------- | ----- | ----------- | ------ |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files | output content of a file or files | `cat $FILE` |
| ls      | directory(optional) | lists the content of the directory | `ls $PATH` |

Approach: Since the file name contains special character i need to provide the relative path instead of only the filename. Basically  instead of `cat file.txt` use `cat ./file.txt`. In this level the - (dash) may be confused with the command flags so relative path is preferred.

```Bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
cat ./-
```
Level 2: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`
