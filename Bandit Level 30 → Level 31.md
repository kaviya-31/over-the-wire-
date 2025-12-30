Level Goal
There is a git repository at ssh://bandit30-git@bandit.labs.overthewire.org/home/bandit30-git/repo via the port 2220. 
The password for the user bandit30-git is the same as for the user bandit30.

Clone the repository and find the password for the next level.


# Login to Bandit level 30
ssh bandit30@bandit.labs.overthewire.org -p 2220

# Move to temporary directory
cd /tmp
mkdir bandit30_repo
cd bandit30_repo

# Clone the git repository (password = bandit30 password)
git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo

# Enter the cloned repository
cd repo

# Check repository status
git status

# List all branches
git branch -a

# List commit history
git log

# List all git tags (important step)
git tag

# Show details of the secret tag
git show secret

# The output reveals the password for Bandit level 31


Screenshot:

<img width="924" height="531" alt="Screenshot 2025-12-30 212643" src="https://github.com/user-attachments/assets/d529c941-6c05-46df-afb9-d65cd9cedba1" />
