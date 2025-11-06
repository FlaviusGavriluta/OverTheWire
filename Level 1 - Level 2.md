# Bandit Level 1 → Level 2
## Level Goal
The password for the next level is stored in a file called - located in the home directory

## Commands you may need to solve this level
[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html)

## Helpful Reading Material
[Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)

[Advanced Bash-scripting Guide - Chapter 3 - Special Characters](https://tldp.org/LDP/abs/html/special-chars.html)


# Solution:
1. Connect to bandit1 through ssh: **ssh bandit1@bandit.labs.overthewire.org -p 2220**
2. Password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

```bash
bandit1@bandit:~$ ls
-
bandit1@bandit:~$ cat < -
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```
