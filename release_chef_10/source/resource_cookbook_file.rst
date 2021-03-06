.. THIS PAGE DOCUMENTS chef-client version 10.latest

=====================================================
cookbook_file 
=====================================================

.. include:: ../../includes_resources_common/includes_resources_common_generic.rst

.. include:: ../../includes_resources/includes_resource_11-4_cookbook_file.rst

Syntax
=====================================================
.. include:: ../../includes_resources/includes_resource_cookbook_file_syntax.rst

Actions
=====================================================
.. include:: ../../includes_resources/includes_resource_11-4_cookbook_file_actions.rst

Attributes
=====================================================
.. include:: ../../includes_resources/includes_resource_11-4_cookbook_file_attributes.rst

Windows File Security
-----------------------------------------------------
.. include:: ../../includes_resources_common/includes_resources_common_windows_security.rst

**Access Control Lists (ACLs)**

.. include:: ../../includes_resources_common/includes_resources_common_windows_security_acl.rst

**Inheritance**

.. include:: ../../includes_resources_common/includes_resources_common_windows_security_inherits.rst

Providers
=====================================================
.. include:: ../../includes_resources_common/includes_resources_common_attributes_provider.rst

.. include:: ../../includes_resources/includes_resource_cookbook_file_providers.rst

File Specificity
=====================================================
.. include:: ../../includes_cookbooks/includes_cookbooks_file_distribution_file_specificity.rst

Examples
=====================================================
|generic resource statement|

**Transfer a file**

.. include:: ../../step_resource/step_resource_cookbook_file_transfer_a_file.rst

**Handle cookbook_file and yum_package resources in the same recipe**

.. include:: ../../step_resource/step_resource_yum_package_handle_cookbook_file_and_yum_package.rst

**Install repositories from a file, trigger a command, and force the internal cache to reload**

.. include:: ../../step_resource/step_resource_yum_package_install_yum_repo_from_file.rst

**Use a case statement**

.. include:: ../../step_resource/step_resource_cookbook_file_use_case_statement.rst
