:original_name: dbss_01_0192.html

.. _dbss_01_0192:

Adding Risky Operations
=======================

After enabling database audit, add and configure risky operations for audit.

.. important::

   One piece of audited data can match only one risky operation rule.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.
-  Database audit has been enabled.

Procedure
---------

#. Log in to the management console.

#. In the navigation tree on the left, choose **Audit Rules**.

#. In the **Instance** drop-down list, select an instance to add risky operations. Click the **Risky Operations** tab. Click **Add** above the risky operation list.

#. On the **Add Risky Operation** page, set the basic information and client IP address. For details about related parameters, see :ref:`Table 1 <dbss_01_0192__table4295843716304>`.


   .. figure:: /_static/images/en-us_image_0000001531047000.png
      :alt: **Figure 1** Setting the basic information and client IP address

      **Figure 1** Setting the basic information and client IP address

   .. _dbss_01_0192__table4295843716304:

   .. table:: **Table 1** Parameters

      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter                                          | Description                                                                                                                                 | Example Value         |
      +====================================================+=============================================================================================================================================+=======================+
      | Name                                               | Custom name of a risky operation                                                                                                            | test                  |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Risk Severity                                      | Severity of a risky operation. The options are as follows:                                                                                  | High                  |
      |                                                    |                                                                                                                                             |                       |
      |                                                    | -  **High**                                                                                                                                 |                       |
      |                                                    | -  **Moderate**                                                                                                                             |                       |
      |                                                    | -  **Low**                                                                                                                                  |                       |
      |                                                    | -  **No risks**                                                                                                                             |                       |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Status                                             | Status of a risky operation                                                                                                                 | |image3|              |
      |                                                    |                                                                                                                                             |                       |
      |                                                    | -  |image1|: enabled                                                                                                                        |                       |
      |                                                    | -  |image2|: disabled                                                                                                                       |                       |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Select Database                                    | Database that the risky operation will be applied to                                                                                        | ``-``                 |
      |                                                    |                                                                                                                                             |                       |
      |                                                    | You can select **ALL** or a specific database.                                                                                              |                       |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Exception Client IP Address or IP Range (Optional) | IP addresses that do not need to be audited.                                                                                                | 192.168.0.0           |
      |                                                    |                                                                                                                                             |                       |
      |                                                    | The IP address can be an IPv4 address (for example, 192.168.1.1) or an IPv6 address (for example, fe80:0000:0000:0000:0000:0000:0000:0000). |                       |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Client IP Address/IP Address Segment (Optional)    | IP address or IP address range of the client                                                                                                | 192.168.0.0           |
      |                                                    |                                                                                                                                             |                       |
      |                                                    | The IP address can be an IPv4 address (for example, 192.168.1.1) or an IPv6 address (for example, fe80:0000:0000:0000:0000:0000:0000:0000). |                       |
      +----------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Set the operation type, operation object, and execution result. For details about related parameters, see :ref:`Table 2 <dbss_01_0192__table1588718356449>`.

   .. _dbss_01_0192__table1588718356449:

   .. table:: **Table 2** Parameters

      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                                      | Example Value         |
      +=======================+==================================================================================================================================================+=======================+
      | Operations            | Type of a risky operation, including **Login** and **Operation**                                                                                 | Operation             |
      |                       |                                                                                                                                                  |                       |
      |                       | When you select the **Operation** check box, you can select **All operations** or the operations in **DDL**, **DML**, and **DCL**.               |                       |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Objects               | Enter the target database, target table, and field information after clicking **Add Operation Object**. Click **OK** to add an operation object. | ``-``                 |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Results               | Set **Affected Rows** and **Operation Duration**. The operation conditions are as follows:                                                       | ``-``                 |
      |                       |                                                                                                                                                  |                       |
      |                       | -  **Greater than**                                                                                                                              |                       |
      |                       | -  **Less than**                                                                                                                                 |                       |
      |                       | -  **Equal To**                                                                                                                                  |                       |
      |                       | -  **Equal to or greater than**                                                                                                                  |                       |
      |                       | -  **Less than or equal to**                                                                                                                     |                       |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **OK**.

.. |image1| image:: /_static/images/en-us_image_0000001562224796.png
.. |image2| image:: /_static/images/en-us_image_0000001561906096.png
.. |image3| image:: /_static/images/en-us_image_0000001562385088.png
