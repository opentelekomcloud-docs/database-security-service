:original_name: dbss_01_0205.html

.. _dbss_01_0205:

Viewing SQL Statement Details
=============================

After connecting the database to the database audit instance, view SQL statements of the database.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.
-  Database audit has been enabled.

Procedure
---------

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Data Reports**. The **Data Reports** page is displayed.

#. In the **Instance** drop-down list, select the instance whose SQL statement information you want to view.

#. Click the **Statements** tab.

#. View SQL statement information.


   .. figure:: /_static/images/en-us_image_0000001294276970.png
      :alt: **Figure 1** Querying SQL statements

      **Figure 1** Querying SQL statements

   To query a specified SQL statement, perform the following steps:

   -  Select **All**, **Last 30 minutes**, **1 hour**, **24 hours**, **7 days**, or **30 days** for **Time** and click |image2| to view SQL statements of the specified time range.
   -  Select **All**, **High**, **Moderate**, **Low**, or **Trusted** for **Risk Severity** and click |image3|. SQL statements of specified severity are displayed in the list.

      .. note::

         A maximum of 10,000 records can be retrieved in a query.

#. In the row containing the desired SQL statement, click **Details** in the **Operation** column.

#. View the SQL statement information in the **Details** dialog box. For details about related parameters, see :ref:`Table 1 <dbss_01_0205__table14884152602217>`.

   .. important::

      The maximum length of an audit statement or result set is 10,240 bytes. Excessive parts are not recorded in audit logs.

   .. _dbss_01_0205__table14884152602217:

   .. table:: **Table 1** Parameters for details of SQL statements

      +---------------------------------+----------------------------------------------------------------------------------+
      | Parameter                       | Description                                                                      |
      +=================================+==================================================================================+
      | Session ID                      | ID of an SQL statement, which is automatically generated                         |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database Instance               | Database where an SQL statement is executed                                      |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database Type                   | Type of the database where an SQL statement is executed                          |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database User                   | Database user for executing an SQL statement                                     |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Client MAC Address              | MAC address of the client where an SQL statement is executed                     |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database MAC Address            | MAC address of the database where an SQL statement is executed                   |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Client IP Address               | IP address of the client where an SQL statement is executed                      |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database IP Address/Domain Name | IP address or the domain name of the database where an SQL statement is executed |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Client Port                     | Port of the client where an SQL statement is executed                            |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Database Port                   | Port of the database where the SQL statement is executed                         |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Client Name                     | Name of the client where an SQL statement is executed                            |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Operation Type                  | Type of an SQL statement operation                                               |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Operation Object Type           | Type of an SQL statement operation object                                        |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Response Result                 | Response by executing an SQL statement                                           |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Affected Rows                   | Number of rows affected by executing an SQL statement                            |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Started                         | Time when an SQL statement starts to be executed                                 |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Ended                           | Time when the SQL statement execution ends                                       |
      +---------------------------------+----------------------------------------------------------------------------------+
      | SQL Statement                   | Name of an SQL statement                                                         |
      +---------------------------------+----------------------------------------------------------------------------------+
      | Request Result                  | Result of requesting for executing an SQL statement                              |
      +---------------------------------+----------------------------------------------------------------------------------+

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
.. |image2| image:: /_static/images/en-us_image_0000001625668645.png
.. |image3| image:: /_static/images/en-us_image_0000001626494753.png
