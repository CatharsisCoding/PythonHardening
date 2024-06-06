# Documentation de l'application de renforcement de la sécurité
## Description
L'application de renforcement de la sécurité est une interface utilisateur graphique (GUI) développée en Python avec PySide6 qui permet d'exécuter diverses tâches de renforcement de la sécurité sur un système Linux.

## Fonctionnalités
L'application offre les fonctionnalités suivantes :

Sécurisation des fichiers : Permet de modifier les permissions des fichiers pour les rendre plus sécurisés.
Mise à jour du système : Met à jour la liste des paquets et les paquets installés sur le système.
Désactivation d'apache2 : Arrête le service Apache HTTP Server.
Configuration du pare-feu : Configure le pare-feu en définissant des politiques par défaut pour les paquets entrants, sortants et en transit, ainsi que des règles spécifiques pour autoriser certaines connexions.
Désactivation du port 80 : Bloque les connexions entrantes sur le port 80.
Scan des vulnérabilités : Utilise l'outil Nmap pour scanner les vulnérabilités de base sur le système local.
## Prérequis

Avant d'exécuter cette application, assurez-vous d'avoir installé les logiciels et les modules nécessaires sur votre système.

### Logiciels requis :

- **iptables** : Un utilitaire de ligne de commande pour configurer le pare-feu du noyau Linux. Vous pouvez l'installer sur Ubuntu en utilisant la commande suivante :
sudo apt update
sudo apt install iptables


- **Apache2** : Un serveur HTTP populaire. Si vous prévoyez d'utiliser la fonctionnalité de désactivation d'Apache2, vous pouvez l'installer sur Ubuntu avec :
sudo apt update
sudo apt install apache2

- **Nmap** : Un scanner de réseau et d'analyse de sécurité. Vous pouvez l'installer sur Ubuntu avec :
sudo apt update
sudo apt install nmap


### Modules Python requis :

- **PySide6** : Une bibliothèque permettant de créer des interfaces graphiques utilisateurs (GUI) en utilisant Qt 6. Vous pouvez l'installer via pip :
pip install PySide6



- **pyqt-tools** : Un ensemble d'outils supplémentaires pour PyQt, y compris le Designer Qt, un outil de conception d'interfaces graphiques. Vous pouvez l'installer via pip :
`pip install pyqt-tools
## Utilisation
L'application est conçue pour être simple et intuitive à utiliser. Voici comment utiliser chaque fonctionnalité :

Sécurisation des fichiers : Cliquez sur le bouton "Sécuriser Fichier" et sélectionnez le fichier à sécuriser. Entrez ensuite votre mot de passe sudo lorsque vous y êtes invité.
Mise à jour du système : Cliquez sur le bouton "Mettre à jour le système" pour mettre à jour le système. Entrez votre mot de passe sudo lorsque vous y êtes invité.
Désactivation d'apache2 : Cliquez sur le bouton "Désactiver apache2" pour arrêter le service Apache2. Entrez votre mot de passe sudo lorsque vous y êtes invité.
Configuration du pare-feu : Cliquez sur le bouton "Configurer le pare-feu" pour configurer le pare-feu avec des règles spécifiques. Entrez votre mot de passe sudo lorsque vous y êtes invité.
Désactivation du port 80 : Cliquez sur le bouton "Désactiver le port 80" pour bloquer les connexions entrantes sur le port 80. Entrez votre mot de passe sudo lorsque vous y êtes invité.
Scan des vulnérabilités : Cliquez sur le bouton "Scan des vulnérabilités" pour scanner les vulnérabilités du système local. Entrez votre mot de passe sudo lorsque vous y êtes invité.
## Remarques
Assurez-vous d'avoir le mot de passe sudoer appropriés pour exécuter les différentes fonctionnalités de l'application.
Certaines fonctionnalités peuvent nécessiter des dépendances supplémentaires telles que Nmap ou iptables, assurez-vous de les installer si nécessaire.
`sudo apt update
sudo apt install nmap iptables
