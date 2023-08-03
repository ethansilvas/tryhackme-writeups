
## Task 1 - Introduction to Operating System Security

computer has hardware like screens, keyboards, motherboard, CPU, RAM... 

operating systems are the interface between apps and hardware 
    they control and drive the hardware
    allow apps to utilize a system's hardware 

all of your devices with an OS hold lots of personal data that you don't want to be seen by threat actors 
    OS hardening is what secures this data from attackers 

![](Images/Pasted%20image%2020230802175330.png)

## Task 2 - Common Examples of OS Security

Three weaknesses targeted by threat actors: 
    1. Authentication and weak passwords
    2. Weak file permissions
    3. Malicious programs

### Authentication and Weak Passwords 

authentication through something you know, have, or are 

weak passwords that don't have unique characters, aren't of sufficient length, or contain dictionary words are weak passwords that are vulnerable to attacks such as brute forces 

### Weak File Permissions

principle of least privilege 

using OS tools like Linux permission groups and chmod are important to ensure that files and folders are accessible only to those who need to see or use them 

### Access to Malicious Programs 

attacks like trojan horses will give root access to your device 

other attacks like ransomware would encrypt all of your data 

![](Images/Pasted%20image%2020230802184703.png)

## Task 3 - Practical Example of OS Security

discover a username and guess the password to gain admin or root access 

**Scenario** - We were hired to check security of company and when we visited the office we noticed a sticky note with "sammie" and "dragon" on it. 

First lets see if those credentials work with the target machine **10.10.246.107** 

![](Images/Pasted%20image%2020230802190507.png)

After entering "dragon" as the password it seems to have worked, and I confirmed with `whoami`: 

![](Images/Pasted%20image%2020230802190554.png)

Next, using the `cat` and `ls` commands I view some of the info available to potential attackers: 

![](Images/Pasted%20image%2020230802190742.png)

We know of two other users who also have a disregard for cybersecurity. Now I will try to brute force access to the user "johnny". 

Using the list of the most commonly used passwords, I tried to guess Johnny's password and was successful: 

![](Images/Pasted%20image%2020230802191311.png)

Viewing Johnny's history we can see that he accidentally typed out the password to the root account:

![](Images/Pasted%20image%2020230802191524.png)

Using this password we gain access to the root account: 

![](Images/Pasted%20image%2020230802191612.png)

![](Images/Pasted%20image%2020230802191642.png)



