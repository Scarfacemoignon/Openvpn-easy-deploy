# 🎯 Openvpn-easy-deploy
Script Bash simple et automatisé pour installer, configurer et gérer un serveur OpenVPN sur Debian, Ubuntu ou CentOS.

# OpenVPN Automated Installer

Ce dépôt contient un script Bash permettant d'installer, configurer et gérer automatiquement un serveur OpenVPN sur un VPS basé sur Debian, Ubuntu ou CentOS.

## 🎯 Objectif

Simplifier le déploiement d'un serveur VPN fonctionnel en quelques minutes, avec :
- Création automatique des certificats via Easy-RSA
- Configuration du routage et de la NAT
- Gestion des clients (création, révocation)
- Désinstallation propre

## 🚀 Fonctionnalités

✅ Installation complète d'OpenVPN et Easy-RSA  
✅ Génération des certificats serveur et client  
✅ Configuration automatique de `iptables` ou `firewalld` pour la redirection du trafic  
✅ Support des distributions suivantes :
- Debian (9+)
- Ubuntu (18.04+)
- CentOS (7+)

✅ Interface interactive :
- **Ajouter un utilisateur**
- **Révoquer un utilisateur**
- **Désinstaller OpenVPN**

✅ Génération d’un fichier `.ovpn` prêt à importer dans vos clients OpenVPN.

## 🛠️ Prérequis

- Un VPS avec accès root
- TUN/TAP activé
- Connexion Internet

## ⚡ Installation

Clonez le dépôt puis exécutez le script :

```bash
git clone https://github.com/Scarfacemoignon/Openvpn-easy-deploy.git
cd Openvpn-easy-deploy/
chmod +x openvpn-install.sh
sudo ./openvpn-install.sh
