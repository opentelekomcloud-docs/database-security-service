:original_name: dbss_01_0001.html

.. _dbss_01_0001:

DBSS
====

Database Security Service (DBSS) is an intelligent database security service. Based on the big data analytics technologies, it can audit your databases, detect SQL injection attacks, and identify high-risk operations.

Supported Databases
-------------------

Database audit provides the audit function in out-of-path mode for the following databases on the management console:

-  Relational Database Service (RDS)
-  Databases built on ECS
-  Databases built on BMS

Database audit supports the following database types and versions.

.. _dbss_01_0001__table1221454114112:

.. table:: **Table 1** Database types and versions supported by database audit

   +-----------------------------------+----------------------------------------+
   | Database Type                     | Edition                                |
   +===================================+========================================+
   | GaussDB(for MySQL)                | MySQL 8.0                              |
   +-----------------------------------+----------------------------------------+
   | RDS for MySQL                     | -  5.6 (5.6.51.1 or later)             |
   |                                   | -  5.7 (5.7.29.2 or later)             |
   |                                   | -  8.0 (8.0.20.3 or later)             |
   +-----------------------------------+----------------------------------------+
   | PostgreSQL                        | -  14 (14.4 or later)                  |
   |                                   | -  13 (13.6 or later)                  |
   |                                   | -  12 (12.10 or later)                 |
   |                                   | -  11 (11.15 or later)                 |
   |                                   | -  9.6 (9.6.24 or later)               |
   |                                   | -  9.5 (9.5.25 or later)               |
   +-----------------------------------+----------------------------------------+
   | SQLServer                         | All editions are supported by default. |
   +-----------------------------------+----------------------------------------+

Service Features
----------------

-  Back up and restore database audit logs and meet the audit data retention requirements.
-  Monitor risks, sessions, session distribution, and SQL distribution in real time.
-  Report alarms for risky behaviors and attacks and responds to database attacks in real time.
-  Locate internal violations and improper operations and keep data assets secure.

Deployed in out-of-path pattern, database audit can perform flexible audit on the database without affecting user services.

-  Monitors database login, operation type (data definition, operation, and control), and operation object based on risky operations to effectively audit the database.
-  Analyzes risks, sessions, and SQL injection to help you master the database situation in a timely manner.
-  Provides a report template library to generate daily, weekly, or monthly audit reports according to your configurations. Sends real-time alarm notifications to help you obtain audit reports in a timely manner.
