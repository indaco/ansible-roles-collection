indaco.fail2ban
=========

Install and configure Fail2Ban jails for SSH and more for Nginx like:

- nginx-noscript
- nginx-badbots
- nginx-nohome
- nginx-noproxy 


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.fail2ban

License
-------

CC-BY-4.0
