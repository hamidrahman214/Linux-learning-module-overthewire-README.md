## Level 5-6 
***Aim:*** To find the password in a file in the `in here` directory with the following properties
- human-readable
- 1033 bytes in size
- not executable

***Action taken:***
- ran the `cd inhere` command to enter the `inhere` directory
- used the `ls` command to list the contents
- After seeing that there are a few directories
- I ran the 'find' command which is used to search for files in a directory hierachy
- I saw an error in my command, I needed to add space to the option `-typef`
```bash
find . -type f -size 1033c ! -executable
```
***options used:***
- `find .` - start the search in the current directory
- `-type f` used to search for only regular files
- `-size 1033c` file size must be exactly 1033 bytes
- `! -executable` File must NOT be executable by the current user

This printed the file `./maybehere07/.file2`
I ran the `cat` command to list the contents in the file
```bash
cat ./maybehere07/.file2
```
***Password:**** `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

<img width="1440" height="564" alt="image" src="https://github.com/user-attachments/assets/5373f31d-be98-494d-89bd-d73124d520b8" />
