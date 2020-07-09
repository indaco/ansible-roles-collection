indaco.oh-my-zsh
=========

A brief description of the role goes here.

Role Variables
--------------

[defaults]
- plugins: list of ZSH plugins to install

Dependencies
------------

It depends on `gantsign.oh-my-zsh` role available on ansible-galaxy

Example Playbook
----------------

    - hosts: servers
      vars:
        oh_my_zsh_plugins:
          - zsh-syntax-highlighting
          - zsh-autosuggestions
          - zsh-completions
      roles:
          - role: indaco.oh-my-zsh
            users:
              - username: '{{ ansible_user }}'
                oh_my_zsh:
                  theme: robbyrussell
                  plugins: "{{ oh_my_zsh_plugins }}"
            plugins: "{{ oh_my_zsh_plugins }}"

License
-------

CC-BY-4.0
