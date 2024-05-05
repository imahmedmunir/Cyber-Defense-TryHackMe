# Link on TryHackMe: [Splunk 2](https://tryhackme.com/r/room/splunk2gcd5)

### Amber Turing was hoping for Frothly to be acquired by a potential competitor which fell through, but visited their website to find contact information for their executive team. 
### What is the website domain that she visited?
Answer: www.berkbeer.com

Query: index="botsv2" sourcetype="stream:http" 
| dedup site
| table site

### Amber found the executive contact information and sent him an email. What image file displayed the executive's contact information? Answer example: /path/image.ext
Answer: /images/ceoberk.png

Hint: check uri-path

### What is the CEO's name? Provide the first and last name.
Answer: Martin Berk

Hint: read the body content

### What is the CEO's email address?
Answer: mberk@berkbeer.com

Hint: read the content 

### After the initial contact with the CEO, Amber contacted another employee at this competitor. What is that employee's email address?
Answer:  hbernhard@berkbeer.com 

### What is the name of the file attachment that Amber sent to a contact at the competitor?
Answer: Saccharomyces_cerevisiae_patent.docx

### What is Amber's personal email address?
Answer: ambersthebest@yeastiebeastie.com

Explanation: As hint is given, read the content and decode them using base64
