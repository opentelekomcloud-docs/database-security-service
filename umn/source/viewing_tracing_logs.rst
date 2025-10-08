:original_name: dbss_01_0144.html

.. _dbss_01_0144:

Viewing Tracing Logs
====================

After you enable CTS, the system starts recording operations on DBSS. Operation records for the last seven days can be viewed on the CTS console.

Viewing a DBSS Trace on the CTS Console
---------------------------------------

#. Log in to the management console.

#. In the navigation pane on the left, click |image1| and choose **Management & Governance** > **Cloud Trace Service**.

#. Choose **Trace List** in the navigation pane.

#. Click **Region** at the top of the **Trace List** page to set the corresponding conditions.

   The following four filters are available:

   -  **Trace Type**, **Trace Source**, **Resource Type**, and **Search By**

      -  Select the filter from the drop-down list. Set **Trace Source** to **DBSS**.
      -  When you select **Trace name** for **Search By**, you also need to select a specific trace name.
      -  When you select **Resource ID** for **Search By**, you also need to select or enter a specific resource ID.
      -  When you select **Resource name** for **Search By**, you also need to select or enter a specific resource name.

   -  **Operator**: Select a specific operator (a user other than tenant).
   -  **Trace Rating**: Available options include **All trace status**, **normal**, **warning**, and **incident**. You can only select one of them.
   -  In the upper right corner of the page, you can query traces in the last 1 hour, last 1 day, last 1 week, or within a customized period.

#. Click **Query**.

#. Click |image2| on the left of a trace to expand its details.


   .. figure:: /_static/images/en-us_image_0217009691.png
      :alt: **Figure 1** Expanding trace details

      **Figure 1** Expanding trace details

#. Click **View Trace** in the **Operation** column. On the displayed **View Trace** dialog box shown in :ref:`Figure 2 <dbss_01_0144__fig9310171012116>`, the trace structure details are displayed.

   .. _dbss_01_0144__fig9310171012116:

   .. figure:: /_static/images/en-us_image_0217011475.png
      :alt: **Figure 2** Viewing a trace

      **Figure 2** Viewing a trace

.. |image1| image:: /_static/images/en-us_image_0000001570429773.png
.. |image2| image:: /_static/images/en-us_image_0210925109.png
