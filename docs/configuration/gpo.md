# Configuration des Group Policy Objects (GPO) sur Windows Server

## Prérequis

Avant de commencer la configuration des GPO, assurez-vous d'avoir les éléments suivants :
- Un serveur Windows Server installé et configuré avec Active Directory
- Un accès administrateur au serveur

## Étapes de configuration

### 1. Création d'une nouvelle GPO

1. Ouvrez "Gestion des stratégies de groupe" à partir du menu Démarrer.
2. Cliquez avec le bouton droit sur le domaine ou l'unité d'organisation (OU) où vous souhaitez créer la GPO et sélectionnez "Créer un objet de stratégie de groupe dans ce domaine, et le lier ici".
3. Entrez un nom pour la nouvelle GPO et cliquez sur "OK".

![Création d'une nouvelle GPO](../images/windows_server_gpo_creation.png)

### 2. Modification des paramètres de la GPO

1. Cliquez avec le bouton droit sur la GPO que vous avez créée et sélectionnez "Modifier".
2. Dans l'éditeur de gestion des stratégies de groupe, naviguez jusqu'à la section des paramètres que vous souhaitez configurer (par exemple, "Configuration de l'ordinateur" ou "Configuration de l'utilisateur").
3. Double-cliquez sur le paramètre que vous souhaitez modifier et configurez-le selon vos besoins.
4. Cliquez sur "OK" pour enregistrer les modifications.

![Modification des paramètres de la GPO](../images/windows_server_gpo_edit.png)

### 3. Application de la GPO

1. Assurez-vous que la GPO est liée au domaine ou à l'OU approprié.
2. Pour forcer l'application de la GPO, ouvrez une invite de commande sur un client et exécutez la commande suivante :
   ```
   gpupdate /force
   ```

![Application de la GPO](../images/windows_server_gpo_apply.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : Les paramètres de la GPO ne s'appliquent pas aux utilisateurs ou aux ordinateurs.**
  - **Solution :** Vérifiez que la GPO est correctement liée au domaine ou à l'OU et que les utilisateurs ou ordinateurs sont membres de cette unité.

- **Problème : Les modifications de la GPO ne prennent pas effet immédiatement.**
  - **Solution :** Exécutez la commande `gpupdate /force` sur les clients pour forcer l'application des modifications.

- **Problème : Les utilisateurs reçoivent des erreurs lors de l'application des GPO.**
  - **Solution :** Vérifiez les journaux d'événements sur les clients et le serveur pour identifier les erreurs spécifiques et résoudre les problèmes.

![Dépannage des problèmes courants](../images/windows_server_gpo_troubleshooting.png)

## Conclusion

Vous avez maintenant configuré les Group Policy Objects (GPO) sur Windows Server. Vous pouvez commencer à gérer les paramètres de configuration des utilisateurs et des ordinateurs selon vos besoins.
