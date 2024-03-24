# Bandit Level 8 → Level 9
## Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material
[Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)

# Solution:
1. Connect to bandit8 through ssh: **ssh bandit8@bandit.labs.overthewire.org -p 2220**
2. Password: TESKZC0XvTetK0S9xNwm25STk5iWrBvP
3. ls: data.txt
4. cat data.txt | sort | uniq -q
5. Found Level 9's password: **EN632PlfYiZbn3PhVK3XOGSlNInNE00t**
