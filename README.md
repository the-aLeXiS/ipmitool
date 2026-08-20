# ipmitool
This project contains the ipmitool executable for Windows and the corresponding dynamic libraries. 

* Code version: commit-4d4f29f
* Serial connection:
   * Configure serial output
    ```
    # Ubuntu 20.04
    # /etc/default/grub
    GRUB_CMDLINE_LINUX="console=tty1 console=ttyS0,115200
    GRUB_TERMINAL="console serial"
    GRUB_SERIAL_COMMAND="serial --speed=115200"
    ```
    * ipmitool -H [IP] -U [USER] -P [PASSWD] -I lanplus sol activate
