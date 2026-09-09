## Level 9 → Level 10

### Objective

Find the password for Level 10 from the `data` file. The password is stored among several human-readable strings and is preceded by several `=` characters.

### Step 1: List the files using ls command

<img width="160" height="34" alt="image" src="https://github.com/user-attachments/assets/6788f333-ff0a-4423-b346-4f719dea31af" />


### Step 2: Find human-readable strings using strings command

<img width="352" height="14" alt="image" src="https://github.com/user-attachments/assets/5cf4b679-e80b-4171-bf14-55d48de4cdcb" />

`strings` displays readable text found inside a file.

### Step 3: Search for the password using grep command

To find the line containing several `=` characters:

<img width="317" height="185" alt="image" src="https://github.com/user-attachments/assets/8a03c5ef-1106-44c0-bcd3-2e21a9445832" />

The output contains the password for **Level 10**.

### Step 4: Exit Level 9

After noting the password:

<img width="348" height="46" alt="image" src="https://github.com/user-attachments/assets/acca7100-3bd2-4334-9286-0b45d7402a2d" />

This closes the current SSH session.

### Step 5: Log in to Level 10 using ssh command: ssh bandit10@bandit.labs.overthewire.org -p 2220

<img width="509" height="184" alt="image" src="https://github.com/user-attachments/assets/d3b7d8b4-feda-44fd-81f6-744c8ea095c9" />

Enter the password obtained from: strings data | grep "=="

### Step 6: Enter the password obtained above

After entering the password, you will be directed to **Level 10** officially.
