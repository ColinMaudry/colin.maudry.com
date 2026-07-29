+++
date = '2026-07-29T20:17:43+02:00'
draft = false
title = 'decp.info devient colibre, et ça change tout'
+++

Je viens de mettre en ligne la troisième version majeure de ma suite d'outils d'exploration des marchés publics.

- la v1 était une preuve de concept
- la v2, mise en production en septembre 2025, a multiplié le nombre d'outils et a fait connaître le projet

Pour marquer le bond de maturité dans le projet, cette v3 s'accompagne d'un renommage, decp.info devient [**colibre**](https://colibre.fr). Plus facile à retenir, ce nouveau nom incarne l'ouverture du projet (code libre, données en [Open Data](https://colibre.fr/a-propos/donnees), projet collaboratif) et ouvre aussi la porte au traitement d'autres données que les Données Essentielles de la Commande Publique (BOAMP, Approch, etc.).

[colibre](https://colibre.fr) professionnalise davantage la solution avec une interface un peu plus travaillée (il reste du boulot !), de meilleures performances, et voit surtout l'arrivée des abonnements, déterminants pour la pérennité de ce fragile projet. Mais c'est plus compliqué que ça. Rentrons dans les détails, et je vous parlerai des nouvelles fonctionnalités et de la vision dans un second article.

![Bannière colibre](/images/og-image.png)

## Un abonnement mensuel à 20 euros HT

Tout d'abord une précision : seules les fonctionnalités les plus avancées exigent un abonnement. À part le partage de vues sur les données, **toutes les fonctionnalités présentes dans decp.info restent gratuites dans colibre**.

Au départ, mon objectif était de laisser decp.info complètement gratuit. D'un côté je proposais un outil utile au plus grand nombre pour démocratiser l'accès à la commande publique, d'un autre je proposais des prestations de conseil et de développement autour du sujet des données de la commande publique, comme je le fais depuis 2016. decp.info me servait alors de produit d'appel, démontrant ma très bonne connaissance des données et des techniques de traitement et de visualisation des données. Avec decp.info, je souhaitais davantage construire une communauté et un [commun numérique](https://fr.wikipedia.org/wiki/Commun_num%C3%A9rique) qu'une clientèle.

Malheureusement, la mayonnaise n'a pas pris. J'ai eu de très bons contacts, mais me diviser entre le développement de decp.info et le développement commercial de mes prestations faisait qu'aucune des deux activités ne décollait vraiment. La fin des aides au développement étasuniennes décidée peu après l'élection de Donald Trump a également mis un point final à mes missions de conseil à l'étranger avec l'[Open Contracting Partnership](https://open-contracting.org), qui représentaient l'essentiel de mes revenus depuis 2024.

Depuis quelques mois, les retours que je recevais des utilisateurs racontaient le rôle important que prenait decp.info dans leur pratique de la commande publique, en particulier pour la veille et le reporting. decp.info apportait de la valeur, et certain·es étaient très supris·es que je propose gratuitement un tel outil. D'autres pensaient que c'était naturel... puisqu'il s'agissait selon eux d'un outil officiel, financé par des fonds publics (j'aurais bien aimé !).

Voilà pourquoi pendant deux mois vous n'avez pas vu beaucoup d'évolutions sur decp.info : [colibre](https://colibre.fr) déployait peu à peu ses ailes.

20 euros. C'est rond, c'est simple, d'après ma courte étude de marché ce n'est pas cher compte tenu des fonctionnalités proposées. D'autant plus que de nombreuses autres [arrivent](https://colibre.fr/a-propos/roadmap). Si cet abonnement ne fonctionne pas, je devrai mettre en pause le développement et me chercher un "vrai" travail.

## Une API pour alimenter vos applications

J'ai également mis en ligne une API JSON riche, accessible via un abonnement spécifique. La documentation technique est [ici](https://colibre.fr/api/v1/swagger). Si cela vous intéresse pour alimenter vos applicatiosn en direct avec des données de qualité, [contactez-moi](https://colibre.fr/a-propos/contact).

## Concevoir avec vous

J'ai accompagné beaucoup de projets de gestion de données des marchés publics, et je sais écouter et traduire les irritants, les besoins, en une solution technique cohérente. C'est pour ces raisons que [colibre](https://colibre.fr) se veut collaboratif : 

- les abonné·es [votent](https://colibre.fr/a-propos/roadmap) pour les prochaines fonctionnalités
- interface de chat 💬 intégrée au site Web pour échanger avec moi quand je suis en ligne (en bas à droite)
- webinaires réguliers pour échanger avec vous (en cours de programmation)
- [lettre d'information](https://6254d9a3.sibforms.com/serve/MUIFAEonUVkoSVrdgey18CTgLyI16xw4yeu-M-YOUzhWE_AgfQfbgkyT7GvA_RYLro9MfuRqkzQxSvu7-uzbMSv2a2ZQPsliM7wtiiqIL8kR2zOvl6m11fb5qjcOxMAYsLiY_YBi3P7NY95CTJ8vRY4CpsDclF2iLooOElKkTgIgi5nePe7zAIrgiYM5v2EuALlGJZMEG9vBP-Cu)

Plus généralement, je trouve mon métier beaucoup plus agréable quand il consiste à construire un outil utile avec les personnes concernées.

## Au-delà de colibre

Les abonnements, nos échanges, tout ceci dépasse la conception d'un outil. Si on prend du recul, et ayant pu comparer avec comment elle est pratiquée à l'étranger, la commande publique française mérite mieux que ce qu'elle est aujourd'hui. La généralisation de la dématérialisation nous a promis la fin de la ressaisie, l'accessibilité des PME à la commande publique, des statistiques enfin fiables, un pilotage fin de la politique d'achat... Presque 10 ans après l'entrée en vigueur de l'obligation de publication des DECP, malgré les annonces, la promesse n'est pas tenue.

Tout ça pour dire que vos abonnements financent également le temps que je passe à 

- analyser la réglementation et les choix techniques faits par le Ministère des Finances et la Commission européenne dans le domaine de la publication de données
- formuler des contre-propositions
- contacter les acheteurs publics lorsque leurs données comportent des anomalies

De nombreuses personnes et organismes poussent dans la même direction :

- des parlementaires comme Simon Uzenat et Dany Wattebled avec [leur commission d'enquête sénatoriale](https://www.senat.fr/travaux-parlementaires/structures-temporaires/commissions-denquete/commission-denquete-sur-les-couts-et-les-modalites-effectifs-de-la-commande-publique-et-la-mesure-de-leur-effet-dentrainement-sur-leconomie-francaise.html)
- des acheteuses comme Magali Chamla-Pernin avec son site [magaliparlemarches.fr](https://magaliparlemarches.fr/), ainsi que les autres membres de l'Association des Acheteurs Publics
- des entrepreneurs comme Victor Lavolé (Temi), Blaise Malta-Bey, Nicolas Valoo (M2BPO), Jessica Poles (Timao), Tanguy Le Hir (Deadline), Alan Bourhis (PublikConnect) et Samuel Goëta (Datactivist)
- des lobbyistes comme Kévin Gernier (Transparency International France) avec [Integrity Watch](https://www.integritywatch.fr/), Emma Taillefer (Anticor) et Karolis Granickas (Open Contracting Partnership)
- et des chercheurs comme Pierre-Henri Morand et Adrien Deschamps (Université d'Avignon)

Merci à eux.

Prochain article : un point sur les nouvelles fonctionnalités et la vision pour les semaines à venir.
