Level Goal
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument.
It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

andit Level 20 → Level 21 Explanation

In this level, a setuid binary is provided in the home directory.
The binary is designed to connect to localhost on a port number supplied
as a command-line argument. After establishing the connection,
it reads a single line of text from the socket.

The received text is then compared with the password of the previous
level, which is bandit20. If the provided text matches the correct
password, the binary sends back the password for the next level,
bandit21.

To solve this level, it is necessary to understand basic networking
and how local ports work. A local listening service must be created
so that the binary has something to connect to.

Netcat is used to open a listening port on localhost.
Once the listener is active, the setuid binary is executed
with the same port number as an argument.

When the connection is established, the listener sends the
bandit20 password through the socket.
Since the binary runs with elevated privileges,
it verifies the password and responds with the bandit21 password.

This level demonstrates how setuid binaries, local networking,
and socket communication work together.
It also highlights why trusting user-controlled network input
can be a security risk.


ScreenShot:
<img width="1441" height="770" alt="Screenshot 2025-12-30 183710" src="https://github.com/user-attachments/assets/119310f5-1f62-4743-bb4c-a018a5f1689d" />

