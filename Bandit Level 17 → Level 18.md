Level Goal
There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19


# OverTheWire Bandit – Password Comparison Level

## Level Goal
There are two files present in the home directory:
- passwords.old
- passwords.new

The password for the next level is stored in `passwords.new` and is the
only line that differs between the two files.

## Given Information
- Both files contain multiple lines of text
- Only one line has been changed
- Identifying this difference reveals the correct password

## Approach
To solve this level, a file comparison method was required.
The `diff` command was used to compare both files line by line
and highlight the modified content.

## Commands Used
diff passwords.old passwords.new

## Explanation
- The `diff` command compares two files
- Lines that differ are clearly marked in the output
- The changed line in `passwords.new` contains the password

## Result
The differing line from `passwords.new` was identified
and extracted as the password for the next level.

## Key Learning
- Understanding file comparison in Linux
- Using `diff` to track changes between files
- Identifying minimal differences in large datasets
- Extracting critical information from command output

## Screenshot Proof
A screenshot is attached showing:
- Both files in the home directory
- The `diff` command execution
- The changed line containing the password

## Notes
After completing this level, logging into the next level may display
a "Byebye!" message. This behavior is expected and relates to the
mechanics of the following level.

screen shot:


<img width="1551" height="852" alt="Screenshot 2025-12-30 150325" src="https://github.com/user-attachments/assets/cbc13f39-dd80-4383-a395-ebba1c145a69" />

