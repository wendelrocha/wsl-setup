# Automatizando o setup do WSL de distros Debian-Like

Este repositório contém os passos para automatizar a preparação do meu ambiente Linux Debian Like, executado sob o WSL-2 (Windows Sub-system for Linux versão 2), utilizando Ansible e Git.  

> **Isenção de Responsabilidade** :

>Este código aplica-se a distribuições Linux, versões 18 e superiores. Para outras distribuições, você deve adapta-lo. 

___

## Preparando o computador

> Leia o arquivo `ubuntu-like.yml`antes de executa-lo, certifique-se de que entendeu tudo o que ele faz.

1. Instale 0 Ansible
```bash
sudo apt update && sudo apt install ansible unzip git -y
```
2. Clone este repositório
```bash
git clone https://github.com/wendelrocha/wsl-setup.git
```

3. Aplique a configuração
```bash
ansible-playbook tools/ubuntu-like.yml --ask-become-pass
```
>Digite sua senha, quando solicitado, para dar permissões de root para algumas ações.
___

# Licença
GPLv3

# Autoria
Criado por [Caio Delgado](https://linktr.ee/caiodelgadonew)
Adaptado por [Wendel Rocha](https://www.linkedin.com/in/wendelrochapro/)

Contribuições são mais que bem-vindas
