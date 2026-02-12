## Level 19-20

***Aim:*** Use the setuid binary in the homedirectory and execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

***Action taken:*** 
- ran the `ls` command
- ran the `./` command to execute the `bandit20-do` binary

```bash
./bandit20-do
```

it printed 

```bash
Run a command as another user.
  Example: ./bandit20-do whoami
```

this showed me that i can run commands as bandit 20

```bash
./bandit20-do cat etc/bandit_pass/bandit20
```

***Level 20 Password:*** `0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO`

<img width="717" height="398" alt="image" src="https://github.com/user-attachments/assets/fc085fa3-fc9e-4e02-83c0-bfc4a377724f" />
