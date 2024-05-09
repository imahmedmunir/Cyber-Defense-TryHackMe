# Link on TryHackMe: [Slingshot](https://tryhackme.com/r/room/slingshot)

### What was the attacker's IP?
Answer: 10.0.2.15

Hint: Look at " transaction.remote_address" filed

### What was the first scanner that the attacker ran against the web server?
Answer: nmap scripting engine

Hint: For finding scanner , look at user agent used.

### What was the User Agent of the directory enumeration tool that the attacker used on the web server?
Answer: Mozilla/5.0 GoBuster

Hint: Still look at user agent, it will give you the name of directory enumeration tool (used to find directories)

### In total, how many requested resources on the web server did the attacker fail to find?
Answer: 1867

Hint: if requested failed or not found status code will be 404

### What is the flag under the interesting directory the attacker found?
Answer: a76637b62ea99acda12f5859313f539a

Hint: backup is interesting directory and look at request_line

### What login page did the attacker discover using the directory enumeration tool?
Answer: /admin-login.php

### What was the user agent of the brute-force tool that the attacker used on the admin panel?
Answer: Mozilla/4.0 Hydra

Hint: look at user agent

### What username:password combination did the attacker use to gain access to the admin page?
Answer: admin:thx1138

Query: http.url: "/admin/"  , you'll find basic authentication. Decode it using base64

### What flag was included in the file that the attacker uploaded from the admin directory?
Answer: THM{ecb012e53a58818cbd17a924769ec447}

Hint: same query above , just look the file being uploaded and expland the message

### What was the first command the attacker ran on the web shell?
Answer: whoami

Hint: explore the same query above , you'll find the answer

### What file location on the web server did the attacker extract database credentials from using Local File Inclusion?
Answer: /etc/phpmyadmin/config-db.php

### What directory did the attacker use to access the database manager?
Answer: /phpmyadmin

### What was the name of the database that the attacker exported?
Answer: customer_credit_cards

### What flag does the attacker insert into the database?
Answer: c6aa3215a7d519eeb40a660f3b76e64c
