:original_name: dbss_01_0191.html

.. _dbss_01_0191:

Enabling or Disabling SQL Injection Detection
=============================================

SQL injection detection is enabled by default. You can disable or enable the detection rules.

.. important::

   One piece of audited data can match only one SQL injection detection rule.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.
-  You can enable SQL injection detection when the status is **Disabled**.
-  You can disable SQL injection detection when the status is **Enabled**.

Disabling SQL Injection Detection
---------------------------------

SQL injection detection is enabled by default. You can disable the detection rules as required. When an SQL injection detection rule is disabled, the audit rule does not take effect.

#. Log in to the management console.

#. Select a region, click |image1|, and choose **Security** > **Database Security Service**. The **Dashboard** page is displayed.

#. In the navigation tree, choose **Rules**.

#. In the **Instance** drop-down list, select the instance for which you want to disable SQL injection detection.

#. Click the **SQL Injection** tab.

   .. note::

      Only user-defined rules can be edited and deleted. Default rules can only be enabled and disabled.

#. Locate the SQL injection rule you want to disable, and click **Disable** in the **Operation** column.


   .. figure:: /_static/images/en-us_image_0000001127129398.png
      :alt: **Figure 1** Disabling an SQL injection detection rule

      **Figure 1** Disabling an SQL injection detection rule

   When the status of an SQL injection detection rule is **Disabled**, SQL injection detection is disabled successfully.

#. In the **Operation** column of a rule, click **Edit**. Configure parameters and click **OK**.


   .. figure:: /_static/images/en-us_image_0000001671055773.png
      :alt: **Figure 2** Editing an SQL injection rule

      **Figure 2** Editing an SQL injection rule

   .. table:: **Table 1** SQL injection rule parameters

      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Parameter               | Description                                                                            | Example Value                  |
      +=========================+========================================================================================+================================+
      | Name                    | Name of an SQL rule.                                                                   | Postal Code SQL injection Rule |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Risk Level              | Level of risks matching a SQL rule. Its value can be:                                  | **Moderate**                   |
      |                         |                                                                                        |                                |
      |                         | -  **High**                                                                            |                                |
      |                         | -  **Moderate**                                                                        |                                |
      |                         | -  **Low**                                                                             |                                |
      |                         | -  **No risk**                                                                         |                                |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Status                  | Enables or disables an SQL injection rule.                                             | |image4|                       |
      |                         |                                                                                        |                                |
      |                         | -  |image2|: enabled                                                                   |                                |
      |                         | -  |image3|: disabled                                                                  |                                |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Test Regular Expression | Regular expression that checks for content in certain pattern.                         | ^\\d{6}$                       |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Data                    | Content that matches the regular expression.                                           | 628307                         |
      |                         |                                                                                        |                                |
      |                         | Enter content and click **Test** to verify that the regular expression works properly. |                                |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+
      | Result                  | Test result. It can be:                                                                | Hit                            |
      |                         |                                                                                        |                                |
      |                         | -  Hit                                                                                 |                                |
      |                         | -  Miss                                                                                |                                |
      |                         |                                                                                        |                                |
      |                         |    .. note::                                                                           |                                |
      |                         |                                                                                        |                                |
      |                         |       If the test result is **Hit**, the regular expression is correct.                |                                |
      |                         |                                                                                        |                                |
      |                         |       If the test result is **Miss**, the regular expression is incorrect.             |                                |
      +-------------------------+----------------------------------------------------------------------------------------+--------------------------------+

#. In the **Operation** column, click **Delete**.

Follow-Up Procedure
-------------------

To restart an SQL injection detection rule, click **Enable** in the **Operation** column of the target rule.


.. figure:: /_static/images/en-us_image_0000001173169443.png
   :alt: **Figure 3** Enabling an SQL injection detection rule

   **Figure 3** Enabling an SQL injection detection rule

When the status of an SQL injection detection rule is **Enabled**, SQL injection detection is enabled successfully.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
.. |image2| image:: /_static/images/en-us_image_0000001671056613.png
.. |image3| image:: /_static/images/en-us_image_0000001671056725.png
.. |image4| image:: /_static/images/en-us_image_0000001622617012.png
