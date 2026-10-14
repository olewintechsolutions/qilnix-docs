---
title: "setup"
---

When a user is upgrading a package with package management software, it is customary for them to be presented with the actions to be executed (usually the list of packages to be upgraded, and possibly the old and new version numbers), and allow them to either accept the upgrade in bulk, or select individual packages for upgrading. Many package managers can be configured to never upgrade certain packages, or to upgrade them only when critical vulnerabilities or instabilities are found in the previous version, as defined by the packager of the software. This process is called upgrade suppression, or version pinning. For instance, to prevent upgrades to the OpenOffice program:

yum supports upgrade suppression with the syntax exclude=openoffice*[10]
pacman with IgnorePkg= openoffice[11] (to suppress upgrading openoffice in both cases)
dpkg and dselect support partial suppression through the hold flag in package selections
APT extends the hold flag through a pinning mechanism,[12] and users can also blacklist a package[13]
aptitude uses hold and forbid flags:[14]
hold: prevents a package from being upgraded or changed during installs/upgrades
forbid: prevents a package from being installed or reinstalled
portage supports suppression through the package.mask configuration file