## Level 18-19

***Aim:*** Access the home directory to read the readme file containing the next password, despite an altered .bashrc that forces an immediate logout on SSH login.

***Action taken:*** 
- ran the usual ssh command to try to log into level 18

I kept getting logged out but I learnt that you can run a command in the server without entering the server by adding the command in quotation marks at the end of the command line

```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"
```

***Level 19 Password:*** `cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8`

<img width="1182" height="1020" alt="image" src="https://github.com/user-attachments/assets/a72483e5-78a4-40af-9818-bff778fc22b9" />
