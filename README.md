# ubuntuscripts


# How to mount usb devices automatically like windows in ubuntu, and unmount it when device removed

1. add udev rules: [usb-slot-assign.rules](/etc/udev/rules.d/100-usb-slot-assign.rules} and [usb-cleanuup.rules](/etc/udev/rules.d/100-usb-slot-cleanup.rules}
2. add scripts to execute when usb mounts [usb-slot-assign](/usr/bin/usb-slot-assign} and [usb-slot-cleanup]{/usr/bin/usb-slot-cleanup)
3. add multipath.conf to resolve usb devices that emit multiple partitions and you need only one
