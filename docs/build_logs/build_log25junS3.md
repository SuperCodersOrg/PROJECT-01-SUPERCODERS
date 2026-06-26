Date : 25 June 2026 (Session 3)
Duration: 3 hours 30 mins

Goal():
Testing thorougly with the main.cpp file for the hashmap and starting to implement the redislite using hashmap 

what I Tried():
Understodd about how everthing works and how dynamic array linkedlist and hashmap will work for the creating of the redis lit. 

Redislite is like a tool which will create realworld application combinining all these implemented data structures.

I have created a flow from my understanding which is given below
Parser

↓

RedisLite

↓

HashMap.find()

↓

Bucket

↓

Linked List Search

↓

Value

Redis Uses the hashmap internally due to which it is fast in nature. It is a in-memory key-value database which is been created in RAM due to which this is much faster than others.

Started with the basic class skeleton for the redislite been created in redislite.hpp 
The redislit function which i will implement in this will be    
SET GET DEL EXISTS DBSIZE and FLUSHALL 