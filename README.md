
Ozone Widget Cartridge on OpenShift
===================

This git repository contains the source for the owf-widget-cartridge RPM package.

Dependencies:

Provides:
 - Ozone Widget template

Building the RPM package
------------------------
Prerequisites

* RHEL or Fedora with the "Development Tools" group installed.  For RHEL, the tito package is available via the [EPEL](https://fedoraproject.org/wiki/EPEL) repository.

* The Tito rpm build tools

> yum install tito

* Git (if not already installed)

> yum install git

* Clone & build the repo

> git clone https://github.com/Shadow-Soft/owf-widget-cartridge.git

> cd owf-widget-cartridge

> rm -fr rel-eng

> tito init (first build after cloning only)

> tito tag (for first build after cloning, only needed when you want to create a new tag...e.g. 'release')

> tito build --rpm --test

Tito will generate the rpm package in /tmp/tito/noarch/owf-cartridge{*}.rpm

