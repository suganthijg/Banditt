## Level 14 → Level 15

### Objective

Find the password for Level 15 by sending the current Level 14 password to a service running on port `30000` on localhost.

### Step 1: Check the current directory using ls command

```bash
ls
```

There may be no relevant file in the home directory.

### Step 2: Send the Level 14 password to port 30000

Use the `nc` command:

```bash
nc localhost 30000
```
<img width="318" height="29" alt="image" src="https://github.com/user-attachments/assets/e0ddba47-b3d9-47d0-ab19-a0e5e02d09cd" />


`nc` (Netcat) is used to communicate with a service through a network connection.

After running the command, paste the **Level 14 password** and press **Enter**.

The service will return the password for **Level 15**.

### Step 3: Exit Level 14

After noting the password:

```bash
exit
```
<img width="427" height="50" alt="image" src="https://github.com/user-attachments/assets/e60d447f-61a0-4074-8791-539d69e456b2" />


This closes the current SSH session.

### Step 4: Log in to Level 15 using ssh command

```bash
ssh bandit15@bandit.labs.overthewire.org -p 2220
```
<img width="578" height="185" alt="image" src="https://github.com/user-attachments/assets/a937699b-1ebe-40fe-aa9f-128c9f6a207f" />

Enter the password obtained from the `nc` command.

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 15** officially.
