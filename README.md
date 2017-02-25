Installation canon LBP-2900 on linux (ubuntu 16.04):
1) install capt drivers
2) copy ccpd to /etc/init.d/
3) copy ccpd1.service to /etc/systemd/system/
4) copy 85-canon-capt.rules to /etc/udev/rules.d
5) disable ccpd (sudo systemctl disable ccpd)

6) update
     sudo udevadm control --reload-rules
     sudo systemctl daemon-reload

7) reboot

8) create printer rule

helper script for automatically create printer (https://github.com/raducotescu/CanonCAPTdriver)