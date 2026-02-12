## Level 12 - 13

***Aim:*** Extract the password for the next level from data.txt, which contains a repeatedly compressed hexdump, by working in a temporary directory under /tmp

***Action taken:***

- Created a secure temporary working directory and confirmed the presence of data.txt.
- Inspected the file and identified it as a hexadecimal dump.
- Reversed the hexdump into its original binary form using xxd.
  
```bash
mkdir /tmp/Dir1
cp data.txt /tmp/Dir1
cd /tmp/Dir1
xxd -r data.txt > reverse.txt
```
- Determined the file type and decompressed it accordingly.

```bash
file reverse.txt
mv reverse.txt reverse.gz
gzip -d reverse.gz
```
Repeated the cycle of:

- identifying the file type,
- renaming when the appropriate file extension was required,
- decompressing with the appropriate tool.

```bash
file <filename>
gunzip <filename>.gz
bunzip2 <filename>.bz2
tar -xf <filename>.tar
```

I repeated steps till i reached file `data8` which was listed as a `ASCII text` file, this was the file that contained the password.

```bash
cat  data8
```

***Level 13 Password:*** `FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn`

<img width="1520" height="664" alt="image" src="https://github.com/user-attachments/assets/db0abfd8-647f-4180-8383-2dc87e6ac97e" />
