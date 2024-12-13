# Configuration de DHCP HA sur Windows Server

## Prérequis

Avant de commencer la configuration de DHCP HA, assurez-vous d'avoir les éléments suivants :
- Deux serveurs Windows Server installés et configurés
- Un accès administrateur aux deux serveurs
- Le rôle DHCP installé sur les deux serveurs

## Étapes de configuration

### 1. Configuration du premier serveur DHCP

1. Ouvrez le Gestionnaire de serveur sur le premier serveur.
2. Cliquez sur "DHCP" dans le menu de gauche.
3. Cliquez avec le bouton droit sur le nom du serveur et sélectionnez "Configurer l'étendue".
4. Suivez les instructions de l'assistant pour créer une nouvelle étendue.
5. Entrez un nom pour l'étendue et configurez les paramètres de plage d'adresses IP (par exemple, de 192.168.1.100 à 192.168.1.200).
6. Configurez les options DHCP nécessaires, telles que la passerelle par défaut, le serveur DNS, et le domaine de recherche.
7. Cliquez sur "Terminer" pour terminer la configuration de l'étendue.

![Configuration du premier serveur DHCP](../images/windows_server_dhcp_ha_first_server.png)

### 2. Configuration du deuxième serveur DHCP

1. Ouvrez le Gestionnaire de serveur sur le deuxième serveur.
2. Cliquez sur "DHCP" dans le menu de gauche.
3. Cliquez avec le bouton droit sur le nom du serveur et sélectionnez "Configurer l'étendue".
4. Suivez les instructions de l'assistant pour créer une nouvelle étendue.
5. Entrez un nom pour l'étendue et configurez les paramètres de plage d'adresses IP (par exemple, de 192.168.1.201 à 192.168.1.254).
6. Configurez les options DHCP nécessaires, telles que la passerelle par défaut, le serveur DNS, et le domaine de recherche.
7. Cliquez sur "Terminer" pour terminer la configuration de l'étendue.

![Configuration du deuxième serveur DHCP](../images/windows_server_dhcp_ha_second_server.png)

### 3. Configuration de la redondance DHCP

1. Sur le premier serveur, ouvrez le Gestionnaire DHCP.
2. Cliquez avec le bouton droit sur l'étendue que vous avez créée et sélectionnez "Configurer la redondance".
3. Suivez les instructions de l'assistant pour configurer la redondance DHCP.
4. Sélectionnez le deuxième serveur DHCP comme partenaire de redondance.
5. Configurez les paramètres de redondance selon vos besoins (par exemple, mode de basculement ou mode de charge partagée).
6. Cliquez sur "Terminer" pour terminer la configuration de la redondance.

![Configuration de la redondance DHCP](../images/windows_server_dhcp_ha_failover.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : Les clients ne reçoivent pas d'adresses IP.**
  - **Solution :** Vérifiez que les services DHCP sont en cours d'exécution sur les deux serveurs et que les étendues sont activées.

- **Problème : Les clients reçoivent des adresses IP incorrectes.**
  - **Solution :** Assurez-vous que les paramètres des étendues DHCP sont correctement configurés et que les options DHCP sont correctement définies sur les deux serveurs.

- **Problème : La redondance DHCP ne fonctionne pas correctement.**
  - **Solution :** Vérifiez que les paramètres de redondance sont correctement configurés et que les deux serveurs peuvent communiquer entre eux.

![Dépannage des problèmes courants](../images/windows_server_dhcp_ha_troubleshooting.png)

## Conclusion

Vous avez maintenant configuré DHCP HA sur Windows Server. Vous pouvez commencer à gérer les adresses IP et les options DHCP avec une haute disponibilité selon vos besoins.
