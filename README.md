# ansible
Library of Ansible Playbooks and roles for Cloudian

Status: `work in progress`/`usable`

## Install Ansible

> Install on a random machine, workstation, VM or inside Container.

- `easy_install pip`
- `pip install ansible`

## Usage

To run any of the playbooks:

- Until there's a dynamic inventory adjust IP addresses in `inventory/topology`
- Customize playbook to your needs (eg. edit Users, Groups)
- Eg. run `ansible-playbook provision-groups.yml` to provision defined Groups
- Run `ansible-playbook provision-users.yml` to create some Users etc.
- Run `ansible-playbook provision-policy` to create a basic RF=3 Storage Policy
- Run `ansible-playbook provision-all` to apply all of the above

When creating users, the first users' S3 keys will be stored in a file `credentials` within `cwd`, ready to be used by AWS CLI.
