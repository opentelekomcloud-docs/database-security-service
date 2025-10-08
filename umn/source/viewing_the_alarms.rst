:original_name: dbss_01_0252.html

.. _dbss_01_0252:

Viewing the Alarms
==================

This section describes how to view and confirm alarms of database audit.

Prerequisites
-------------

-  You have applied for a database audit instance and the **Status** is **Running**.
-  Database audit has been enabled.
-  You have configured alarm notifications.

Procedure
---------

#. Log in to the management console.

#. Click the name of an instance, click the **Alarm Monitoring** tab.

#. View the alarm information, as shown in :ref:`Figure 1 <dbss_01_0252__fig2691832172511>`. For details about related parameters, see :ref:`Table 1 <dbss_01_0252__table1025994517211>`.

   .. _dbss_01_0252__fig2691832172511:

   .. figure:: /_static/images/en-us_image_0000001522903594.png
      :alt: **Figure 1** Viewing the alarms

      **Figure 1** Viewing the alarms

   .. _dbss_01_0252__table1025994517211:

   .. table:: **Table 1** Parameters of alarms

      +-----------------------------------+--------------------------------------------------------+
      | Parameter                         | Description                                            |
      +===================================+========================================================+
      | Time                              | Time when an alarm occurred.                           |
      +-----------------------------------+--------------------------------------------------------+
      | Type                              | Alarm type. The options are as follows:                |
      |                                   |                                                        |
      |                                   | -  Audit traffic exceeds threshold                     |
      |                                   | -  CPU exceptions                                      |
      |                                   | -  Memory exceptions                                   |
      |                                   | -  Disk exceptions                                     |
      |                                   | -  Insufficient audit log storage                      |
      |                                   | -  Log backup to OBS failed                            |
      |                                   | -  Agent exceptions                                    |
      +-----------------------------------+--------------------------------------------------------+
      | Alarm Risk Severity               | Risk severity of an alarm. The options are as follows: |
      |                                   |                                                        |
      |                                   | -  **High**                                            |
      |                                   | -  **Moderate**                                        |
      |                                   | -  **Low**                                             |
      +-----------------------------------+--------------------------------------------------------+
      | Cleared                           | Time when an alarm is cleared                          |
      +-----------------------------------+--------------------------------------------------------+
      | Confirmed Or Not                  | Confirmation status of an alarm.                       |
      +-----------------------------------+--------------------------------------------------------+
      | Description                       | Description of an alarm                                |
      +-----------------------------------+--------------------------------------------------------+

Follow-Up Procedure
-------------------

.. note::

   You can select multiple alarms to be confirmed and click **Batch Confirm** to batch confirm alarms.
