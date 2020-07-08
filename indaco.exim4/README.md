Role Name
=========

Install and configure Exim4 to be used as MTA with Gmail

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

[defaults]
- exim4_email_login: "<YOUR_EMAIL_ADDRESS>"
- exim4_email_password: "<YOUR_EMAIL_PASSWORD>"
- local_user_email: ""


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

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
