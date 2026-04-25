+++
date = '2025-09-20T10:15:08+02:00'
draft = false
title = 'Sortie de decp.info v2 🎉'
tags = []
categories= []
+++

Après 6 mois de travail, je viens de mettre en ligne [decp.info v2](https://decp.info). Cet outil a pour objectif de démocratiser la compréhension des marchés publics grâce à la mise en valeur des données d'attribution. Le projet a consisté à rassembler les données disponibles, à les retraiter, puis à développer une interface claire et fonctionnelle. Sur ce dernier point, il y a encore fort à faire... et votre contribution est la bienvenue !

<!-- more -->

## Pourquoi decp.info ?

J'ai déjà écrit [un petit historique du projet](/posts/2025-09-19-petite-histoire-de-decp.info/). Dans cet article, je vais vous parler du résultat. decp.info est à la fois le nom de mon projet et l'adresse du site Web destiné aux usagers finaux.

Le projet : rassembler l'intégralité des données de [marchés publics](https://fr.wikipedia.org/wiki/March%C3%A9_public) français dans [un seul jeu de données](https://www.data.gouv.fr/datasets/donnees-essentielles-de-la-commande-publique-consolidees-format-tabulaire/), diffusé gratuitement et sans limite d'usage ([données ouvertes](https://fr.wikipedia.org/wiki/Donn%C3%A9es_ouvertes)). Ces données sont effet essentielles pour comprendre comment une part significative de l'argent public est dépensé (170 milliards d'euros en 2023, [voir page 4 du recensement](https://www.economie.gouv.fr/files/files/directions_services/daj/marches_publics/oecp/recensement/Chiffres_recensement_2023.pdf?v=1755762613)). Par leur richesse, elles donnent des détails importants sur les choix politiques et économiques des acheteurs publics : qui achète local ? Qui favorise les PME ? Combien coûte l'entretien des espaces verts, ou les cabinets de conseil ? Ce projet vise à mettre à disposition des outils [libres](https://fr.wikipedia.org/wiki/Logiciel_libre) et gratuits afin que chaque citoyen et citoyenne, entreprise, journaliste, chercheur et chercheuse, association, administration, puisse trouver les réponses à ces questions. Ces outils seront mis en ligne en libre accès sur le site [decp.info](https://decp.info).

Dans un monde idéal, cette tâche d'intérêt général serait financée par l'argent public et menée à bien par le Ministère des Finances. Malheureusement, même si le ministère [rassemble des données](https://www.data.gouv.fr/fr/datasets/donnees-essentielles-de-la-commande-publique-fichiers-consolides/), beaucoup de données manquent à l'appel (au moins les marchés publics de l'État, les plateformes éditées par Atexo, les profils d'acheteurs marchés-sécurisés, Klekoon et achatpublic.com).

## Fonctionnalités disponibles

### Le grand tableau

Tout d'abord, en [page d'accueil](https://decp.info), vous trouvez un grand tableau qui liste tous les marchés publics agrégés (1,3 million à l'écriture de cet article). En cliquant sur __Mode d'emploi__ vous afficherez les instructions pour filtrer et télécharger les données. Chaque colonne peut effectivement faire l'objet d'un filtre textuel ou numérique. Par exemple, taper "rennes" sous l'en-tête de colonne **acheteur_nom** puis taper Entrée filtrera tous les marchés publics dont le nom de l'acheteur contient le texte "rennes". Pour trouver un acheteur ou un titulaire, la recherche par SIRET ou SIREN (colonnes **acheteur_id** et **titulaire_id**) est beaucoup plus précise.

Après avoir appliquer quelques filtres, vous pouvez masquer certaines colonnes qui ne vous intéresse pas en cliquant sur le bouton **Colonnes affichées**, et décocher ces colonnes. Vous pouvez également trier les données en cliquant sur les petites flèches grises à gauche de chaque nom de colonne.

Enfin, vous avez la possibilité de télécharger au format Excel les données ainsi filtrées et triées en cliquant sur le bouton **Télécharger au format Excel**.

### Les statistiques

La deuxième partie du site Web est consacrée aux visualisations de données. Elle n'en affiche aujourd'hui que trois, mais cette partie va probablement évoluer assez rapidement en donnant la possibilité de configurer des filtres temporels (ex : une année) ou géographiques (ex : les données des marchés attribués en Bretagne)

## La suite

Ce ne sont pas les idées qui manquent pour exploiter ces données ! 

- échanger avec les plateformes dont les données de marchés publics ne sont pas encore publiées ou mal publiées (marches-publics.info, marches-securises.fr, klekoon.fr)
- page de zoom sur un acheteur/un fournisseur avec visualisations de données
- comptes utilisateur pour sauvegarder des filtres, recevoir des alertes lors de la publication de certains marchés
- ajouter les données des contrats de concessions
- ajouter de nouvelles colonnes :
  - commune, département, région des acheteurs/titulaires
  - distance en kilomètres entre acheteur et titulaire
  - population des acheteurs (commune, département, région)
  - rapprochement codes NAF fournisseurs et codes CPV des marchés publics pour faciliter la prospection
- ... et tout ce à quoi je n'ai pas encore pensé

Tout ceci ne peut cependant rester gratuit que si le projet est financé. Les contributions peuvent prendre plusieurs formes :
- financement de nouvelles fonctionnalités : je (via [ma société](https://annuaire-entreprises.data.gouv.fr/entreprise/colmo-989393350)) vous fais un devis, vous validez, vous me payez sur facture. Ces fonctionnalités sont alors développées en priorité
- contributions de code via des *pull requests* sur [les dépôts Github](https://decp.info/a-propos). J'ai déjà eu la chance de recevoir les contributions de [trois informaticiens de talent](https://github.com/ColinMaudry/decp-processing?tab=readme-ov-file#contributeurs-%EF%B8%8F).
- aide au déploiement : analyse des données pour repérer les manques ou les bugs, identification de nouvelles sources de données pertinentes, identification de financeurs potentiels, partage du projet dans vos réseaux
- achat de prestations de conseil et développement pour la publication de vos données de marchés publics ou l'exploitation des DECP (via [ma société](https://annuaire-entreprises.data.gouv.fr/entreprise/colmo-989393350))

Dans tous les cas votre participation sera mise en valeur via les différents canaux de communication.

[Parlons-en !](/pages/contact/)
