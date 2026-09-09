## Level 10 → Level 11

### Objective

Find the password for Level 11. The `data` file contains the password encoded in **Base64**.

### Step 1: List the files using ls command

<img width="177" height="33" alt="image" src="https://github.com/user-attachments/assets/7fa2055c-05dc-4816-893d-7970cc34be33" />

### Step 2: Decode the text using base64 command

<img width="353" height="30" alt="image" src="https://github.com/user-attachments/assets/96ab5743-0469-41e7-b116-e763f4431eec" />

Use:
base64 -d data.txt

`base64 -d` decodes the Base64 encoded content into readable text.

The output is the password for **Level 11**.

### Step 4: Exit Level 10

After noting the password:

<img width="390" height="56" alt="image" src="https://github.com/user-attachments/assets/b5d716ad-85ec-41fa-827e-0a630fa6aaa2" />

This closes the current SSH session.

### Step 5: Log in to Level 11 using ssh command : ssh bandit11@bandit.labs.overthewire.org -p 2220

<img width="566" height="182" alt="image" src="https://github.com/user-attachments/assets/5384baf3-8338-4da0-99b5-2e0202c78125" />

Enter the password obtained from: base64 -d data.txt

### Step 6: Enter the password obtained above

After entering the password, you will be directed to **Level 11** officially.
