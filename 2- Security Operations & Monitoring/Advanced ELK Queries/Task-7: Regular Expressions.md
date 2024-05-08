## Regular expressions (regex) are powerful tools for pattern matching in text data. They allow you to search for complex patterns that cannot easily be found using simple query strings or wildcards. 

Example:
- **Description Starting with "s" or "m" and Containing "user":**
    ```
    Description:/(s|m).*/ AND /user.*/
    ```
    This query searches for entries in the "Description" field that start with either "s" or "m" and contain the word "user".

### How many incidents are there where a "client_list" file was affected by ransomware?
Answer: 70

Query: incident_type:/Ransomware.*/ AND /client_list.*/

### What is the name of the affected system at the earliest incident date that EVenis investigated with a filename containing the word "project"?
Answer: file-server-78

Run this Query and sort the timing filed 
Query: team_members.name:EVenis AND /.*project.*/
