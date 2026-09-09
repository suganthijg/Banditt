## Level 2 → Level 3

### Objective

Find the password for Level 3 from a file whose name contains spaces.

### Step 1: List the files using ls command

<img width="219" height="38" alt="image" src="https://github.com/user-attachments/assets/cc83a61a-44f8-4723-8689-f99b686bcab7" />

The output shows a file named:
--spaces in this filename--

### Step 2: Read the file using cat command

Since the filename contains spaces, enclose the filename in quotation marks:

<img width="421" height="23" alt="image" src="https://github.com/user-attachments/assets/080bf3bc-d7e5-4e08-b230-7f91e2dc368f" />

The quotation marks tell Linux to treat the entire text as a single filename.

The output is the password for **Level 3**.

### Step 3: Exit Level 2

After noting the password: use exit command

<img width="363" height="46" alt="image" src="https://github.com/user-attachments/assets/c7d16417-ae58-4ac8-ad85-c43d5a35e9c5" />

This closes the current SSH session.

### Step 4: Log in to Level 3 using ssh command

<img width="529" height="173" alt="image" src="https://github.com/user-attachments/assets/436488bc-e021-49ca-959d-2f1404b4d159" />

Enter the password obtained from: cat "--spaces in this filename--"

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 3** officially.
