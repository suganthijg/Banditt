## Level 1 → Level 2

### Objective

Find the password for Level 2 from a file named `-`.

### Step 1: List the files using ls command
<img width="206" height="38" alt="Image" src="https://github.com/user-attachments/assets/c7e62eba-7293-4694-84d6-7b7d60126b39" />

### Step 2: Read the file using cat./- command

Since `-` has a special meaning in Linux, use `./-` to specify the file:
<img width="270" height="33" alt="Image" src="https://github.com/user-attachments/assets/6168a23d-a7de-41f6-9490-b89b9e43fd44" />

The output is the password for **Level 2**.

### Step 3: Exit Level 1
After noting the password:
use exit command:
<img width="441" height="47" alt="Image" src="https://github.com/user-attachments/assets/c65c5ac2-89bc-4aa0-9abd-e9f376302e85" />
This closes the current SSH session.

### Step 4: Log in to Level 2 using ssh bandit2@bandit.labs.overthewire.org -p 2220
<img width="489" height="173" alt="image" src="https://github.com/user-attachments/assets/20dc0657-d0ca-43c0-b387-4138d440f1a8" />
Enter the password obtained from `cat ./-` and you will be directed to Level 2 officially
<img width="815" height="387" alt="Image" src="https://github.com/user-attachments/assets/ac173f4e-1603-4515-950a-d28932c13641" />
