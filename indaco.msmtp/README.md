# indaco.msmtp

Ansible role to install and configure [msmtp](https://marlam.de/msmtp/) as a lightweight SMTP client on Debian/Ubuntu systems.

## Default Variables

The following variables should be customized:

- `msmtp_email_login`: SMTP account username/email
- `msmtp_email_password`: SMTP account password

## Optional Variables

- `msmtp_host`: SMTP server (default: `smtp.gmail.com`)
- `msmtp_port`: SMTP port (default: `587`)
- `msmtp_from`: From address (default: `{{ msmtp_email_login }}`)
- `msmtp_set_default_mta`: Install msmtp-mta to replace sendmail (default: `true`)
- `msmtp_aliases`: List of mail aliases (default: `default` and `root` mapped to login email)
- `msmtp_accounts`: List of additional SMTP accounts (default: `[]`)

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: indaco.msmtp
      vars:
        msmtp_email_login: "your_email@gmail.com"
        msmtp_email_password: "your_app_password"
```

### Multiple Accounts

```yaml
- hosts: all
  roles:
    - role: indaco.msmtp
      vars:
        msmtp_email_login: "your_email@gmail.com"
        msmtp_email_password: "your_app_password"
        msmtp_accounts:
          - name: work
            host: smtp.office365.com
            port: 587
            from: "work@example.com"
            user: "work@example.com"
            password: "work_password"
```

## License

CC-BY-4.0
