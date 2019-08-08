========================
OpenStack Summit Counter
========================

**DEVELOPMENT HAS MOVED** to https://opendev.org/x/osc-summit-counter and the bug/feature tracker to https://storyboard.openstack.org/#!/project/1100


The ``summit count`` plugin for python-openstackclient helps the user
determine the number of summits they have attended since the beginning
of their interaction with OpenStack.

Installing
==========

::

  $ pip install openstack-summit-counter

Using
=====

::

  $ openstack summit count $first [$current]

For example, if your first summit was for the "Folsom" series and the
next summit is for "Rocky"::

  $ openstack summit count folsom rocky

  +---------+-------+
  | Field   | Value |
  +---------+-------+
  | Summits | 13    |
  +---------+-------+

Can also be used for counting PTGs. For example::

  $ openstack ptg count pike rocky

  +-------+-------+
  | Field | Value |
  +-------+-------+
  | PTGs  | 3     |
  +-------+-------+
