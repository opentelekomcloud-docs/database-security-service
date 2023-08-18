:original_name: dbss_01_0362.html

.. _dbss_01_0362:

Adding an SQL Injection Rule
============================

You can add SQL injection rules to audit your databases.

Prerequisites
-------------

-  You have purchased a database audit instance and the **Status** is **Running**.
-  You have added a database and enabled database audit.
-  A database has been added.

Procedure
---------

#. Log in to the management console.

#. Click **Add Rule** and configure parameters.


   .. figure:: /_static/images/en-us_image_0000001622135884.png
      :alt: **Figure 1** Adding an SQL injection rule

      **Figure 1** Adding an SQL injection rule

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
      | Status                  | Enables or disables an SQL injection rule.                                             | |image3|                       |
      |                         |                                                                                        |                                |
      |                         | -  |image1|: enabled                                                                   |                                |
      |                         | -  |image2|: disabled                                                                  |                                |
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

#. Confirm the information and click **OK**.

.. |image1| image:: /_static/images/en-us_image_0000001671056613.png
.. |image2| image:: /_static/images/en-us_image_0000001671056725.png
.. |image3| image:: /_static/images/en-us_image_0000001622617012.png
