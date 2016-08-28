tpbat-utils-acpi
================

Some simple utility scripts and config files around tpacpi-bat.

battery-charge-levels
---------------------
Contains "normal" battery charge thresholds. This file should be placed in /etc/ folder and may be edited to change what "normal" means. By default it contains vaules that help to prelong li-ion battery life. 
See <http://www.thinkwiki.org/wiki/Maintenance#Battery_treatment> for details and values sane for other types of batteries.

battery-get-charge-levels
-------------------------
Prints current battery charge thresholds.

battery-set-normal-charge-levels
--------------------------------
Sets battery charge thresholds to the values from /etc/battery-charge-levels.

battery-force-charge
--------------------
Sets battery start charge threshold to a value just below the stop charge threshold from /etc/battery-charge-levels, forcing a charge.

battery-charge-full
-------------------
Resets battery charge thresholds to default values resulting in an uncoditional charge up to 100%.

tpbat.sudoers
-------------
If this file is placed in /etc/sudoers.d folder then tpacpi-bat and all the below scripts can be called by members of sudo group without a password.

