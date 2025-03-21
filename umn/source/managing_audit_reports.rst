:original_name: dbss_01_0196.html

.. _dbss_01_0196:

Managing Audit Reports
======================

By default, database audit complies with a full audit rule, which is used to audit all databases that are successfully connected to the database audit instance. After connecting the database to the database audit instance, view report templates and report results.

Prerequisites
-------------

-  Database audit has been enabled.
-  Audit reports have been generated.

Viewing a Report
----------------

#. Log in to the management console.
#. In the navigation tree on the left, choose **Reports**.
#. In the **Instance** drop-down list, select the instance whose report information you want to view.
#. Viewing reports

   .. note::

      -  Enter a report name in the upper right corner to search.
      -  A real-time report is automatically generated in PDF format.
      -  Locate the row that contains the report to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box. When a report is deleted, you need to manually generate a report if you want to view the report result.

Viewing a Report Template
-------------------------

#. Log in to the management console.
#. In the navigation tree on the left, choose **Reports**.
#. In the **Instance** drop-down list, select the instance whose report template you want to view.
#. Click the **Report Management** tab.
#. View the report template.

   .. note::

      -  Report types include **Compliance report**, **Overview report**, **Database report**, **Client report**, and **Database operation report**.
      -  You can enable or disable scheduled tasks, or set their frequency to daily, weekly, or monthly.
      -  To modify the scheduled task of a report template, click **Schedule Task** in the **Operation** column. Modify and save the settings, click **Generate Report**, and you can check the reports.
