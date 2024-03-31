# WRITEUP

Certainly! Here's an explanation of each column in the table:

1. **Command**: name of the command
2. **Input**: input required for the command.
3. **Description**: provide a brief description of what the command does or its purpose.
4. **Syntax**: syntax or usage of the command.

# Level 0

Problem Statement: Initiate bandit challenge

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |

Approach: Connect to the remote system via ssh using the given credentials.

```Bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

# Level 0 - 1

Problem Statement: Read file

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

# Level 1 - 2

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

# Level 2 - 3

Problem Statement: Read dash files

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files                        | output content of a file or files                       | `cat $FILE`                 |
| ls      | directory(optional)               | lists the content of the directory                      | `ls $PATH`                  |

Approach: Use `ls` to list all the files in the current directory. Since the file name contains spaces , we need to enclose it with single/double quotes `cat "file name with spaces"`. Another way is to escape every space with backslash `cat file\ name\ with\ spaces`

```Bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
ls
cat "spaces in this filename"
```

OR

```Bash
cat spaces\ in\ this\ filename
```

Password for Level 3: `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`

# Level 3 - 4

Problem Statement: Read hidden file

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files                        | output content of a file or files                       | `cat $FILE`                 |
| cd      | directory                         | change the directory                                    | `cd $PATH`                  |
| ls      | directory(optional)               | lists the content of the directory                      | `ls $PATH`                  |

Approach: Use `cd $PATH` to change the directory. Then use `ls` with `-a` option to display all including hidden files and directories. Then use `cat` to read the file.

```Bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
cd inhere
ls -a
cat .hidden
```

Password for Level 4: `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`

# Level 4 - 5

Problem Statement: find human readable file

| Command | Input                             | Description                                             | Syntax                      |
| ------- | --------------------------------- | ------------------------------------------------------- | --------------------------- |
| ssh     | username<br>password<br>ip & port | connect securely to remote machine and get shell access | `ssh username@host -p PORT` |
| cat     | file/files                        | output content of a file or files                       | `cat $FILE`                 |
| cd      | directory                         | change the directory                                    | `cd $PATH`                  |
| ls      | directory(optional)               | lists the content of the directory                      | `ls $PATH`                  |
| file    | file                              | return the file type                                    | `file $FILE`                |

Approach: Use `cd $PATH` to change the directory. Then use `find *` to list the file type of all the files

```Bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
cd inhere
ls -a
file *
cat ./-file07
```

Password for Level 5: `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`
