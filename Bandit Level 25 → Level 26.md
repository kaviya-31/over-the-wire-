Level Goal
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else.
Find out what it is, how it works and how to break out of it.

NOTE: if you’re a Windows user and typically use Powershell to ssh into bandit: Powershell is known to cause issues with the intended solution to this level.
You should use command prompt instead.

Bandit Level 25 → Level 26 Explanation :


In this level, logging in to bandit26 is intentionally restricted.
Although the SSH login succeeds, the default shell is not /bin/bash.
Instead, bandit26 uses a different shell designed to limit user actions.

The goal is to identify which shell is being used
and understand how it behaves.
By checking the user configuration files,
the shell type can be determined.

The restricted shell prevents execution of normal commands
and exits automatically under certain conditions.
Understanding its limitations is essential to progressing.

By carefully interacting with the shell,
it is possible to exploit its behavior
and escape into a full interactive shell.
This usually involves leveraging built-in commands
or editor features allowed by the restricted environment.

Once the shell is successfully escaped,
normal command execution becomes possible.
This allows access to files that contain
the password for the next level.

This level teaches how restricted shells work
and why improper shell restrictions can be bypassed.
It also highlights the importance of understanding
default user environments in system security.


Screenshots:

<img width="1373" height="567" alt="Screenshot 2025-12-30 235011" src="https://github.com/user-attachments/assets/80b10a9e-e1b0-4074-97ba-810d20f07b6f" />

<img width="1066" height="143" alt="Screenshot 2025-12-30 235105" src="https://github.com/user-attachments/assets/480be785-9950-4645-871f-bbdadc3dae51" />

<img width="1039" height="378" alt="image" src="https://github.com/user-attachments/assets/099c0cf7-0692-4454-a647-11bc336898b4" />  




