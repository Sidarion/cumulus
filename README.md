# Ansible Role: cumulus

Capable of generating configuration files for Cumulus Linux based switches.
This role aims to generate config files based on variables pulled from netbox 
and parsed to the right format with the ansible templating engine. Configuration 
files are automatically pushed to the switches.

This allows for convenient management of Cumulus switches through the GUI of netbox.

## Requirements
- [Ranges](https://github.com/Sidarion/nand-push/tree/master/network-orchestrator/filter_plugins) 
  filter plugin from the [NAND-push](https://github.com/Sidarion/nand-push) repository.
  The interfaces template will not work without this.

## Strongly recommended (almost required)
**Since this role was writte for the [NAND-push](https://github.com/Sidarion/nand-push) software stack, 
standalone use might be limited and heavy editing of role files will be necessary.**

Please see the [NAND-push](https://github.com/Sidarion/nand-push) repository 
to get more information about the project and how to setup the framework.

## Capabilities
The following configurations are possible with this role:
- interfaces
- frr
- DHCP relays
- hosts file
- istallation of packages
- installation and setup of etckeeper
- misc parameters such as DNS, NTP, SNMP

Handlers are in place to restart services when necessary.

## License
GPL-3.0

## Author Information
This role was created by [Sidarion](https://github.com/Sidarion).
