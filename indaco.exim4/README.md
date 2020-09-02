indaco.exim4
=========

Install and configure Exim4 to be used as MTA with Gmail

Role Variables
--------------

[defaults]
- exim4_email_login: "<YOUR_EMAIL_ADDRESS>"
- exim4_email_password: "<YOUR_EMAIL_PASSWORD>"
- local_user_email: ""


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.exim4
           exim4_mailname: "{{ inventory_hostname }}"
           exim4_dc_other_hostnames: "{{ inventory_hostname }}"
           exim4_dc_postmaster: "{{ ansible_user }}"
           exim4_email_login: "{{ exim4_gmail_login }}"
           exim4_email_password: "{{ exim4_gmail_password }}"
           local_user_email: "{{ admin_email_address }}"

License
-------

CC-BY-4.0
