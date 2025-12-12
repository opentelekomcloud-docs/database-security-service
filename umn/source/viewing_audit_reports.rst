:original_name: dbss_01_0248.html

.. _dbss_01_0248:

Viewing Audit Reports
=====================

By default, database audit complies with a full audit rule, which is used to audit all databases that are connected to the database audit instance. After connecting the database to the database audit instance, generate an audit report and preview online or download it.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.
-  Database audit has been enabled.

Report Types
------------

Database audit provides eight types of report templates. :ref:`Table 1 <dbss_01_0248__table5352332171212>` lists the report names. You can generate reports and set report tasks as needed.

.. _dbss_01_0248__table5352332171212:

.. table:: **Table 1** Description

   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Template Name                       | Report Type               | Description                                                                                                                                                                                                                   |
   +=====================================+===========================+===============================================================================================================================================================================================================================+
   | Database Security General Report    | Overview report           | Provides the overall audit status of the database, including risks, sessions, and login status to better manage databases.                                                                                                    |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Database Security Compliance Report | Compliance report         | This report helps database administrators and auditors detect abnormal behaviors, locate problems, and manage information.                                                                                                    |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | SOX Report                          | Compliance report         | Complies with the Sarbanes-Oxley Act (SOX) to provide statics on and evaluate database operations. This report helps database administrators and auditors detect abnormal behaviors, locate problems, and manage information. |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Database Server Analysis Report     | Database report           | Provides statistics and analysis on active users, user IP addresses, database logins and requests, database usage duration, and database performance.                                                                         |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | Client IP Address Analysis Report   | Client report             | Provides statistics on client applications, database users, and SQL statements collected from user IP addresses.                                                                                                              |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | DML Command Report                  | Database operation report | Analyzes user and privileged operations based on DML commands.                                                                                                                                                                |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | DDL Command Report                  | Database operation report | Analyzes user and privileged operations based on DDL commands.                                                                                                                                                                |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | DCL Command Report                  | Database operation report | Analyzes user and privileged operations based on DCL commands.                                                                                                                                                                |
   +-------------------------------------+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Step 1: Generating a Report
---------------------------

You can generate reports immediately or periodically. You can also customize the generation time, frequency, and format of reports.

-  **Method 1: Generating a Report Immediately**

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Reports**.

#. In the **Instance** drop-down list, select the instance whose instance report you want to generate.

#. Click the **Report Management** tab.

#. In the **Operation** column of a report template, click **Generate Report**.


   .. figure:: /_static/images/en-us_image_0000001581231593.png
      :alt: **Figure 1** Report template list

      **Figure 1** Report template list

#. In the displayed dialog box, click |image2| to set the start time and end time of the report, and select the database for which you want to generate a report.


   .. figure:: /_static/images/en-us_image_0000001530712248.png
      :alt: **Figure 2** Generate Report

      **Figure 2** Generate Report

#. Click **OK**.

-  **Method 2: Setting Periodic Report Release**

#. Log in to the management console.

#. Select a region, click |image3|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Reports**.

#. In the **Instance** drop-down list, select the instance for which you want to set a report task.

#. Click the **Report Management** tab.

#. Locate the target template and click **Schedule Task** in the **Operation** column.


   .. figure:: /_static/images/en-us_image_0000001530872056.png
      :alt: **Figure 3** Setting a task

      **Figure 3** Setting a task

#. In the displayed dialog box, set the parameters of the scheduled task. For details about related parameters, see :ref:`Table 2 <dbss_01_0248__table7222934463>`.


   .. figure:: /_static/images/en-us_image_0000001531037008.png
      :alt: **Figure 4** Setting a scheduled task

      **Figure 4** Setting a scheduled task

   .. _dbss_01_0248__table7222934463:

   .. table:: **Table 2** Parameters for setting a task

      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                                                                             | Example Value         |
      +=======================+=========================================================================================================================================================================================+=======================+
      | Enable Task           | Status of a scheduled task.                                                                                                                                                             | |image6|              |
      |                       |                                                                                                                                                                                         |                       |
      |                       | -  |image4|: disabled                                                                                                                                                                   |                       |
      |                       | -  |image5|: enabled                                                                                                                                                                    |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Message Notifications | Enables or disables notifications.                                                                                                                                                      | |image9|              |
      |                       |                                                                                                                                                                                         |                       |
      |                       | |image7|: enabled                                                                                                                                                                       |                       |
      |                       |                                                                                                                                                                                         |                       |
      |                       | |image8|: disabled                                                                                                                                                                      |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | SMN Topic             | Select an existing topic from the drop-down list or click **View Topic** and create an SMN topic on the displayed page for configuring the terminals for receiving alarm notifications. | ``-``                 |
      |                       |                                                                                                                                                                                         |                       |
      |                       | For details about topics and subscriptions, see *Simple Message Notification User Guide*.                                                                                               |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Report Type           | Type of a report. The options are as follows:                                                                                                                                           | Weekly                |
      |                       |                                                                                                                                                                                         |                       |
      |                       | -  **Daily**                                                                                                                                                                            |                       |
      |                       | -  **Weekly**                                                                                                                                                                           |                       |
      |                       | -  **Monthly**                                                                                                                                                                          |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Execution Mode        | Execution mode of the report. The options are as follows:                                                                                                                               | Periodically          |
      |                       |                                                                                                                                                                                         |                       |
      |                       | -  **Once**                                                                                                                                                                             |                       |
      |                       | -  **Periodically**                                                                                                                                                                     |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Time                  | Time when the report is executed                                                                                                                                                        | 10:00                 |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Format                | Only the PDF format is supported.                                                                                                                                                       | PDF                   |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Database              | Database for which you want to execute the report task                                                                                                                                  | ``-``                 |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **OK**.

Step 2: Previewing and Downloading Audit Reports
------------------------------------------------

Before previewing or downloading an audit report, ensure that its **Status** is **100%**.

.. important::

   To preview a report online, use Google Chrome or Mozilla FireFox.

#. Log in to the management console.

#. Select a region, click |image10|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Reports**.

#. In the **Instance** drop-down list, select the instance whose report you want to preview or download.

#. Locate the target template, and click **Preview** or **More** > **Download** in the **Operation** column to preview or download the report.


   .. figure:: /_static/images/en-us_image_0000001581439873.png
      :alt: **Figure 5** Previewing or downloading an audit report

      **Figure 5** Previewing or downloading an audit report

.. |image1| image:: /_static/images/en-us_image_0000001529391298.png
.. |image2| image:: /_static/images/en-us_image_0000001148025398.png
.. |image3| image:: /_static/images/en-us_image_0000001074398929.png
.. |image4| image:: /_static/images/en-us_image_0000001570821361.png
.. |image5| image:: /_static/images/en-us_image_0000001581357417.png
.. |image6| image:: /_static/images/en-us_image_0000001530568420.png
.. |image7| image:: /_static/images/en-us_image_0000001581127865.png
.. |image8| image:: /_static/images/en-us_image_0000001581247597.png
.. |image9| image:: /_static/images/en-us_image_0000001581447801.png
.. |image10| image:: /_static/images/en-us_image_0000001074398929.png
