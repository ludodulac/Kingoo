# KINGOO

KINGOO est un jeu web d'observation et de concentration : le joueur doit retrouver le lion orange parmi un nombre croissant de lions.

## Principe

- 300 tableaux à difficulté progressive ;
- trois essais par partie ;
- un nouveau lion rejoint chaque tableau ;
- la taille et la disposition des lions évoluent avec la progression ;
- certains paliers introduisent des mouvements, clignotements, recouvrements et effets visuels/sonores ;
- des jalons de progression déclenchent des célébrations et repères visuels.

Le comportement réellement implémenté dans `index.html` reste la source technique de vérité.

## Structure actuelle

Le projet est volontairement simple et statique :

- `index.html` contient l'interface, les styles et la logique principale du jeu ;
- `assets/` contient les visuels utilisés par le jeu ;
- `.github/` contient l'automatisation éventuelle du dépôt ;
- `AI_START_HERE.md` est le point d'entrée obligatoire pour toute nouvelle conversation IA travaillant sur le projet.

Aucune étape de build n'est nécessaire pour exécuter le jeu dans sa forme actuelle.

## Développement assisté par IA

Avant toute modification importante, lire `AI_START_HERE.md` et suivre son protocole : inspection de l'état réel de `main`, préservation des mécaniques existantes, vérification des frontières de progression et indexation de l'état du projet avant passation.

Une nouvelle fonctionnalité doit être ajoutée sans supprimer silencieusement un comportement existant. Les changements touchant la progression doivent être vérifiés autour des seuils concernés, pas seulement sur un tableau isolé.

## Historique

Ce dépôt correspond désormais à KINGOO. Les anciennes références à Bibit ne décrivent plus le produit actuel et ne doivent pas guider les décisions techniques futures.
