:original_name: dbss_01_0313.html

.. _dbss_01_0313:

Constraints
===========

Database audit is subject to certain constraints.

Supported Database Types
------------------------

The following types of databases on the management console can be audited in out-of-path mode:

-  RDS instances
-  Databases built on ECS
-  Databases built on BMS

Supported Database Versions
---------------------------

The following database versions can be audited.

.. table:: **Table 1** Database types and versions supported by database audit

   ================== =========
   Database Type      Edition
   ================== =========
   GaussDB(for MYSQL) MYSQL 8.0
   ================== =========

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
