# ucs-demo-deployment
Ansible scripts to deploy a demo environment like demo.univention.de

Many parts are copy&paste from https://github.com/univention/schulangebot

## Prerequisites

### UCS

* an UCS instance in "appliance mode" (unjoined)
* the instance needs an IP via DHCP

### Ansible Host

If you're running Ubuntu 18.04 you need a newer ansible version:

    sudo apt install software-properties-common
    sudo apt-add-repository --yes --update ppa:ansible/ansible
    sudo apt install -y ansible ansible-lint sshpass

## steps done by the script

* join the instance
* upgrade to the latest UCS release
* install a license
* install a bunch of apps
* install the meta package which configures the demo

Beside the last step everything can be used also for an productive UCS environment.
