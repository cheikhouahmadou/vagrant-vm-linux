"# vagrant-vm-linux" 
Création de VM Linux avec vagrant
Ce fichier Vagrantfile configure une machine virtuelle avec Vagrant et VirtualBox.
Il utilise l'image de base Ubuntu 14.04 64-bit (nommée ubuntu/trusty64). 
La machine est configurée pour ne pas vérifier les mises à jour de l'image et 
redirige le port 8080 de la VM vers le port 8082 de l'hôte pour l'accès web.
Il définit également un réseau privé avec une adresse IP statique 192.168.33.10 et 
synchronise un dossier de l'hôte ./tomcatwebapps avec le dossier /opt/tomcat/webapps de la 
VM pour partager des fichiers.
La configuration de VirtualBox inclut l'activation de l'interface graphique pour la VM, 
un nom personnalisé serveurweb-tomcat, et une allocation de 1 Go de RAM.
<img width="552" alt="c1" src="https://github.com/user-attachments/assets/0712afc0-d5a7-4a6b-a37d-e668f3ff8bf7" />

La commande vagrant validate sert à vérifier si le fichier Vagrantfile est syntaxiquement 
correct et s'il n'y a pas d'erreurs évidentes dans la configuration de la machine virtuelle. 
Cependant, cette commande ne démarre pas la machine virtuelle ni ne crée d'instances. Elle permet 
simplement de s'assurer que la configuration est valide avant d'exécuter des commandes comme vagrant up ou vagrant provision.
<img width="460" alt="c2" src="https://github.com/user-attachments/assets/55e0a18c-3422-4e69-a18d-91691949c551" />

La commande vagrant up est utilisée pour démarrer la machine virtuelle définie dans le fichier Vagrantfile.
<img width="958" alt="c3" src="https://github.com/user-attachments/assets/753dd28d-28d7-4706-9a87-2de59a6a68b8" />

La commande vagrant ssh permet de se connecter à la machine virtuelle (VM) en utilisant SSH 
(Secure Shell). Une fois exécutée, elle ouvre un terminal directement dans la VM, vous permettant
de l'utiliser comme si vous étiez connecté à un serveur distant.

<img width="367" alt="c4" src="https://github.com/user-attachments/assets/8bd88d9f-cefb-4fba-8d8b-d08226663793" />

