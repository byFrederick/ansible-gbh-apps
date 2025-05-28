# GBH Demo Apps Deployment using Ansible
## Contents

- [Description](#description)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Final Thoughts](#final-thoughts)

## Description

Ansible playbooks to deploy demo-api and demo-webapp on an server.

## Prerequisites
- Target VM needs to have apt packet manager (Ubuntu/Debian).

## Setup

To deploy all the components, follow this instructions:

```bash
curl -s -L https://github.com/byFrederick/ansible-gbh-apps/archive/refs/tags/v0.0.1.tar.gz | tar xz
cd ansible-gbh-apps-0.0.1
vi inventories/nonprod/hosts.ini #Modify based on your target VM information
vi ansible.cfg #Modify ssh private key path
ansible-playbook playbooks/main.yaml
```

Your components will be up and running. By default, demo-api is listening on port 3001 and webapp on port 80

## Final Thoughts

- It wasn’t clear if I had to deploy both apps on one VM or on separate VMs, so I put everything on one server (not ideal). But, the playbooks are created in a way that using separate VMs is possible with minor modifications.