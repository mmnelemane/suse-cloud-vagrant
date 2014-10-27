# Vagrant resources for SUSE Cloud

This repository contains resources for rapid virtualized deployment of
[SUSE Cloud](https://www.suse.com/products/suse-cloud/) via
[Vagrant](http://www.vagrantup.com/).

## Contents

*   Resources for [automatically preparing and presenting demos](demos/)
    of functionality within SUSE Cloud - these essentially reduce the
    task of setup to a one-line command.
*   A [HOWTO guide](docs/HOWTO.md) documenting how to use Vagrant and
    the provided [`Vagrantfile`](vagrant/Vagrantfile) to deploy a SUSE
    Cloud environment of (by default) 4 VMs via a single `vagrant up`
    command.  Use this instead of one of the [demos](demos/) if you
    want more manual control over the setup of Crowbar barclamps and
    OpenStack.

Currently the
[Vagrant boxes and .iso images required](docs/prerequisites.md#vagrant-boxes)
are built on SUSE's Internal Build Service (a.k.a. IBS) which is
accessible only to SUSE employees.  (Employees please see
[this etherpad](https://etherpad.nue.suse.com/p/cloud-vagrant).)
However the goal is to make the Vagrant boxes available in the near
future via https://vagrantcloud.com/suse so that they will be
automatically downloaded on demand.  If you are external and would
like these files urgently, please
[contact us](https://forums.suse.com/forumdisplay.php?65-SUSE-Cloud)
and we can probably sort something out!

### Building the Vagrant boxes

See the [vagrant/building-boxes/](vagrant/building-boxes/) subdirectory.

## Support, bugs, development etc.

If you experience a bug or other issue, or want to check the list
of known issues and other ongoing development, please refer to the
[github issue tracker](https://github.com/SUSE-Cloud/suse-cloud-vagrant/issues/).

## History

The resources were originally built for
[an OpenStack HA workshop session given on 2014/05/15 at the OpenStack summit in Atlanta](http://openstacksummitmay2014atlanta.sched.org/event/d3db2188dfed4459f8fbd03f5b405b81#.U4C6NXWx1Qo).
Video, slides, and other material from that workshop are available
[here](https://github.com/aspiers/openstacksummit2014-atlanta).
