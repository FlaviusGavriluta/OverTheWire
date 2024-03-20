# Bandit Level 0 → Level 1
## Level Goal
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Commands you may need to solve this level

[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html)

# Solution:
1. Connect to bandit0 through ssh: **ssh bandit0@bandit.labs.overthewire.org -p 2220**
2. Password: bandit0
3. ls: readme (file)
4. cat readme
5. Found Level 1's password: **NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**
