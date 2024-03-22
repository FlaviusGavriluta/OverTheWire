# Bandit Level 5 → Level 6
## Level Goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

## Commands you may need to solve this level
[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html)

# Solution:
1. Connect to bandit5 through ssh: **ssh bandit5@bandit.labs.overthewire.org -p 2220**
2. Password: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
3. ls: inhere (folder)
4. cd inhere
5. ls: maybehere00  maybehere02  maybehere04  maybehere06  maybehere08  maybehere10  maybehere12  maybehere14  maybehere16  maybehere18
    maybehere01  maybehere03  maybehere05  maybehere07  maybehere09  maybehere11  maybehere13  maybehere15  maybehere17  maybehere19 (folders)
6. find . -type f -size 1033c ! -executable -exec file {} + | grep "ASCII test": ./maybehere07/.file2: ASCII text, with very long lines (1000)
7. cat ./maybehere07/.file2
8. Found Level 6's password: **P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU**
