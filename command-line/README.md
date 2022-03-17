# Learn the Command Line

## Navigating the File System

### Helper Commands

Helper commands for the command line include:

- `clear` to clear the terminal
- `tab` to autocomplete the line
- `↑` and `↓` to cycle through previous commands

---

### Print Working Directory (pwd)

The shell command `pwd` displays the file path from the root directory to the current working directory.

```none
test@ESPRIMO-P520:~$ pwd
/home/test
```

---

### Make Directory (mkdir)

The shell command `mkdir` is used to make a new directory in the filesystem according to its argument. If a file path is given, the new directory will be placed at the end. Otherwise, it will create a new directory in the current working directory.

```none
mkdir Python
```

---

### List (ls)

The shell command `ls` is used to list the contents of a directory. If no arguments are given, it will list the contents of the current working directory.

```none
test@ESPRIMO-P520:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

---

### Change Directory (cd)

The shell command `cd` is used to move throughout the filesystem of a computer. It accepts a variety of arguments:

- Full file paths.
- Names of children of the current directory.
- `..` the parent of the current directory.

```none
test@ESPRIMO-P520:~$ cd Python/Tutorial-01/
test@ESPRIMO-P520:~/Python/Tutorial-01$ pwd
/home/test/Python/Tutorial-01
test@ESPRIMO-P520:~/Python/Tutorial-01$ cd ..
test@ESPRIMO-P520:~/Python$ cd ../..
test@ESPRIMO-P520:/home$ cd effie/
```

---

### Create New File (touch)

The shell command `touch` creates a new file in the current working directory with the name provided.

```none
test@ESPRIMO-P520:~/Python/Tutorial-01$ touch hello.py
test@ESPRIMO-P520:~/Python/Tutorial-01$ ls
hello.py
```
