# Ansible Automation Platform & GitHub Actions

**A showcase of integrating [Ansible](https://www.ansible.com/) playbooks with GitHub Actions for automated workflows.**

[🌐 View the GitHub Pages site »](https://cdm227.github.io/AAP/)

---

## 🚀 Overview

This project demonstrates how you can use GitHub Actions to trigger and orchestrate Ansible playbooks for various automation tasks, such as deploying web servers or running tests locally.

You’ll find:
- Example Ansible playbooks for common automation scenarios
- Ready-to-use GitHub Actions workflows that interact with these playbooks
- Guidance for connecting your own infrastructure (with secrets/keys)

---

## 📂 Repository Structure

| Location                                     | Description                                         |
|-----------------------------------------------|-----------------------------------------------------|
| `playbooks/deploy_playbook.yml`               | Example playbook for local deployment               |
| `playbooks/deploy_web_server.yml`             | Example playbook for web server deployment          |
| `.github/workflows/test_playbook.yml`         | Workflow to test local playbook                     |
| `.github/workflows/deploy_playbook.yml`       | Workflow to deploy web server                       |
| `.github/workflows/int_ansible.yml`           | Workflow for integrating Ansible triggers           |
| `inventory/hosts.ini`                         | Inventory file for Ansible                          |

---

## ⚡ How to Use

1. **Configure Your Inventory**

   Place your inventory file here:
   ```
   inventory/hosts.ini
   ```

2. **Set Up Secrets**

   > **Note:** You must add valid secrets (e.g., SSH keys, API tokens) to your repository for the workflows to access your infrastructure.

3. **Triggering Workflows**

   - **Local Playbook Test:**  
     `.github/workflows/test_playbook.yml` — runs `playbooks/deploy_playbook.yml` on localhost.
   - **Web Server Deployment:**  
     `.github/workflows/deploy_playbook.yml` — runs `playbooks/deploy_web_server.yml` on your target web server(s).
   - **Manual Integration:**  
     `.github/workflows/int_ansible.yml` — customize this workflow to define when and how to trigger your playbooks.

---

## 🛠️ Features

- Example Ansible playbooks for different scenarios
- GitHub Actions workflows for CI/CD automation
- Documentation available on [GitHub Pages](https://cdm227.github.io/AAP/)
- Easy to extend for your own infrastructure

---

## ⚠️ Known Issues

- **Secrets Missing:**  
  The provided workflows require valid secrets and SSH keys.  
  _Current configuration uses dummy IPs and has no SSH connectivity._
- **Merge Request Errors:**  
  Errors are expected due to the use of dummy data.

---

## 📖 Documentation

For full documentation and usage examples, visit the [project website](https://cdm227.github.io/AAP/).

---

## 🤝 Contributing

Feel free to open issues or submit pull requests for improvements!

---

## License

MIT
