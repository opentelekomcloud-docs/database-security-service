:original_name: dbss_01_0186.html

.. _dbss_01_0186:

Step 1: Add a Database
======================

Database audit supports databases built on ECS, BMS, and RDS on the console. After applying for a database audit instance, you need to add the database to be audited to the instance.

Prerequisites
-------------

You have applied for a database audit instance and the **Status** is **Running**.

Adding a Database
-----------------

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Databases**.

#. In the **Instance** drop-down list, select the instance whose database is to be added.

#. Click **Add Database**.

#. In the dialog box displayed, set the database information. In the dialog box displayed, set the database information, as shown in :ref:`Figure 1 <dbss_01_0186__fig425613335010>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0186__table17265155610212>`.

   .. _dbss_01_0186__fig425613335010:

   .. figure:: /_static/images/en-us_image_0000001347187761.png
      :alt: **Figure 1** Add Database dialog box

      **Figure 1** Add Database dialog box

   .. _dbss_01_0186__table17265155610212:

   .. table:: **Table 1** Parameters

      +-----------------------+-------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                 | Example               |
      +=======================+=============================================================+=======================+
      | Database Type         | Supported database type. You can select RDS.                | RDS database          |
      +-----------------------+-------------------------------------------------------------+-----------------------+
      | Database Type         | Supported database type. You can select GaussDB(for MySQL). | GaussDB(for MySQL)    |
      |                       |                                                             |                       |
      |                       | You do not need to install an agent on the database.        |                       |
      +-----------------------+-------------------------------------------------------------+-----------------------+

#. Click **OK**. Then a database in the **Disabled** state has been added to the database list. See :ref:`Figure 2 <dbss_01_0186__fig977312338295>`. You do not need to manually install an agent.

   .. _dbss_01_0186__fig977312338295:

   .. figure:: /_static/images/en-us_image_0000001293789358.png
      :alt: **Figure 2** Successfully adding a database

      **Figure 2** Successfully adding a database

   .. note::

      -  After adding the database, confirm that the database information is correct. If the database information is incorrect, locate the target database and click **Delete** in the **Operation** column, and add the database again.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
