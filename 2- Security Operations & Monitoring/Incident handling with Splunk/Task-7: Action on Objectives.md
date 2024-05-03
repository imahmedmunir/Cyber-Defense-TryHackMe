### Q1: What is the name of the file that defaced the imreallynotbatman.com website ?
Answer: poisonivy-is-coming-for-you-batman.jpeg

### Q2: Fortigate Firewall 'fortigate_utm' detected SQL attempt from the attacker's IP 40.80.148.42. 
### What is the name of the rule that was triggered during the SQL Injection attempt?

Answer: HTTP.URI.SQL.Injection

As hint is given for this question, run the following query and check for attack field::
index=botsv1 dest=192.168.250.70 sourcetype=fortigate_utm src="40.80.148.42" eventtype=ftnt_fortigate_utm 
