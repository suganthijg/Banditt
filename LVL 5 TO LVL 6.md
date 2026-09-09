## Level 5 → Level 6

### Objective

Find the password for Level 6 from a file inside the `inhere` directory.

### Step 1: List the files using ls command

<img width="179" height="35" alt="image" src="https://github.com/user-attachments/assets/dddfb22d-2ae0-400d-a12d-0066a5908432" />

### Step 2: Enter the `inhere` directory

<img width="233" height="19" alt="image" src="https://github.com/user-attachments/assets/39517ec7-1d7f-4a75-ae88-80df5b710a02" />

`cd` is used to move into the `inhere` directory.

### Step 3: List the directories using ls command

<img width="218" height="15" alt="image" src="https://github.com/user-attachments/assets/5f3e3c07-6da2-4c0b-b723-5323deda1ba5" />

The output shows multiple directories such as:

<img width="635" height="52" alt="image" src="https://github.com/user-attachments/assets/04675c0a-bb4a-434d-b427-03af39b2783b" />

### Step 4: Read the required file using cat command

The required file is located inside `maybehere07` and is named `.file2`.

<img width="341" height="31" alt="image" src="https://github.com/user-attachments/assets/f19d1561-ebfa-415b-ad5f-2777fd50b34e" />

`./` refers to the current directory, and `.file2` is a hidden file.

This is the password for **Level 6**.

### Step 5: Exit Level 5

After noting the password:

<img width="711" height="41" alt="image" src="https://github.com/user-attachments/assets/59e77b05-1a4d-49b0-89ba-ea75d1e95818" />

This closes the current SSH session.

### Step 6: Log in to Level 6 using ssh command using :  ssh bandit6@bandit.labs.overthewire.org -p 2220
 
<img width="574" height="171" alt="image" src="https://github.com/user-attachments/assets/532f7ad2-1435-4b92-97e7-120045704395" />

Enter the password obtained from: cat ./maybehere07/.file2

### Step 7: Enter the password obtained above

After entering the password, you will be directed to **Level 6** officially.
