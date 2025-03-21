:original_name: dbss_01_0047.html

.. _dbss_01_0047:

Managing an SQL Whitelist
=========================

You can edit, disable, and delete the added SQL statement whitelist.

Prerequisites
-------------

The SQL statement to be associated has been added to the whitelist.

Procedure
---------

#. Log in to the management console.
#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.
#. In the navigation tree on the left, choose **Audit Rules**.
#. In the **Instance** drop-down list, select the instance whose session information you want to view.
#. Click the **SQL Whitelist** tab to view all SQL statement whitelists.
#. Manage the whitelist.

   -  Click **Edit** in the **Operation** column of the target SQL statement to modify the description and applied database.

   -  Click **Disable** in the **Operation** column of the target SQL statement. The disabled statement does not execute the rule in the audit.

      .. note::

         After the SQL statement is disabled, there is a delay of about 1 minute.

   -  Click **Delete** in the **Operation** column of the target SQL statement. The deleted SQL statement cannot be restored. You can only add the SQL statement to the whitelist again. The SQL statement will be scanned again.

      To delete multiple SQL statements from the whitelist, select the SQL statements to be deleted, click **Delete All** and confirm the deletion.

      .. note::

         After the SQL whitelist is modified, the modification does not take effect on the audited data.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
