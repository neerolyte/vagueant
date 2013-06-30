Vagueant is vaguely like Vagrant for linux containers (lxc).
It automates lxc configuration.

These days you probably want to switch to https://github.com/fgrehm/vagrant-lxc though.

[![Build Status](https://travis-ci.org/neerolyte/vagueant.png?branch=master)](https://travis-ci.org/neerolyte/vagueant)

The way Vagueant is designed it's currently possible for a vagueant.conf to run arbitrary commands *on your parent host* system - I do not intend to fix this. I am building Vagueant as a stop gap to bridge the difference in the speed of lxc and usability of Vagrant, hopefully one day Vagrant itself will support lxc.

It's currently only tested under Ubuntu.

To start using it, first install lxc:

    apt-get install lxc

To create your first vagueant config, run:

    vagueant init

To build a lxc from a vagueant.conf, run:

    vagueant up

To connect to the lxc, you can use ssh:

    vagueant ssh [-c <command>]

or the console:

    vagueant console
