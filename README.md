OVPNAutoStart
=============

This repo is used for storing scripts and related files for making an OpenVPN client start on boot within a debian system.


#####There are two main files: 

* **Openvpn** - this is the bash script that actually does the startup, the script is mainly unmodified, all credit goes to the original author below.
* **Openvpn-startup** - this file specifies the config file(s) that are to be run with openVPN on startup.

#####Installation:
- Install OpenVPN, create your config file and place it in a location easily accessible.
- Download both these scripts mentioned above and place them in /etc/init.d
- make them executable with chmod +x
- run the following command to make them run at startup "update-rc.d openvpn defaults"
- reboot and test!

#####Original version by Robert Leslie
<rob@mars.org>, edited by iwj and cs
Modified for openvpn by Alberto Gonzalez Iniesta <agi@inittab.org>
Modified for restarting / starting / stopping single tunnels by Richard Mueller <mueller@teamix.net>
