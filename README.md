"# vagrant-vm-linux" 
Création de VM Linux avec vagrant
Ce fichier Vagrantfile configure une machine virtuelle avec Vagrant et VirtualBox. Il utilise l'image de base Ubuntu 14.04 64-bit (nommée ubuntu/trusty64). La machine est configurée pour ne pas vérifier les mises à jour de l'image et redirige le port 8080 de la VM vers le port 8082 de l'hôte pour l'accès web.
Il définit également un réseau privé avec une adresse IP statique 192.168.33.10 et synchronise un dossier de l'hôte ./tomcatwebapps avec le dossier /opt/tomcat/webapps de la VM pour partager des fichiers.
La configuration de VirtualBox inclut l'activation de l'interface graphique pour la VM, un nom personnalisé serveurweb-tomcat, et une allocation de 1 Go de RAM.
<img width="552" alt="c1" src="https://github.com/user-attachments/assets/0712afc0-d5a7-4a6b-a37d-e668f3ff8bf7" />
