Level Goal
The password for the next level is stored in a file readme in the homedirectory.
Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

# Bandit Level 18 → Level 19

## Level Goal
The password for the next level is stored in a file called `readme`
in the home directory.  
Unfortunately, `.bashrc` has been modified to automatically log you out
when you log in using SSH.

---

## Problem
- SSH login immediately logs out
- `.bashrc` executes a logout command
- Interactive shell access is blocked

---

## Key Concept
SSH allows executing a command directly at login
without starting an interactive shell.

---

## Command Used
```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme


Screenshot:

<img width="1679" height="863" alt="Screenshot 2025-12-30 151026" src="https://github.com/user-attachments/assets/4008a8fe-6956-421f-bddf-20da91fe2bea" />
