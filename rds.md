## Task 1: Creating an Amazon RDS database
In this task, you create a MySQL database in your virtual private cloud (VPC). MySQL is a popular open-source relational database management system (RDBMS), so there are no software licensing fees.

On the Services  menu, choose RDS.
Choose Create database
For this lab, you will keep the Choose a database creation method as Standard create to understand the full set of features available.

Under Engine options, select  MySQL.\
For Version, keep MySQL 8.0.28.
In the options, you might notice Amazon Aurora. Aurora is a global-scale relational database service built for the cloud with full MySQL and PostgreSQL compatibility. If your company uses large-scale MySQL or PostgreSQL databases, Aurora can provide enhanced performance.
```
MySQL version 8.0.28
```
![image](./images/database-creation.png)
In the Templates section, select  Dev/Test (This instance is intended for development use outside of a production environment).\
You can now select a database configuration, including software version, instance class, storage, and login settings. The Multi-AZ deployment option automatically creates a replica of the database in a second Availability Zone for high availability.\

In the Availability and durability section, choose Single DB instance

In the Settings section next, configure the following options:
```
DB instance identifier: inventory-db

Master username: admin

Master password: lab-password
Confirm password: lab-password
```
- Note: Please use these values verbatim, do not make any changes.

In the Instance configuration section, configure the following options for DB instance class:
Choose  Burstable classes (includes t classes).
```
Choose db.t3.micro.
```

