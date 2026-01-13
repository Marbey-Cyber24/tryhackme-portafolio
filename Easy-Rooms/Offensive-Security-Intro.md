# Offensive Security Intro – TryHackMe

Room: https://tryhackme.com/room/offensivesecurityintro

## Objective
Hack the FakeBank application and transfer money as an attacker.

## Tools Used
- Gobuster
- Web browser (Firefox)
- Linux terminal

## Steps

1. I scanned the website to find hidden directories:
gobuster -u http://fakebank.thm -w wordlist.txt dir

2. I discovered a hidden page:
/bank-transfer

3. I opened it in the browser:
http://fakebank.thm/bank-transfer

4. I accessed the admin transfer portal.

5. I transferred $2000 from account 2276 to my account 8881.

6. The site confirmed:
“BANK-HACKED”

## Result
The attack was successful and the money was transferred.

## What I learned
- How directory brute-forcing works
- How attackers find hidden admin pages
- How web vulnerabilities can lead to financial fraud
