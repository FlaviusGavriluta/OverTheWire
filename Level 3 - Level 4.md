# Bandit Level 3 → Level 4
## Level Goal
The password for the next level is stored in a hidden file in the inhere directory.

## Commands you may need to solve this level
[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html)

# Solution:
1. Connect to bandit3 through ssh: **ssh bandit3@bandit.labs.overthewire.org -p 2220**
2. Password: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
3. ls: inhere (folder)
4. cd inhere
5. ls -a: .hidden (file)
6. cat .hidden
7. Found Level 4's password: **2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe**
