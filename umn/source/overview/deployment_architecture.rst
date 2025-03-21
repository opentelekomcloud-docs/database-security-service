:original_name: dbss_01_0181.html

.. _dbss_01_0181:

Deployment Architecture
=======================

Database audit is deployed in out-of-path pattern. It can audit databases built on ECS, BMS and RDS on the management console.


.. figure:: /_static/images/en-us_image_0273147489.png
   :alt: **Figure 1** Database audit deployment architecture

   **Figure 1** Database audit deployment architecture

The agent deployment for database audit is as follows:

-  For databases built on ECS or BMS, agents must be deployed on the database side.
-  For relational databases, agents must be deployed on the application or proxy side.
