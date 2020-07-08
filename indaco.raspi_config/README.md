indaco.raspi_config
=========

Configure the Raspberry Pi instead to execute the raspi-config command manually.

Role Variables
--------------

[defaults]

- system_hostname: raspberry
- system_locale:  en_US.UTF-8
- system_language: en_US.UTF-8
- system_timezone: Europe/Rome
- raspi_config_boot_cli: "B1"
- raspi_config_expanded_filesystem: True
- raspi_config_memory_split_gpu: 16
- raspi_config_enable_camera: 0


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.raspi_config

License
-------

CC-BY-4.0
