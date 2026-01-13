# Offensive Security Intro – TryHackMe

Room: https://tryhackme.com/room/offensivesecurityintro  
Category: Web Exploitation  
Difficulty: Easy  
Status: Completed  

---

##  Executive Summary

During this assessment, a vulnerable banking web application was tested.  
By performing directory enumeration, a hidden administrative transfer page was discovered.  
This allowed an attacker to move money between accounts without authentication, resulting in full compromise of the system’s financial integrity.

---

##  Objective

Identify hidden functionality within the FakeBank web application and exploit it to perform an unauthorized money transfer.

---

##  Tools Used

- Gobuster  
- Firefox Browser  
- Linux Terminal (TryHackMe VM)  

---

##  Methodology

1. Reconnaissance of the web server  
2. Enumeration of hidden directories  
3. Identification of vulnerable endpoints  
4. Exploitation of business logic  
5. Validation of the attack  

---

##  Technical Walkthrough

### 1. Directory Enumeration

Gobuster was used to brute-force directories on the target website.

```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir
