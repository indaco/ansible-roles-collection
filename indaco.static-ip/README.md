indaco.static-ip
=========

Configure DHCP service to assign a static ip address

Role Variables
--------------

[defaults]

- iface: eth0
- ip_address: "{{ ansible_host }}"
- router_address: 192.168.1.1
- dns_address: 1.1.1.1

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.static-ip

License
-------

CC-BY-4.0
