
### What version of TOR Browser did Amber install to obfuscate her web browsing? Answer guidance: Numeric with one or more delimiter.
Answer: 7.0.4

Query: index="botsv2" tor amber (look at image field)

### What is the public IPv4 address of the server running www.brewertalk.com?
Answer:52.42.208.228

Query: index="botsv2" brewertalk.com and look at destination IP address (public not private)

### Provide the IP address of the system used to run a web vulnerability scan against www.brewertalk.com.
Answer: 45.77.65.211

Query: index="botsv2" brewertalk.com and look at source IP address

### The IP address from Q#2 is also being used by a likely different piece of software to attack a URI path. What is the URI path? Answer guidance: 
### Include the leading forward slash in your answer. Do not include the query string or other parts of the URI. Answer example: /phpinfo.php
Answer: /member.php

Query: index="botsv2" src_ip="45.77.65.211" (look at uri_path field which uri being hit maximum number of times)

### What SQL function is being abused on the URI path from the previous question?
Answer: updatexml

Query: index="botsv2" src_ip="45.77.65.211" uri_path="/member.php"
| dedup form_data
| table form_data

### What was the value of the cookie that Kevin's browser transmitted to the malicious URL as part of an XSS attack? Answer guidance: 
### All digits. Not the cookie name or symbols like an equal sign.
Answer: 1502408189

Query: index="botsv2" kevin sourcetype="stream:http" tag=error | table cookie

### What brewertalk.com username was maliciously created by a spear phishing attack?
Answer: kIagerfield

Query: index="botsv2" sourcetype="stream:http" 1bc3eab741900ab25c98eee86bf20feb (look at form data)
