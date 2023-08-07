:original_name: dbss_01_0203.html

.. _dbss_01_0203:

Viewing the Instance Overview
=============================

This section describes how to view the instance overview, including the basic information, network settings and associated databases.

Prerequisites
-------------

You have applied for a database audit instance and the **Status** is **Running**.

Procedure
---------

#. View the basic information, network settings, and associated databases about the instance. See :ref:`Figure 1 <dbss_01_0203__fig1428710201627>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0203__table9339755215>`.

   .. _dbss_01_0203__fig1428710201627:

   .. figure:: /_static/images/en-us_image_0000001530573878.png
      :alt: **Figure 1** Viewing the instance overview

      **Figure 1** Viewing the instance overview

   .. _dbss_01_0203__table9339755215:

   .. table:: **Table 1** Parameters of the instance overview

      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      | Category              | Parameter             | Description                                                                                                                                  |
      +=======================+=======================+==============================================================================================================================================+
      | Basic Info            | Name                  | Instance name. You can click |image1| next to **Name** to change it.                                                                         |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Status                | Running status of an instance. The options are as follows:                                                                                   |
      |                       |                       |                                                                                                                                              |
      |                       |                       | -  **Running**                                                                                                                               |
      |                       |                       | -  **Creating**                                                                                                                              |
      |                       |                       | -  **Faulty**                                                                                                                                |
      |                       |                       | -  **Disabled**                                                                                                                              |
      |                       |                       | -  **Frozen**                                                                                                                                |
      |                       |                       | -  **Frozen for legal management**                                                                                                           |
      |                       |                       | -  **Frozen due to abuse**                                                                                                                   |
      |                       |                       | -  **Frozen due to lack of identity verification**                                                                                           |
      |                       |                       | -  **Frozen for partnership**                                                                                                                |
      |                       |                       | -  **Creation failed**                                                                                                                       |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | ID                    | Instance ID, which is automatically generated                                                                                                |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | AZ                    | Availability Zone (AZ) where an instance resides                                                                                             |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Version               | Version of the DBSS instance when you create the DBSS instance. The version of the DBSS instance created at different time may be different. |
      |                       |                       |                                                                                                                                              |
      |                       |                       | Impact scope of DBSS instance versions:                                                                                                      |
      |                       |                       |                                                                                                                                              |
      |                       |                       | -  Supported database types                                                                                                                  |
      |                       |                       | -  Supported database versions                                                                                                               |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Remarks               | Remarks about an instance. You can click |image2| next to **Remarks** to modify it.                                                          |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Edition               | Edition of an instance                                                                                                                       |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Created               | Time when an instance is created                                                                                                             |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      | Network Settings      | VPC                   | VPC where an instance resides                                                                                                                |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Security Group        | Security group where an instance resides                                                                                                     |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Subnet                | Subnet where an instance resides                                                                                                             |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      |                       | Private IP Address    | IP address of an instance                                                                                                                    |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+
      | Associated Database   | ``-``                 | Database information associated with an instance                                                                                             |
      |                       |                       |                                                                                                                                              |
      |                       |                       | Click **Manage Database**, and the **Databases** page is displayed.                                                                          |
      +-----------------------+-----------------------+----------------------------------------------------------------------------------------------------------------------------------------------+

.. |image1| image:: /_static/images/en-us_image_0000001435874465.png
.. |image2| image:: /_static/images/en-us_image_0000001385674488.png
