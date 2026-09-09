## Level 8 → Level 9

### Objective

Find the password for Level 9. The password is the only line in the `data` file that occurs only once.

### Step 1: List the files using ls command

<img width="167" height="36" alt="image" src="https://github.com/user-attachments/assets/6fb72e3e-6666-42e4-8750-1823f79cdd8f" />

### Step 2: Find the unique line using sort and uniq commands

<img width="305" height="29" alt="image" src="https://github.com/user-attachments/assets/eed98d2e-0f00-4c6e-8998-7f640c8902f9" />

`sort` arranges the lines in order, and `uniq -u` displays the line that occurs only once.

The output is the password for **Level 9**.

### Step 3: Exit Level 8

After noting the password:

<img width="410" height="58" alt="image" src="https://github.com/user-attachments/assets/fc24138b-4afc-477a-8fd5-d5161df2fa77" />

This closes the current SSH session.

### Step 4: Log in to Level 9 using ssh command :ssh bandit9@bandit.labs.overthewire.org -p 2220

<img width="497" height="175" alt="image" src="https://github.com/user-attachments/assets/aacc0add-b3af-49d2-90b2-fd0615c9eefa" />

Enter the password obtained from: sort data.txt | uniq -u

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 9** officially.
