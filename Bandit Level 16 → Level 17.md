Level Goal
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

Helpful note: Getting “DONE”, “RENEGOTIATING” or “KEYUPDATE”? Read the “CONNECTED COMMANDS” section in the manpage.

# OverTheWire Bandit – Level 17

Goal:
Find the password by comparing two files and identifying the changed line.

Commands used:
diff passwords.old passwords.new

Key learning:
- Comparing files using diff
- Identifying differences between file versions
- Extracting specific information from command output

Screenshot proof attached.


<img width="1551" height="852" alt="image" src="https://github.com/user-attachments/assets/b2a57039-776d-4d37-954a-d53b3e99b0d0" />
