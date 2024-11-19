# Utiliser l'aide de Nexthink Assist

Nexthink Assist est le point d'entrée unifié de la gestion de l'expérience des employés numériques sur l'ensemble de la plate-forme Infinity. Intégrée directement dans la navigation de recherche, Nexthink Assist utilise les derniers grands modèles de langues d'OpenAI et Anthropic pour aider les équipes informatiques à voir, diagnostiquer et corriger instantanément les défis DEX grâce à la puissance de l'IA générative. En particulier, Nexthink Assist permet aux utilisateurs d'effectuer des recherches contextuelles dans la documentation des produits, extraire des données sur les performances de l'appareil, les sessions utilisateur et les applications, et créer rapidement des campagnes Nexthink en utilisant des requêtes de langage naturel.

<figure><img src="../../.gitbook/assets/AboutAssist.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
L'Assistance Nexthink est actuellement en **bêta** et s'améliore constamment. Au fur et à mesure de son évolution, il peut occasionnellement fournir des renseignements qui nécessitent une vérification. Ensuite, nous vous recommandons de confirmer vos résultats pour vous assurer de l'exactitude lors de l'utilisation de l'aide Nexthink Assist.
{% endhint %}

## Commencer avec l'aide de Nexthink Assist <a href="#how-to-get-started-with-assist" id="how-to-get-started-with-assist"></a>

Tout d'abord, assurez-vous que votre rôle vous permet de voir l'aide de Nexthink **.** Reportez-vous à la section [Permissions](./#permissions) pour plus d'informations.&#x20

Pour accéder à Nexthink Assist, sélectionnez **Nexthink** **Assister** dans le menu principal.

<figure><img src="../../.gitbook/assets/Assist - 1721048792.png" alt=""><figcaption></figcaption></figure>

La fenêtre Nexthink Assist s'affiche, vous permettant de taper votre texte dans la barre de recherche. Utilisez les options suivantes pour obtenir les informations dont vous avez besoin :

- **Recherche**: Tapez le texte dans la barre de recherche **sans appuyer sur Entrée** pour effectuer des recherches à travers différents paramètres. Consultez la documentation [Utilisation de Search](https://docs.nexthink.com/platform/user-guide/search-and-nexthink-assist/using-search) pour plus d'informations.&#x20
- **Assistance** : Tapez du texte dans la barre de recherche et **appuyez sur Entrée** pour créer des enquêtes et des campagnes, ou pour obtenir des réponses relatives à Nexthink Infinity.

<figure><img src="../../.gitbook/assets/Assist - 1721114015.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Tapez au moins **3 mots** et appuyez sur la touche **Entrée** pour activer **l'assistance**. Pour continuer à utiliser **Search** en mode standard, tapez le nom d'un binaire, d'un périphérique ou d'un paquet.
{% endhint %}

Utilisez Nexthink Assist pour simplifier les enquêtes de construction, simplifier la création de campagnes et répondre à vos questions sur Nexthink Infinity.

- **Demandez à propos de Nexthink**: L'assistance active la recherche contextuelle dans la documentation des produits pour vous permettre de démarrer rapidement, avec les informations et le contexte dont vous avez besoin.
- **Données de requête** : L'assistance vous aide à extraire des données et à trouver rapidement des réponses sur les performances de la console, , les données des utilisateurs et des sessions, les informations des applications et bien plus encore pour résoudre les problèmes de manière proactive.
- **Créer**: L'aide vous aide à créer des campagnes Nexthink et rend la création de campagnes instantanée. Composez une demande rapide en langage naturel, et regardez Nexthink faire le reste.

En plus de ses trois principales capacités, Assistez à répondre à vos questions sur tous les objets de configuration Nexthink Infinity disponibles dans votre environnement. Utilisez Aide pour obtenir des réponses sur les tableaux de bord, les moniteurs, les packs de bibliothèques, et plus encore.

<figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

Une fois que vous avez envoyé votre question à Assist, elle génère et exécute une requête NQL, crée une campagne ou fournit une réponse à partir de la documentation.&#x20

Posez des questions de suivi sur le même sujet pour maintenir la conversation en cours. Pour démarrer une conversation à partir de zéro, cliquez sur le bouton de réinitialisation dans le coin supérieur droit de la fenêtre d'assistance Nexthink Assist.&#x20

<figure><img src="../../.gitbook/assets/Assist - 1723097609.png" alt=""><figcaption></figcaption></figure>

Imaginez que vous travailliez pour une entreprise avec un département commercial à Boston. Ce service s'est plaint de problèmes avec la qualité des appels MS Teams. Vous décidez d'enquêter sur ce problème en utilisant Nexthink Assist. Les sections de documentation suivantes fournissent des directives sur l'utilisation de Nexthink Assist avec des exemples liés à ce cas d'utilisation.

## Interroger les données avec l'aide

Pour identifier la cause du problème de qualité des appels MS Teams, demander à l'aide de _afficher la force moyenne du signal Wi-Fi par ville américaine triée par ordre croissant_ et **appuyez sur Entrée**. La requête que crée Assist révèle immédiatement que le bureau de Boston a la pire force de signal Wi-Fi.

<figure><img src="../../.gitbook/assets/Assist - 1723097426.png" alt=""><figcaption></figcaption></figure>

Poursuivez la conversation avec Assist dans la même fenêtre et demandez une _liste d'employés du service commercial à Boston_. Ensuite, cliquez sur **Voir dans les Enquêtes** pour accéder au module **Enquêtes** et obtenir la liste complète. Reportez-vous à la documentation [Éditeur Visuel](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/visual-editor) et à [Éditeur NQL](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/nql-editor) pour plus d'informations sur Investigations.

<figure><img src="../../.gitbook/assets/Assist - 1723097541.png" alt=""><figcaption></figcaption></figure>

### **Données hors portée de l'assistance**

[Modèle de données NQL Nexthink ](../nexthink-query-language-nql/nql-data-model.md) fournit un aperçu des données collectées par Nexthink . L'assistance prend actuellement en charge la plupart du modèle de données NQL, **exclut** les champs personnalisés et la liste des champs ci-dessous\*\*:\*\*

| Espace de noms                         | Tables non prises en charge                                                                                            |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| application                            | réseau\_application                                                                              |
| Alerte                                 | impact                                                                                                                 |
| Appareil                               | appareil/local\_admins                                                                           |
| action\_distante | exécution\_résumé                                                                                |
| Service                                | Tous                                                                                                                   |
| logiciel\_mesure | Tous                                                                                                                   |
| connexion                              | <p>udp_event<br>tcp_event</p>                                                                                          |
| session                                | <p>connectez<br>déconnectez<br>lifecycle_event<br>verrouillez<br>déconnectez<br>déverrouiller</p>                      |
| web                                    | <p>error_summary<br>event_summary<br>transaction_summary<br>page_view_summary<br>page_view/detailed_page_load_time</p> |
| flux de travail                        | exécution\_résumé                                                                                |

{% hint style="info" %}
Le temps de réponse de l'aide peut varier, et il arrive que certaines requêtes générées par l'aide ne s'affichent pas correctement dans [l'éditeur visuel](https://docs.nexthink.com/platform/user-guide/investigations/creating-investigations/visual-editor).
{% endhint %}

## Créer des campagnes avec l'aide

Une fois que vous avez identifié le problème de la puissance du signal Wi-Fi dans le bureau de Boston, la prochaine étape consiste à informer tous les employés concernés par une campagne Nexthink . #x20

Utilisez Aide pour _créer une campagne pour informer les employés que le bureau de Boston a des problèmes de Wi-Fi._ L'assistance crée cette campagne – questions et réponses – selon vos instructions.

<figure><img src="../../.gitbook/assets/Assist - 1723097717.png" alt=""><figcaption></figcaption></figure>

Si vous souhaitez améliorer votre campagne, tapez des commandes supplémentaires dans la barre de recherche pour fournir des conseils supplémentaires. &#x20

<figure><img src="../../.gitbook/assets/Assist - 1723196848.png" alt=""><figcaption></figcaption></figure>

Si vous êtes satisfait de la campagne suggérée, tapez simplement **Oui** dans la barre de recherche pour l'enregistrer comme brouillon dans le module **Campagnes** et définissez les utilisateurs ciblés et le mécanisme de déclenchement. Reportez-vous à la documentation [Créer des campagnes](https://docs.nexthink.com/platform/user-guide/campaigns/creating-campaigns) pour plus d'informations sur la façon de finaliser un brouillon de campagne et de le distribuer entre les publics sélectionnés.&#x20

### Les types de campagnes d'aide peuvent créer <a href="#what-type-of-questions-can-assist-answer" id="what-type-of-questions-can-assist-answer"></a>

L'assistance peut vous aider à compléter la section de contenu de n'importe quelle [campagne Nexthin](https://docs.nexthink.com/platform/user-guide/campaigns/creating-campaigns/types-of-campaigns). Exemples:

- _Créer une enquête d'utilisation de l'appareil _
- _Créez une campagne pour informer les utilisateurs des problèmes de connexion Wi-Fi en cours dans notre bureau_
- _Créer une enquête de satisfaction informatique_

Reportez-vous à la documentation sur les [campagnes engageantes](https://docs.nexthink.com/platform/user-guide/campaigns/getting-started-with-campaigns/conducting-engageing-campaigns) pour plus d'informations sur la création de campagnes efficaces.&#x20

## Demander de l'aide à propos du Nexthink Infinity

Les problèmes de connexion Wi-Fi sont très fréquents et peuvent se reproduire. Utilisez l'un des moniteurs disponibles dans la bibliothèque Nexthink pour surveiller efficacement les problèmes de Wi-Fi et prendre des mesures pour résoudre le problème. Demander une aide pour activer le moniteur dans le module Alertes.&#x20

<figure><img src="../../.gitbook/assets/Assist - 1723204902.png" alt=""><figcaption></figcaption></figure>

L'assistance utilise les ressources de la documentation Nexthink Infinity pour fournir la meilleure réponse. Pour de plus amples informations ou instructions, reportez-vous aux pages de documentation pertinentes et aux formations liées par Assist en bas de sa réponse.

### Les types de questions peuvent répondre à <a href="#what-type-of-questions-can-assist-answer" id="what-type-of-questions-can-assist-answer"></a>

Aidez à répondre à vos questions en utilisant la documentation Nexthink Infinity, qui inclut les sources de documentation en produit et en ligne.&#x20

Exemples de questions:

- _Comment configurer un webhook ?_
- _Quelle est la différence entre les navigations dures et douces ?_&#x20
- _Quelle est la limite des campagnes que je peux créer dans Expérience en milieu de travail ?_&#x20

## Foire aux questions <a href="#title-text" id="title-text"></a>

<details>

<summary>I'm getting unexpected answers from Assist. Que puis-je faire?</summary>

Il se peut que la réponse à votre question soit basée sur un sujet que Nexthink Assist ne supporte pas. Reportez-vous à la section [Quel type d'enquêtes peut aider à créer ?](using-nexthink-assist.md#what-type-of-investigations-can-assist-create) pour plus de détails.

L'assistance utilise le langage naturel pour répondre à vos questions. Parfois, vous pouvez constater que l'Assistance ne peut pas répondre à votre question ou que la réponse est incorrecte. Voici quelques recommandations sur la meilleure façon de formuler vos questions :

- **Soyez clair et précis** : fournissez des informations claires sur le problème que vous étudiez. Évitez les questions vagues ou ambiguës qui peuvent conduire à des résultats inexacts.
- **Utilisez des mots-clés ciblés** : Utilisez des mots-clés pertinents liés au problème que vous essayez de résoudre dans la mesure du possible. Cela aide à comprendre le contexte et à fournir des réponses plus précises.
- **Encadrez vos questions** : Structurez vos instructions sous forme de questions ou de commandes spécifiques. Par exemple, au lieu de taper des erreurs _Find dans Teams_, essayez _Combien d'appels d'équipes ont eu une mauvaise qualité au cours des dernières 24 heures ?_
- **Expérimentation et itération** : Si vous ne obtenez pas les résultats souhaités initialement, n'hésitez pas à affiner vos demandes. Aider à apprendre et à s'améliorer au fil du temps, donc expérimenter avec des expressions différentes peut vous aider à obtenir de meilleurs résultats.

Pour plus d'informations sur l'écriture efficace des prompts, complétez le cours en ligne [_Comment accélérer le travail avec Nexthink Assist_](https://learn.nexthink.com/courses/how-to-fast-track-work-with-nexthink-assist) disponible sur Nexthink Learn.

</details>

<details>

<summary>How can I share feedback on Assist with the Nexthink team?</summary>

Aidez-nous à améliorer Aide en partageant vos commentaires en utilisant les icônes pouce-haut et pouce-bas situées dans le coin inférieur droit de la dernière réponse d'Assist.

<summary>As Nexthink admin, can I pilot the usage of Assist before exposing it to a broader user group?</summary>

Oui, les administrateurs de Nexthink peuvent piloter l'utilisation de l'aide en désactivant sélectivement et en activant les autorisations d'assistance de certains rôles.&#x20

</details>

<details>

<summary>Does Assist apply View-domain constraints and permissions?</summary>

Oui, le domaine View s'applique à l'assistance. Par exemple, les utilisateurs de Nexthink interrogeant des données avec Assist obtiennent les mêmes résultats que l'exécution de la requête dans NQL ou dans l'éditeur Visuel.&#x20

Ensuite, impose également des autorisations avant d'exécuter une tâche. Par exemple, pour voir et utiliser la fonctionnalité **Créer** des campagnes dans Nexthink Assist, assurez-vous que votre rôle a la permission de _modifier les campagnes_. Sans cette autorisation, vous ne pouvez pas créer de campagnes et vous recevrez le message d'erreur suivant : _Vous n'avez pas les droits suffisants pour effectuer cette action. Veuillez contacter votre administrateur._&#x20

</details>

<details>

<summary>Is Nexthink Assist an add-on product? Nécessite une licence supplémentaire?</summary>

Nexthink Assist est une fonctionnalité Infinity, qui fait partie du produit de base de Workplace Experience et est disponible sans frais supplémentaires.

</details>
