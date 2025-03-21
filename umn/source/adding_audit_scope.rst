:original_name: dbss_01_0190.html

.. _dbss_01_0190:

Adding Audit Scope
==================

By default, database audit complies with a full audit rule, which is used to audit all databases that are connected to the database audit instance. You can also add audit scope and specify the databases to be audited.

.. important::

   By default, the full audit rule takes effect even if other rules exist. To make another audit rule take effect, disable the full audit rule first.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.

-  Database audit has been enabled.

Procedure
---------

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree on the left, choose **Rules**.

#. In the **Instance** drop-down list, select an instance to add audit scope.

#. **Add Audit Scope** above the audit scope list.

   .. note::

      -  By default, database audit complies with a **full audit rule**, which is used to audit all databases that are connected to the database audit instance. This audit rule is enabled by default. You can disable it but cannot delete it.
      -  To make a custom rule take effect, disable the full audit rule first.

#. In the displayed dialog box, set the audit scope, as shown in :ref:`Figure 1 <dbss_01_0190__fig97457713117>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0190__table474657203117>`.

   .. _dbss_01_0190__fig97457713117:

   .. figure:: /_static/images/en-us_image_0000001173318613.png
      :alt: **Figure 1** Add Audit Scope dialog box

      **Figure 1** Add Audit Scope dialog box

   .. _dbss_01_0190__table474657203117:

   .. table:: **Table 1** Parameters

      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                        | Example Value         |
      +=======================+====================================================================================================================================+=======================+
      | Name                  | Name of the custom audit scope                                                                                                     | audit00               |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Database Name         | Database to be added to the audit scope                                                                                            | db03                  |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Operations            | Audited operation type. It can be **Login** or **Operation**.                                                                      | Login                 |
      |                       |                                                                                                                                    |                       |
      |                       | When you select the **Operation** check box, you can select **All operations** or the operations in **DDL**, **DML**, and **DCL**. |                       |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Database Account      | (Optional) Database username.                                                                                                      | ``-``                 |
      |                       |                                                                                                                                    |                       |
      |                       | You can specify multiple accounts, separated by commas (,).                                                                        |                       |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Exception IP Address  | (Optional) IP addresses that do not need to be audited.                                                                            | ``-``                 |
      |                       |                                                                                                                                    |                       |
      |                       | .. note::                                                                                                                          |                       |
      |                       |                                                                                                                                    |                       |
      |                       |    If an IP address is set as both a source and an exception IP address, the IP address will not be audited.                       |                       |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Source IP Address     | (Optional) IP address or IP address range used for accessing the database to be audited                                            | ``-``                 |
      |                       |                                                                                                                                    |                       |
      |                       | The IP address must be an internal IP address in IPv4 or IPv6 format.                                                              |                       |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Source Port           | (Optional) Port number used for accessing the database to be audited                                                               | ``-``                 |
      +-----------------------+------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **OK**.

   When the audit scope is added successfully, it is displayed in the audit scope list in the state of **Enabled**.

Related Operations
------------------

In addition to adding the audit scope, you can enable or disable SQL injection detection and add risky operations to set audit rules for database audit.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
