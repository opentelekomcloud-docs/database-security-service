:original_name: dbss_01_0185.html

.. _dbss_01_0185:

Applying for a Database Audit Instance
======================================

Before using the database audit function, you need to apply for a database audit instance.

Ensure the VPC of the database audit instance is the same as that of the node (application side or database side) where you plan to install the database audit agent. Otherwise, the instance will be unable to connect to the agent or perform audit.

Impact on the System
--------------------

Database audit works in out-of-path mode, which neither affects user services nor conflicts with the local audit tools.

Procedure
---------

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the upper right corner of the page, click **Apply for Database Audit**.

#. On the **Apply for Database Audit** page, select an **AZ** and a **Type**.

   -  **AZ**: If resources are sold out in an AZ, **Sold out in this AZ** will be displayed for the AZ. In this case, select another AZ.
   -  **Type**: For details about the supported editions, see :ref:`Editions <dbss_01_0268>`.

#. Set database audit parameters. See :ref:`Table 1 <dbss_01_0185__table4295843716304>`.

   .. _dbss_01_0185__table4295843716304:

   .. table:: **Table 1** Parameters

      +-----------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                                                                                       | Example Value         |
      +=======================+===================================================================================================================================================================================================+=======================+
      | VPC                   | You can select an existing VPC, or click **View VPC** to create one.                                                                                                                              | vpc-sec               |
      |                       |                                                                                                                                                                                                   |                       |
      |                       | .. note::                                                                                                                                                                                         |                       |
      |                       |                                                                                                                                                                                                   |                       |
      |                       |    -  Select the VPC of the node (application or database side) where you plan to install the agent.                                                                                              |                       |
      |                       |    -  To change the VPC of a DBSS instance, unsubscribe from it and apply for a new one.                                                                                                          |                       |
      |                       |                                                                                                                                                                                                   |                       |
      |                       | For more information about VPC, see *Virtual Private Cloud User Guide*.                                                                                                                           |                       |
      +-----------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Security Group        | The security group configured for the instance is displayed on the page. Once a security group is selected for an instance, the instance is protected by the access rules of this security group. | sg                    |
      |                       |                                                                                                                                                                                                   |                       |
      |                       | For more information about security groups, see *Virtual Private Cloud User Guide*.                                                                                                               |                       |
      +-----------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Subnet                | The **Subnet** drop-down list displays all available subnets.                                                                                                                                     | public_subnet         |
      |                       |                                                                                                                                                                                                   |                       |
      |                       | For more information about subnets, see *Virtual Private Cloud User Guide*.                                                                                                                       |                       |
      +-----------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Instance Name         | Custom name of the instance                                                                                                                                                                       | DBSS-test             |
      +-----------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Confirm the configuration and click **Next**.

#. On the details confirmation page, you can click .

   On the **Instances** page, you can view the created database audit instance.

   If the **Status** is **Running**, you have successfully applied for the database audit instance.

.. |image1| image:: /_static/images/en-us_image_0000001078852871.png
