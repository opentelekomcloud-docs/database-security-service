:original_name: dbss_01_0213.html

.. _dbss_01_0213:

Managing Database Audit Instances
=================================

Prerequisites
-------------

-  Before restarting and disabling an instance, ensure that its **Status** is **Running**.

Viewing the Instance
--------------------

#. View the database audit instances information. For details about related parameters, see :ref:`Table 1 <dbss_01_0213__table1025994517211>`.


   .. figure:: /_static/images/en-us_image_0000001570553141.png
      :alt: **Figure 1** Viewing database audit instances

      **Figure 1** Viewing database audit instances

   .. note::

      -  You can click the name of an instance to view its overview.
      -  Select an instance status from the **All statuses** drop-down list in the upper right corner of the list, or enter a key word of an instance to search for it.

   .. _dbss_01_0213__table1025994517211:

   .. table:: **Table 1** Parameters

      +--------------------------------------+--------------------------------------------------------------------------------------------------+
      | Parameter                            | Description                                                                                      |
      +======================================+==================================================================================================+
      | Instance Name/ID                     | Name and ID of an instance. Instance ID is automatically generated.                              |
      +--------------------------------------+--------------------------------------------------------------------------------------------------+
      | Specifications                       | Edition of an instance                                                                           |
      +--------------------------------------+--------------------------------------------------------------------------------------------------+
      | Status                               | Running status of an instance. The options are as follows:                                       |
      |                                      |                                                                                                  |
      |                                      | -  **Running**                                                                                   |
      |                                      | -  **Creating**                                                                                  |
      |                                      | -  **Faulty**                                                                                    |
      |                                      | -  **Disabled**                                                                                  |
      |                                      | -  **Frozen**                                                                                    |
      |                                      | -  **Frozen for legal management**                                                               |
      |                                      | -  **Frozen due to abuse**                                                                       |
      |                                      | -  **Frozen due to lack of identity verification**                                               |
      |                                      | -  **Frozen for partnership**                                                                    |
      |                                      | -  **Creation failed**                                                                           |
      +--------------------------------------+--------------------------------------------------------------------------------------------------+
      | Associated Databases/Total Databases | Number of databases an instance has associated with and Number of databases an instance supports |
      +--------------------------------------+--------------------------------------------------------------------------------------------------+
      | Operation                            | Operations can be performed on the instance. The options are as follows:                         |
      |                                      |                                                                                                  |
      |                                      | -  Configure Rules                                                                               |
      |                                      | -  Enable                                                                                        |
      |                                      | -  Disable                                                                                       |
      |                                      | -  Restart                                                                                       |
      |                                      | -  View Details                                                                                  |
      |                                      | -  Delete                                                                                        |
      +--------------------------------------+--------------------------------------------------------------------------------------------------+

   .. note::

      You can perform the following operations on instances as required:

      -  Restart

         Locate the row that contains the desired instance, choose **More** > **Restart** in the **Operation** column, and click **OK** in the displayed dialog box.

      -  Enable

         Locate the row that contains the desired instance, choose **More** > **Enable** in the **Operation** column, and click **OK** in the displayed dialog box.

      -  Disable

         Locate the row that contains the desired instance, choose **More** > **Disable** in the **Operation** column, and click **OK** in the displayed dialog box. When an instance is disabled, the audit function is disabled for the databases on the instance.

      -  Delete

         Locate the row that contains the instance that failed to be created, choose **More** > **Delete** in the **Operation** column, and click **Delete** in the displayed dialog box. Deleted instances will not be displayed in the instance list.

      -  View Details

         Locate the row that contains the instance that failed to be created, choose **More** > **View Details** in the **Operation** column. In the dialog box that is displayed, view the instance creation failure details.
