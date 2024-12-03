# Ansible Project: Network Configuration and Monitoring Automation

## Project Description

This project is designed to automate network configuration and monitoring tasks using Ansible. It targets network devices such as Junos (Juniper), IOS (Cisco), and EOS (Arista), providing automated configuration for SNMP, NETCONF, and syslog settings. 
 

## ⚠️ NOTE  
This project was developed and tested in a **Red Hat environment**, and the configurations are optimized for Red Hat-based systems.


## 📦 Collections Integration
Installation and usage of Ansible collections via private Automation Hub repositories.


## Key Features
- **Automated SNMP Configuration**: Automatically configures SNMP settings across Cisco, Juniper, and Arista devices.
- **NETCONF Configuration**: Configures and enables NETCONF on Junos devices.
- **Syslog Configuration**: Automatically sets up syslog on Cisco devices for centralized logging.
- **Cross-Vendor Support**: Supports multiple network operating systems (Junos, IOS, EOS) for consistent network management.
- **Verification Playbooks**: Includes playbooks to verify the configuration on managed devices.

## 🌐 Network Device Automation
Configuration of SNMP and syslog for various network device groups:
- **Juniper** (NETCONF and SNMP)
- **Cisco** (SNMP)
- **Arista** (SNMP)

## 📂 Project Structure  

```
simplify-review/
├── ansible.cfg          # Configuration file for collections and repositories
├── collections/         # Directory for Ansible collections
│   └── requirements.yml # List of required collections
├── monitoring.yml       # Main playbook for configuring SNMP and syslog
├── resource_modules.yml # Playbook for listing supported resource modules
├── tasks/               # Task files for device-specific configurations
│   ├── juniper_netconf_enable.yml
│   ├── juniper_snmp.yml
│   ├── cisco_snmp.yml
│   └── arista_snmp.yml
└── syslog.yml           # Playbook for syslog configuration


