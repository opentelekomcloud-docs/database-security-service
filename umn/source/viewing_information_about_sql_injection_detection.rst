:original_name: dbss_01_0207.html

.. _dbss_01_0207:

Viewing Information About SQL Injection Detection
=================================================

This section describes how to view SQL injection detection information of a database audit instance.

Prerequisites
-------------

-  Database audit has been enabled.

Procedure
---------

#. Log in to the management console.

#. In the navigation tree on the left, choose **Audit Rules**.

#. In the **Instance** drop-down list, select the instance for which you want to view SQL injection detection. Click the **SQL Injection** tab.

#. View information about SQL injection detection. For details about related parameters, see :ref:`Table 1 <dbss_01_0207__table964761214306>`.


   .. figure:: /_static/images/en-us_image_0000001523031304.png
      :alt: **Figure 1** Viewing information about the SQL injection detection

      **Figure 1** Viewing information about the SQL injection detection

   .. note::

      -  Select a risk severity from the **All risk severities** drop-down list in the upper right corner of the list, or enter a key word of an SQL injection rule name to search.
      -  Click **Set Priority** in the **Operation** column of an SQL injection rule to change its priority.

   .. _dbss_01_0207__table964761214306:

   .. table:: **Table 1** Parameters

      +-----------------------------------+------------------------------------------------------------------------+
      | Parameter                         | Description                                                            |
      +===================================+========================================================================+
      | Name                              | Name of the SQL injection detection                                    |
      +-----------------------------------+------------------------------------------------------------------------+
      | Command Feature                   | Command features of the SQL injection detection                        |
      +-----------------------------------+------------------------------------------------------------------------+
      | Risk Severity                     | Risk level of the SQL injection detection. The options are as follows: |
      |                                   |                                                                        |
      |                                   | -  **High**                                                            |
      |                                   | -  **Moderate**                                                        |
      |                                   | -  **Low**                                                             |
      |                                   | -  **No risks**                                                        |
      +-----------------------------------+------------------------------------------------------------------------+
      | Status                            | Status of the SQL injection detection. The options are as follows:     |
      |                                   |                                                                        |
      |                                   | -  **Enabled**                                                         |
      |                                   | -  **Disabled**                                                        |
      +-----------------------------------+------------------------------------------------------------------------+
      | Operation                         | Operations on an SQL injection rule. The options are as follows:       |
      |                                   |                                                                        |
      |                                   | -  **Set Priority**                                                    |
      |                                   | -  **Disable**                                                         |
      |                                   | -  **Edit**                                                            |
      |                                   | -  **Delete**                                                          |
      +-----------------------------------+------------------------------------------------------------------------+
