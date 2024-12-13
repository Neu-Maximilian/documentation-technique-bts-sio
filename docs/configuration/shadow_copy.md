# Configuration de Shadow Copy sur Windows Server

## Prérequis

Avant de commencer la configuration de Shadow Copy, assurez-vous d'avoir les éléments suivants :
- Un serveur Windows Server installé et configuré
- Un accès administrateur au serveur

## Étapes de configuration

### 1. Activation de Shadow Copy

1. Ouvrez l'Explorateur de fichiers.
2. Cliquez avec le bouton droit sur le volume pour lequel vous souhaitez activer Shadow Copy et sélectionnez "Propriétés".
3. Allez à l'onglet "Versions précédentes".
4. Cliquez sur "Activer" pour activer Shadow Copy sur ce volume.

![Activation de Shadow Copy](../images/windows_server_shadow_copy_enable.png)

### 2. Configuration des paramètres de Shadow Copy

1. Une fois Shadow Copy activé, cliquez sur "Paramètres".
2. Configurez les paramètres de Shadow Copy selon vos besoins, tels que la taille maximale de stockage et l'horaire des copies.
3. Cliquez sur "OK" pour enregistrer les paramètres.

![Configuration des paramètres de Shadow Copy](../images/windows_server_shadow_copy_settings.png)

### 3. Restauration de fichiers à partir de Shadow Copy

1. Pour restaurer un fichier à partir de Shadow Copy, cliquez avec le bouton droit sur le fichier ou le dossier et sélectionnez "Restaurer les versions précédentes".
2. Sélectionnez la version que vous souhaitez restaurer et cliquez sur "Restaurer".

![Restauration de fichiers à partir de Shadow Copy](../images/windows_server_shadow_copy_restore.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : Shadow Copy ne s'active pas.**
  - **Solution :** Vérifiez que le service "Cliché instantané des volumes" est en cours d'exécution et que le volume dispose de suffisamment d'espace libre.

- **Problème : Les versions précédentes ne sont pas disponibles.**
  - **Solution :** Assurez-vous que Shadow Copy est activé sur le volume et que les paramètres de stockage sont correctement configurés.

- **Problème : Les utilisateurs ne peuvent pas accéder aux versions précédentes.**
  - **Solution :** Vérifiez que les utilisateurs ont les autorisations nécessaires pour accéder aux versions précédentes et que les paramètres de sécurité sont correctement configurés.

![Dépannage des problèmes courants](../images/windows_server_shadow_copy_troubleshooting.png)

## Conclusion

Vous avez maintenant configuré Shadow Copy sur Windows Server. Vous pouvez commencer à utiliser les versions précédentes pour restaurer des fichiers selon vos besoins.
