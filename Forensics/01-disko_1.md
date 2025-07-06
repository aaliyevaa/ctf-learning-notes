# Challenge: DISKO 1

Source: picoCTF  

Category: Forensics 
 
Difficulty: Easy
  
Given file: disko-1.dd.gz


## Description

Can you find the flag in the given disk image?


## Hints

Maybe Strings could help? If only there was a way to do that?


##  Tools

-gzip  

-strings


## Steps Taken

1. Decompress the file:

    ```bash
    gzip -d  disko-1.dd.gz
    ```

2. Look for flag in the decompressed file:

    ```bash
    strings disko-1.dd | grep -i 'picoctf'
    ```


## What I learned 

1. .gz files are compressed files using gzip.

2. There are 2 ways to decompress and replace the file.gz with file:

    ```bash
    gunzip file.gz
    gzip -d file.gz
    ```

3. To decompress and keep the original file:
    
    ```bash
    gzip -dk file.gz
    ```

4. .dd files are disk images, a partial or complete copy of a storage device.

5. strings shows any readable text inside a file. 
