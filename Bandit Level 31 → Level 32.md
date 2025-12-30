Level Goal
There is a git repository at ssh://bandit31-git@bandit.labs.overthewire.org/home/bandit31-git/repo via the port 2220.
The password for the user bandit31-git is the same as for the user bandit31.

Clone the repository and find the password for the next level.


# Login to Bandit level 31
ssh bandit31@bandit.labs.overthewire.org -p 2220

# Move to temporary working directory
cd /tmp
mkdir bandit31_repo
cd bandit31_repo

# Clone the git repository (password = bandit31 password)
git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo

# Enter the repository
cd repo

# Check repository contents
ls -la

# Read README file
cat README.md

# Create the required file as instructed
echo "May I come in?" > key.txt

# Add the file to git
git add key.txt

# Commit the changes
git commit -m "Added key file"

# Push changes to remote repository
git push origin master

# Server responds with the password for Bandit level 32


Screenshot:


<img width="892" height="530" alt="Screenshot 2025-12-30 213020" src="https://github.com/user-attachments/assets/1bdb8958-fd6c-4456-9041-0839f529e986" />



