# Link on Tryhackme: [Incident Handling with Splunk](https://tryhackme.com/r/room/splunk201)

### Task-1 : ONLY Reading

## Task-2: ONLY Reading

## Task-3: ONLY Reading

## Task-4 : Reconnaissance Phase

Run this query on search header first
(index="botsv1" imreallynotbatman.com src_ip="40.80.148.42" sourcetype=suricata)

Q1: One suricata alert highlighted the CVE value associated with the attack attempt. What is the CVE value?
Answer: CVE-2014-6271

Q2: What is the CMS our web server is using?
Answer: joomla

(after search query , look at the url)

Q3: What is the web scanner, the attacker used to perform the scanning attempts?
Answer: acunetix 

(look at the user agent)

Q4: What is the IP address of the server imreallynotbatman.com?
Answer: 192.168.250.70

(Look at desination IP address)
