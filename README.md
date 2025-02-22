# Switch Port Configuration Automation

Ansible playbook for automating switch port configurations based on room numbers and wall points.

## Files:
- dynamic_interface_config.yml: Main playbook
- wall_point_mapping.yml: Maps wall points to switch interfaces
- switch_mapping.yml: Maps switches to rooms
- vlan_mapping.yml: VLAN configurations
- interface_descriptions.yml: Port descriptions

## Usage:
Run with AWX/Tower using the provided survey or manually with:
```ansible-playbook dynamic_interface_config.yml -e "room=ROOMNUMBER wall_point=NUMBER device_type=TYPE"```
