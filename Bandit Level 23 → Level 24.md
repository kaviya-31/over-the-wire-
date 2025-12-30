Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler.
Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script.
This is a very big step and you should be proud of yourself when you beat this level!

NOTE 2: Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…


Bandit Level 23 → Level 24 Explanation

In this level, a program is executed automatically at regular intervals
using the cron job scheduler. The cron configuration can be found
inside the /etc/cron.d/ directory.

The cron job runs a script with the privileges of bandit24.
This script is designed to execute shell scripts placed
inside a specific directory.

To solve this level, it is necessary to create a custom shell script.
This script will be executed automatically by the cron job.
Writing the first shell script is an important learning step
in understanding Linux automation.

The shell script is used to access protected information
and redirect the output to a readable location.
Since the script runs with higher privileges,
it can read files not normally accessible.

After execution, the shell script is automatically removed.
Because of this behavior, keeping a backup copy is important.
Once the cron job runs, the output file created by the script
contains the password for the next level.

This level demonstrates how cron jobs can execute user-provided scripts
and highlights the security risks of improper task scheduling.
It also builds confidence in creating and using shell scripts.


Screenshot:

<img width="1504" height="829" alt="Screenshot 2025-12-30 192639" src="https://github.com/user-attachments/assets/a00f2aa6-2e10-4609-be6b-22345d4a0690" />
