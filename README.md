# Exercice 02

## Objectifs
- Utiliser les branches
- Utiliser les commandes de reset et checkout
- Utiliser la remise
- Utiliser le reflog
- Utiliser les différents modes de fusions

## Procédure
- Cloner le dépôt distant vers un dossier local "Exercice02"
- Visualiser toutes les branches avec la commande *log* et ses paramètres
- Fusionner la branche hotfix01 avec la branche master et vérifier avec *log*
- Annuler la fusion en mode fast-forward
- Refaire cette fusion en mode "no fast-forward" pour que l'historique affiche bien un décrochement, en mettant comme commentaire "Prise en compte du HotFix1"
- Vérifier avec *log*
- Créer une branche "feature4" depuis master
- Basculer sur cette branche
- Supprimer le fichier "EditionPaie.p" avec un *rm*
- Annuler la suppression
- Modifier le fichier "EditionPaie.p" en ajoutant après la ligne de commentaire du 18/09/2018 : "/* 19/09/2018 : Fonctionnalité 4 */"
- Modifier le fichier "EditionPaie.p" en corrigeant la date du 10/09/2018 par le 11/09/2018
- Faire un *diff* pour voir les différences
- Commiter cette modification avec comme libellé "Fonctionnalité 4"
- Supprimer la branche "feature4" en forçant la suppression
- Visualiser les branches restantes
- Annuler la suppression de la branche (feature4 doit pointer sur le dernier commit) et repositionner la branche master sur le commit précécent
- Basculer sur la branche feature4
- Modifier le fichier "EditionPaie.p" en ajoutant après la ligne de commentaire du 19/09/2018 : "/* 19/09/2018 : Autre Fonctionnalité 4 */" et sauvegarder
- Basculer sur master
- Utiliser la remise pour pouvoir basculer sur master
- Revenir sur la branche feature4
- Récupérer le contenu de la remise
- Ajouter et commiter cette modification avec ce libellé : "Nouvelle fonctionnalité 4"
- Visualiser la différence entre la branche feature2 et la branche feature4
- Fusionner feature4 dans master (en fast-forward : donc sans décrochement dans le graphe)
- Fusionner feature2 dans master (en fast-forward : donc sans décrochement dans le graphe) et résoudre le conflit (voir le fichier à obtenir ci-dessous)

## Contenu du fichier fusionné

```javascript
/* Programme d'édition de la paie */

/* Version mise en production le 15/09/2018 */
/* 11/09/2018 : Fonctionnalité 1 créée par ElMagnifico */
/* 16/09/2018 : Fonctionnalité 2 créée par ElMagnifico */
/* 18/09/2018 : Correctif urgent de production par ElMagnifico */
/* 19/09/2018 : Fonctionnalité 4 */
/* 19/09/2018 : Autre Fonctionnalité 4 */

/* Ajout correctif */
RUN pi_charge_tous_les_agents.

RUN pi_imprime_en_texte.

/* F2 */
RUN pi_charge_paie.
```

## Solution 
Dans le fichier "soluce.txt"
