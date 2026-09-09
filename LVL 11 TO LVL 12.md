## Level 11 → Level 12

### Objective

Find the password for Level 12. The contents of the `data.txt` file have been encrypted using **ROT13**.

### Step 1: List the files using ls command

<img width="161" height="26" alt="image" src="https://github.com/user-attachments/assets/1a94738d-dbca-4177-a21e-90a4756cab71" />

### Step 2: Read the file using cat command

<img width="441" height="29" alt="image" src="https://github.com/user-attachments/assets/0b255e7a-c655-469b-a8c2-3a78a7503c61" />

The output contains encrypted text.

### Step 3: Decode the text using tr command
<img width="443" height="25" alt="image" src="https://github.com/user-attachments/assets/df080f6e-41eb-4bb4-b804-c5892b8ea9ae" />

Use the following command:

`tr` replaces each letter with the letter **13 positions away** in the alphabet.

For example:

* `A` → `N`
* `B` → `O`
* `N` → `A`

The output is the password for **Level 12**.

### Step 4: Exit Level 11

After noting the password:

<img width="404" height="47" alt="image" src="https://github.com/user-attachments/assets/eb0185a1-85cd-4552-bd9c-534ba46acb88" />

This closes the current SSH session.

### Step 5: Log in to Level 12 using ssh command

<img width="551" height="191" alt="image" src="https://github.com/user-attachments/assets/b432c902-c1b6-4939-bd0a-d1b5f612f057" />

Enter the password obtained from: cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

### Step 6: Enter the password obtained above

After entering the password, you will be directed to **Level 12** officially.
