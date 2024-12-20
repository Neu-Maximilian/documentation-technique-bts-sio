# Installation et Configuration d'un Client Windows pour Rejoindre un Domaine

## Prérequis

Avant de commencer, assurez-vous d'avoir les éléments suivants :
- Un ordinateur avec une version compatible de Windows installée
- Une connexion réseau fonctionnelle
- Les informations d'identification pour rejoindre le domaine (nom de domaine, nom d'utilisateur, et mot de passe)

## Étapes d'installation et de configuration initiale

### 1. Installation de Windows

1. Démarrez le système à partir d'un support d'installation de Windows.
2. Sélectionnez la langue, le format de l'heure et du clavier, puis cliquez sur "Suivant".

![Sélection de la langue](../images/windows-client/client_windows_install_selection_langue.png)

3. Cliquez sur "Installer maintenant" pour lancer l'installation.

![Installer maintenant](../images/windows-client/client_windows_install_install_now.png)

4. Entrez la clé de licence si demandée, puis cliquez sur "Suivant".

![Clé de licence](../images/windows-client/client_windows_install_cle_licence.png)

5. Choisissez l'édition de Windows à installer et acceptez les termes du contrat de licence.

![Choix de l'édition](../images/windows-client/client_windows_install_edition.png)
![Acceptation du contrat](../images/windows-client/client_windows_install_cgu.png)

6. Sélectionnez le type d'installation. Choisissez "Personnalisé" pour effectuer une installation propre.

![Type d'installation](../images/windows-client/client_windows_install_type_install.png)

7. Choisissez la partition où installer Windows, puis cliquez sur "Suivant".

![Sélection de la partition](../images/windows-client/client_windows_install_selection_partition.png)

8. L'installation commence. Attendez que le système redémarre automatiquement.

![Installation en cours](../images/windows-client/client_windows_install_instalation.png)

9. Une fois l'installation terminée, le système redémarre sur l'écran de configuration initiale.

![Fin de l'installation](../images/windows-client/client_windows_install_fin_boot.png)

### 2. Configuration initiale de Windows

1. Sélectionnez la langue et la disposition du clavier.

![Sélection de la langue](../images/windows-client/client_windows_initial_setup_lang.png)
![Disposition du clavier](../images/windows-client/client_windows_initial_setup_keyboard.png)

2. Ajoutez un second clavier si nécessaire, ou cliquez sur "Ignorer".

![Second clavier](../images/windows-client/client_windows_initial_setup_2nd_keyboard.png)

3. Connectez-vous à Internet pour que Windows puisse appliquer les mises à jour.

![Connexion à Internet](../images/windows-client/client_windows_initial_setup_internet.png)
![Connexion Internet établie](../images/windows-client/client_windows_initial_setup_internet_2.png)

4. Créez un compte utilisateur principal. Entrez un nom d'utilisateur et un mot de passe.

![Nom d'utilisateur](../images/windows-client/client_windows_initial_setup_main_user.png)
![Mot de passe](../images/windows-client/client_windows_initial_setup_main_user_pass.png)

5. Configurez les questions de sécurité pour la récupération du mot de passe.

![Questions de sécurité](../images/windows-client/client_windows_initial_setup_security_question.png)

6. Décidez si vous souhaitez activer Cortana et configurez les paramètres de confidentialité selon vos préférences.

![Configuration de Cortana](../images/windows-client/client_windows_initial_setup_cortana.png)

7. Attendez que Windows applique les paramètres. Vous arriverez ensuite sur le bureau.

![Premier démarrage](../images/windows-client/client_windows_initial_setup_first_login.png)

## Rejoindre un Domaine

### 1. Accéder aux Paramètres de Domaine

1. Ouvrez les "Paramètres" en cliquant sur le menu Démarrer, puis allez dans **Système** > **Informations**.
2. Sous la section "Paramètres de nom de l’ordinateur, de domaine et de groupe de travail", cliquez sur **Modifier les paramètres**.

### 2. Configuration du Domaine

1. Dans la fenêtre "Propriétés système", cliquez sur le bouton **Modifier**.
2. Dans la section "Membre de", sélectionnez **Domaine** et entrez le nom du domaine.
3. Cliquez sur **OK**.

### 3. Authentification et Finalisation

1. Entrez les informations d'identification d'un compte autorisé à joindre des machines au domaine.
2. Redémarrez l'ordinateur lorsque vous y êtes invité.
3. Une fois redémarré, connectez-vous avec un compte utilisateur du domaine.

## Conclusion

Votre client Windows est maintenant configuré et connecté au domaine. Vous pouvez désormais gérer les paramètres du système et accéder aux ressources du réseau selon les autorisations configurées.

