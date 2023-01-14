# Trabalho prático da UC de Aplicações e Serviços de Computação em Nuvem - Ano Letivo 2022/2023

Grupo 21

* Simão Cunha (a93262)
* Tiago Silva (a93277)
* Gonçalo Braz (a93178)
* Gonçalo Pereira (a93168)
* Hugo Fernandes (pg50419)
 
Comandos Ansible:
* Criação do cluster GKE
```
ansible-playbook create-gke-cluster.yml -i inventory/gcp.yml
```
* Destruição do cluster GKE
```
ansible-playbook destroy-gke-cluster.yml -i inventory/gcp.yml
```
* Deploy Ghost
```
ansible-playbook deploy-ghost.yml -i inventory/gcp.yml -e @mail_cred.enc --ask-vault-pass
```
* Uneploy Ghost
```
ansible-playbook undeploy-ghost.yml -i inventory/gcp.yml
```