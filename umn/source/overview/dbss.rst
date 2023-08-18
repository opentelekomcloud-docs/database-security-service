:original_name: dbss_01_0001.html

.. _dbss_01_0001:

DBSS
====

Database Security Service (DBSS) is an intelligent database security service. Based on the machine learning mechanism and big data analytics technologies, it can audit your databases, detect SQL injection attacks, and identify high-risk operations.

Supported Databases
-------------------

Database audit provides the audit function in out-of-path mode for the following databases on the management console:

-  RDS instances
-  Databases built on ECS
-  Databases built on BMS

Database audit supports the following database types and versions.

.. table:: **Table 1** Database types and versions supported by database audit

   ================== =========
   Database Type      Edition
   ================== =========
   GaussDB(for MYSQL) MYSQL 8.0
   ================== =========

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
