# mikrotik-tools

## check_mikrotik_bgp

check_mikrotik_bgp is a nagios check which allows you to detect if the
BGP session to a particular peer on your Mikrotik router is down.

## check_mikrotik_vrrp

check_mikrotik_vrrp checks if a configured VRRP interface is in a
particular state (master/backup).

## Requirements

The scripts require the Mtik.pm module from the following repository:
https://github.com/elcamlost/mikrotik-perl-api

To get the current version, do:

wget https://raw.githubusercontent.com/elcamlost/mikrotik-perl-api/master/Mtik.pm

To install, copy the script plus the Mtik.pm module to the nagios
plugins directory. E.g. on Debian systems:

    cp check_mikrotik_* Mtik.pm /usr/lib/nagios/plugins/
