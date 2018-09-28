# Ansible Role: GCP Mailgun

Sets up Mailgun relay in Postfix to allow sending emails in GCP

## Example Playbook

```
- hosts: all

  vars:
    smtp_login: MAILGUN_SMTP_USERNAME
    smtp_password: MAILGUN_SMTP_PASSWORD

  tasks:
  - include_role:
      name: thinkingmachines.gcp-mailgun
```
