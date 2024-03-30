# Bandit Level 13 → Level 14
## Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

## Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

## Helpful Reading Material
[SSH/OpenSSH/Keys](https://help.ubuntu.com/community/SSH/OpenSSH/Keys)

# Solution:
1. Connect to bandit13 through ssh: **ssh bandit13@bandit.labs.overthewire.org -p 2220**
2. Password: wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
3. ls: sshkey.private
4. file sshkey.private: sshkey.private: PEM RSA private key
5. pwd: /home/bandit13
6. ssh -i /home/bandit13/sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
7. yes
8. cat /etc/bandit_pass/bandit14
9. Found Level 14's password: **fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq**
