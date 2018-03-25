# Example of Ansible infrastructure repository.

[In Russian](README_ru.md)

## Description
* All roles installed by `ansible-galaxy install -r requirements.yml` with fixed versions
* Environments described in `environments` folder with their own variables.
* All playbooks in `playbooks` folder.
* By default `ini` format of `inventory` is used. Starting from 2.4 you can use `yml` format.


## How to use
* Clone this repo && cd into
* Create vault.key - `echo 'key' > vault.key`
* Include roles in requirements.yml && download them with ansible-galaxy
* Write playbooks in `playbooks` folder
* Fill inventory and group_vars
* Run `ansible-playbook -i environments/env playbooks/your_playbook.yml`
