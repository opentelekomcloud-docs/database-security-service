:original_name: dbss_01_0046.html

.. _dbss_01_0046:

Adding an SQL Whitelist
=======================

You can add risky SQL statements to the whitelist. The SQL statements in the whitelist will be ignored during the audit.

Constraints and Limitations
---------------------------

The risky SQL statements can be added to the whitelist in data reports.

Adding Scanned SQL Statements
-----------------------------

#. Log in to the management console.
#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.
#. In the navigation tree on the left, choose **Data Reports**. The **Data Reports** page is displayed.
#. In the **Instance** drop-down list, select the instance whose session information you want to view.
#. Click the **Statements** tab to view risky SQL statements.
#. Add SQL statements to the whitelist.

   -  Add a single SQL statement.

      a. Click **Add to Whitelist** in the **Operation** column of the target SQL statement.
      b. In the displayed dialog box, select the database and description of the target SQL statement.
      c. Click **OK**.

   -  Add SQL statements in batches.

      a. Select the target SQL statement and click **One-Clink Whitelisting**.
      b. In the displayed dialog box, select the database and description of the target SQL statement.
      c. Click **OK**.

Add a customized SQL statement.
-------------------------------

#. Log in to the management console.
#. Select a region, click |image2|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.
#. In the navigation tree on the left, choose **Audit Rules**.
#. In the **Instance** drop-down list, select the instance whose session information you want to view.
#. Click the **SQL Whitelist** tab and click **Add an SQL whitelist**.
#. In the dialog box that is displayed, enter the **SQL Statement**, **Applied to the Database**, and **Description**. Confirm the settings and click **OK**.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
.. |image2| image:: /_static/images/en-us_image_0000001074398929.png
