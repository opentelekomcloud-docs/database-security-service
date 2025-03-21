:original_name: dbss_01_0267.html

.. _dbss_01_0267:

Managing Privacy Data Protection Rules
======================================

You can view, enable, edit, disable, or delete data masking rules.

Prerequisites
-------------

You have applied for a database audit instance and the **Status** is **Running**.

Viewing Privacy Data Protection Rules
-------------------------------------

#. Log in to the management console.

#. In the navigation tree, choose **Rules**.

#. In the **Instance** drop-down list, select an instance to view its privacy data protection rule.

#. View the rules. For details about related parameters, see :ref:`Table 1 <dbss_01_0267__table881122114911>`.

   .. note::

      -  **Store Result Set**

         You are advised to disable |image1|. After this function is disabled, database audit will not store the result sets of user SQL statements.

         Do not enable this function if you want to prepare for PCI DSS/PCI 3DS CSS certification.

         **Note**: The result set storage supports only the database audit in agent mode.

      -  **Mask Privacy Data**

         You are advised to enable |image2|. After this function is enabled, you can configure masking rules to prevent privacy data leakage.

   .. _dbss_01_0267__table881122114911:

   .. table:: **Table 1** Masking rule parameters

      +-----------------------------------+--------------------------------------------------------------------------+
      | Parameter                         | Description                                                              |
      +===================================+==========================================================================+
      | Rule Name                         | Rule name                                                                |
      +-----------------------------------+--------------------------------------------------------------------------+
      | Rule Type                         | Rule type.                                                               |
      |                                   |                                                                          |
      |                                   | -  Default                                                               |
      |                                   | -  User-defined                                                          |
      +-----------------------------------+--------------------------------------------------------------------------+
      | Regular Expression                | Regular expression that specifies the sensitive data pattern             |
      +-----------------------------------+--------------------------------------------------------------------------+
      | Substitution Value                | Value used to replace sensitive data specified by the regular expression |
      +-----------------------------------+--------------------------------------------------------------------------+
      | Status                            | Status of a rule. Its value can be:                                      |
      |                                   |                                                                          |
      |                                   | -  **Enabled**                                                           |
      |                                   | -  **Disabled**                                                          |
      +-----------------------------------+--------------------------------------------------------------------------+

   .. note::

      You can perform the following operations on a rule:

      -  Disable

         Locate the row that contains the rule to be disabled and click **Disable** in the **Operation** column. A disabled rule cannot be used.

      -  Edit

         Locate the row that contains the rule to be modified, click **Edit** in the **Operation** column, and modify the rule in the displayed dialog box.

      -  Delete

         Locate the row that contains the rule to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box.

.. |image1| image:: /_static/images/en-us_image_0000001193982039.png
.. |image2| image:: /_static/images/en-us_image_0000001530562784.png
