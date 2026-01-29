## Level 6-7
***Aim:*** Find the password somewhere on the server and has all of the following properties:
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size

***Action taken:***
- I used the `find` command similar to the previous level
```bash
find / -type f -user bandit7 -group bandit6 -size 33c
```
`/` was used after the `find` command to search the entire filesystem, starting from the root directory
After seeing many permission denied messages, i redirected all of them to /dev/null by adding 2> /dev/null to my command
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2> /dev/null
```
I ended up finding only one file `/var/lib/dpkg/info/bandit7.password`
i followed it with the `cat` command
```bash
cat /var/lib/dpkg/info/bandit7.password
```
***Password:*** `morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`

<img width="830" height="299" alt="image" src="https://github.com/user-attachments/assets/61e2b910-a153-443f-9859-ba2acd99ce9d" />

After seeing many permission denied messages,I redirected all of them to /dev/null by adding 2> /dev/null to my command

This printed the file `./maybehere07/.file2`
I ran the `cat` command to list the contents in the file
```bash
cat ./maybehere07/.file2
```
***Pasword:*** `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

<img width="3" height="1" alt="image" src="https://github.com/user-attachments/assets/5754a7fc-9e87-4e63-9585-b1f7f489a89f" />
