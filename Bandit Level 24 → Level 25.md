Level Goal

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode.
There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time

Bandit Level 24 → Level 25 Explanation:

In this level, a daemon is actively listening on port 30002.
The daemon verifies two inputs before responding.
First, it requires the password from the previous level, bandit24.
Second, it requires a secret numeric four-digit PIN code.

The PIN code cannot be obtained directly from the system.
The only possible way to find it is by brute-forcing
all combinations from 0000 to 9999.

A key detail in this level is that the daemon
does not require a new connection for each attempt.
This allows multiple PIN combinations to be tested
within a single network session.

By automating the input process,
each PIN is sent sequentially along with the correct password.
When the correct combination is submitted,
the daemon returns the password for bandit25.

This level introduces the concept of brute-force attacks
and demonstrates how weak authentication mechanisms
can be exploited when rate limiting is not enforced.
It also highlights the importance of secure service design
and protection against repeated authentication attempts.


Screenshots:
<img width="1475" height="879" alt="Screenshot 2025-12-30 193454" src="https://github.com/user-attachments/assets/56e86974-3716-46bd-810c-aca77046ef8f" />

<img width="1462" height="792" alt="Screenshot 2025-12-30 193401" src="https://github.com/user-attachments/assets/0970c573-7cd0-416b-9040-dbcf7264d28e" />

