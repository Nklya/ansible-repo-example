# Example of Ansible infrastructure repository.

## Description
* All roles installed by `ansible-galaxy install -r requirements.yml` with fixed versions
* Environments described in `environments` folder with their own variables.
* All playbooks in `playbooks` folder.


## How to use
* Clone this repo && cd into
* Create vault.key - `echo 'key' > vault.key`
* Include needed roles in requirements.yml && download them with ansible-galaxy
* Write playbooks
* Fill inventory and group_vars
* Run `ansible-playbook -i environments/env playbooks/your_playbook.yml`
