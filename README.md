# lab-iac

    Escolhi separar o projeto do [lab-iac-base](https://github.com/CringerLabs/lab-iac-base) e deste para poder separar melhor as configurações iniciais das configurações de todas as máquinas. A lista de máquinas foi passada no inventário.

    Segue abaixo um desenho preliminar desse Challenge.
    ![](images/cringerlabs_company.png)


## Zabbix

Instalação do Zabbix 5 com MySQL Community 8.
```
ansible-playbook install-zabbix.yml
```


## ELK

Instalação do ELK Stack juntamente com um filtro preparado para monitoramento de atividades no Linux, todos os comandos digitados no bash do Linux, serão enviados para o ELK e será possível a visualização pela interface.
```
ansible-playbook install-elk.yml
```


## Gitlab

Instalação do repositório GIT.
```
ansible-playbook install-gitlab.yml
```


## Foreman

Instalação do pack de ferramentas Foreman, para atigir o ciclo de vida tambem do sistema operacional.
```
ansible-playbook install-foreman.yml
```


## AWX

Instalação do AWX, interface para gerenciamento de jobs ansible no ambiente.
```
ansible-playbook install-awx.yml
```



