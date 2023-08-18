:original_name: dbss_01_0197.html

.. _dbss_01_0197:

Managing Backup Audit Logs
==========================

After backing up audit logs, you can view or delete backup audit logs.

Prerequisites
-------------

-  Database audit has been enabled.
-  You have backed up audit logs.

Viewing Backup Audit Logs
-------------------------

#. View the backup audit log information. For details about related parameters, see :ref:`Table 1 <dbss_01_0197__table964761214306>`.

   Click |image1| in the upper right corner of the list and select the start time and end time to view backup logs in a specified time range.

   .. _dbss_01_0197__table964761214306:

   .. table:: **Table 1** Parameters of audit logs

      ============ ===============================================
      Parameter    Description
      ============ ===============================================
      Log Name     Name of a log, which is automatically generated
      Backup Time  Time when a log is backed up
      File Size    Log file size
      Backup Mode  Log backup mode.
      Backup Scope Backup time window
      Task Status  Backup status of a log
      ============ ===============================================

   .. note::

      Locate the row that contains the log to be deleted, click **Delete** in the **Operation** column, and click **OK** in the displayed dialog box.

.. |image1| image:: /_static/images/en-us_image_0000001147869404.png
