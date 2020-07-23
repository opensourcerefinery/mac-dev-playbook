# Mac Development Ansible Playbook

This repository is a fork of Jeff Geerlings excellent repository: https://github.com/geerlingguy/mac-dev-playbook
It is a stripped version suited to my needs.

For installation:
 
    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ mkdir projects && cd projects
    $ git clone git@github.com:ricbra/mac-dev-playbook.git
    $ cd mac-dev-playbook
    $ ansible-galaxy install -r requirements.yml
    
    For Ansible < 2.0
    $ ansible-playbook -i inventory --ask-sudo-password main.yml 
    For Ansible >= 2.0 use 
    $ ansible-playbook -i inventory --ask-become-pass main.yml 
    
    $ cd ~/dotfiles
    $ bin/install
    $ bin/setup_osx



## Current Manual Setup

- Tunnel Blick (VPN)
- id_rsa (with passphrase)
- Docker Desktop on Mac https://docs.docker.com/docker-for-mac/install/


#### Tunnelblick

https://gitlab.datacomp-intranet.com/system/awesomeness/-/wikis/vpn/vpn-tips
https://tunnelblick.net/downloads

- get keys and config from john

## Needs testing

- brew cask install keeweb
- brew cask install mysqlworkbench

## Missing

- postman
- ring central

## Undecided

- virtual box
- munki

## Standard Computer setup

## Developer Computer setup

* mkdir ~/development && cd development
  * this is where all projects go

### Docker Config

#### minimum resources

* Ram: 4 Gb
* Cpu: 4 Cpu
* Hard Drive: 64 Gb

#### recommended for full stck

* Ram: 8 Gb
* Cpu: 8 Cpu
* Hard Drive: 128 Gb