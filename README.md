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






