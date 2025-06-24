:original_name: dbss_01_0266.html

.. _dbss_01_0266:

Configuring Privacy Data Protection Rules
=========================================

To mask sensitive information in entered SQL statements, you can enable the function of masking privacy data and configure masking rules to prevent sensitive information leakage.

Prerequisites
-------------

-  Database audit has been enabled.

Procedure
---------

#. Log in to the management console.

#. In the navigation tree on the left, choose **Audit Rules**.

#. In the **Instance** drop-down list, select the instance whose privacy data protection rule is to be configured.

#. Click the **Privacy Data Protection** tab.

   .. note::

      Only user-defined rules can be edited and deleted. Default rules can only be enabled and disabled.

#. Enable or disable **Store Result Set** and **Mask Privacy Data**.

   -  **Store Result Set**

      You are advised to disable |image1|. After this function is disabled, database audit will not store the result sets of user SQL statements.

      Do not enable this function if you want to prepare for PCI DSS/PCI 3DS CSS certification.

      **Note**: The result set storage supports only the database audit in agent mode.

   -  **Mask Privacy Data**

      You are advised to enable |image2|. After this function is enabled, you can configure masking rules to prevent privacy data leakage.

#. Click **Add Rule**. In the displayed **Add Rule** dialog box, set the data masking rule, as shown in :ref:`Figure 1 <dbss_01_0266__fig45721822818>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0266__table4295843716304>`.

   .. _dbss_01_0266__fig45721822818:

   .. figure:: /_static/images/en-us_image_0000001531043744.png
      :alt: **Figure 1** Add Rule dialog box

      **Figure 1** Add Rule dialog box

   .. _dbss_01_0266__table4295843716304:

   .. table:: **Table 1** Rule parameters

      +--------------------+--------------------------------------------------------------------------+---------------+
      | Parameter          | Description                                                              | Example Value |
      +====================+==========================================================================+===============+
      | Rule Name          | Name of a rule                                                           | test          |
      +--------------------+--------------------------------------------------------------------------+---------------+
      | Regular Expression | Regular expression that specifies the sensitive data pattern             | ``-``         |
      +--------------------+--------------------------------------------------------------------------+---------------+
      | Substitution Value | Value used to replace sensitive data specified by the regular expression | ###           |
      +--------------------+--------------------------------------------------------------------------+---------------+

#. Click **OK**.

   A masking rule in the **Enabled** status is added to the rule list.

Verifying a Rule
----------------

Perform the following steps to check whether a rule takes effect. The audit information about passport No. in a MySQL database is used as an example.

#. Enable **Mask Privacy Data**, and ensure the "Passport NO." masking rule is enabled, as shown in :ref:`Figure 2 <dbss_01_0266__fig10156628163415>`.

   .. _dbss_01_0266__fig10156628163415:

   .. figure:: /_static/images/en-us_image_0000001581444553.png
      :alt: **Figure 2** Enabled rule

      **Figure 2** Enabled rule

#. Log in to the database as user **root** through the MySQL database client.

#. On the database client, enter an SQL statement.

   **select** **\* from db where HOST=**"*Passport NO.*";

#. In the navigation pane, choose **Dashboard**.

#. In the navigation tree on the left, choose **Data Reports**. The **Data Reports** page is displayed.

#. Set filtering conditions to find the entered SQL statement.

#. In the row containing the SQL statement, click **Details** in the **Operation** column.

#. Check the SQL statement information in **SQL Statement**.

Common Operations
-----------------

After adding a user-defined masking rule, you can perform the following operations on it:

-  Disable

   Locate the row that contains the rule to be disabled and click **Disable** in the **Operation** column. A disabled rule cannot be used.

-  Edit

   Locate the row that contains the rule to be modified, click **Edit** in the **Operation** column, and modify the rule in the displayed dialog box.

-  Delete

   Locate the row that contains the rule to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box.

.. |image1| image:: /_static/images/en-us_image_0000001193982039.png
.. |image2| image:: /_static/images/en-us_image_0000001530562784.png
