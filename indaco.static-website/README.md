indaco.static-website
=========

A brief description of the role goes here.

Role Variables
--------------

[defaults]

- website_name: example.com
- certbot_admin_email: admin@example
- site_root_folder: /data


Dependecies
-----------

- indaco.nginx
- indaco.firewall

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.static-website

License
-------

CC-BY-4.0
