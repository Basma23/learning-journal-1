# DATABASE NORMALIZATION
**Database normalization** is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. 

There are three normal forms most databases adhere to using.  As tables satisfy each successive database normalization form, they become less prone to database modification anomalies and more focused toward a sole purpose or topic.

**Reasons for Database Normalization**
- Minimize duplicate data 
- minimize or avoid data modification issues
- simplify queries. 

**Data Duplication and Modification Anomalies**

Duplicated information presents two problems:
1- It increases storage and decrease performance.
2- It becomes more difficult to maintain data changes

**Definition of Database Normalization**
There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 

The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. 
1- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
2- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
3- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key.

