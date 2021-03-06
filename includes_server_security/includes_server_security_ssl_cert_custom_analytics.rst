.. This is an included how-to. 


The |chef analytics| server can be configured to use |ssl| certificates by adding the following settings in the server configuration file:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Setting
     - Description
   * - ``ssl['certificate']``
     - |ssl_certificate|
   * - ``ssl['certificate_key']``
     - |ssl_certificate key|

and setting their values to define the path to the certificate and the path to the certificate key, similar to the following:

.. code-block:: ruby

   ssl['certificate']  = "/etc/pki/tls/certs/your-host.crt"
   ssl['certificate_key']  = "/etc/pki/tls/private/your-host.key"

Save the file, and then run the following command:

.. code-block:: bash

   $ sudo opscode-analytics-ctl reconfigure
