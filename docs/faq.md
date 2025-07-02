# FAQ & Troubleshooting

## Why do my workflows fail with authentication or SSH errors?

- Check that you’ve set up required secrets (SSH keys, credentials) in your repo’s GitHub Actions secrets.
- Make sure your hosts in `inventory/hosts.ini` are reachable and correct.

## Why does the workflow fail on merge requests?

- This project uses dummy IPs and no real SSH keys for demonstration.
- Replace with your own host data and secrets for real deployments.

## Where should I put my inventory file?

- Place it in `inventory/hosts.ini` as referenced in the playbooks and README.

## Can I contribute?

- Absolutely! Open issues or pull requests on [GitHub](https://github.com/cdm227/AAP).

## What is the license?

- MIT. See the [LICENSE](LICENSE) file.
