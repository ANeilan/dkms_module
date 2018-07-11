dkms-workstation
================

DKMS wrapper for VMware Workstation kernel dependencies. The module allows DKMS
to trigger Workstation kernel module build automatically during the reboot that
follows a kernel upgrade.

# Requirements
The wrapper requires DKMS (normally available through your distribution package
manager) and an installation of VMware Workstation.

# Installation
Clone the repository to (or copy its content to) /usr/src/vmware-modules-14.
Then, as root, declare and setup the module in DKMS using the following command:

```
# dkms install vmware-modules/14 -k $(uname -r)
```
