## Note: First turn off the KQL search and you'll see lucene search

### Fuzzy searching is handy for finding documents with typos or inconsistencies in the data. It allows a specified number of character differences between the search term and the actual field value. For example, searching for "server" can return documents with variations like "serber" or "server01". Use the format `field_name:search_term~fuzziness_value` to perform a fuzzy search. In Kibana, switch to Lucene syntax for fuzzy searching, as boosting only works in Lucene.


### Including the misspellings, how many incidents has JLim handled where he misspelt the word “true”?
Answer: 110

Query: incident_comments:true~1  AND team_members.name:"JLim"

### How many incidents has JLim handled where he misspelt the word “negative”?
Answer: 4

Trick and Query:
First find correctly spelled words and then with mispelled words , you'll know the differece;
First query: incident_comments:negative  AND team_members.name:"JLim" (will return 115)
Second query: incident_comments:negative~2  AND team_members.name:"JLim" (will return 119)
