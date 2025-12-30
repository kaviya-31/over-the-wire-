Level Goal
To gain access to the next level, you should use the setuid binary in the homedirectory. 
Execute it without arguments to find out how to use it. 
The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.


# Bandit Level 19 → Level 20

## Level Goal
To gain access to the next level, you must use the **setuid binary** present in the home directory.  
Run the binary without arguments to understand its usage.  
After using it correctly, the password for the next level can be found in the usual location:
`/etc/bandit_pass/bandit20`.

---

## Step 1: List Files in Home Directory
```bash
ls -l
You will notice a file with setuid permissions:

-rwsr-x--- 1 bandit20 bandit19 ... bandit20-do

Step 2: Execute the SetUID Binary
./bandit20-do


This shows that the binary allows execution of commands as user bandit20.

Step 3: Read the Password File
./bandit20-do cat /etc/bandit_pass/bandit20

Explanation

The binary runs with bandit20 privileges

It bypasses normal permission restrictions

This allows access to protected files

Result

The password for Bandit Level 20 is successfully displayed.

ScreenShot:

<img width="1443" height="882" alt="Screenshot 2025-12-30 151434" src="https://github.com/user-attachments/assets/a3bff08f-67c8-4fc3-8826-56d3925abc19" />

