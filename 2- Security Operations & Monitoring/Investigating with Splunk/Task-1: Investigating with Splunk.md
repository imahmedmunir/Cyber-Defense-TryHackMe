# Link on TryHackMe : [Investigating with Splunk](https://tryhackme.com/r/room/investigatingwithsplunk)

### How many events were collected and Ingested in the index main?
Answer: 12256

Hint: Search on search header of splunk "index=main"

### On one of the infected hosts, the adversary was successful in creating a backdoor user. What is the new username?
Answer: A1berto

Hint: Search for process creation ID on web and search on splunk search bar

### On the same host, a registry key was also updated regarding the new backdoor user. What is the full path of that registry key?
Answer: HKLM\SAM\SAM\Domains\Account\Users\Names\A1berto

Hint: write only "index=main" on search bar and go to category field. You'll see registry added & deleted (dig deeper)

### Examine the logs and identify the user that the adversary was trying to impersonate.
Answer: Alberto

Hint: As backdoor created was "A1berto" and when you see the users, it was Alberto

### What is the command used to add a backdoor user from a remote computer?
Answer: "C:\windows\System32\Wbem\WMIC.exe" /node:WORKSTATION6 process call create "net user /add A1berto paw0rd1"

Hint: Look for commandLined field 

### How many times was the login attempt from the backdoor user observed during the investigation?
Answer: 0 

Hint: Very tricky , there were no logs from A1bert

### What is the name of the infected host on which suspicious Powershell commands were executed?
Answer: James.browne

Hint: Just type powershell and look for hosts

### PowerShell logging is enabled on this device. How many events were logged for the malicious PowerShell execution?
Answer: 79

Hint: Also tricky , look for event ID of powershell logging and search on splunk (eventID 4103)

### An encoded Powershell script from the infected host initiated a web request. What is the full URL?
Answer: hxxp[://]10[.]10[.]10[.]5/news[.]php

Explanation: As hint is provided to defang the url but where from you bring it. It is quiet hard
type powershell in splunk search bar and you'll get the Hash

Use Cyber chef: Firstly from base64 then again text decoder UTF_16LE(1200)

#### aAB0AHQAcAA6AC8ALwAxADAALgAxADAALgAxADAALgA1AA==')));$t='/news.php'
you'll find some raw data with '/news.php'
Select part before it and again use the same decoding mathodology, it will give you answer. Just defang it


