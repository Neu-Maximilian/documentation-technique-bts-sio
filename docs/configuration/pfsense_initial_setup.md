# Configuration initiale de pfSense

## Configuration des interfaces réseau

1. Après le premier démarrage, vous serez invité à configurer les interfaces réseau.
2. Assignez les interfaces réseau pour le WAN et le LAN. Par exemple :
    - WAN : em0
    - LAN : em1
3. Confirmez les interfaces assignées.

![Configuration des interfaces réseau](../images/pfsense/pfsense_interfaces.png)

## Configuration des adresses IP

1. Configurez l'adresse IP pour l'interface LAN. Par exemple :
    - Adresse IP : 192.168.100.254
    - Masque de sous-réseau : 24 (255.255.255.0)
2. Configurez l'adresse IP pour l'interface WAN selon votre configuration réseau.

![Configuration des adresses IP](../images/pfsense/pfsense_ip_config.png)

## Utilisation de l'assistant de configuration

1. Accédez à l'interface web de pfSense en entrant l'adresse IP de l'interface LAN dans un navigateur web (par exemple, http://192.168.100.1).
2. Connectez-vous avec les identifiants par défaut :
    - Nom d'utilisateur : admin
    - Mot de passe : pfsense
3. L'assistant de configuration se lancera automatiquement.
![Utilisation de l'assistant de configuration](../images/pfsense/pfsense_setup_wizard.png)

### Étape 0 : Reconnaissance du support

1. Lisez et reconnaissez les informations de support fournies par pfSense.
2. Cliquez sur "Next" pour continuer.

![Reconnaissance du support](../images/pfsense/pfsense_support_acknowledgement.png)

### Étape 1 : Informations générales

1. Configurez le nom d'hôte, le domaine et les serveurs DNS.
    - Nom d'hôte : RTE-STG01
    - Domaine : cci-campus.lan
    - Serveurs DNS : 8.8.8.8, 8.8.4.4 (ou ceux de votre choix)
2. Cliquez sur "Next" pour continuer.

![Informations générales](../images/pfsense/pfsense_general_info.png)

### Étape 2 : Configuration de l'heure

1. Configurez le fuseau horaire approprié pour votre région.
2. Cliquez sur "Next" pour continuer.

![Configuration de l'heure](../images/pfsense/pfsense_time_config.png)

### Étape 3 : Configuration du WAN

1. Configurez les paramètres de l'interface WAN selon votre fournisseur d'accès Internet.
2. Cliquez sur "Next" pour continuer.

![Configuration du WAN](../images/pfsense/pfsense_wan_config.png)

### Étape 4 : Configuration du LAN

1. Vérifiez les paramètres de l'interface LAN.
2. Cliquez sur "Next" pour continuer.

![Configuration du LAN](../images/pfsense/pfsense_lan_config.png)

### Étape 5 : Configuration du mot de passe administrateur

1. Changez le mot de passe administrateur par défaut pour des raisons de sécurité.
2. Cliquez sur "Next" pour continuer.

![Configuration du mot de passe administrateur](../images/pfsense/pfsense_admin_password.png)

### Étape 6 : Finalisation

1. Cliquez sur "Reload" pour appliquer les modifications et redémarrer pfSense.
2. L'assistant de configuration est maintenant terminé.

![Finalisation](../images/pfsense/pfsense_finish.png)

Votre pfSense est maintenant configuré et prêt à être utilisé.

## Note sur les configurations

Dans le cadre de ce projet, les configurations sont les suivantes pour le site de Strasbourg :

- **Nom d'hôte** : RTE-STG01
- **Domaine** : cci-campus.lan
- **Serveurs DNS** : 8.8.8.8, 8.8.4.4
- **Adresse IP LAN** : 192.168.100.254
- **Masque de sous-réseau LAN** : 24 (255.255.255.0)
- **Identifiants** :
      - Nom d'utilisateur : admin
      - Mot de passe : P@ssword10

Et pour le site de Mulhouse :

- **Nom d'hôte** : RTE-MUL01
- **Domaine** : cci-campus.lan
- **Serveurs DNS** : 8.8.8.8, 8.8.4.4
- **Adresse IP LAN** : 192.168.200.254
- **Masque de sous-réseau LAN** : 24 (255.255.255.0)
- **Identifiants** :
      - Nom d'utilisateur : admin
      - Mot de passe : P@ssword10

Assurez-vous de remplacer ces valeurs par celles qui sont appropriées pour votre environnement spécifique si nécessaire.
