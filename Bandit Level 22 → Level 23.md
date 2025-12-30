Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. 
Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: Looking at shell scripts written by other people is a very useful skill.
The script for this level is intentionally made easy to read. 
If you are having problems understanding what it does, try executing it to see the debug information it prints.

Bandit Level 22 → Level 23 Explanation

In this level, a program is executed automatically at fixed intervals
using the cron job scheduler. The goal is to identify the command
that is being run by cron and understand its behavior.

Cron job configurations are stored inside the /etc/cron.d/ directory.
By inspecting the files in this directory, the active cron job
for this level can be identified.

The cron configuration shows a shell script being executed
periodically with the privileges of bandit23.
This script is intentionally written in a simple and readable manner
to help in understanding its functionality.

By opening the script, the logic of the program becomes clear.
The script processes the password for the next level
and writes it to a specific location in the filesystem.

Executing the script manually helps in observing its debug output.
This makes it easier to track file paths and variable usage.
Once the output file location is identified,
the password for the next level can be accessed.

This level emphasizes the importance of reviewing cron jobs,
analyzing shell scripts, and understanding automated task execution.
It also demonstrates how scheduled jobs can unintentionally
expose sensitive information.


Screenshot:

<img width="1686" height="902" alt="Screenshot 2025-12-30 190225" src="https://github.com/user-attachments/assets/ec7bca3b-e02a-46b5-9ed9-ffa512aa5eb8" />
