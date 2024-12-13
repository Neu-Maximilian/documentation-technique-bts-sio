# Installation de TrueNAS Scale

## Prérequis matériels

Avant de commencer l'installation de TrueNAS Scale, assurez-vous d'avoir le matériel suivant :
- Un ordinateur ou un serveur avec un processeur 64 bits
- Au moins 8 Go de RAM (16 Go ou plus recommandés)
- Au moins 16 Go d'espace disque pour l'installation (32 Go ou plus recommandés)
- Un lecteur USB ou un CD/DVD pour l'installation

## Étapes d'installation

### 1. Téléchargement de l'image d'installation

1. Rendez-vous sur le site officiel de TrueNAS : [https://www.truenas.com/download-truenas-scale/](https://www.truenas.com/download-truenas-scale/)
2. Sélectionnez la version de TrueNAS Scale que vous souhaitez installer.
3. Téléchargez l'image d'installation.

![Téléchargement de l'image d'installation](../images/truenas_scale_download.png)

### 2. Création du support d'installation

1. Si vous avez téléchargé l'image USB, utilisez un outil comme Rufus pour créer une clé USB bootable.
2. Si vous avez téléchargé l'image CD, gravez l'image sur un CD/DVD.

![Création du support d'installation](../images/truenas_scale_usb_creation.png)

### 3. Démarrage à partir du support d'installation

1. Insérez la clé USB ou le CD/DVD dans l'ordinateur ou le serveur sur lequel vous souhaitez installer TrueNAS Scale.
2. Démarrez l'ordinateur et accédez au menu de démarrage (généralement en appuyant sur une touche comme F12, F2, ou ESC).
3. Sélectionnez le support d'installation (USB ou CD/DVD) comme périphérique de démarrage.

![Démarrage à partir du support d'installation](../images/truenas_scale_boot_menu.png)

### 4. Installation de TrueNAS Scale

1. Une fois que l'ordinateur a démarré à partir du support d'installation, vous verrez l'écran de bienvenue de TrueNAS Scale.
2. Sélectionnez "Install" pour commencer l'installation.

![Écran de bienvenue de TrueNAS Scale](../images/truenas_scale_welcome.png)

3. Suivez les instructions à l'écran pour configurer les paramètres de base (langue, disposition du clavier, etc.).
4. Sélectionnez le disque sur lequel vous souhaitez installer TrueNAS Scale.
5. Choisissez le type de partitionnement (généralement "Auto" pour une installation standard).
6. Confirmez les paramètres et lancez l'installation.

![Installation de TrueNAS Scale](../images/truenas_scale_installation.png)

### 5. Configuration initiale

1. Une fois l'installation terminée, redémarrez l'ordinateur.
2. Retirez le support d'installation (clé USB ou CD/DVD).
3. Lors du premier démarrage, vous serez invité à configurer les paramètres de base (nom d'utilisateur, mot de passe, etc.).
4. Suivez les instructions à l'écran pour terminer la configuration initiale.

![Configuration initiale de TrueNAS Scale](../images/truenas_scale_initial_setup.png)

### 6. Accès à l'interface web

1. Une fois la configuration initiale terminée, connectez un ordinateur au réseau local de TrueNAS Scale.
2. Ouvrez un navigateur web et accédez à l'adresse IP de TrueNAS Scale (par défaut, [http://192.168.1.1](http://192.168.1.1)).
3. Connectez-vous à l'interface web avec les identifiants que vous avez configurés lors de l'installation.

![Accès à l'interface web de TrueNAS Scale](../images/truenas_scale_web_interface.png)

4. Changez le mot de passe par défaut et configurez les paramètres supplémentaires selon vos besoins.

![Changement du mot de passe par défaut](../images/truenas_scale_change_password.png)

## Conclusion

Vous avez maintenant installé et configuré TrueNAS Scale sur votre matériel. Vous pouvez commencer à configurer des partages de fichiers, des services de stockage, et d'autres fonctionnalités avancées selon vos besoins.
