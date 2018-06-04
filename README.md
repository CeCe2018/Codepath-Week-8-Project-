# Codepath-Week-8-Project-
# Project 8 - Pentesting Live Targets

Time spent: 3 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: _SQL Injection_________________

Vulnerability #2: ____Session Hijacking/Fixation_____________


## Green

Vulnerability #1: _____User Enumeration_____________

Vulnerability #2: ______Cross-site Scripting____________


## Red

Vulnerability #1: _Cross-site Request Forgery________________

Vulnerability #2: __Insecure Direct Object Reference________________


## Notes

Describe any challenges encountered while doing the work
I had challenges proving website (red) had a Cross Site Forgery Request vulnerability, I tried multiple times with different methods trying to find the vulnerability but I couldn't do it. I only knew it had the vulnerability by process of elimination basically.
The Session Hijacking/Forgery also had its challenges as well. I tried using a different browser but for some reason it still did not work.


## Concept Review


Which attacks were easiest to execute? Which were the most difficult? The easiest to execute were Insecure Direct Object Reference, User Enumeration, and Cross Site Scripting. The most difficult would definitely be Cross Site Request Forgery and Session Hijacking/Fixation.


What is a good rule of thumb which would prevent accidentally username enumeration vulnerabilities like the one created here? Try to expose as few details as possible. On servers, conceal which operating systems are being used and what the installed software and configurations 
are.

Many SQL Injections use OR as part of the injected code. (For example: ' OR 1=1 --'.) Could AND work just as well in place of OR? (For example: ' AND 1=1 --'.) Why or why not? It depends on the parameters and filters implemented in the code. If "AND" is filtered it will not be successful, if it isn't filter SQLi should work.

