--------Level 0-----------

CONNECTING TO THE SERVER 

The first step is to connect to the Bandit server using SSH (Secure Shell).
Open Command Prompt and enter:ssh bandit0@bandit.labs.overthewire.org -p 2220
![image alt](https://github.com/suganthijg/Banditt/blob/bf96f81936257b0cab7d6e8e67463a1f4757bfb2/Screenshot%202026-09-09%20184402.png)
Here:

* `ssh` → connects to a remote server.
* `bandit0` → username.
* `bandit.labs.overthewire.org` → server address.
* `-p 2220` → connects through port `2220`.

When prompted for the password, enter the password provided for Level 0.

If the login is successful, you will see:
<img width="812" height="430" alt="Image" src="https://github.com/user-attachments/assets/d057bbf3-1d85-4edf-8a42-717d6e267feb" />
This means you are successfully logged in to the Bandit server as `bandit0`.

Level 0 is complete. We can now move on to **Level 0 → Level 1**.
