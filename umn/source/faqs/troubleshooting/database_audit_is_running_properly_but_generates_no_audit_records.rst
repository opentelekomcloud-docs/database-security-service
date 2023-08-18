:original_name: dbss_01_0256.html

.. _dbss_01_0256:

Database Audit Is Running Properly But Generates No Audit Records
=================================================================

Symptom
-------

The functions of the database audit instance are normal. When there is database traffic, audit information about the executed SQL statement cannot be found in the SQL statement list.

Possible Causes
---------------

-  SSL is enabled for the database.
-  ForceEncryption is enabled for the SQL Server database protocol.
-  The data volume is too large. As a result, the Agent process is suspended. You are advised to restart the container or optimize audit rules to reduce the data volume.

.. note::

   -  If SSL is enabled for a database, the database cannot be audited.
   -  If ForceEncryption is enabled for a database, database audit cannot obtain file content from the database for analysis.

Disabling Database SSL
----------------------

The MySQL database client is used as an example. Perform the following steps:

#. Log in to the MySQL database client as user **root**.

#. Run the following command to check the connection mode of the MySQL database:

   **\\s**

   -  If information similar to the following is displayed, SSL has been disabled for the MySQL database. Go to :ref:`4 <dbss_01_0256__li2733444154714>`.

      ::

         SSL:                    Not in use

   -  If information similar to the following is displayed, SSL has been enabled for the MySQL database. Go to :ref:`3 <dbss_01_0256__li135454178327>`.

      ::

         SSL:                    Cipher in use is XXX-XXX-XXXXXX-XXX

#. .. _dbss_01_0256__li135454178327:

   Log in to the MySQL database in SSL mode.

   a. Run the following command to exit from the MySQL database:

      **exit**

   b. .. _dbss_01_0256__li161711332142914:

      Log in to the MySQL database as user **root**.

      Add the following parameters at the end of the login command:

      **--ssl-mode=DISABLED**

      or

      **--ssl=0**

      .. important::

         If you log in to the MySQL database in SSL mode, you can only disable SSL for this login. To use the database audit function, log in to the MySQL database in the mode described in :ref:`3.b <dbss_01_0256__li161711332142914>`.

   c. Run the following command to check the connection mode of the MySQL database:

      **\\s**

      If information similar to the following is displayed, SSL has been disabled for the MySQL database. Go to :ref:`4 <dbss_01_0256__li2733444154714>`.

      ::

         SSL:                    Not in use

#. .. _dbss_01_0256__li2733444154714:

   Run an SQL statement and search for it in the SQL statement list.

   -  If the SQL statement is found, the problem has been solved.
   -  If the SQL statement is not found, the problem persists. In this case, :ref:`Disable ForceEncryption for the SQL Server protocol <dbss_01_0256__section139091244945>`.

.. _dbss_01_0256__section139091244945:

Disabling ForceEncryption for the SQL Server Protocol
-----------------------------------------------------

#. Open the **SQL Server Configuration Manager** dialog box.
#. Select **SQL Server Network Configuration**.
#. Right-click **Protocols for MSSQLSERVER** and choose **Properties**.
#. Click the **Flags** tab. Set **ForceEncryption** to **No**.
#. Restart the SQL Server service for the modification to take effect.
#. Run an SQL statement and search for it in the SQL statement list.

   -  If the SQL statement is found, the problem has been solved.
   -  If the SQL statement is not found, the problem persists. Contact customer service.
