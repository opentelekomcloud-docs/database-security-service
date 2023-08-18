:original_name: dbss_01_0226.html

.. _dbss_01_0226:

How Do I Back Up the Database Audit Logs?
=========================================

Database audit supports manual backup and automatic backup. Audit logs are backed up to OBS. Buckets will be automatically created and will incur a separate bill.

Perform the following operations to automatically back up audit logs.

Automatically Backing Up Database Audit Logs
--------------------------------------------

#. Log in to the management console.

#. In the navigation tree on the left, choose **Settings**.

#. In the **Instance** drop-down list, select the required instance and click the **Backup and Restoration** tab.

#. Click **Configure**. In the displayed dialog box, set the parameters, as shown in :ref:`Figure 1 <dbss_01_0226__en-us_topic_0145057228_fig559320113012>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0226__en-us_topic_0145057228_table18602206309>`.

   .. _dbss_01_0226__en-us_topic_0145057228_fig559320113012:

   .. figure:: /_static/images/en-us_image_0000001294284718.png
      :alt: **Figure 1** Configure Automatic Backup dialog box

      **Figure 1** Configure Automatic Backup dialog box

   .. _dbss_01_0226__en-us_topic_0145057228_table18602206309:

   .. table:: **Table 1** Parameters

      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                          | Example Value         |
      +=======================+======================================================================================================================+=======================+
      | Automatic Backup      | Status of automatic backup                                                                                           | |image3|              |
      |                       |                                                                                                                      |                       |
      |                       | -  |image1|: enabled                                                                                                 |                       |
      |                       | -  |image2|: disabled                                                                                                |                       |
      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Backup Period         | Automatic backup period. Its options are as follows:                                                                 | Daily                 |
      |                       |                                                                                                                      |                       |
      |                       | -  **Daily**                                                                                                         |                       |
      |                       | -  **Hourly**                                                                                                        |                       |
      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Started               | Start time of the backup. Click |image4| to configure.                                                               | 2020/01/14 20:27:08   |
      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Bucket Name           | Name of the OBS bucket used for backup. Its options are as follows:                                                  | 20f18-7a5a-4042       |
      |                       |                                                                                                                      |                       |
      |                       | -  Create Default Bucket                                                                                             |                       |
      |                       | -  Select Bucket                                                                                                     |                       |
      |                       |                                                                                                                      |                       |
      |                       | .. note::                                                                                                            |                       |
      |                       |                                                                                                                      |                       |
      |                       |    -  If you click **Create Default Bucket**, you will be prompted to authorize OBS for exporting audit log backups. |                       |
      |                       |    -  Audit logs can be exported only to the bucket created by DBSS.                                                 |                       |
      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Export Directory      | Directory for storing backup files in the OBS bucket.                                                                | test                  |
      +-----------------------+----------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **OK**.

   .. note::

      After the automatic backup function is configured, new data in the database will be backed up one hour later. Then you can view the backup information.

.. |image1| image:: /_static/images/en-us_image_0000001581367781.png
.. |image2| image:: /_static/images/en-us_image_0000001530888000.png
.. |image3| image:: /_static/images/en-us_image_0000001530889940.png
.. |image4| image:: /_static/images/en-us_image_0000001147868462.png
