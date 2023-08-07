:original_name: dbss_01_0283.html

.. _dbss_01_0283:

How Do I Disable SSL for a Database?
====================================

If SSL is enabled for a database, the database cannot be audited. To use database audit, disable SSL first.

The MySQL database client is used as an example. Perform the following steps:

#. Log in to the MySQL database client as user **root**.

#. Run the following command to check the connection mode of the MySQL database:

   **\\s**

   -  If information similar to the following is displayed, SSL has been disabled for the MySQL database.

      ::

         SSL:                    Not in use

   -  If information similar to the following is displayed, SSL has been enabled for the MySQL database. Go to :ref:`3 <dbss_01_0283__li10221135254320>`.

      ::

         SSL:                    Cipher in use is XXX-XXX-XXXXXX-XXX

#. .. _dbss_01_0283__li10221135254320:

   Log in to the MySQL database in SSL mode.

   a. Run the following command to exit from the MySQL database:

      **exit**

   b. Log in to the MySQL database as user **root**.

      Add the following parameters at the end of the login command:

      **--ssl-mode=DISABLED**

      Or

      **--ssl=0**

      .. important::

         If you logged in to the MySQL database in SSL mode, you can disable SSL only for this login. To use the database audit function, log in to the MySQL database as instructed in this step.

   c. Run the following command to check the connection mode of the MySQL database:

      **\\s**

      If information similar to the following is displayed, SSL has been disabled for the MySQL database.

      ::

         SSL:                    Not in use
