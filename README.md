# TryHackMe
Documenting my journey exploring TryHackMe

_Exploring TryHackMe to expand my hands on practice reinforcing technical capabilities with a pen test lens and its fun!_

[View My TryHackMe Profile](https://tryhackme.com/p/zcurry.zinc)



**Linux Commands**
- whoami - Returns the machine information
- echo - Returns a command
- ls - List what in the current folder
- cd - change directory or move into a folder
- cat - shows the contents of a file
- pwd - prints the working directory
- dirb - returns hidden pages [for example dirb www.BigBusiness.com returns unindexed admin pages] _Helpful in capture the flag to find unprotected pages_
- find - search for files [for example find -name passwords.txt]
- grep - searches inside for text [for example grep "password123" passwords.txt]
- & - Runs commands and does not wait
- && - Runs commands and waits for the first to finish
- ">" - Used to redirect output and over writes the file
- ">>" - The redirector does the same thing, but instead of overwriting, it will just add the output to the bottom of the file



**SOC Simulator**</br>
Step 1: Find all true positives</br>
Step 2: Read the documentation</br>
Step 3: Investigate the alert queue</br>
Step 4: Take ownership of an alert</br>
Step 5: Deep dive into the SIEM [Splunk]</br>


**Alert 1:** Inbound Email Containing Suspicious External Link</br>
Decision: True Positive</br>
Explanation: The link within the email is to another company impersonating Human Resources to our employee redirecting them to an external website.</br>

**Alert 2:** Access to Blacklisted External URL Blocked by Firewall</br>
Decision: True Positive</br>
Explanation: Known malicious IP - Escalate for further review as to why our IP tried to access was it by accident, a phishing breach, or an inside threat.</br>

**Alert 3:** Inbound Email Containing Suspicious External Link </br>
Decision: True Positive</br>
Explanation: The sender and external link are impersonating Microsoft.</br>
