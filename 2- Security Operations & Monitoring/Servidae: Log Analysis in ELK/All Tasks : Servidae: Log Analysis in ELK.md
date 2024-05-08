# Link on TryHackMe: [Servidae: Log Analysis in ELK](https://tryhackme.com/r/room/servidae)

## Task -1 : reading only

## Task -2 : The Elastic Stack

### What is the name of the open-source search engine library that Elasticsearch is built on?
Answer: Apache Lucene

### Which component of the Elastic Stack would you use to perform advanced filtering and processing of data before it gets stored?
Answer: Logstash

## Task -3: A Compromised Workstation: Scenario  (only reading)

## Task -4 : Kibana: Basics 

### Update the date and time filter as specified. How many total hits were captured within the selected time period?
Answer: 920

## Task -5: Kibana: Fields and Values

### Look at the Top values under the destination.ip field. Which IP address stands out?
Answer: 84.237.252.156

### Use an IP address lookup tool (such as iplocation.io). What country does this IP address originate from?
Answer: Latvia

### Which process name is running the most frequently on the compromised workstation?
Answer: curl.exe

## Task -6: Kibana: Sorting and Filtering

### What was the process ID (PID) of the potentially malicious PowerShell script?
Answer: 6712

### What was the parent process name of the process that spawned powershell.exe?
Answer: explorer.exe

## Task -7: Indicators of Compromise: Discovery

### What is the domain name of the attacker's server hosting the winPEAS executable?
Answer: evilparrot.thm

### What is the full path of the HKEY_LOCAL_MACHINE registry entry that was queried?
Answer: HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\Installer

## Task -8: Indicators of Compromise: Privilege Escalation

### What is the name of the malicious .msi file?
Answer: Adminshell.msi

## Task -9: ndicators of Compromise: Persistence

### What is the name of the user account that the attacker created to maintain privileged access?
Answer: Backdoor

### What is the flag sent via cURL requests to the evilparrot.thm server?
Answer: THM{C4N_y0U_h34r_m3}

### What is the name of the registry value that the attacker added?
Answer: Backdoorshell

## Task -10: Indicators of Compromise: Lateral Movement

### What was the password that the attacker used to access Bill's user account on the internal payroll website?
Answer: Password123

### What flag was included within the HTTP requests during the attacker's successful logins?
Answer: THM{1m_1N_Y0ur_P4YR0LL}

### What was the session cookie value that the attacker included in the cURL request at 18:58:08.001?
Answer: dt5qhq423goknmq269rg1tal1a

### What is the name of the sensitive file that the attacker downloaded?
Answer: bank-details.csv
