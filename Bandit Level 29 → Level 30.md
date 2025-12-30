Level Goal
There is a git repository at ssh://bandit29-git@bandit.labs.overthewire.org/home/bandit29-git/repo via the port 2220.
The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

Bandit Level 29 → Level 30 Explanation

In this level, the password for the next level
is stored inside a remote Git repository.
The repository can be accessed using SSH
through port 2220.

The repository belongs to the user bandit29-git.
Login authentication uses the same password
as the bandit29 user account.

After cloning the repository locally,
the available branches should be examined.
Not all information is stored
in the default branch.

By listing and switching between branches,
additional files and content become visible.
One of the branches contains the password
for the next level.

This level highlights the importance of
understanding Git branching concepts.
It demonstrates how sensitive information
can be hidden in non-default branches.
The challenge emphasizes careful review
of all branches in a repository.


Screenshot:


<img width="803" height="547" alt="Screenshot 2025-12-30 211912" src="https://github.com/user-attachments/assets/fd820509-cb8a-4774-b9fa-70550bbb2468" />

