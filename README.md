# zabbix-agent-box

| License | Versioning | Build |
| ------- | ---------- | ----- |
| [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) | [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release) | [![Build status](https://ci.appveyor.com/api/projects/status/400mqb6pns4rveb8/branch/master?svg=true)](https://ci.appveyor.com/project/nikAizuddin/zabbix-agent-box/branch/master) |

Developer box for [Zabbix](https://github.com/zabbix/zabbix) agent.


## Getting Started

Clone this repository and `cd`:
```
$ git clone --recursive https://github.com/extra2000/zabbix-agent-box.git
$ cd zabbix-agent-box
```


## Creating Vagrant Box

Copy example pillar file for Zabbix agent. Optionally you may want to edit the values in the pillar file:
```
$ cp -v salt/roots/pillar/zabbix_agent.sls.example salt/roots/pillar/zabbix_agent.sls
```

Copy vagrant file from `vagrant/examples/` and then create the vagrant box (you can change to `--provider=libvirt` if you want to use Libvirt provider):
```
$ cp -v vagrant/examples/Vagrantfile.zabbix-agent-box.fedora-33.x86_64.example vagrant/Vagrantfile.zabbix-agent-box
$ vagrant up --provider=virtualbox
```

Provision the vagrant box:
```
$ vagrant ssh zabbix-agent-box -- sudo salt-call state.highstate
```

Deploy Zabbix Server, Web, Agent, and Postgres containers:
```
$ vagrant ssh zabbix-agent-box -- sudo salt-call state.sls zabbix_agent
```
