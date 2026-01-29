## Level 8-9
***Aim:*** Find the password on a file called data.txt on the only line of text that occurs once

***Action taken:***
- I used the `ls` command to list the files in the home directory
- After seeing that data.txt was available, i ran the `sort` command to list the text of the file in alphabetical order
```bash
sort data.txt
```
- To clean up all the files presented I used the pipe operator and added in the `uniq -u` command to only print unique lines
```bash
sort data.txt | uniq -u
```
It printed `4CKMh1JI91bUIZZPXDqGanal4xvAg0JM` 

***Level 9 Password:*** `4CKMh1JI91bUIZZPXDqGanal4xvAg0JM`

<img width="476" height="217" alt="image" src="https://github.com/user-attachments/assets/45342177-0df0-4942-a328-681d5d917454" />

<img width="500" height="84" alt="image" src="https://github.com/user-attachments/assets/f8bde1bb-a97e-4e77-b346-5b810c555184" />
