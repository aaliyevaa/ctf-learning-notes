# Challenge: hashcrack

## Details:

- Source: picoCTF 2025
- Category: Cryptography
- Difficulty: Easy
- Date Completed: 26.07.2025
- Access the server: nc verbal-sleep.picoctf.net 57819


## Description

A company stored a secret message on a server which got breached due to the admin using weakly hashed passwords. Can you gain access to the secret stored within the server?


## Hints

1. Understanding hashes is very crucial. ![Read more here](https://primer.picoctf.org/#_hashing)
2. Can you identify the hash algorithm? Look carefully at the length and structure of each hash identified.
3. Tried using any hash cracking tools?


## Tools

1. ![Online Hash Cracker Tool](https://crackstation.net/)


## Steps taken

1. I accessed the server and was given a hash. In order to procede I needed to find the password. I used the online tool to crack the hashes and capture the flag.
2. There were 3 different hashes; md5, sha1 and sha256 respectively.


## What I learned

1. Although there are ways to crack hashes manually, there are certain useful online tools as well.
2. MD5 algorithm is fast, but broken. It is possible to create different inputs that have the same hash, which is called collisions.


## Useful References

1. ![CTF Handbook 101 - Cryptography](https://ctf101.org/cryptography/overview/)
