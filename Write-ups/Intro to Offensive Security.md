Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

## Task 1 - What is Offensive Security

**Offensive security** - process of breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access to them 
    find vulnerabilities 
    recommending patches 

**Defensive security** - protecting an organization's network and computer systems by analyzing and securing any potential digital threats
    investigate infected computers and devices 
    monitor infrastructure 
    track down cyber criminals

![](Images/Pasted%20image%2020230720212247.png)
    Answer: Offensive Security

## Task 2 - Hacking your first machine

Objective - use GoBuster to brute-force FakeBank's website to find hidden directories and pages 

most companies have pages that are accidentally not made private, allowing attackers to find them

```bash
gobuster -u http://fakebank.com -w wordlist.txt dir
```

-u = website to scan 
-w = list of words to iterate through to find hidden pages 

![](Images/Pasted%20image%2020230720212802.png)

visiting the found bank-transfer page:

![](Images/Pasted%20image%2020230720213108.png)

as an ethical hacker, you would (with permission) find vulnerabilities in the app and report them to the bank

## Task 3 Careers in cyber security 

how to become hacker or defender? 
    learn area of cyber security you are interested in and regularly practice these types of exercises 

what types of careers? 
    pen tester 
    red teamer 
    security engineer
