### Q1:Sysmon also collects the Hash value of the processes being created. What is the MD5 HASH of the program 3791.exe?
Answer: MD5=AAE3F5A29935E6ABCC2C2754D12A9AF0

After running following query, check the commandline field ::
index=botsv1 "3791.exe" sourcetype=xmlwineventlog EventCode=1

### Q2: Looking at the logs, which user executed the program 3791.exe on the server?
Answer: NT AUTHORITY\IUS

After running following query, check the user field ::
index=botsv1 "3791.exe" sourcetype=xmlwineventlog EventCode=1

### Q3: Search hash on the virustotal. What other name is associated with this file 3791.exe?
Answer: ab.exe
