=====================================================
Install |chef analytics_title|
=====================================================

.. include:: ../../includes_analytics/includes_analytics.rst

Prerequisites
=====================================================
The |chef analytics| server shares the :doc:`same prerequisites </install_server_pre>` as the |chef server|:

* An x86_64 compatible system architecture; |redhat enterprise linux| and |centos| may require updates prior to installation
* A resolvable hostname that is specified using a FQDN or an IP address
* A connection to |ntp| to prevent clock drift
* A local mail transfer agent that allows the |chef server| to send email notifications
* Using |cron| and the ``/etc/cron.d`` directory for periodic maintenance tasks
* Disabling the |apache qpid| daemon on |centos| and |redhat| systems
* A local user account under which services will run
* A local user account for |postgresql|
* A group account under which services will run

Hostnames
-----------------------------------------------------
.. include:: ../../includes_install/includes_install_analytics_hostname.rst

.. warning:: The |fqdn| for the |chef analytics| server should not exceed 64 characters when using |open ssl|. |open ssl| requires the ``CN`` in a certificate to be no longer than 64 characters. By default, |chef analytics| uses the |fqdn| of the server to determine the common name (``CN``). If the |fqdn| of the |chef analytics| server is longer than 64 characters, the ``chef-server-ctl reconfigure`` command will not fail, but an empty certificate file will be created. |nginx| will not start if a certificate file is empty.

Install the Server
=====================================================
The |chef analytics| add-on can be installed in a standalone configuration or combined with |chef server oec| on a single node.

Standalone
-----------------------------------------------------
.. include:: ../../includes_install/includes_install_analytics_standalone.rst

Combined
-----------------------------------------------------
.. include:: ../../includes_install/includes_install_analytics_combined.rst

