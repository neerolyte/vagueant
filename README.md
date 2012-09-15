Vagueant is vaguely like Vagrant for linux containers (lxc).
It automates lxc configuration.

It's currently only tested under Ubuntu.

To start using it, first install lxc:

    apt-get install lxc

To create your first vagueant config, run:

    vagueant init

To build a lxc from a vagueant.conf, run:

    vagueant up
