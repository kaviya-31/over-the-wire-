Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data

# OverTheWire Bandit – Level 11

Goal:
Find the password stored in a file encoded using ROT13.

Command used:
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

Key learning:
- Understanding ROT13 substitution cipher
- Using tr for character translation
- Working with simple text ciphers in Linux

Screenshot proof attached.

<img width="1410" height="634" alt="Screenshot 2025-12-27 225141" src="https://github.com/user-attachments/assets/7b74c37b-45f4-414e-9e68-b939a4e9ce12" />
