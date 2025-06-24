:original_name: dbss_01_0356.html

.. _dbss_01_0356:

Step 2: Enable Database Audit
=============================

By default, database audit complies with a **full audit rule**, which is used to audit all databases that are connected to the database audit instance. You can enable audit and check audit results. For details, see :ref:`Viewing the Audit Dashboard <dbss_01_0204>`.

Enabling Database Audit
-----------------------

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Databases**.

#. Select a database audit instance from the **Instance** drop-down list.

#. In the **Operation** column of the database you want to audit, click **Enable**.

   The **Audit Status** of the database is **Enabled**. You do not need to restart the database.


   .. figure:: /_static/images/en-us_image_0000001347194069.png
      :alt: **Figure 1** Enabling database audit

      **Figure 1** Enabling database audit

Verifying Audit Results
-----------------------

#. Run an SQL statement (for example, **show databases**) in the target database.
#. Log in to the management console.
#. Select a region, click |image2|, and choose **Security** > **Database Security Service**. The database audit service page is displayed.
#. In the left navigation pane, choose **Dashboard**.
#. In the navigation tree on the left, choose **Data Reports**. The **Data Reports** page is displayed.
#. In the **Instance** drop-down list, select the instance that audits the target database.
#. Click the **Statements** tab.
#. Set the start and end time, and click **Submit**.

.. |image1| image:: /_static/images/en-us_image_0000001090901115.png
.. |image2| image:: /_static/images/en-us_image_0000001385655312.png
