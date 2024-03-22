# Bandit Level 4 → Level 5
## Level Goal
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

## Commands you may need to solve this level
[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html)

# Solution:
1. Connect to bandit4 through ssh: **ssh bandit4@bandit.labs.overthewire.org -p 2220**
2. Password: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
3. ls: inhere (folder)
4. cd inhere
5. ls: -file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09 (files)
6. cat < -file07
7. Found Level 5's password: **lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR**
