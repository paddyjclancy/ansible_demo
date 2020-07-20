# Ansible and Infrastructure as code

## Ansible - Introduction

- Ansible is a high level language, meaning it is highly abstracted. 
- Ansible can deal with many different environments and package managers.
- Built on Python, Open Source, fits perfectly into DevOps.

--> Flexibility, Ease of use, Robustness & Cost (Pillars of DevOps)

- Increases robustness as you are making Infrastructure as Code & Its a CM tool.

- Allows us to setup, track & manage Several machines!

### Installing Ansible

- On Windows, use a Linux Sub-system to install it - OR - Install it on a VM
- On Mac, Use Python or HomeBrew. 

## How to connect through SSH

- After setting up Password Authentication

1. In Ansible machine, ssh-keygen
2. ssh-copy-id <Target Machine IP>

## Test if ansible can connect to agent nodes

- ansible ping -m all

## Now its time to run our playbook for DB

1. Lets run the `ansible-playbook playbook_db.yml` first to get our db machine setup. Make sure you are in the ansible directory. use pwd to make sure.
2. We can check that the service is running by bashing `systemctl status mongod`

- We should see that the mongod.service is active and running!

## Now its time to run our playbook for Web App

1. Run `ansible-playbook playbook.yml`

- Great, our app is running!

## How to get /posts working

- At the moment posts is not working after forver start app.js from within the playbook
- However if we vagrant reload, and go straight in the web machine, run forever start app.js  |  it now works. On to more debugging...




