:original_name: dbss_01_0239.html

.. _dbss_01_0239:

Configuring Alarm Notifications
===============================

After configuring alarm notifications, you can receive DBSS alarms on database risks. If this function is not enabled, you have to log in to the management console to view alarms.

-  Alarm notifications may be mistakenly blocked. If you have enabled notifications but not received any, check whether they have been blocked as spasms.
-  The system collects alarm statistics every 5 minutes and sends alarm notifications (if any).
-  You can also enable report notifications to get notified when the reports you subscribed to are generated. For details, see :ref:`Viewing Audit Reports <dbss_01_0248>`.

Prerequisites
-------------

You have applied for a database audit instance and the **Status** is **Running**.

Procedure
---------

#. In the navigation tree on the left, choose **Settings**.

#. In the **Instance** drop-down list, select an instance to configure alarm notifications.

#. Click the **Alarm Notifications** tab.

#. Set alarm notifications. For details about related parameters, see :ref:`Table 1 <dbss_01_0239__table29461252153613>`.


   .. figure:: /_static/images/en-us_image_0000001173357101.png
      :alt: **Figure 1** Configuring alarm notifications

      **Figure 1** Configuring alarm notifications

   .. _dbss_01_0239__table29461252153613:

   .. table:: **Table 1** Alarm notification parameters

      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter                  | Description                                                                                                                                                | Example Value         |
      +============================+============================================================================================================================================================+=======================+
      | Message Notifications      | Enables or disables notifications.                                                                                                                         |                       |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Daily Alarm Notifications  | Total number of alarms allowed to be sent every day                                                                                                        | 30                    |
      |                            |                                                                                                                                                            |                       |
      |                            | .. important::                                                                                                                                             |                       |
      |                            |                                                                                                                                                            |                       |
      |                            |    NOTICE:                                                                                                                                                 |                       |
      |                            |                                                                                                                                                            |                       |
      |                            |    -  If the number of alarms exceeds this value on a day, no more notification will be sent on that day.                                                  |                       |
      |                            |    -  There is no fixed time point for sending alarm notifications. The system collects statistics every 5 minutes and sends alarm notifications (if any). |                       |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Alarm Risk Severity        | Risk severity of the risk log. The options are as follows:                                                                                                 | High                  |
      |                            |                                                                                                                                                            |                       |
      |                            | -  **High**                                                                                                                                                |                       |
      |                            | -  **Moderate**                                                                                                                                            |                       |
      |                            | -  **Low**                                                                                                                                                 |                       |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | CPU Alarm Threshold (%)    | CPU alarm threshold of an audit instance. When the threshold is exceeded, an alarm notification is generated.                                              | 80                    |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Memory Alarm Threshold (%) | Memory alarm threshold of an audit instance. When the threshold is exceeded, an alarm notification is generated.                                           | 80                    |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Disk Alarm Threshold (%)   | Disk alarm threshold of an audit instance. When the threshold is exceeded, an alarm notification is generated.                                             | 80                    |
      +----------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **Apply**.
