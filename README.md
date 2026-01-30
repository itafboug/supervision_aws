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
