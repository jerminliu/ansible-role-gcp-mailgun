# Ansible playbooks

Playbooks for common tasks

- [mailgun-postfix](mailgun-postfix.yml) - Sets up Mailgun relay in Postfix to allow sending emails in GCP

  ```
    ansible-playbook \
      -i $HOST, \
      -e "smtp_login=$SMTP_LOGIN" \
      -e "smtp_password=$SMTP_PASSWORD" \
      mailgun-postfix.yml
  ```
