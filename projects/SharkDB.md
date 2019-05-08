---
layout: project
type: project
image: images/shark1.png
title: SharksDatabase
permalink: projects/sharkDB
# All dates must be YYYY-MM-DD format!
date: 2017-12-08
labels:
  - Database
  - SQL
summary: I developed a database for an aquarium concentrated on sharks.
---

<div class="ui small rounded images">
</div>

For this project, I needed to develop a theoretical database for a subject of my choice. I chose to develop a database for sharks
at an aquarium. I created 4 tables that had primary and secondary keys so that there were relationships between tables. I filled 
all tables with at least 20 pieces of data. I also created queries of things a person working at an aquarium might want to see. For
an example there is an employee schedule table. Also, I created forms in the database so that data insertion would be easier.

By completing this project I became familiar with creating tables using SQL as well as joining tables. I was able to identify 
relationships between tables. This project required lots of planning to organize the tables how I desired. To avoid redoing the
database more than twice, an Entity-Relationship diagram was created to help organize the tables before actually creating the
database.

Here is an example of the SQL used to create the SharkInfo table:

```SQL
CREATE TABLE SharkInfo(  
SharkId CHAR(20) NOT NULL UNIQUE,  
FOREIGN KEY (SharkId) REFERENCES Sharks(SharkId),  
SharkType CHAR(20) NOT NULL,  
ScientificName CHAR(50) NOT NULL,  
Gender CHAR(7) NOT NULL,  
[Length(ft)] DOUBLE NOT NULL,  
[Weight(lbs)] DOUBLE NOT NULL,  
Age CHAR(2) NOT NULL,  
CHECK (Age < 30 And Age > 0)  
);  

Database provided on request.
