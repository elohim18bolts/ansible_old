# Ansible Setup

Please create an **inventory** file with the correct host groups. The `ansible_user` is `ansible`

## Roles
1. Base
2. Workstation
3. Vms
4. Server

## Base

Create and setup the **ansible** user. This user has sudo privs, and is used for system mainteinance.

## Workstations

Install basic packages in a machine use for work porpuse.

**Run command:**

To run the command check for the avialables tasks and select the one you prefer, or none to install all.

***Note:*** You have to specified the username created during the installation process.

```
ansible-playbook playbook.yml --user ansible --extra-vars "{home_user: username}"


## Server

Install server tools.