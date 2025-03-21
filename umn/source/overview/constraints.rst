:original_name: dbss_01_0313.html

.. _dbss_01_0313:

Constraints
===========

Database audit is subject to certain constraints.

Supported Database Types
------------------------

The following types of databases on the management console can be audited in out-of-path mode:

-  Relational Database Service (RDS)
-  Databases built on ECS
-  Databases built on BMS

Databases That Need Agents
--------------------------

The following database versions can be audited.

.. table:: **Table 1** Database types and versions supported by database audit

   +-----------------------------------+----------------------------------------+
   | Database Type                     | Edition                                |
   +===================================+========================================+
   | GaussDB(for MYSQL)                | MYSQL 8.0                              |
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

Supported OSs
-------------

To use database audit, you need to install its agent on database nodes or application nodes. The database audit agent can run on the 64-bit Linux.

-  For more information, see :ref:`Table 2 <dbss_01_0313__table11754943124117>`.

   .. _dbss_01_0313__table11754943124117:

   .. table:: **Table 2** Supported Linux OS versions

      +-----------------------------------+-----------------------------------+
      | System Name                       | System version                    |
      +===================================+===================================+
      | CentOS                            | -  CentOS 7.0 (64bit)             |
      |                                   | -  CentOS 7.1 (64bit)             |
      |                                   | -  CentOS 7.2 (64bit)             |
      |                                   | -  CentOS 7.3 (64bit)             |
      |                                   | -  CentOS 7.4 (64bit)             |
      |                                   | -  CentOS 7.5 (64bit)             |
      |                                   | -  CentOS 7.6 (64bit)             |
      |                                   | -  CentOS 8.1 (64bit)             |
      |                                   | -  CentOS 8.2 (64bit)             |
      +-----------------------------------+-----------------------------------+
      | Debian                            | -  Debian 7.5.0 (64bit)           |
      |                                   | -  Debian 8.2.0 (64bit)           |
      |                                   | -  Debian 8.8.0 (64bit)           |
      |                                   | -  Debian 9.0.0 (64bit)           |
      |                                   | -  Debian 10.0.0 (64bit)          |
      +-----------------------------------+-----------------------------------+
      | Fedora                            | -  Fedora 24 (64bit)              |
      |                                   | -  Fedora 25 (64bit)              |
      +-----------------------------------+-----------------------------------+
      | SUSE                              | -  SUSE 11 SP4 (64bit)            |
      |                                   | -  SUSE 12 SP1 (64bit)            |
      |                                   | -  SUSE 12 SP2 (64bit)            |
      +-----------------------------------+-----------------------------------+
      | Ubuntu                            | -  Ubuntu 14.04 (64bit)           |
      |                                   | -  Ubuntu 16.04 (64bit)           |
      |                                   | -  Ubuntu 18.04 (64bit)           |
      |                                   | -  Ubuntu 20.04 (64-bit)          |
      +-----------------------------------+-----------------------------------+
      | EulerOS                           | -  Euler 2.2 (64bit)              |
      |                                   | -  Euler 2.3 (64bit)              |
      +-----------------------------------+-----------------------------------+
      | Oracle Linux                      | -  Oracle Linux 6.9 (64bit)       |
      |                                   | -  Oracle Linux 7.4 (64bit)       |
      +-----------------------------------+-----------------------------------+

Other Constraints
-----------------

-  If SSL is enabled for a database, the database cannot be audited. To use database audit, disable SSL first.
-  In some SQL Server databases, complex **declare** statements, **select** functions, and symbol statements that cannot be identified by the system may fail to be parsed.
