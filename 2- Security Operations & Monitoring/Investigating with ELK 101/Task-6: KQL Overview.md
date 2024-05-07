# [Kibana Query Language (KQL) Overview](https://tryhackme.com/r/room/investigatingwithelk101)

### Create a search query to filter out the logs from Source_Country as the United States and show logs from User James or Albert. How many records were returned?
Answer: 161

Query: Source_Country : "United States" and UserName : "Albert" or UserName : "James" 

### As User Johny Brown was terminated on 1st January 2022, create a search query to determine how many times a VPN connection was observed after his termination.
Answer: 1

Query: UserName : "Johny Brown" 
