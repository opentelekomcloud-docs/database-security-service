:original_name: dbss_01_0284.html

.. _dbss_01_0284:

How Does Database Audit Process Logs?
=====================================

Database audit logs are stored in a log database and processed based on disk usage.

-  If the disk usage of the log database is 85% or higher, the system automatically deletes the audit logs generated on the earliest date until the disk usage drops below 85%.
-  If the disk usage is 90% or higher, database audit stops and the system no longer saves new audit logs.
