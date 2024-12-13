# Configuration de la Sauvegarde Windows sur Windows Server

## Prérequis

Avant de commencer la configuration de la Sauvegarde Windows, assurez-vous d'avoir les éléments suivants :
- Un serveur Windows Server installé et configuré
- Un accès administrateur au serveur

## Étapes de configuration

### 1. Installation de la fonctionnalité Sauvegarde Windows

1. Ouvrez le Gestionnaire de serveur.
2. Cliquez sur "Ajouter des rôles et des fonctionnalités".
3. Sélectionnez "Installation basée sur un rôle ou une fonctionnalité" et cliquez sur "Suivant".
4. Sélectionnez le serveur sur lequel vous souhaitez installer la fonctionnalité Sauvegarde Windows et cliquez sur "Suivant".
5. Cochez la case "Sauvegarde Windows Server" et cliquez sur "Suivant".
6. Cliquez sur "Ajouter des fonctionnalités" lorsque la fenêtre contextuelle s'affiche, puis cliquez sur "Suivant".
7. Cliquez sur "Installer" pour commencer l'installation de la fonctionnalité Sauvegarde Windows.

![Installation de la fonctionnalité Sauvegarde Windows](../images/windows_server_backup_installation.png)

### 2. Configuration de la sauvegarde planifiée

1. Une fois l'installation terminée, ouvrez l'outil "Sauvegarde Windows Server" à partir du menu Démarrer.
2. Cliquez sur "Sauvegarde planifiée" dans le volet de droite.
3. Suivez les instructions de l'assistant pour configurer une nouvelle sauvegarde planifiée.
4. Sélectionnez les éléments à sauvegarder (par exemple, volumes, dossiers, fichiers) et configurez les paramètres de sauvegarde selon vos besoins.

![Configuration de la sauvegarde planifiée](../images/windows_server_backup_scheduled.png)

### 3. Exécution d'une sauvegarde manuelle

1. Dans l'outil "Sauvegarde Windows Server", cliquez sur "Sauvegarde unique" dans le volet de droite.
2. Suivez les instructions de l'assistant pour configurer et exécuter une sauvegarde manuelle.
3. Sélectionnez les éléments à sauvegarder et configurez les paramètres de sauvegarde selon vos besoins.

![Exécution d'une sauvegarde manuelle](../images/windows_server_backup_manual.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : La sauvegarde échoue.**
  - **Solution :** Vérifiez que le service "Sauvegarde Windows Server" est en cours d'exécution et que le volume de destination dispose de suffisamment d'espace libre.

- **Problème : Les sauvegardes planifiées ne s'exécutent pas.**
  - **Solution :** Assurez-vous que les paramètres de planification sont correctement configurés et que le serveur est allumé et connecté au réseau au moment de la sauvegarde.

- **Problème : Les fichiers sauvegardés ne peuvent pas être restaurés.**
  - **Solution :** Vérifiez que les fichiers de sauvegarde ne sont pas corrompus et que les paramètres de restauration sont correctement configurés.

![Dépannage des problèmes courants](../images/windows_server_backup_troubleshooting.png)

## Conclusion

Vous avez maintenant configuré la Sauvegarde Windows sur Windows Server. Vous pouvez commencer à planifier et exécuter des sauvegardes selon vos besoins.
