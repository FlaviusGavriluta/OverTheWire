# Bandit Level 12 → Level 13
## Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

## Helpful Reading Material
[Hex dump on Wikipedia](https://en.wikipedia.org/wiki/Hex_dump)

# Solution:
1. Connect to bandit11 through ssh: **ssh bandit11@bandit.labs.overthewire.org -p 2220**
2. Password: JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
3. mkdir /tmp/CyberSec
4. cp data.txt /tmp/CyberSec
5. cd /tmp/CyberSec
6. mv data.txt compressed_data.txt
7. file compressed_data.txt: compressed_data.txt: ASCII text
8. xxd -r compressed_data.txt > decompressed_data
9. file decompressed_data: decompressed_data: gzip compressed data, was "data2.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 573
10. gzip -dc decompressed_data > data2.bin
11. file data2.bin: data2.bin: bzip2 compressed data, block size = 900k
12. bunzip2 data2.bin
13. file data2.bin.out: data2.bin.out: gzip compressed data, was "data4.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 20480
14. gzip -dc data2.bin.out > data.bin
15. file data.bin: data.bin: POSIX tar archive (GNU)
16. tar -xf data.bin
17. file data5.bin: data5.bin: POSIX tar archive (GNU)
18. file data6.bin 
19. 
20. Found Level 12's password: ****
