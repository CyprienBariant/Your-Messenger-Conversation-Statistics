# Visualisez vos propres données

T’es-tu déjà posé certaines questions sur une de tes conversations Messenger ?

-	Combien **de messages et de réacts** ont été envoyés par chacun ?
-	Qui a reçu **le plus de réacts par message ?**
-	Qui **m’apprécie le plus ?** Qui **m’apprécie le moins ?**
-	Comment **maximiser le nombre de réacts** sur mes messages ?
-	Quel est le **réact le plus utilisé** ?
-	Combien de **messages, photos, gifs et réacts** ont été envoyés au total ?
-	Quel message détient le **record de réacts ?**
-	**Quand** est-ce que j’envoie **le plus de messages ?**

Ce dashboard répond à toutes ces questions, et bien d’autres !

**Vous trouverez un exemple de dashboard sur les fichier .pbix [ici](https://github.com/CyprienBariant/Your-Messenger-Conversation-Statistics/blob/main/French%20Version/FR%20-%20Stats%20de%20Votre%20Conversation%20Messenger.pbix).** Vous avez juste à télécharger Power BI Desktop gratuitement [ici](https://www.microsoft.com/fr-FR/download/details.aspx?id=58494) pour l’ouvrir.
 
![image](https://user-images.githubusercontent.com/104278342/200259291-3188e625-8296-48e7-b0c9-61369606ddba.png)
 
## Vous voudriez alimenter le dashboard de vos propres données à la place ?

À cause de problèmes de protection des données, Facebook a décidé de donner à l’utilisateur la possibilité de récupérer tout les informations qu’il souhaite sur lui-même. Ce fichier, incluant les données des conversations Messenger, est directement disponible depuis les paramètres du site Facebook ! Pourquoi pas prendre avantage de cette fonctionnalité ?

Avant de demander le fichier, **veuillez mettre en anglais ou en français la langue de Facebook.** Pour une meilleure qualité de restitution des données, changez le site en la langue que vous utilisez le moins dans la conversation que vous souhaiteriez analyser, entre le français et l’anglais. Cela sera utile car c’est grâce à la structure des phrases que le dashboard détermine si vous avez envoyé un message ou effectué une action – comme changé le surnom d’un participant ou bien rejoins un appel de groupe. Notez que seule la langue du site (Facebook.com) est prise en compte, pas celles des applications Facebook et Messenger.

Je vous donnerai le procédé étape par étape, en français et en anglais, pour récupérer les fichiers avec Facebook.

### Comment changer la langue sur Facebook

Depuis Facebook.com, connectez-vous puis cliquez sur « Compte (votre photo de profil en haut à droite) -> Paramètres et confidentialité -> Langue ». Vous aurez ensuite qu’à modifier la langue, soit en « English (US) » ou « English (UK) » pour l’anglais ou en « Français (France) ».
Vous pouvez aussi changer la langue de Facebook depuis un téléphone, mais vous devez vous rendre sur Facebook.com depuis votre navigateur et sélectionner « Version pour ordinateur ».

## Comment demander vos données

**Avec Facebook en français :** Cliquez sur « Compte (votre photo de profil en haut à droite) -> Paramètres et confidentialité -> Paramètres -> Vos informations Facebook -> Télécharger vos informations ». Sur la nouvelle fenêtre, cliquez sur "Demander un téléchargement" et sélectionnez votre profil Facebook. Allez dans "Sélectionner les types d'informations", sélectionnez seulement "Messages" (la troisième case) et appuyez sur "Suivant". Sélectionnez la période que vous souhaitez, changez le format sur "JSON" et la qualité du contenu multimédia sur "Faible" et appuyez sur « Envoyer la demande ».

**Avec Facebook en anglais :** Cliquez sur « *Account* (votre photo de profil en haut à droite) -> *Settings and privacy* -> *Settings* -> *Your Facebook information* -> *Download your information* ». Sur la nouvelle fenêtre, cliquez sur "*Request a download*" et sélectionnez votre profil Facebook. Allez dans "*Select types of information*", sélectionnez seulement "*Messages*" (la troisième case) et appuyez sur "*Next*". Sélectionnez la période que vous souhaitez dans "*Date range*", changez le format sur "JSON" et "*Media quality*" sur "*Low*" et appuyez sur « *Submit Request* ».

Il est aussi possible de demander les fichiers depuis votre téléphone, mais la langue des fichiers restera celle de Facebook.com :

#### Demandez vos données sur l’application Facebook depuis un Android

Rendez-vous dans le menu burger tout en haut à droite de l’application, puis cliquez sur l’icône de paramètres qui est aussi en haut à droite. Descendez jusqu’à la section « Vos informations » et allez dans « Télécharger vos informations ». Sur la nouvelle fenêtre, cliquez sur "Demander un téléchargement" et sélectionnez votre profil Facebook. Allez dans "Sélectionner les types d'informations", sélectionnez seulement "Messages" (la troisième case) et appuyez sur "Suivant". Changez le format sur "JSON" et la qualité du contenu multimédia sur "Faible", sélectionnez la période que vous souhaitez, et appuyez sur « Envoyer la demande ».

#### Demandez vos données sur l’application Facebook depuis un IPhone

Rendez-vous dans le menu (votre photo de profil tout en bas à droite de l’application), puis cliquez sur l’icône de paramètres en haut à droite. Allez dans « Paramètres du profil », puis descendez jusqu’à la section « Vos informations Facebook » et allez dans « Télécharger les informations du profil ». Appuyez sur « Tout désélectionner » et sélectionnez seulement « Messages » (la troisième case). Allez tout en bas de la page, sélectionnez la période que vous souhaitez dans « Période », le format JSON, la qualité des photos faible, puis appuyez sur « Créer un fichier ».

Facebook vous enverra généralement un mail sous deux jours pour vous informer que votre fichier et prêt.

## Comment charger vos données dans le dashboard

Une fois que vos fichiers sont prêts, **vous pouvez les télécharger** depuis les paramètres du site ou de l’application mobile. Il y aura sans doute plusieurs fichiers zip, mais seulement l’un d’entre eux contient tous les messages. Malheureusement, vous ne pouvez pas connaître en avance lequel des fichiers contient les messages, bien qu’ils soient le plus probablement dans les plus gros fichiers.
Pour atteindre les fichiers de messages, ouvrez un zip et allez dans le dossier « messages ». S’il contient des fichiers JSON tels que « autofill_information » ou « secret_groups », c’est que vous être sûrement dans le bon. **Allez dans « inbox » et choisissez le dossier de la conversation que vous souhaiteriez analyser.** S’il ne contient pas de fichiers JSON nommés « message_*x* », alors essayez de nouveau avec un autre fichier zip. Une fois que vous avez trouvé les fichiers « message_*x* », **copiez-les dans le dossier local de votre choix.**

**Ensuite, ouvrez le [fichier .pbix ci-joint](https://github.com/CyprienBariant/Your-Messenger-Conversation-Statistics/blob/main/FR%20-%20Stats%20de%20Votre%20Conversation%20Messenger.pbix).** Si besoin, téléchargez Power BI Desktop [ici](https://www.microsoft.com/fr-FR/download/details.aspx?id=58494) gratuitement. **Allez dans « Fichier -> Options et paramètres -> Paramètres de la source de données -> Changer la source… » et sélectionnez le dossier dans lequel vous venez juste d’insérer les fichiers de message.** Appuyez sur « Appliquer les modifications » sur la bannière qui apparaît.

Si une erreur survient au moment d’appuyer sur « Appliquer les modifications », cliquez sur le bouton « Transformez les données » situé au milieu du bandeau supérieur. Une nouvelle fenêtre s’ouvrira. En bas du panneau latéral gauche, cliquez successivement sur les cinq tables (messages, participants, aggregated, messages_words et group). Ensuite, cliquez sur « Fermer & appliquer » en haut à gauche de la fenêtre.

**Les données vont ensuite se charger dans le dashboard** et remplacer le modèle d’exemple. Comptez approximativement 2min pour 2 fichiers de message, 10min pour 4 fichiers de message et 45min pour 10 fichiers de message.

**Et voilà ! Vous avez accès aux statistiques de votre conversation.**

Dans le mode éditeur, **notez que vous devez CTRL + Clic** à la place de juste cliquer sur les boutons. Pour avoir une vue plus large du dashboard, vous pouvez cliquer sur la flèche pointant vers le haut située en haut à droite et sur la double flèche pointant vers la droite située en haut du panneau « Visualisations » ou « Champs ». La vue du dashboard s’agrandira pour s’ajuster à la page.

## Explorer les statistiques de votre conversation en mode présentation

Si vous préférez naviguer sur le dashboard dans le mode présentation, **Sélectionnez « Publier » sur la droite du bandeau supérieur** et entrez une adresse mail professionnelle ou scolaire. Si besoin, suivez le lien qui est apparu pour créer un compte. Ensuite, sélectionnez « Mon espace de travail » ou allez sur Power BI Service [ici](https://go.microsoft.com/fwlink/?LinkId=2183346&clcid=0x40c&cmpid=pbi-home-body-snn-signin) pour créer un autre espace de travail destiné à ce dashboard. Il se chargera dans Power BI Service très rapidement. 
Pour voir le dashboard en mode présentation, **allez sur [Power BI Service](https://go.microsoft.com/fwlink/?LinkId=2183346&clcid=0x40c&cmpid=pbi-home-body-snn-signin), puis dans « Mon espace de travail »** ou l’autre espace tout juste créé. Sur la droite du bandeau supérieur, l’icône rectangulaire vous permettra de voir le dashboard en plein écran.

#### Accéder au mode présentation sans compte professionnel ou scolaire

Si vous n’avez pas d’adresse mail Microsoft professionnelle ou scolaire, **vous pouvez essayez gratuitement Office 365 pour un mois [ici](https://www.microsoft.com/fr-fr/microsoft-365/enterprise/compare-office-365-plans?rtc=3).** Sélectionnez « Essayez gratuitement » en bas de « Office 365 E3 » et suivez les étapes indiquées. Pour être sûr de ne pas payer à la fin du mois d’essai, utilisez une carte à usage unique, disponible sur des applications comme Revolut. Sinon, immédiatement après la souscription, allez [ici](https://admin.microsoft.com/adminportal/home?#/subscriptions), cliquez sur les trois points et sélectionnez « Annuler l’abonnement ». Votre compte restera valide pendant 30 jours, et vous ne payerai rien.

Par la suite, vous aurez toujours la possibilité d’obtenir un autre essai gratuit avec le même numéro de téléphone, tant que vous utilisez une autre adresse mail.

## Partager les statistiques de votre conversation avec des amis

Quelque que soit votre compte, **vous avez la possibilité de commencer un essai gratuit de « Power BI Pro »**, qui permet de partager les dashboards avec d’autres utilisateurs Pro. Une solution plus facile pour partager les dashboards et d’**utiliser le même compte à plusieurs.** Sinon, vous pouvez directement **envoyer le .pbix à vos amis.** Si vous avez déjà chargé des données, les destinataires n’auront pas besoin de les charger à nouveau.

**Joyeuse exploration !**
