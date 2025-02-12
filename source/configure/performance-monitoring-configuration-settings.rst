:orphan:
:nosearch:

Configure performance monitoring by going to **System Console > Environment > Performance Monitoring**, or by editing the ``config.json`` file as described in the following tables. Changes to configuration settings in this section require a server restart before taking effect.

Enable performance monitoring
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Available in legacy Enterprise Edition E20*

+-----------------------------------------------+---------------------------------------------------------------------+
| Enable or disable performance monitoring.     | - System Config path: **Environment > Performance Monitoring**      |
|                                               | - ``config.json setting``: ``".MetricsSettings.Enable": false",``   |
| - **true**: Performance monitoring data       | - Environment variable: ``MM_METRICSSETTINGS_ENABLE``               |
|   collection and profiling is enabled.        |                                                                     |
| - **false**: **(Default)** Mattermost         |                                                                     |
|   performance monitoring is disabled.         |                                                                     |
+-----------------------------------------------+---------------------------------------------------------------------+
| See the `performance monitoring </scale/performance-monitoring.html>`__ documentation                               |
| to learn more.                                                                                                      |
+-----------------------------------------------+---------------------------------------------------------------------+

Listen address for performance
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Available in legacy Enterprise Edition E20*

+---------------------------------------------------------------+-------------------------------------------------------------------------+
| The port the Mattermost server will listen on to expose       | - System Config path: **Environment > Performance Monitoring**          |
| performance metrics, when enabled.                            | - ``config.json setting``: ``".MetricsSettings.ListenAddress": 8067",`` |
|                                                               | - Environment variable: ``MM_METRICSSETTINGS_LISTENADDRESS``            |
| Numerical input. Default is **8067**.                         |                                                                         |
+---------------------------------------------------------------+-------------------------------------------------------------------------+
