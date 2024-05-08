### How many "Data Leak" incidents have a severity level of 9 and up?
Answer: 52

Query: incident_type : "Data Leak" AND severity_level >= 9

### How many incidents before December 1st, 2022 has AJohnston investigated where the affected system is either an Email or Web server?
Answer: 63

Query: @timestamp<=2022-01-12 AND affected_systems.system_name : "Email" or "Web Server" AND  team_members.name : "AJohnston" 

### From the incident IDs 1 to 500, what is the email address of the SOC Analyst that left a comment on an incident that the data leak on file-server-65 is a false positive?
Answer: jlim@cybert.com

Query: After query look into logs where at file-server-56
