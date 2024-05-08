## Note: stay in lucene search format

### Proximity searches find documents with terms close to each other. Use the format `field_name:"search term"~slop_value` in KQL. For instance:

- To find "server" and "error" within 1 word: `log_message:"server error"~1`
- For "failed login" with no gap: `log_message:"failed login"~0`
In Kibana, use Lucene syntax. For example: `log_message:"server error"~4`. Use operators like AND and OR for complex queries, such as `log_message:"server error"~1 OR "login server"~1`.


### How many incidents are there when you want to look for the words "data leak" and "true negative" in the comments that are at least 3 words in between them?
Answer: 33

Query: incident_comments: "data leak true negative"~3

### How many incidents has AJohnston investigated that have the words "detected" and "negative" in the comments that are two words apart?
Answer: 40

Query:   incident_comments: "detected negative"~2 AND team_members.name:"AJohnston"
