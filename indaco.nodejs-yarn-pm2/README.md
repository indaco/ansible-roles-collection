indaco.nodejs-yarn-pm2
=========

Install and configure NodeJS, NPM, YARN and PM2. It also create and setup a
PM2 startup script to ensure PM" is up and running at system boot.

Role Variables
--------------

[defaults]

- nodejs_version: 12.x
- pm2_version: latest

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.nodejs-yarn-pm2

License
-------

CC-BY-4.0
