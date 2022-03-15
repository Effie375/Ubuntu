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
effie@ubuntu:~$ pwd
/home/effie
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
effie@ubuntu:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

---

### Change Directory (cd)

The shell command `cd` is used to move throughout the filesystem of a computer. It accepts a variety of arguments:

- Full file paths.
- Names of children of the current directory.
- `..` the parent of the current directory.

```none
effie@ubuntu:~$ cd Python/Tutorial-01/
effie@ubuntu:~/Python/Tutorial-01$ pwd
/home/effie/Python/Tutorial-01
effie@ubuntu:~/Python/Tutorial-01$ cd ..
effie@ubuntu:~/Python$ cd ../..
effie@ubuntu:/home$ cd effie/
```

---

### Create New File (touch)

The shell command `touch` creates a new file in the current working directory with the name provided.

```none
effie@ubuntu:~/Python/Tutorial-01$ touch hello.py
effie@ubuntu:~/Python/Tutorial-01$ ls
hello.py
```
