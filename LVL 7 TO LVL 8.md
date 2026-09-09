## Level 7 → Level 8

### Objective

Find the password for Level 8. The password is stored in `data.txt` next to the word `millionth`.

### Step 1: List the files using ls command

<img width="161" height="27" alt="image" src="https://github.com/user-attachments/assets/3a1467c1-026c-4296-abaf-939e4cc71dc1" />

### Step 2: Find the password using grep command

<img width="340" height="28" alt="image" src="https://github.com/user-attachments/assets/6980973d-1fa2-4644-a0a1-f67647a95ddf" />

`grep` is used to search for a specific word or pattern inside a file.

The output is:

<img width="370" height="24" alt="image" src="https://github.com/user-attachments/assets/b5b00b56-bd9a-430d-97c7-8c77b91091aa" />

The value next to `millionth` is the password for **Level 8**.

### Step 3: Exit Level 7

After noting the password:

<img width="409" height="51" alt="image" src="https://github.com/user-attachments/assets/35616478-7b29-494f-8571-fed1b196ecad" />

This closes the current SSH session.

### Step 4: Log in to Level 8 using ssh command : ssh bandit8@bandit.labs.overthewire.org -p 2220

<img width="483" height="171" alt="image" src="https://github.com/user-attachments/assets/baa386fb-9158-44e7-8971-14b8d8652098" />

Enter the password obtained from: grep millionth data.txt

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 8** officially.
