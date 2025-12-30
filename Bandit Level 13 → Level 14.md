Level Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14.
For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. 
Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.



# OverTheWire Bandit – Level 14

Goal:
Retrieve the password from a file inside a directory you normally cannot read.

Commands used:
ls -l /var/lib/bandit14
cat /var/lib/bandit14/README

Key learning:
- Accessing files with limited permissions
- Using absolute paths to read files
- Understanding Linux file permissions

Screenshot proof attached.


<img width="871" height="522" alt="Screenshot 2025-12-28 143343" src="https://github.com/user-attachments/assets/55507474-6d6e-4e73-aebf-37b1117190ce" />
