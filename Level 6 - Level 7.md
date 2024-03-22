# Bandit Level 6 → Level 7
## Level Goal
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

## Commands you may need to solve this level
[ls](https://man7.org/linux/man-pages/man1/ls.1.html) , [cd](https://man7.org/linux/man-pages/man1/cd.1p.html) , [cat](https://man7.org/linux/man-pages/man1/cat.1.html) , [file](https://man7.org/linux/man-pages/man1/file.1.html) , [du](https://man7.org/linux/man-pages/man1/du.1.html) , [find](https://man7.org/linux/man-pages/man1/find.1.html) , [grep](https://man7.org/linux/man-pages/man1/grep.1.html)

# Solution:
1. Connect to bandit6 through ssh: **ssh bandit6@bandit.labs.overthewire.org -p 2220**
2. Password: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
6. find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null: /var/lib/dpkg/info/bandit7.password
7. cat ./maybehere07/.file2
8. Found Level 7's password: **z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S**
