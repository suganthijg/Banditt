## Level 13 → Level 14

### Objective

Log in to Level 14 using the SSH private key provided in the home directory.

### Step 1: List the files using ls command

<img width="200" height="38" alt="image" src="https://github.com/user-attachments/assets/6c751fad-3434-407e-b4a3-aaf7977acb27" />

### Step 2: Use the SSH private key to log in

The `sshkey.private` file contains the private key required to access Level 14.

Use:

```bash
ssh -i sshkey.private bandit14@localhost
```
<img width="685" height="198" alt="image" src="https://github.com/user-attachments/assets/67402a4a-e62b-4d7b-9824-98584c3b2260" />


* `-i` → specifies the private key file.
* `sshkey.private` → the private key provided for this level.
* `bandit14@localhost` → connects to the Level 14 account on the same server.

### Step 3: Enter the password if prompted

Usually, the private key allows you to log in without entering a password.

After successful login, you will see:

<img width="139" height="57" alt="image" src="https://github.com/user-attachments/assets/4a150d90-80e1-43ea-afd1-21d003743623" />


This means you have successfully reached **Level 14**.

### Step 4: Exit Level 13

If you need to return to the previous session:

```bash
exit
```

This closes the SSH session.

### Result

You have successfully completed **Level 13 → Level 14** using the provided SSH private key.
