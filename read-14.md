##### [back-home](https://mhd22.github.io/301-reading-notes/)


# Read: 14a - DB Normalization

## Reasons for Database Normalization

***There are three main reasons to normalize a database.*** 

* The first is to minimize duplicate data. 
* The second is to minimize or avoid data modification issues.
* And the third is to simplify queries. 

#### _____________________________________________

### Data Duplication and Modification Anomalies

*Duplicated information presents two problems:*

1. It increases storage and decrease performance.
2. It becomes more difficult to maintain data changes.



**There are three modification anomalies that can occur:**

1. Insert Anomaly:
There are facts we cannot record until we know information for the entire row.  In our example we cannot record a new sales office until we also know the sales person.  Why?  Because in order to create the record, we need provide a primary key.  In our case this is the EmployeeID.

2. Update Anomaly:

In this case we have the same information in several rows. For instance if the office number changes, then there are multiple updates that need to be made.  *If we don’t update all rows, then inconsistencies appear*.

3. Deletion Anomaly:

![image](https://www.essentialsql.com/wp-content/uploads/2014/06/Intro-Deletion-Anomaly.png)

Deletion of a row causes removal of more than one set of facts.  For instance, if John Hunt retires, then deleting that row cause us to lose information about the New York office.

#### _____________________________________________

## Definition of Database Normalization:

**There are three common forms of database normalization: `1st`, `2nd`, and `3rd` normal form. They are also abbreviated as `1NF`, `2NF`, and `3NF` respectively.**

*The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in detail, let’s summarize the various forms:*

* `First Normal Form` – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

* `Second Normal Form` – The table is in first normal form and all the columns depend on the table’s primary key.

* `Third Normal Form` – the table is in second normal form and all of its columns are not transitively dependent on the primary key

#### _____________________________________________

## Conclusion:

*For now it’s important to understand there are three rules for database normalization that upon each other.*
*Some people make database normalization seem complicated.*
*but it doesn’t have to be, and once you understand it, it becomes intuitive.*

#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.