# Password Cracking Techniques

## Prerequisites
- Basic knowledge of Linux commands.
- A computer with internet access.
- Hashcat and John the Ripper installed (you can use Kali Linux for pre-installed tools).

## Overview
Password cracking is a method used in penetration testing to determine the strength of passwords used in a system. This project will guide you through password cracking techniques using tools like Hashcat and John the Ripper.

## Step-by-Step Guide

### Step 1: Set Up the Environment
1. **Install Kali Linux**:
   - Download Kali Linux from [https://www.kali.org/downloads/](https://www.kali.org/downloads/).
   - Install Kali Linux in a virtual machine or on a physical machine. If you're using VirtualBox, you can import the Kali Linux OVA file.

2. **Ensure Tools Are Installed**:
   - Open a terminal in Kali Linux and verify that Hashcat and John the Ripper are installed:
   ```bash
   hashcat --version
   john --version

# Password Cracking Techniques

## Step 2: Create Sample Password Hashes

### Generate Sample Passwords:
Create a file named `passwords.txt` with some sample passwords:  
<img src="https://github.com/user-attachments/assets/d5a5c760-dff2-4b52-b705-e77d1d6bfd8b" alt="Sample Password File">

### Hash the Passwords:
Use `openssl` to hash the passwords in MD5 format:  
<img src="https://github.com/user-attachments/assets/3d09b74d-b5a8-4032-bb0c-17e38bd9ab7e" alt="Hashed Passwords">

---

## Step 3: Crack Passwords with John the Ripper

### Prepare the Hashes for John:
Create a file named `hashes_john.txt` and add the hashes from `hashed_passwords.txt` in a format John can understand:  
<img src="https://github.com/user-attachments/assets/8feca984-40f5-43f5-9159-940b94c7ba46" alt="Hashes for John the Ripper">

### Run John the Ripper:
Use John to crack the hashed passwords:
```bash
john --wordlist=passwords.txt hashes_john.txt








# Password-Cracking-Techniques


**Installed hashcat and john, Made a password.txt file with few  sample passwords:
![image](https://github.com/user-attachments/assets/d5a5c760-dff2-4b52-b705-e77d1d6bfd8b)

**Hash the Passwords:**

**Crach Password with John the Ripper:**
 The file `hashed_password.txt` will contain the MD5 hashes of the sample passwords.
![image](https://github.com/user-attachments/assets/3d09b74d-b5a8-4032-bb0c-17e38bd9ab7e)

**Create a file named hashes_john.txt' and add the hashes from 'hashes_password.txt in a format john can understand**
![image](https://github.com/user-attachments/assets/8feca984-40f5-43f5-9159-940b94c7ba46)

**Run John the Ripper (Use john to crack the hashed passwords**
![image](https://github.com/user-attachments/assets/cb26f583-cc10-45dd-a919-1b993d889b0a)

 Once Hashcat finishes, view the cracked passwords in `cracked_passwords.txt".
 ![image](https://github.com/user-attachments/assets/0237fb16-cb70-4346-b116-c3e5f2e190cd)


**Run Hashcat(Use Hashcat to crack the hashed passwords.):**
![image](https://github.com/user-attachments/assets/a61b8930-0ea1-48cf-aae0-743f8dad3774)

especifies MD5 hashes, `-a e` specifies a dictionary attack, and `-` specifies the output file.

3. View the Cracked Passwords:
Once Hashcat finishes, view the cracked passwords in `cracked_password.txt`.



