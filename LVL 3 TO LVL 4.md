## Level 3 → Level 4

### Objective

Find the password for Level 4 from a hidden file inside the `inhere` directory.

### Step 1: List the files using ls command

<img width="155" height="29" alt="image" src="https://github.com/user-attachments/assets/290da1ea-defc-45b5-b9e7-e2c5461d9b87" />

### Step 2: Enter the `inhere` directory

Use the `cd` command to move into the directory:

<img width="269" height="29" alt="image" src="https://github.com/user-attachments/assets/a0910875-1506-4da7-90f2-085797e7e457" />

`cd` is used to change the current directory.

### Step 3: List the hidden files using ls -la command

<img width="515" height="69" alt="image" src="https://github.com/user-attachments/assets/3afc60ed-c80a-48ed-b21a-5d4196545384" />

The output shows a hidden file:

<img width="344" height="18" alt="image" src="https://github.com/user-attachments/assets/4c26add3-6d6d-4ccd-97cd-b5fd8b70199b" />

`-a` displays all files, including hidden files.

### Step 4: Read the hidden file using cat command

<img width="343" height="30" alt="image" src="https://github.com/user-attachments/assets/44cc8e05-890d-4e0d-9133-0d54a06a6aca" />

The output is the password for **Level 4**.

### Step 5: Exit Level 3

After noting the password:

<img width="400" height="53" alt="image" src="https://github.com/user-attachments/assets/5af70509-4166-4d23-931d-08f3aff9e374" />

This closes the current SSH session.

### Step 6: Log in to Level 4 using ssh command: ssh bandit4@bandit.labs.overthewire.org -p 2220
<img width="491" height="173" alt="image" src="https://github.com/user-attachments/assets/24f3b6b1-4502-43a3-a4d5-848ab4547c7d" />

Enter the password obtained from: cat .hidden

### Step 7: Enter the password obtained above

After entering the password, you will be directed to **Level 4** officially.
