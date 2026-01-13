# Offensive Security Intro – TryHackMe

Room: https://tryhackme.com/room/offensivesecurityintro

## Objective
Exploit the FakeBank application to find hidden functionality and transfer money as an attacker.

## Tools Used
- Gobuster
- Firefox browser
- Linux terminal (TryHackMe VM)

## Steps

### 1. Scan the website for hidden directories
```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir


![Gobuster](screenshots/gobuster.png)
