# ansible
Library of Ansible Playbooks and roles for Cloudian

Status: `work in progress`

## Install Ansible

> Install on a random machine, workstation, VM or inside Container.

- `easy_install pip`
- `pip install ansible`

## Usage

To run any of the playbooks:

- Until there's a dynamic inventory adjust IP addresses in `inventory/topology`
- Set S3 endpoint in `group_vars/s3_admin.yml`
- customize playbook to your needs (eg. edit Users and Groups)
- eg. run `ansible-playbook provision-groups.yml` to provision defined Groups
- run `ansible-playbook provision-users.yml` to create some Users etc.
