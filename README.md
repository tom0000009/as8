# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

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

Vulnerability #1: Session Hijacking

Vulnerability #2: __________________


## Green

Vulnerability #1: Insecure Direct Object Reference (IDOR)

Vulnerability #2: Cross-Site Scripting (XSS)


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work

python sqlmap.py --wizard
never returned anything for the login pages or user editing pages in red, blue, and green when using the default settings
anything beyond the defaults wouldn't work

you can hijack another session in blue by changing your phsessid
was signed onto different accounts in firefox and chrome
had firefox change its phsessid to match chrome's and then logged out
refreshed the page on chrome and was logged out

you can find information on employess not listed on the green "Find a Salesperson" page
by visiting the page of one of listed employees and then changing the id on the address bar.(IDOR)

xss can be abuse using the feedback section in green 
