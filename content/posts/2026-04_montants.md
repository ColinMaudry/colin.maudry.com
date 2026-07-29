+++
date = '2026-04-25T16:55:00+02:00'
draft = true
title = '2026 04_montants'
+++

# Les montants aberrants dans les DECP ma tentative pour y remédier

Depuis le début de mes travaux sur les Données Essentielles de la Commande Publique, j'ai un peu laissé de côté les analyses impliquant des agrégations de montants. Et oui, faire la somme des [marchés attribués](https://decp.info/acheteurs/26760192000015) par l'EHPAD Lefebvre-Blondel-Dubus à Gaillefontaine (Seine-Maritime,[carte](https://cartes.app/?allez=Gaillefontaine|r1920473|1.61541|49.65323#9.2/49.6039/1.7849)) et se retrouver avec le coût d'un programme spatial international, ça fait un peu bizarre. Et ce n'est pas un cas isolé.

Mais pourquoi ? Pourquoi des acheteurs, au moment de saisir le montant de l'attribution d'un marché de glaces et desserts surgelés décident de saisir un montant astronomique ? Avec un peu de chance j'aurai réussi à obtenir le témoignage de l'EHPAD en question pour la publication de cet article, mais je formule tout de même quelques hypothèses, non exclusives :

- l'acheteur ne sait pas vraiment à combien va s'élever ce marché, et la semantique indique "montant forfaitaire ou maximum estimé" (c'est dans l'article 1 de [l'arrêté](https://www.legifrance.gouv.fr/loda/id/LEGIARTI000046888863))
- dans la même veine, l'acheteur se dit que si il met trop peu et que finalement ça dépasse, ça va faire des problèmes
- l'acheteur se dit que de toute façon personne ne regardera cette donnée, alors on s'en fout un peu

C'est vrai qu'un marché c'est pas toujours facile à estimer, et quelque part on touche sans doute dans certains cas au manque de formation de certains acheteurs publics. Vaste sujet, et hors de mon champ de compétence. Mais même pour les fines fleurs de la 🏛️ Commande Publique 🏛️, l'intérêt de saisir les données essentielles n'est pas forcément évident. D'où l'intérêt de parler de decp.info autour de vous !

Résultat, decp.info ne propose pas de stats sur les montants de marchés publics, ce qui est fort dommage car je sais bien que c'est ce qui vous intéresse.

## Données officielles ou données modifiées ?

Restons sur notre exemple, un marché de desserts glacés pour un EHPAD qui s'élève à 12 milliards d'euros. Il va donc polluer les sommes, médianes et moyennes de tous les marchés de l'acheteur, de Seine-Maritime, de Normandie, de denrées alimentaires, etc.

Il y a trois approches : supprimer, ajuster ou laisser tel quel.

D'après le [code source](https://github.com/139bercy/decp-augmente/blob/0adf77f1081601fa83a3bffd28462946dd128839/nettoyage.py#L455-L500) de traitement des DECP publié par la DAJ de Bercy, ils ont clairement choisi leur camp. Pour la production de ses fameux rapports annuels (à confirmer auprès de la DAJ), tous les marchés de plus de 3 milliards d'euros sont supprimés. Plus de marché, plus de problème. Les marchés dont le montant comporte une suite de chiffres répétée (exemple : 999 999 988), et donc pouvant trahir une certaine approximation, subissent le même sort.

Cette approche a le bénéfice d'écarter certains marchés vraiment louches, et donc de produire des stats plausibles, où les ordres de grandeur sont respectés. Mais par la même occasion on invisibilise les autres données de marchés publics qu'on a pourtant sous la main, c'est franchement dommage. Et puis il y a peut-être des faux positifs.

Laisser tel quel, c'est que j'ai fait jusqu'à présent : pas de stats sur les montants, pas de problème. Mais on passe à côté d'infos dont la totalité des praticants de la commande publique est friande : prospection, sourcing, détection des atteintes à la probité, tous ces cas d'usage s'appuient sur les montants. Ça ne pouvait plus durer !

## Ma proposition

Il reste donc une troisième approche, ajuster les montants. L'idée générale est qu'un montant de marché publics est corrélé à certains facteurs, et qu'on peut donc comparer les marchés entre eux sur la base de ces facteurs et faire ressortir des marchés dont le montant est très loin des autres.

J'ai choisi de m'appuyer sur les facteurs suivants :

- durée du marché
- population (si c'est une commune)
- catégorie de l'entreprise titulaire (PME, entreprise intermédiaire, grande entreprise)
- catégorie de l'acheteur (commune, groupement de commune, État, région, etc.)
- technique d'achat (marché ou accord cadre)
- type d'achat (deux premiers chiffres du code CPV)
-
