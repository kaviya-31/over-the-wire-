# Login to Bandit level 33
ssh bandit33@bandit.labs.overthewire.org -p 2220

# Move to home directory
cd ~

# List all files, including hidden
ls -la

# Look for unusual files or directories
cat .hidden
cat .secret
cat password.txt

# If nothing obvious, check subdirectories
find . -type f -exec ls -l {} \;

# Check for setuid binaries or executable scripts
find . -type f -executable -exec ls -l {} \;

# If you find an interesting binary or script, run it
./some_binary

# Sometimes the password is revealed after running it or reading hidden files
# Use 'cat' on any files that seem suspicious

# Output should reveal the password for Bandit level 34 



Screenshot:


<img width="710" height="548" alt="Screenshot 2025-12-30 220008" src="https://github.com/user-attachments/assets/dadf7cca-5d8e-4276-967f-89cda8691177" />

