Bash script for controlling ACPI charge behavior under Linux.

Run without params to see current state and usage:


```
$ battery

Detected battery BAT0 at /sys/class/power_supply/BAT0

Usage: [full|<max>|<min> <max>|discharge]

        full        Charge to max
        <max>       Do not charge above <max> percentage
        <min> <max> Start charging once below <min> percentage, but do not charge above <max> percentage
        discharge   Force discharging, even if AC is connected (DON'T FORGET TO TURN OFF! :) )

Current settings:

        charge_behaviour: [auto] inhibit-charge force-discharge
        start_threshold:  70
        end_threshold:    80

Current state:

        charge: 79%
        status: Not charging
```