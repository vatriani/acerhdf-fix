acerhdf-fix

activate acerhdf kernelmodule by systemd

- integrate Kernelpatch of the new acerhdf module 0.5.30b-linux3.8
- systemd integration for acerhdf
- helperscript to turn acerhdf on and of



how to install:
---

copying acerhdf bash script to /usr/bin
# cp acerhdf /usr/bin/

copying acerhdf.service to
# cp acerhdf.service /etc/systemd/system/

enable new service
# systemctl enable acerhdf.service



optional:
---
integrate new acerhdf version to kernel sources
# patch -Np1 -i acerhdf.patch



change-log:
---
v1	all things running



tested systems:
---
acer aspire one a110l