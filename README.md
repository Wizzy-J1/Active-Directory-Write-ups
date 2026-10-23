# Active Directory Writeups

A collection of my hands-on Active Directory labs, documenting the techniques, tools, findings, and lessons learned as I continue to develop my penetration testing skills.

## Lab Writeups


### ShadowGate (HackSmarter)
Description: This was an internal black-box pentest where I started without any credentials. During enumeration, I found an account vulnerable to AS-REP Roasting and retrieved a password hash that could be cracked offline. I then continued enumerating the Active Directory environment and identified an ESC8 vulnerability involving AD CS. To investigate the issue, I used PetitPotam to trigger authentication from the target machine and Certipy to set up a listener and attempt to relay the incoming NTLM authentication to the AD CS Web Enrollment service. This lab helped me understand how authentication coercion and NTLM relay can be abused when AD CS is misconfigured, and why securing certificate services is important in an Active Directory environment.
Writeup: https://lnkd.in/dZU3-SqU



### MartiniAD (HackSmarter)
Description: An internal black-box Active Directory penetration test demonstrating credential discovery, user enumeration, and the extraction of user, service account, Administrator, and KRBTGT credentials through hands-on exploitation.
Writeup: https://tinyurl.com/mw2tkhb3


### Arasaka (HackSmarter)
Description: This lab demonstrates how misconfigured Active Directory permissions, weak service account security, and AD CS vulnerabilities can be exploited to escalate privileges and achieve domain compromise. It highlights the importance of auditing permissions, securing service accounts, and properly configuring certificate services.
Writeup: https://tinyurl.com/yc6rm6e2


### BuildingMagic (HackSmarter)
Description: Exploiting the SeBackupPrivilege permission to gain full control of the Domain Controller in a simulated Active Directory environment.
Writeup: https://tinyurl.com/yynn5snf


### Welcome (HackSmarter)
Description: This walkthrough explores how misconfigured Active Directory permissions and vulnerable Active Directory Certificate Services (AD CS) configurations can create attack paths to domain compromise.
Writeup: https://tinyurl.com/ntdb78h3


### Soupeedecode (TryHackMe)
Description: A guide on my methodology for achieving full compromise of the Soupedecode Active Directory lab on TryHackMe, detailing each step and technique used.
Read the full walkthrough on Medium: (https://medium.com/@wizzyj3756/soupedecode-walkthrough-9a9da4640999)
