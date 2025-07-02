# Playbook Examples

This project includes sample Ansible playbooks to help you automate:

## Localhost Playbook

- **File:** `playbooks/deploy_playbook.yml`
- **Workflow:** `.github/workflows/test_playbook.yml`
- **Purpose:** Run a simple deployment on localhost for testing purposes.

## Web Server Playbook

- **File:** `playbooks/deploy_web_server.yml`
- **Workflow:** `.github/workflows/deploy_playbook.yml`
- **Purpose:** Deploy and configure a web server on your target hosts.

## Inventory

Make sure to set up your hosts in `inventory/hosts.ini`:

```ini
[web]
192.0.2.1 ansible_user=youruser
```

Modify the playbooks or inventory as needed to match your infrastructure.
