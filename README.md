# ansible
Library of Ansible Playbooks and roles for Cloudian

Status: `work in progress`/`usable`

## Install Ansible

> Install on a random machine, workstation, VM or inside Container.

- `easy_install pip`
- `pip install ansible botocore boto3`

## Usage

To run any of the playbooks:

- Until there's a dynamic inventory adjust IP addresses in `inventory/topology`
- Edit `group_vars/cloudian.yml` to set S3 endpoint and perhaps adjust passwords
- Customize playbook to your needs (eg. edit Users, Groups etc.)
- Eg. run `ansible-playbook provision-groups.yml` to provision defined Groups
- Run `ansible-playbook provision-policy.yml` to create a basic RF=3 Storage Policy
- Run `ansible-playbook provision-users.yml` to create some Users and Buckets etc.
- Or, just run `ansible-playbook provision-all.yml` to apply all of the above

When creating Users, The users' S3 keys will be stored in a file `credentials` within `cwd`, ready to be used by AWS CLI.
