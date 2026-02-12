## Level 17-18

***Aim:*** find the password from the only line in file `passwords.new` that's different to file `passwords.old`

***Action taken:*** 
- I ran the `man diff` command and it mentioned that it compares files line by line
- used the `ls` command to list the contents
- ran the diff command to compare both files.

```bash
diff passwords.old passwords.new
```

showed 2 passwords which means that they were the different lines. I then ran the `grep` command to check if the password was from file `passwords.new`

```bash
grep x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO passwords.new
```
and it showed up which confirmed it.

***Level 18 Password:*** `x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO`
