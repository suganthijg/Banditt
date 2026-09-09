## Level 10 → Level 11

### Objective

Find the password for Level 11. The `data` file contains the password encoded in **Base64**.

### Step 1: List the files using ls command

<img width="221" height="36" alt="image" src="https://github.com/user-attachments/assets/412c7c89-dce2-4ad7-a4de-8d00b881995d" />

### Step 2: Decode the text using base64 command

Use:

<img width="404" height="26" alt="image" src="https://github.com/user-attachments/assets/45c16bcb-7d66-4c2e-bd01-6883d726a586" />

`base64 -d` decodes the Base64 encoded content into readable text.

The output is the password for **Level 11**.

### Step 3: Exit Level 10

After noting the password:

<img width="356" height="49" alt="image" src="https://github.com/user-attachments/assets/8f96d776-a092-4ecb-959e-1404d0be47a0" />

This closes the current SSH session.

### Step 4: Log in to Level 11 using ssh command: ssh bandit11@bandit.labs.overthewire.org -p 2220

<img width="599" height="173" alt="image" src="https://github.com/user-attachments/assets/20df67bd-00e5-4f70-b074-7941fc784416" />


Enter the password obtained from: base64 -d data.txt

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 11** officially.
