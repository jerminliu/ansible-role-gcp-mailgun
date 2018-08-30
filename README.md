# Ansible playbooks

Playbooks for common tasks

- [mailgun-postfix](mailgun-postfix.yml)

  ```
    ansible-playbook \
      -i $HOST, \
      -e "smtp_login=$SMTP_LOGIN" \
      -e "smtp_password=$SMTP_PASSWORD" \
      mailgun-postfix.yml
  ```
