# Ansible for Deployment Laravel appplication

Quickly provision laravel application all along with Apache2, php7.1-fpm, and MySQL server.

## Requirements
- Git
- Ansible 2+

## Installation
First, you need to install Git and Ansible :
```
sudo apt update
sudo apt install git ansible
git clone https://github.com/samsulmaarif/ansible-deploy-laravel.git
cd ansible-deploy-laravel
```

- Then you need to customize the playbook `deploy.yml` (or create a new one) to suit your needs. 
- Customize all variable in `group_vars/all.yml`.
- Edit your host in `inventory/host` (or create a new one)
- Run `ansible-playbook -i inventory/hosts deploy.yml --ask-become-pass` and enter your sudo password to run the playbook.

## Note
- This playbook only tested with Ubuntu 16.04 host.
- This is a **just work** playbook and may be does not contain a best practice. 