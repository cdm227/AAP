# GitHub Actions Workflows

Example workflows for automating with Ansible:

## Test Playbook Workflow

- **File:** `.github/workflows/test_playbook.yml`
- **Runs:** `playbooks/deploy_playbook.yml` on localhost

## Deploy Playbook Workflow

- **File:** `.github/workflows/deploy_playbook.yml`
- **Runs:** `playbooks/deploy_web_server.yml` on target hosts

## Integration Workflow

- **File:** `.github/workflows/int_ansible.yml`
- **Customize:** Use this to define when/how to trigger your Ansible playbooks

---

**Note:**  
Workflows require valid GitHub secrets (SSH keys, etc.) and a properly configured inventory.

You can trigger workflows manually or via repository events (push, PR, etc.).
