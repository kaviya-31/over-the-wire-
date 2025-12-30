Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed.
For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”.
Then copy the datafile using cp, and rename it using mv (read the manpages!)

# OverTheWire Bandit – Level 13

Goal:
Log in to the next level using an SSH private key.

Commands used:
chmod 600 sshkey.private
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220

Key learning:
- Using SSH key-based authentication
- Securing private keys with correct permissions
- Logging in without a password

Screenshot proof attached.

<img width="1789" height="833" alt="Screenshot 2025-12-28 141941" src="https://github.com/user-attachments/assets/15f0de8a-a9e9-411c-b00e-30a0e86d853b" />



