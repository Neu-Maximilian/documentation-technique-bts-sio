# Configuration de DHCP sur Windows Server

## Prérequis

Avant de commencer la configuration de DHCP, assurez-vous d'avoir les éléments suivants :
- Un serveur Windows Server installé et configuré
- Un accès administrateur au serveur

## Étapes de configuration

### 1. Installation du rôle DHCP

1. Ouvrez le Gestionnaire de serveur.
2. Cliquez sur "Ajouter des rôles et des fonctionnalités".
3. Sélectionnez "Installation basée sur un rôle ou une fonctionnalité" et cliquez sur "Suivant".
4. Sélectionnez le serveur sur lequel vous souhaitez installer le rôle DHCP et cliquez sur "Suivant".
5. Cochez la case "Serveur DHCP" et cliquez sur "Suivant".
6. Cliquez sur "Ajouter des fonctionnalités" lorsque la fenêtre contextuelle s'affiche, puis cliquez sur "Suivant".
7. Cliquez sur "Installer" pour commencer l'installation du rôle DHCP.

![Installation du rôle DHCP](../images/windows_server_dhcp_installation.png)

### 2. Configuration de la portée DHCP

1. Une fois l'installation terminée, ouvrez le Gestionnaire DHCP à partir du menu Démarrer.
2. Cliquez avec le bouton droit sur le nom du serveur et sélectionnez "Nouvelle portée".
3. Suivez les instructions de l'assistant pour créer une nouvelle portée.
4. Entrez un nom pour la portée et configurez les paramètres de plage d'adresses IP (par exemple, de 192.168.1.100 à 192.168.1.200).

![Configuration de la portée DHCP](../images/windows_server_dhcp_scope.png)

### 3. Configuration des options DHCP

1. Dans le Gestionnaire DHCP, cliquez avec le bouton droit sur la portée que vous avez créée et sélectionnez "Configurer les options".
2. Configurez les options DHCP nécessaires, telles que la passerelle par défaut, le serveur DNS, et le domaine de recherche.
3. Cliquez sur "Appliquer" pour enregistrer les paramètres.

![Configuration des options DHCP](../images/windows_server_dhcp_options.png)

### 4. Activation de la portée DHCP

1. Dans le Gestionnaire DHCP, cliquez avec le bouton droit sur la portée que vous avez créée et sélectionnez "Activer".
2. Confirmez l'activation de la portée.

![Activation de la portée DHCP](../images/windows_server_dhcp_activate.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : Les clients ne reçoivent pas d'adresses IP.**
  - **Solution :** Vérifiez que le service DHCP est en cours d'exécution et que la portée est activée.

- **Problème : Les clients reçoivent des adresses IP incorrectes.**
  - **Solution :** Assurez-vous que les paramètres de la portée DHCP sont correctement configurés et que les options DHCP sont correctement définies.

- **Problème : Le serveur DHCP ne répond pas aux requêtes.**
  - **Solution :** Vérifiez que le service DHCP est en cours d'exécution et que les paramètres de pare-feu permettent le trafic DHCP.

![Dépannage des problèmes courants](../images/windows_server_dhcp_troubleshooting.png)

## Conclusion

Vous avez maintenant configuré DHCP sur Windows Server. Vous pouvez commencer à gérer les adresses IP et les options DHCP selon vos besoins.
