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
* Aceder ao cluster no terminal
```
gcloud container clusters get-credentials ascn-cluster --zone europe-west1-b --project ascn-grupo21
```
```
kubectl get all
```