indaco.python38openssl
=========

Install and configure both OpenSSL and Python3.8 with OpenSSL support from the sources

Role Variables
--------------

[defaults]

- openssl_version: 1.1.1g
- python_version: 3.8.3

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.python38openssl

License
-------

CC-BY-4.0
