# Ansible Role: GCP Mailgun

Sets up Mailgun relay in Postfix to allow sending emails in GCP

## Install

1. Add as ansible-galaxy requirement:
    ```yaml
    # requirements.yaml
    - src: https://github.com/thinkingmachines/ansible-role-gcp-mailgun
    ```
2. Install
    ```yaml
    ansible-galaxy install -r requirements.yml
    ```

## Example Playbook

```yaml
- hosts: all
  become: yes
  become_user: root

  vars:
    smtp_login: MAILGUN_SMTP_USERNAME
    smtp_password: MAILGUN_SMTP_PASSWORD

  tasks:
  - include_role:
      name: ansible-role-gcp-mailgun
```
