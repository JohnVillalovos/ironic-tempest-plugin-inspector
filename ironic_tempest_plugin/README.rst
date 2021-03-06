=======================================
Tempest Integration of ironic-inspector
=======================================

This directory contains Tempest tests to cover the ironic-inspector project.

It uses tempest plugin to automatically load these tests into tempest. More
information about tempest plugin could be found here:
`Plugin <https://docs.openstack.org/tempest/latest/plugin.html>`_

The legacy method of running Tempest is to just treat the Tempest source code
as a python unittest:
`Run tests <https://docs.openstack.org/tempest/latest/overview.html#legacy-run-method>`_

There is also tox configuration for tempest, use following regex for running
introspection tests::

    $ tox -e all-plugin -- inspector_tempest_plugin
