# dev-setup
This repo contains scripts for installing dev tools on a new Ubuntu 22.04 system

## Ansible installation
Having ansible installed in your system helps to automate the first time setup process

```
sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt install ansible
```

Install the playbooks to setup your system
```
ansible-playbook setup_langs.yaml --ask-become-pass
ansible-playbook dev_utilities_setup.yaml --ask-become-pass
```
