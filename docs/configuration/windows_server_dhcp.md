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

![Configuration requise pour DHCP](../images/windows-dhcp/windows_server_dhcp_conf_requise.png)

### 2. Configuration initiale du rôle DHCP

1. Une fois l'installation terminée, une fenêtre s’ouvre automatiquement pour la configuration post-installation. Cliquez sur "Configurer" pour commencer.

![Description du rôle DHCP](../images/windows-dhcp/windows_server_dhcp_conf_description.png)

2. Suivez les étapes pour autoriser le serveur DHCP dans Active Directory. Cela garantit que le serveur est reconnu et autorisé à distribuer des adresses IP.

![Autorisation de DHCP](../images/windows-dhcp/windows_server_dhcp_conf_autorisation.png)

### 3. Configuration de la portée DHCP

1. Une fois l'installation terminée, ouvrez le Gestionnaire DHCP à partir du menu Démarrer.
2. Cliquez avec le bouton droit sur le nom du serveur et sélectionnez "Nouvelle portée".
3. Suivez les instructions de l'assistant pour créer une nouvelle portée.

![Lancement de l’assistant de nouvelle portée](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_assistant.png)

4. Entrez un nom pour la portée et configurez les paramètres de plage d'adresses IP.

![Nom de la nouvelle portée](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_nom.png)
![Configuration de la plage IP](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_plage_ip.png)

5. Définissez une plage d'exclusion si nécessaire.

![Plage d'exclusion](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_exclusion.png)

6. Configurez la durée des baux DHCP.

![Durée des baux](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_bail.png)

7. Ajoutez des paramètres supplémentaires tels que la passerelle par défaut, le serveur DNS, et les paramètres WINS.

![Passerelle par défaut](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_passrelle.png)
![Configuration DNS](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_dns.png)
![Paramètres WINS](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_wins.png)

8. Terminez la création de la portée.

![Fin de l’assistant de nouvelle portée](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_fin.png)

### 4. Configuration des options DHCP

1. Dans le Gestionnaire DHCP, cliquez avec le bouton droit sur la portée que vous avez créée et sélectionnez "Configurer les options".
2. Configurez les options DHCP nécessaires, telles que la passerelle par défaut, le serveur DNS, et le domaine de recherche.

![Options des serveurs DHCP IPv4](../images/windows-dhcp/windows_server_dhcp_options_serveurs_ipv4.png)

3. Cliquez sur "Appliquer" pour enregistrer les paramètres.

### 5. Activation de la portée DHCP

1. Dans le Gestionnaire DHCP, cliquez avec le bouton droit sur la portée que vous avez créée et sélectionnez "Activer".
2. Confirmez l'activation de la portée.

![Activation de la portée](../images/windows-dhcp/windows_server_dhcp_nouvelle_etendue_activer.png)

### 6. Réservation d'adresses IP (optionnel)

1. Si vous souhaitez réserver une adresse IP pour un client spécifique, accédez à la section "Réservations" dans le Gestionnaire DHCP.
2. Cliquez avec le bouton droit et sélectionnez "Nouvelle réservation".
3. Entrez le nom, l’adresse IP, l’adresse MAC du client, et une description si nécessaire.

![Création d'une réservation](../images/windows-dhcp/windows_server_dhcp_reservation.png)
![Réservation complétée](../images/windows-dhcp/windows_server_dhcp_reservation_1.png)

## Dépannage

### Problèmes courants et solutions

- **Problème : Les clients ne reçoivent pas d'adresses IP.**
  - **Solution :** Vérifiez que le service DHCP est en cours d'exécution et que la portée est activée.

- **Problème : Les clients reçoivent des adresses IP incorrectes.**
  - **Solution :** Assurez-vous que les paramètres de la portée DHCP sont correctement configurés et que les options DHCP sont correctement définies.

- **Problème : Le serveur DHCP ne répond pas aux requêtes.**
  - **Solution :** Vérifiez que le service DHCP est en cours d'exécution et que les paramètres de pare-feu permettent le trafic DHCP.

## Conclusion

Vous avez maintenant configuré DHCP sur Windows Server. Vous pouvez commencer à gérer les adresses IP et les options DHCP selon vos besoins.

