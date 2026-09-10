## Level 11 → Level 12

### Objective

Find the password for Level 12. The contents of `data.txt` are encrypted using **ROT13**.

### Step 1: List the files using ls command

<img width="182" height="30" alt="image" src="https://github.com/user-attachments/assets/9a8f42cd-f2a7-4d6b-8188-9de1a9ad320e" />

### Step 2: Read the file using cat command
The output is:

<img width="443" height="30" alt="image" src="https://github.com/user-attachments/assets/7ca63be4-9749-40b2-a8e0-69a6470f492b" />

The text is encrypted using ROT13.

### Step 3: Decode the text using tr command
<img width="480" height="29" alt="image" src="https://github.com/user-attachments/assets/5d1e8433-ad05-490a-9547-5cc4859f1cac" />

`tr` replaces each letter with the letter 13 positions away in the alphabet, which decodes the ROT13 text.

The output is:

```text
The password is GROozWPO8QyN0mGrjUkID0WCYkZiQxrN
```

The value after **"The password is"** is the password for **Level 12**.

### Step 4: Exit Level 11

After noting the password:



This closes the current SSH session.

### Step 5: Log in to Level 12 using ssh command

```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

Enter the password obtained from:

```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

### Step 6: Enter the password obtained above
<img width="552" height="329" alt="image" src="https://github.com/user-attachments/assets/552c2d1b-9621-4ef4-8287-618202400238" />

After entering the password, you will be directed to **Level 12** officially.
