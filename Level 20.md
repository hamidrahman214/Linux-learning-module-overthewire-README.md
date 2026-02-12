## Level 20

***Aim:*** Use the setuid binary in the home directory to authenticate with the previous level’s password over a local network connection and retrieve the password for the next level.

***Action taken:*** 
- Opened two terminals logged in as the same user to allow simultaneous listening and connecting
- Initially attempted to use `nc -l 1234`, which resulted in the connection stalling
- Switched to `ncat`, which provided reliable socket handling and maintained the connection as expected

```bash
ncat -l 12345
```

In a second terminal, executed the setuid binary with the same port:

```bash
./setuid_binary 12345
```

- After the connection was established, entered the previous level’s password into the listening terminal.
- The binary validated the input and returned the password for the next level.

***Level 20 Password:*** `EeoULMCra2q0dSkYj561DX7s1CpBuOBt`


Note: I initially used `nc -l 1234`, but later realised that the port wasn't explicitly specified. After adding the `-p` option to bind the listener to the correct port, the connection worked as expected.

```bash
nc -l -p 12334
```

<img width="792" height="139" alt="image" src="https://github.com/user-attachments/assets/a71518d3-2c40-4c8f-9084-3d023aba0e31" />
