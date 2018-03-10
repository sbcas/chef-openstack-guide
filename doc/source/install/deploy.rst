.. _deploy:

===========================
Deploy OpenStack using Chef
===========================

Deploy OpenStack cookbooks with Chef and test the setup using Tempest and
`InSpec <https://www.inspec.io>`_.

* Software requirements:

  * Ubuntu 16.04 LTS or CentOS 7
  * `Chef Development Kit <https://downloads.chef.io/chefdk>`_ 2.3 or greater
  * `Vagrant <https://www.vagrantup.com>`_ 2.0 or greater
  * `VirtualBox <https://www.virtualbox.org>`_ 5.2 or greater

* Hardware requirements:

  * At least 4GB of memory for a basic control plane, more for more services.
    8GB minimum recommended for a standard out-of-the-box experience.
  * At least 10GB of storage.

.. code-block:: bash

  $ git clone git://git.openstack.org/openstack/openstack-chef-repo
  $ cd openstack-chef-repo
  $ kitchen list
  $ kitchen converge [all|centos|ubuntu]
  $ kitchen verify   [all|centos|ubuntu]
  $ kitchen destroy  [all|centos|ubuntu]


