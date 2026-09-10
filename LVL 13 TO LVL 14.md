## Level 13 → Level 14

### Objective

Log in to Level 14 using the SSH private key provided in the home directory.

### Step 1: List the files using ls command

```bash
ls
```

The output shows:

```text
sshkey.private
```

### Step 2: Use the SSH private key to log in

The `sshkey.private` file contains the private key required to access Level 14.

Use:

```bash
ssh -i sshkey.private bandit14@localhost
```

* `-i` → specifies the private key file.
* `sshkey.private` → the private key provided for this level.
* `bandit14@localhost` → connects to the Level 14 account on the same server.

### Step 3: Enter the password if prompted

Usually, the private key allows you to log in without entering a password.

After successful login, you will see:

```text
bandit14@bandit:~$
```

This means you have successfully reached **Level 14**.

### Step 4: Exit Level 13

If you need to return to the previous session:

```bash
exit
```

This closes the SSH session.

### Result

You have successfully completed **Level 13 → Level 14** using the provided SSH private key.
