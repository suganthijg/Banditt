###  Level 6 → Level 7

### Objective

Find the password for Level 7 from a file somewhere on the server.

### Step 1: Find the required file using find command

The password is stored in a file with these properties:

* owned by user `bandit7`
* owned by group `bandit6`
* exactly 33 bytes in size

Use:

<img width="569" height="44" alt="image" src="https://github.com/user-attachments/assets/e21f6c39-bf9c-461c-ad4d-ea7d887d3a3d" />

`find /` searches from the root directory.

* `-user bandit7` → file is owned by `bandit7`.
* `-group bandit6` → file belongs to group `bandit6`.
* `-size 33c` → file size is exactly 33 bytes.
* `2>/dev/null` → hides permission-denied error messages.

The command will show the location of the required file.

### Step 2: Read the required file using cat command

Use the path shown by the `find` command:

<img width="439" height="32" alt="image" src="https://github.com/user-attachments/assets/72d36f3e-28cf-4012-a073-6dc19f6fce1f" />

The output is the password for **Level 7**.

### Step 3: Exit Level 6

After noting the password:

<img width="400" height="47" alt="image" src="https://github.com/user-attachments/assets/c9031a44-2226-4551-8ce6-e97781ec9f54" />

This closes the current SSH session.

### Step 4: Log in to Level 7 using ssh command: ssh bandit7@bandit.labs.overthewire.org -p 2220

<img width="503" height="186" alt="image" src="https://github.com/user-attachments/assets/0e11a491-0bbd-4111-8394-b5b983a749db" />

Enter the password obtained from the file.

### Step 5: Enter the password obtained above

After entering the password, you will be directed to **Level 7** officially.
