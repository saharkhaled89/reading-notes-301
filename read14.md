# Database Normalization

**Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.**

# Reasons for Database Normalization

**There are three main reasons to normalize a database:**

*  minimize duplicate data

* minimize or avoid data modification issues

* simplify queries

# Data Duplication and Modification Anomalies

**Notice that for each SalesPerson we have listed both the SalesOffice and OfficeNumber.  There is duplicate sales person data.  Duplicated information presents two problems:**

* It increases storage and decrease performance.
* It becomes more difficult to maintain data changes.

# Insert Anomaly

**Database Normalization -  Insert Anomaly**

*There are facts we cannot record until we know information for the entire row.  In our example we cannot record a new sales office until we also know the sales person.  Why?  Because in order to create the record, we need provide a primary key.  In our case this is the EmployeeID.*

# Definition of Database Normalization

**There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively.**

* **First Normal Form** – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

* **Second Normal Form** – The table is in first normal form and all the columns depend on the table’s primary key.

* **Third Normal Form** – the table is in second normal form and all of its columns are not transitively dependent on the primary key



