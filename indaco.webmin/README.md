indaco.webmin
=========

Install and configure Webmin

Role Variables
--------------

[defaults]

- webmin_deb_file: "webmin_1.953_all.deb"
- webmin_port: "10000"


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.webmin

License
-------

CC-BY-4.0
