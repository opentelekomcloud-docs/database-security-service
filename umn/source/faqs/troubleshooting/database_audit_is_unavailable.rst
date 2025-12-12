:original_name: dbss_01_0235.html

.. _dbss_01_0235:

Database Audit Is Unavailable
=============================

Symptom
-------

After the database traffic is triggered, you cannot find the audit information about an executed statement in the SQL statement list.

In this case, perform the following operations to troubleshoot the problem:

-  :ref:`Checking Database Information and Audit Function Settings <dbss_01_0235__section8232320142510>`
-  :ref:`Checking Audited Database Settings <dbss_01_0235__section1815818210314>`
-  :ref:`Checking Database Agent Status <dbss_01_0235__section439162819315>`
-  :ref:`Checking the Security Group Rules of the Database Audit Instance <dbss_01_0235__section20936182118324>`

.. _dbss_01_0235__section8232320142510:

Checking Database Information and Audit Function Settings
---------------------------------------------------------

#. Log in to the management console.

#. Check whether the database information is correct.

   -  If the database information is correct, go to :ref:`3 <dbss_01_0235__li941038153911>`.
   -  If the database information is incorrect, click **Delete** to delete the database, and then click **Add Database** to add the database again.

      -  If the fault is rectified, no further operation is required.
      -  If the problem persists, go to :ref:`3 <dbss_01_0235__li941038153911>`.

#. .. _dbss_01_0235__li941038153911:

   Check whether the database audit function is enabled.

   -  If **Audit Status** is **Enabled**, go to :ref:`Checking Audited Database Settings <dbss_01_0235__section1815818210314>`.
   -  If **Audit Status** is **Disabled**, click **Enable** to enable the database audit function.

      -  If the fault is rectified, no further operation is required.
      -  If the problem persists, go to :ref:`Checking Audited Database Settings <dbss_01_0235__section1815818210314>`.

.. _dbss_01_0235__section1815818210314:

Checking Audited Database Settings
----------------------------------

-  If **Status** is **Enabled**, go to :ref:`Checking Database Agent Status <dbss_01_0235__section439162819315>`.
-  If **Status** is **Disabled**, click **Enable** to enable the desired audit scope rule of the database.

   -  If the fault is rectified, no further operation is required.
   -  If the problem persists, go to :ref:`Checking Database Agent Status <dbss_01_0235__section439162819315>`.

.. _dbss_01_0235__section439162819315:

Checking Database Agent Status
------------------------------

#. Log in to the node where the agent is installed as user **root** by using a cross-platform remote access tool (for example, PuTTY) via SSH.

#. Run the following command to view the running status of the agent program:

   **ps** **-ef|grep** **audit_agent**

   -  If the following information is displayed, the agent is running properly. Go to :ref:`4 <dbss_01_0235__li321115454910>`.

      ::

         /opt/dbss_audit_agent/bin/audit_agent

   -  If no information is displayed, the agent does not run properly. Go to :ref:`3 <dbss_01_0235__li10382244413>`.

#. .. _dbss_01_0235__li10382244413:

   Run the following command to restart the agent:

   **service** **audit_agent** **restart**

   -  If the fault is rectified, no further operation is required.
   -  If the problem persists, go to :ref:`4 <dbss_01_0235__li321115454910>`.

#. .. _dbss_01_0235__li321115454910:

   Run the following command to check the communication status between the agent and database audit instance:

   **tailf** **/opt/dbss_audit_agent/log/audit_agent.log**

   -  If information similar to the following is displayed, the communication between the agent and database audit instance is normal. Go to :ref:`Verifying the Result <dbss_01_0235__section02572203259>`.


      .. figure:: /_static/images/en-us_image_0291724693.png
         :alt: **Figure 1** Normal communication

         **Figure 1** Normal communication

   -  If information similar to the following is displayed, the communication between the agent and database audit instance is abnormal. Go to :ref:`Checking the Security Group Rules of the Database Audit Instance <dbss_01_0235__section20936182118324>`.


      .. figure:: /_static/images/en-us_image_0291724694.png
         :alt: **Figure 2** Communication error

         **Figure 2** Communication error

.. _dbss_01_0235__section20936182118324:

Checking the Security Group Rules of the Database Audit Instance
----------------------------------------------------------------

#. Go to the **Database Security Service** page.

#. In the navigation tree on the left, choose **Database Audit** > **Databases**. The **Databases** page is displayed.

#. Select an instance where the database is located from the **Instance** drop-down list.

#. Record the IP address of the agent node.

   Click |image2| next to the database to view the information of its agent, and record **Installing Node IP Address**.

#. Add an inbound rule for the installing node.

   a. Click **OK**.

.. _dbss_01_0235__section02572203259:

Verifying the Result
--------------------

In your database, run an SQL statement on the node where the agent is installed, and then search for the statement in the SQL statement list.

-  If the SQL statement is found, the problem has been solved.
-  If the SQL statement is not found, the problem persists. Contact customer service.

.. |image1| image:: /_static/images/en-us_image_0000001074398929.png
.. |image2| image:: /_static/images/en-us_image_0000001072223296.png
