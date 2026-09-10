## Level 15 → Level 16

### Objective

Find the password for Level 16 by connecting to a service on port `30001` using SSL/TLS.

### Step 1: Connect to the SSL service using openssl command

```bash
openssl s_client -connect localhost:30001
```
<img width="544" height="128" alt="image" src="https://github.com/user-attachments/assets/d743392f-f238-4b52-8d68-2a23c147d591" />

`openssl s_client` is used to establish a secure SSL/TLS connection with the service.
<img width="826" height="191" alt="image" src="https://github.com/user-attachments/assets/955d723a-769a-42c0-b834-98af2dc88d70" />

### Step 2: Enter the Level 15 password

After the connection is established, enter the **Level 15 password** and press `Enter`.

The server will verify the password and display:


<img width="308" height="71" alt="image" src="https://github.com/user-attachments/assets/35312eaf-ceca-429e-8b2b-ff8f7146fd6a" />


It will then provide the password for **Level 16**.

### Step 3: Exit Level 15

After noting the password:

<img width="488" height="51" alt="image" src="https://github.com/user-attachments/assets/769172ee-b071-4dfd-ac0f-77d0b2362b05" />


This closes the current SSH session.

### Step 4: Log in to Level 16 using ssh command : ssh bandit16@bandit.labs.overthewire.org -p 2220

<img width="558" height="174" alt="image" src="https://github.com/user-attachments/assets/ece0d4ac-f69e-4b89-9ad6-520c78211045" />

Enter the password obtained from the `openssl s_client` command.

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 16** officially.
