# Bandit Level 10 → Level 11
## Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material
[Base64 on Wikipedia](https://en.wikipedia.org/wiki/Base64)

# Solution:
1. Connect to bandit10 through ssh: **ssh bandit10@bandit.labs.overthewire.org -p 2220**
2. Password: G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
3. ls: data.txt
4. base64 -d data.txt
5. Found Level 11's password: **6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM**
