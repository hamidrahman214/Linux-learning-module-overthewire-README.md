## Level 9-10
***Aim:*** Find the password on a file called data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

***Action taken:***
- I used the `ls` command to list the files in the home directory
- After seeing that data.txt was available, i ran the `strings` command to list the human readable text in the file
```bash
strings data.txt
```
To then only get text that contained several `=`, i included the 'grep ====' command which then printed the password
```bash
strings data.txt | grep =
```
***Level 10 Password:*** `FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`

<img width="557" height="268" alt="image" src="https://github.com/user-attachments/assets/cb01d389-c6ef-473b-a23d-22d02163c4fd" />
