# Automatizando o setup do WSL de distros Debian-Like

Este repositório contém os passos para automatizar e acelerar o fluxo de trabalho e preparação do meu ambiente Linux, executado sob o WSL-2 (Windows Sub-system for Linux versão 2), utilizando Ansible e Git.  

> **Isenção de Responsabilidade** :  
> Those scripts are ubuntu related with major version 18+, for other distributions you'll need to adapt it
___

## Prepare Workstation

> Read the `ubuntu.yml` file before applying and be sure to understand everything that will be done.

1. Install Ansible
```bash
sudo apt update && sudo apt install ansible unzip git -y
```
2. Clone this repository
```bash
git clone https://github.com/caiodelgadonew/tools.git
```

3. Apply the configuration
```bash
ansible-playbook tools/ubuntu.yml --ask-become-pass
```
>Type your password when asked to give root permissions for some actions.
___

# License
GPLv3

# Author Information
Created by [Caio Delgado](https://linktr.ee/caiodelgadonew)

Contributions are more than welcome!
