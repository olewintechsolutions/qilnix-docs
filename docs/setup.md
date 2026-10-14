---
title: "setup"
---


yum supports upgrade suppression with the syntax exclude=openoffice*[10]
pacman with IgnorePkg= openoffice[11] (to suppress upgrading openoffice in both cases)
dpkg and dselect support partial suppression through the hold flag in package selections
APT extends the hold flag through a pinning mechanism,[12] and users can also blacklist a package[13]
aptitude uses hold and forbid flags:[14]
hold: prevents a package from being upgraded or changed during installs/upgrades
forbid: prevents a package from being installed or reinstalled
portage supports suppression through the package.mask configuration file