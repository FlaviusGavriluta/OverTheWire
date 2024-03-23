# Bandit Level 7 → Level 8
## Level Goal
The password for the next level is stored in the file data.txt next to the word millionth

## Commands you may need to solve this level
[man](https://man7.org/linux/man-pages/man1/man.1.html), grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

# Solution:
1. Connect to bandit7 through ssh: **ssh bandit7@bandit.labs.overthewire.org -p 2220**
2. Password: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
3. ls: data.txt
4. grep "millionth" data.txt
5. Found Level 8's password: **TESKZC0XvTetK0S9xNwm25STk5iWrBvP**
