# ansible
Library of Ansible Playbooks and roles for Cloudian

Status: `work in progress`

## Install Ansible

- `easy_install pip`
- `pip install ansible`

## Usage

To run any of the playbooks:

- Until there's a dynamic inventory adjust IP addresses in `inventory/topology`
- customize playbook to your needs (eg. set admin-API endpoint, users and groups)
- eg. run `ansible-playbook provision.yml`
