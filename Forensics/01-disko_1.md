# Challenge: DISKO 1

Source: picoCTF 
Category: Forensics
Difficulty: Easy
Given file: disko-1.dd.gz


## Goal

Find the flag in the given disk image.


##  Tools

gzip
strings


## Steps Taken

1. Decompress the file:
    gzip -d  disko-1.dd.gz

2. Look for flag in the decompressed file:
    strings disko-1.dd | grep -i 'picoctf'


## What I learned 

- .gz files are compressed files using gzip.
- There are 2 ways to decompress and replace the file.gz with file:
    1. gunzip file.gz
    2. gzip -d file.gz
- To decompress and keep the original file:
    gzip -dk file.gz
- .dd files are disk images, a partial or complete copy of a storage device.
- strings shows any readable text inside a file. 
