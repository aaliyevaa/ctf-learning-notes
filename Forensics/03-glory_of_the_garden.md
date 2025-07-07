## Challenge: Glory of the Garden

# Details

- Source: picoCTF 2019
- Category: Forensics
- Difficulty: Easy
- Given file: garden.jpg


# Description

The garden contains more than it seems


# Hints

What is a hex editor?


# Tools

- xxd


# Steps taken

1. Analyze the hex codes of the image which contained the flag.


# What I learned

1. A hex editor lets us look at raw binary data in hexadecimal form. We can see how it exists on the disk, including hidden, deleted or embedded data.

2. Hex editors are useful in recovering deleted data.

3. CLI tools are:
    - xxd - built in hexdump tool in Linux
    - hexdump - prints hex view of the files
    - hd - alternative to hexdump

4. All file types start with a specific series of numbers showing their extension. If a file extension is faked, the header will expose it.


# Helpful References

1. [Hex Editor](https://ctf101.org/forensics/what-is-a-hex-editor/)
