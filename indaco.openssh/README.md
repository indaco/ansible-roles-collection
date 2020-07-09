indaco.openssh
=========

Install and configure OpenSSH server.

Role Variables
--------------

[defaults]

- sshd_port: '22'
- sshd_log_level: 'INFO'
- sshd_login_grace_time: '120'
- sshd_permit_root_login: 'no'
- sshd_strict_modes: 'yes'
- sshd_max_auth_tries: '6'
- sshd_max_sessions: '10'
- sshd_pubkey_authentication: 'yes'
- sshd_authorized_keys_file: '%h/.ssh/authorized_keys'
- sshd_password_authentication: 'no'
- sshd_permit_empty_passwords: 'no'
- sshd_challenge_response_authentication: 'no'
- sshd_use_pam: 'no'
- sshd_allow_agent_forwarding: 'yes'
- sshd_x11_forwarding: 'yes'
- sshd_print_motd: 'yes'
- sshd_print_lastlog: 'yes'
- sshd_use_dns: 'no'
- sshd_accept_env: 'LANG LC_*'
- sshd_subsystem: 'sftp /usr/lib/openssh/sftp-server'
- pub_key_file: '<YOUR_PUBLIC_KEY_FILE_PATH_HERE>'

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: indaco.openssh

License
-------

CC-BY-4.0
