# Bandit Level 9 → Level 10
## Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

# Solution:
1. Connect to bandit9 through ssh: **ssh bandit9@bandit.labs.overthewire.org -p 2220**
2. Password: EN632PlfYiZbn3PhVK3XOGSlNInNE00t
3. ls: data.txt
4. strings data.txt | grep "^===" Or strings data.txt | grep "^===" | grep -oP '=+[[:print:]]+' | grep -oP '[[:print:]]+$'
5. Found Level 10's password: **G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s**
