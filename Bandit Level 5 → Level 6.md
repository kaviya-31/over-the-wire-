Level goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

# OverTheWire Bandit – Level 6

Goal:
Find the password stored in a file owned by user bandit7 and group bandit6.

Command used:
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password

Key learning:
- Using find with user and group filters
- Redirecting permission errors to /dev/null
- Searching the entire filesystem safely

Screenshot proof attached.

<img width="1738" height="871" alt="Screenshot 2025-12-27 220352" src="https://github.com/user-attachments/assets/0fb9e1fc-4604-407a-8bbb-96cdce759328" />
