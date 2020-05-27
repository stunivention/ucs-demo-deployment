# ucs-demo-deployment
Ansible scripts to deploy a demo environment like demo.univention.de

Many parts are copy&paste from https://github.com/univention/schulangebot

## Prerequisites

* an UCS instance in "appliance mode" (unjoined)
* the instance needs an IP via DHCP

## steps done by the script

* join the instance
* upgrade to the latest UCS release
* install a license
* install a bunch of apps
* install the meta package which configures the demo

Beside the last step everything can be used also for an productive UCS environment.
