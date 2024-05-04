# Link on TryHackMe: [Identify and Investigate an Infected Host](https://tryhackme.com/r/room/benign)

### How many logs are ingested from the month of March, 2022?
Answer: 13959

Hint: after selecting "index=win_eventlogs", select data from when to show

### Imposter Alert: There seems to be an imposter account observed in the logs, what is the name of that user?
Answer: Amel1a

Query: index=win_eventlogs AND stats count by UserName

### Which user from the HR department was observed to be running scheduled tasks?
Answer: Chris.fort

Query: index=win_eventlogs AND schtasks

### Which user from the HR department executed a system process (LOLBIN) to download a payload from a file-sharing host.
Answer: haroon

Query: index=win_eventlogs AND certutil.exe (hint provided on tryhackme)

### To bypass the security controls, which system process (lolbin) was used to download a payload from the internet?
Answer: certutil.exe

### What was the date that this binary was executed by the infected host? format (YYYY-MM-DD)
Answer: 2022-03-04

### Which third-party site was accessed to download the malicious payload?
Answer: https://controlc.com/e4d11035

### What is the name of the file that was saved on the host machine from the C2 server during the post-exploitation phase?
Answer: benign.exe

### The suspicious file downloaded from the C2 server contained malicious content with the pattern THM{..........}; what is that pattern?
Answer: THM{KJ&*H^B0}

Caution: visit this link (https://controlc.com/e4d11035) to read content but in safe environment , preferrably in attackbox of tryhackme  

### What is the URL that the infected host connected to?
Answer: https://controlc.com/e4d11035
