:original_name: dbss_01_0200.html

.. _dbss_01_0200:

Management an Audit Scope
=========================

After adding an audit scope, you can view, enable, edit, disable, or delete the audit scope.

Prerequisites
-------------

-  The audit scope has been added.
-  Before enabling, editing, or deleting the audit scope, ensure that the status of audit scope is **Disabled**.
-  Before disabling the audit scope, ensure that the status of audit scope is **Enabled**.

Precautions
-----------

By default, database audit complies with a **full audit rule**, which is used to audit all databases that are connected to the database audit instance. This audit rule is enabled by default. You can disable it but cannot delete it.

Viewing the Audit Scope
-----------------------

#. Log in to the management console.

#. In the navigation tree on the left, choose **Audit Rules**.

#. In the **Instance** drop-down list, select an instance to view audit scope.

#. View the audit scope information. For details about related parameters, see :ref:`Table 1 <dbss_01_0200__table964761214306>`.


   .. figure:: /_static/images/en-us_image_0000001523190264.png
      :alt: **Figure 1** Viewing the audit scope

      **Figure 1** Viewing the audit scope

   .. note::

      Enter the key word of an audit scope to search.

   .. _dbss_01_0200__table964761214306:

   .. table:: **Table 1** Parameters

      +-----------------------------------+----------------------------------------------------------------+
      | Parameter                         | Description                                                    |
      +===================================+================================================================+
      | Name                              | Name of the audit scope                                        |
      +-----------------------------------+----------------------------------------------------------------+
      | Exception IP Address              | Whitelisted IP addresses within the audit scope                |
      +-----------------------------------+----------------------------------------------------------------+
      | Source IP Address                 | IP address or IP address range used for accessing the database |
      +-----------------------------------+----------------------------------------------------------------+
      | Source Port                       | Port number of the IP address to be audited                    |
      +-----------------------------------+----------------------------------------------------------------+
      | Database Name                     | Database in the audit scope                                    |
      +-----------------------------------+----------------------------------------------------------------+
      | Database Account                  | Database username                                              |
      +-----------------------------------+----------------------------------------------------------------+
      | Status                            | Status of the audit scope. The options are as follows:         |
      |                                   |                                                                |
      |                                   | -  **Enabled**                                                 |
      |                                   | -  **Disabled**                                                |
      +-----------------------------------+----------------------------------------------------------------+

   .. note::

      You can perform the following operations on audit scopes as required:

      -  Enable

         Locate the row that contains the audit scope to be enabled, and click **Enable** in the **Operation** column. Databases within the scope will be audited.

      -  Edit (supported in customized audit scopes only)

         Locate the row that contains the audit scope to be edited, click **Edit** in the **Operation** column, and modify the scope in the displayed dialog box.

      -  Disable

         Locate the row that contains the audit scope to be disabled, click **Disable** in the **Operation** column, and click **OK** in the displayed dialog box. When the audit scope is disabled, the audit scope rule will not be executed in the audit.

      -  Delete (supported in customized audit scopes only)

         Locate the row that contains the audit scope to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box. You need to add the audit scope again if it is deleted and you want to audit it.
