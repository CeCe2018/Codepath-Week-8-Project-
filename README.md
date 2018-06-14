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

![cedeiysha mayweather sql injection 2](https://user-images.githubusercontent.com/23458001/41395753-a1168c0e-6f63-11e8-8fa1-ad349d685fd2.png)
![cedeiysha mayweather sql injection](https://user-images.githubusercontent.com/23458001/41395754-a12be824-6f63-11e8-9404-188f6d42b111.png)

Vulnerability #2: ____Session Hijacking/Fixation_____________

## Green

Vulnerability #1: _____User Enumeration_____________

![cedeiysha mayweather user enumeration 2](https://user-images.githubusercontent.com/23458001/41395755-a148e51e-6f63-11e8-8c6a-1ba63a6f5761.png)
![cedeiysha mayweather user enumeration](https://user-images.githubusercontent.com/23458001/41395757-a162d794-6f63-11e8-822b-68cc0841bbec.png)

Vulnerability #2: ______Cross-site Scripting____________

![cedeiysha mayweather cross site scripting 1](https://user-images.githubusercontent.com/23458001/41395748-a0b66e5a-6f63-11e8-8c77-a820f783aaf5.png)
![cedeiysha mayweather cross site scripting](https://user-images.githubusercontent.com/23458001/41395749-a0ccd532-6f63-11e8-9265-7155e9cb3096.png)


## Red

Vulnerability #1: _Cross-site Request Forgery________________

Vulnerability #2: __Insecure Direct Object Reference________________

![cedeiysha mayweather insecure direct object reference 2](https://user-images.githubusercontent.com/23458001/41395751-a0e54248-6f63-11e8-8be2-5730da12d03a.png)
![cedeiysha mayweather insecure direct object reference](https://user-images.githubusercontent.com/23458001/41395752-a0fd5c66-6f63-11e8-9459-88f14672468b.png)

## Notes

Describe any challenges encountered while doing the work
I had challenges proving website (red) had a Cross Site Forgery Request vulnerability, I tried multiple times with different methods trying to find the vulnerability but I couldn't do it. I only knew it had the vulnerability by process of elimination basically.
The Session Hijacking/Forgery also had its challenges as well. I tried using a different browser but for some reason it still did not work.


## Concept Review


Which attacks were easiest to execute? Which were the most difficult? The easiest to execute were Insecure Direct Object Reference, User Enumeration, and Cross Site Scripting. The most difficult would definitely be Cross Site Request Forgery and Session Hijacking/Fixation.


What is a good rule of thumb which would prevent accidentally username enumeration vulnerabilities like the one created here? Try to expose as few details as possible. On servers, conceal which operating systems are being used and what the installed software and configurations 
are.

Many SQL Injections use OR as part of the injected code. (For example: ' OR 1=1 --'.) Could AND work just as well in place of OR? (For example: ' AND 1=1 --'.) Why or why not? It depends on the parameters and filters implemented in the code. If "AND" is filtered it will not be successful, if it isn't filter SQLi should work.

