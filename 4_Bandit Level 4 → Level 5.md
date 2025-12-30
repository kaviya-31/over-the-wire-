Level Goal
The password for the next level is stored in the only human-readable file in the inhere directory.
Tip: if your terminal is messed up, try the “reset” command.

# OverTheWire Bandit – Level 5

Goal:
Find the password stored in a file that is human-readable, 1033 bytes in size, and not executable.

Command used:
cd inhere
find . -type f -size 1033c ! -executable
cat ./maybehere07/.file2

Key learning:
- Using find with size, type, and permission filters
- Navigating directories to locate specific files

Screenshot proof attached.

<img width="1452" height="861" alt="Screenshot 2025-12-27 220413" src="https://github.com/user-attachments/assets/9af7acff-ddf1-47a8-99ed-5a3ebe39d420" />
