# rpi4_with_wifi

# Running rpi4 with systemd
1. Add DISTRO_FEATURES_append "systemd" to the local.conf
Exmaple 
```
DISTRO_FEATURES_append = " bluez5 bluetooth wifi systemd" # in local.conf
VIRTUAL-RUNTIME_init_manager = "systemd"

bitbake rpi-basic-image

# Connecting wifi

```
connmanctl enable wifi
connmanctl scan wifi
conmanctl services
```
