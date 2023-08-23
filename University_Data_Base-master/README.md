This SQL project is an intricate database system crafted using SQL (DDL, DML) and PL/SQL languages, specifically designed around the Entity Relationship Diagram (ERD) provided as a JPG file in the project files link.

**Project Contents:**

**DDL**

**Tables:**
The project encompasses 24 tables (excluding the log ones) that meticulously store essential data as records (rows). These tables establish relationships among students, teachers, courses, and more than 15 other objects within the database.

**Log Tables:**
Each of the 24 tables has a corresponding log table, which plays a pivotal role in recording every manipulation (DML) made within the table. These log tables keep a detailed record of who performed the changes, what alterations were made, and when these changes took place.

**Triggers:**
A remarkable feature of this database is the extensive use of triggers. For each log table, three triggers are employed, resulting in a total of 72 triggers within the database. These triggers are responsible for automatically saving records about manipulations performed in the original tables into the log tables. They capture insertion, update, and deletion operations, along with the user responsible and the timestamp of the operation.

**Procedures:**
To cater to the multitude of users within the database, procedures have been developed. These procedures handle insertions into the student and employee tables, providing each individual with a unique username. Utilizing PL/SQL, these procedures also handle the execution of sequences, eliminating the need to manually input IDs for every insertion operation in the aforementioned tables.

**Sequences:**
The project employs three sequences to automate the generation of IDs for both male and female students, as well as employees. The sequence for male students resets annually, generating IDs from 1(year)0001 to 1(year)9999. This design allows for easy registration of students, and additional IDs can be accommodated simply by appending zeroes after the year.

**Roles:**
Security is a paramount concern, and to ensure data integrity, roles have been established. Each student has a specific role that restricts them from altering any records other than their own, thus enhancing data security within the database.

**Views:**
For efficiency and enhanced security, a set of views has been created. These views facilitate complex queries and contribute to smoother database operations.

**DML**

**Existing Records:**
Pre-loaded records serve as a validation mechanism for the functionality of the database. These records can be retained, deleted, or omitted as required.

**PL/SQL:**
The project intricately employs PL/SQL in triggers and procedures, enriching the project's functionality and capabilities.
