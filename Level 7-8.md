## Level 7-8
***Aim:*** Find the password on a file called data.txt next to the word millionth

***Action taken:***
- I used the `ls` command to list the files in the home directory
- After seeing that data.txt was available, i ran the `vim` command to try looking for millionth
```bash
vim data.txt
```
There were manynlines of text so i used the `grep` command which can be used to search for keywords.
```bash
grep millionth data.txt
```
It printed `millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc` 

***Password:*** `dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc`

<img width="559" height="193" alt="image" src="https://github.com/user-attachments/assets/9eff9ef3-90e7-4cc7-bcd5-b476b5f2b2a6" />
