:original_name: dbss_01_0142.html

.. _dbss_01_0142:

Auditable Operations
====================

Cloud Trace Service (CTS) records all cloud service operations on DBSS, including requests initiated from the management console or open APIs and responses to the requests, for tenants to query, audit, and trace.

:ref:`Table 1 <dbss_01_0142__table52008441163754>` lists DBSS operations recorded by CTS.

.. _dbss_01_0142__table52008441163754:

.. table:: **Table 1** DBSS operations that can be recorded by CTS

   ====================== ============= ==============
   Operation              Resource Type Trace Name
   ====================== ============= ==============
   Creating an instance   dbss          createInstance
   Deleting an instance   dbss          deleteInstance
   Starting an instance   dbss          startInstance
   Stopping an instance   dbss          stopInstance
   Restarting an instance dbss          rebootInstance
   ====================== ============= ==============
