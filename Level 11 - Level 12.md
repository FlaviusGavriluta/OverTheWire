# Bandit Level 11 → Level 12
## Level Goal
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Helpful Reading Material
[Rot13 on Wikipedia](https://en.wikipedia.org/wiki/ROT13)

# Solution:
1. Connect to bandit11 through ssh: **ssh bandit11@bandit.labs.overthewire.org -p 2220**
2. Password: 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
3. ls: data.txt
4. tr 'A-Za-z' 'N-ZA-Mn-za-m' < data.txt
5. Found Level 12's password: **JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv**
