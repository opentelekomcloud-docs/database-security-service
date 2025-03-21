:original_name: dbss_01_0201.html

.. _dbss_01_0201:

Managing Risky Operations
=========================

After adding a risky operation, you can view the risk, enable, edit, disable, or delete the risky operation, or set its priority.

Prerequisites
-------------

-  The risky operation has been added.
-  Before enabling the risky operation, ensure that its status is **Disabled**.
-  Before disabling the risky operation, ensure that its status is **Enabled**.

Sets the Priority of the Risky Operation
----------------------------------------

#. Log in to the management console.
#. In the navigation tree, choose **Rules**.
#. In the **Instance** drop-down list, select an instance to set risky operation priority. Click the **Risky Operations** tab.
#. In the **Operation** column of the desired risky operation, click **Set Priority**.
#. In the displayed dialog box, select a priority and click **OK**.

Viewing the Risky Operation
---------------------------

#. Log in to the management console.

#. In the navigation tree, choose **Rules**.

#. In the **Instance** drop-down list, select an instance to view risky operations.

#. Click the **Risky Operations** tab.

#. View the risky operation information. For details about related parameters, see :ref:`Table 1 <dbss_01_0201__table964761214306>`.

   .. note::

      Select a risk severity from the **All risk severities** drop-down list in the upper right corner of the list, or enter a key word of a risky operation name to search.

   .. _dbss_01_0201__table964761214306:

   .. table:: **Table 1** Parameters

      +-----------------------------------+-------------------------------------------------------------------+
      | Parameter                         | Description                                                       |
      +===================================+===================================================================+
      | Name                              | Name of the risky operation                                       |
      +-----------------------------------+-------------------------------------------------------------------+
      | Category                          | Category of the risky operation                                   |
      +-----------------------------------+-------------------------------------------------------------------+
      | Feature                           | Feature of the risky operation                                    |
      +-----------------------------------+-------------------------------------------------------------------+
      | Risk Severity                     | Risk severity of the risky operation. The options are as follows: |
      |                                   |                                                                   |
      |                                   | -  **High**                                                       |
      |                                   | -  **Moderate**                                                   |
      |                                   | -  **Low**                                                        |
      |                                   | -  **No risks**                                                   |
      +-----------------------------------+-------------------------------------------------------------------+
      | Status                            | Status of the risky operation. The options are as follows:        |
      |                                   |                                                                   |
      |                                   | -  **Enabled**                                                    |
      |                                   | -  **Disabled**                                                   |
      +-----------------------------------+-------------------------------------------------------------------+

   .. note::

      You can perform the following operations on risky operations as required:

      -  Enable

         Locate the row that contains the risky operation to be enabled, and click **Enable** in the **Operation** column. The operation will be audited.

      -  Edit

         Locate the row that contains the risky operation to be edited, click **Edit** in the **Operation** column, and modify the operation in the displayed dialog box.

      -  Disable

         Locate the row that contains the risky operation to be disabled, click **Disable** in the **Operation** column, and click **OK** in the displayed dialog box. When a risky operation is disabled, the risky operation rule will not be executed in the audit.

      -  Delete

         Locate the row that contains the risky operation to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box. You need to add the risky operation again if a risky operation is deleted and you need to audit its rule.
