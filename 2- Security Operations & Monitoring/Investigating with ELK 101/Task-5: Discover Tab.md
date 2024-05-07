# [Discover Tab](https://tryhackme.com/r/room/investigatingwithelk101)

### Select the index vpn_connections and filter from 31st December 2021 to 2nd Feb 2022. How many hits are returned?
Answer: 2861

Hint: Select the mentioned data and see how many of events appear within that duration

### Which IP address has the max number of connections?
Answer: 238.163.231.224

Hint: Look at fields in left hand panel and click the source IP , you'll find the top 5 highest used IP.

### Which user is responsible for max traffic?
Answer: James

Hint: Look at username field

### Create a table with the fields IP, UserName, Source_Country and save
Answer: Expand the document (log events) and click addition button to create table with above mentioned fields

### Apply Filter on UserName Emanda; which SourceIP has max hits?
Answer: 107.14.1.247

Hint: Apply filter username and it will show the source IP on the table you created before this quesiton

### On 11th Jan, which IP caused the spike observed in the time chart?
Answer: 172.201.60.191

Hint: Either select date from data selection with time or just click the highest spike on time panel 

### How many connections were observed from IP 238.163.231.224, excluding the New York state?
Answer: 48

Hint: Add two filters : first source IP is 238.163.231.224 
                      : Second Source State is not New york
