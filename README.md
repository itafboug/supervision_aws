# Supervision Centralisée AWS avec Zabbix

## Description
Déploiement d'une infrastructure de monitoring Zabbix sur AWS pour surveiller un parc hybride Linux/Windows.

##  Objectifs
- Déployer Zabbix en conteneurs Docker sur AWS
- Installer les agents Zabbix sur Linux et Windows
- Centraliser le monitoring dans une interface unique

##  Architecture
- **Serveur Zabbix** : t3.large Ubuntu avec Docker
- **Client Linux** : t3.medium Ubuntu
- **Client Windows** : t3.large Windows Server

##  Technologies
- AWS EC2, VPC, Security Groups
- Docker, Docker Compose
- Zabbix 6.4
- Ubuntu 24.04, Windows Server 2022

## 📁 Structure
## Configuration Docker Compose

Le fichier `docker-compose.yml` définit trois services :
1. **zabbix-db** : Base de données MySQL pour stocker les données de monitoring
2. **zabbix-server** : Serveur Zabbix principal (port 10051)
3. **zabbix-web** : Interface web Nginx (port 80)

Les services communiquent via un réseau Docker dédié et utilisent des volumes persistants pour la conservation des données.
