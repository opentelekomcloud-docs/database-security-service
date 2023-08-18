:original_name: dbss_01_0268.html

.. _dbss_01_0268:

Editions
========

Database audit provides basic, professional, and advanced editions. You can select one of them as needed.

:ref:`Table 1 <dbss_01_0268__en-us_topic_0110856029_table8767123235>` describes the database audit editions.

.. _dbss_01_0268__en-us_topic_0110856029_table8767123235:

.. table:: **Table 1** Database audit editions

   +-----------------+-------------------+------------------+------------------------------------------------------+
   | Version         | Maximum Databases | System Resource  | Performance                                          |
   +=================+===================+==================+======================================================+
   | Basic           | 3                 | -  CPU: 4 vCPUs  | -  Peak QPS: 3,000 queries/second                    |
   |                 |                   | -  Memory: 16 GB | -  Database load rate: 3.6 million statements/hour   |
   |                 |                   | -  Disk: 500 GB  | -  Stores 400 million online SQL statements.         |
   |                 |                   |                  | -  Stores 5 billion archived SQL statements.         |
   +-----------------+-------------------+------------------+------------------------------------------------------+
   | Professional    | 6                 | -  CPU: 8 vCPUs  | -  Peak QPS: 6,000 queries/second                    |
   |                 |                   | -  Memory: 32 GB | -  Database load rate: 7.2 million statements/hour   |
   |                 |                   |                  | -  Stores 600 million online SQL statements.         |
   |                 |                   |                  | -  Stores 10 billion archived SQL statements.        |
   +-----------------+-------------------+------------------+------------------------------------------------------+
   | Advanced        | 30                | -  CPU: 16 vCPUs | -  Peak QPS: 30,000 queries/second                   |
   |                 |                   | -  Memory: 64 GB | -  Database load rate: 10.80 million statements/hour |
   |                 |                   |                  | -  Stores 1.5 billion online SQL statements.         |
   |                 |                   |                  | -  Stores 60 billion archived SQL statements.        |
   +-----------------+-------------------+------------------+------------------------------------------------------+

.. note::

   -  A database instance is uniquely defined by its database IP address and port.

      The number of database instances equals the number of database ports. If a database IP address has N database ports, there are N database instances.

      Example: A user has two database IP addresses, IP\ :sub:`1` and IP\ :sub:`2`. IP\ :sub:`1` has a database port. IP\ :sub:`2` has three database ports. IP\ :sub:`1` and IP\ :sub:`2` have four database instances in total. To audit all of them, select professional edition DBSS, which supports a maximum of six database instances.

   -  To change the edition of a DBSS instance, unsubscribe from it and apply for a new one.

   -  Online SQL statements are counted based on the assumption that the capacity of an SQL statement is 1 KB.
