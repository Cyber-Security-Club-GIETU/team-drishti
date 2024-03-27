# Level 0

Problem Statement: Initiate bandit challenge

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |

Approach: Connect to the remote system via ssh using the given credentials.

```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

# Level 0 -> 1

Problem Statement: Read readme file

| Command | Input               | Description                        | Syntax      |
| ------- | ------------------- | ---------------------------------- | ----------- |
| cat     | file/files          | output content of a file or files  | `cat $FILE` |
| ls      | directory(optional) | lists the content of the directory | `ls $PATH`  |

Approach: Use `ls` command first to see what is inside the home directory and then use `cat` command on the required file

```Bash
ls
cat readme
```

Password for Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

# Level 1 -> 2

Problem Statement: Read dash files

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files                        | output content of a file or files                       | `cat $FILE`                 |
| ls      | directory(optional)               | lists the content of the directory                      | `ls $PATH`                  |

Approach: Since the file name contains special character i need to provide the relative path instead of only the filename. Basically instead of `cat file.txt` use `cat ./file.txt`. In this level the - (dash) may be confused with the command flags so relative path is preferred.

```Bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
cat ./-
```

Password for Level 2: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`
