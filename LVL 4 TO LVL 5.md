## Level 4 → Level 5

### Objective

Find the password for Level 5 from the only human-readable file inside the `inhere` directory.

### Step 1: List the files using ls command

<img width="161" height="26" alt="image" src="https://github.com/user-attachments/assets/23a1a34d-c3be-4fa3-991b-7eb3c77beb71" />

### Step 2: Enter the `inhere` directory

<img width="212" height="31" alt="image" src="https://github.com/user-attachments/assets/c3837b7d-5be0-4eb7-a09a-05df7445da63" />

`cd` is used to change the current directory.

### Step 3: List the files using ls command

<img width="265" height="17" alt="image" src="https://github.com/user-attachments/assets/f8a5138d-4505-4cbf-ac32-d2113ad9d256" />

You will see several files:

<img width="669" height="32" alt="image" src="https://github.com/user-attachments/assets/b7fdba82-b838-41ed-855a-04f16f90fd9e" />

### Step 4: Check the type of each file

Use the `file` command:

<img width="470" height="157" alt="image" src="https://github.com/user-attachments/assets/fe658512-4b44-43f1-8c5f-b3b2832d9b51" />

`file` identifies the type of data stored in each file.

Among the files, one will be identified as **ASCII text** (human-readable).

### Step 5: Read the human-readable file

For example, if the output shows that `-file07` is ASCII text:

<img width="296" height="35" alt="image" src="https://github.com/user-attachments/assets/71f3c5bc-4a1d-4b49-8600-21b20c8305fb" />

The output is the password for **Level 5**.

### Step 6: Exit Level 4

After noting the password:

<img width="374" height="44" alt="image" src="https://github.com/user-attachments/assets/8ccb49eb-0f25-4199-bff6-f385155fc82e" />

This closes the current SSH session.

### Step 7: Log in to Level 5 using ssh command : ssh bandit5@bandit.labs.overthewire.org -p 2220


Enter the password obtained from the human-readable file.

### Step 8: Enter the password obtained above

After entering the password, you will be directed to **Level 5** officially.
