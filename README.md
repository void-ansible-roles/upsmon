upsmon
======


What is does this role do?
--------------------------

This role installs and configures upsmon to monitor a NUT server for a feed UPS.

Meta
----

Files Managed:
  * /etc/ups/upsmon.conf
  * /etc/iptables.d/upsmon.rules

Defaults Provided:
  * None

Variables Required:
  * monitor_UPS
    - ID: ID for the monitored UPS
    - host: host where the NUT server is running
    - power_factor: power_factor supplied by this UPS
    - mode: mode of operation for this UPS
  * nut_monitor_passwd: password for the nutnet

Optional Variables:
  * None

Files Required:
  * None

Optional Files:
  * None

Conflicting Roles:
  * None

Depends On:
  * network
