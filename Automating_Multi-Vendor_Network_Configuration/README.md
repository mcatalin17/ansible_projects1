# Ansible Project: Network Configuration and Monitoring Automation

## Project Description

This project is designed to automate network configuration and monitoring tasks using Ansible. It targets network devices such as Junos (Juniper), IOS (Cisco), and EOS (Arista), providing automated configuration for SNMP, NETCONF, and syslog settings. The goal is to enhance network management by automating tedious configuration tasks, ensuring consistency across the devices, and simplifying monitoring setup.

The project includes various playbooks and roles for automating tasks like enabling NETCONF on Junos devices, configuring SNMP on Cisco and Arista devices, and setting up syslog for logging purposes. 

## Key Features
- **Automated SNMP Configuration**: Automatically configures SNMP settings across Cisco, Juniper, and Arista devices.
- **NETCONF Configuration**: Configures and enables NETCONF on Junos devices.
- **Syslog Configuration**: Automatically sets up syslog on Cisco devices for centralized logging.
- **Cross-Vendor Support**: Supports multiple network operating systems (Junos, IOS, EOS) for consistent network management.
- **Verification Playbooks**: Includes playbooks to verify the configuration on managed devices.

## Technologies Used

- **Ansible**: Used for automating configuration management and provisioning of network devices.
- **Junos (Juniper)**: Configurations for enabling NETCONF and SNMP.
- **IOS (Cisco)**: SNMP and syslog configuration.
- **EOS (Arista)**: SNMP configuration.

## Project Structure

The project is organized into the following components:

- **Playbooks**:
  - `monitoring.yml`: Main playbook to configure monitoring settings (NETCONF and SNMP).
  - `verify_monitoring.yml`: Verifies the success of the configuration changes.
- **Roles**:
  - `network.base`: Contains roles for configuring network devices.
- **Tasks**:
  - Tasks for each device type (Junos, Cisco, Arista) to configure SNMP, NETCONF, and syslog settings.
  
## Installation

1. **Clone the repository**:

```bash
git clone https://github.com/yourusername/ansible-network-config.git
cd ansible-network-config
