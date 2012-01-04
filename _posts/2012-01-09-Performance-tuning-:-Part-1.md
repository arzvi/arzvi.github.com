---
Layout: blog
title: Performance Tuning tips for the lonely developer
summary: Series of posts to help the lonely developer tune his query and DB2 database code 
---

# {{ page.title }}

__09 Dec 2012 - Bangalore, India__
'There are tons of material on performance tuning and optimization for SQL and DB2 code online. Then why is this undertaking?' You may ask. What I felt reading each piece of knowledge from disparate sources when I started as a junior guy at my company were fear, confusion and very little success with huge time and effort put on it. There are great blog posts and reference materials that helped me gain confidence and understanding and confidence on working with DB2, and they will be listed during the end of the series. 
What I am trying to achieve here is to layout an interconnected knowledge pools to help the reader easily understand the basis of performance tuning and help him/her take a path to achieving good throughputs in their projects. 

###What is performance? 
Simply stated, it denotes the throughput of the object in question with the given resources. The object in question is our SQL and code (SPs/triggers/anonymous code blocks etc.) and the resource is our database composed of certain amount of memory and the priority assigned to the programmer as per the SLA agreed by the company. 

###What is performance tuning? 
The word 'performance' gets defined more along the lines of getting the 'maximum' throughput , and tuning is the way to achieve that. 


What do you have? 

1. data
2. requirement
3. SLA
4. factors that 'might' influence your codes throughput

To give a brief idea on what the above are :

1 Data - a flat file, a database or a schema or set of tables with data. 
2 Requirement - what is being expected out from your code - the functional correctness part.
3 SLA- What is the time duration within which the functionality is expected to get achieved. 
4 factors - job priorities (WLM), database resources or your next cabin developer who might try to hijack the entire database by running a table scan over a billion row table. Everything counts. 

Now when a junior developer starts working on a project, he might not know _everything about the data_ or the _factors_ and all he knows is the requirement and part of the _data_ that directly influences his work - i.e., the tables/schema. 

What do you ned to know to churn out good code in DB2? 
* [1. Understanding about the table constraints, RIs , data types and table indexes ][newpage]
* [2. Table statistics and their influence][newpage]
* [3. Tablespaces, index space, bufferpools and their related knowledge][newpage]
* [4. TBD][newpage]
* [5. TBD][newpage]
[newpage]: /assets/tbdeveloped.md "The page is yet to be written" 

I will work on mostly UDB as it is what I have experience on. Please subscribe to the email list to get notified as and when new content gets uploaded to this series. 

