# 1/c Faith Arnold - CNS Homework #7 - 25 October 2023
## Research a Vulnerable Service

For this homework and and in choosing the an exploit for Lab 10, I decided to select a MySQL password brute force exploit using nmap scans and Metasploit. I can upon this exploit when looking through the Metasploit documentation website. I found a page specifically on MySQL exploits, including details on dumping, querying, and reverse shell. 

The website I am referencing can be found at this link: https://docs.metasploit.com/docs/pentesting/metasploit-guide-mysql.html

In the lab, I will need to add MySQL to the server I will be exploiting, and I plan to use an Ubuntu Linux Server.

I found documentation on how to install and configure a MySQL server at this link: https://ubuntu.com/server/docs/databases-mysql
 
After downloading MySQL to the server, I will follow the instructions detailed in from the Metasploit documentation except using nmap commands to brute force the password.

## Locate Vulnerability Information

While there are no CVE's related to a MySQL brute force exploit, there are a few CWE's that are related to this weakness. The CWE that relates most to this exploit is CWE-307: Improper Restriction of Excessive Authentication. This entry highlights the importance of impolementing the mechanisms to limit authentication attempts, which prevent the success of brute force attacks. 
