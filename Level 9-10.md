## Level 9-10
***Aim:*** Find the password on a file called data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

***Action taken:***
- I used the `ls` command to list the files in the home directory
- After seeing that data.txt was available, i ran the `strings` command to list the human readable text in the file
```bash
strings data.txt
```
To then only get text that contained a `=`, i included the 'grep =' command which then printed the password
```bash
strings data.txt | grep =
```
***Level 10 Password:*** `FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`
