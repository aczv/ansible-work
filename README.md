# ansible-work

Ansible playbooks to provision developer machine.

## Prepare controll machine

Install Ansible:

    https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

Install common tools:

    sudo apt-get install git mc

## Prepare target machines

Install OpenSSH Server:

    sudo apt install openssh-server

Copy SSH keys to remote machines, e.g.:

    ssh-copy-id localhost

Run add-hoc command on all servers:

    ansible all -a "uname -a"

