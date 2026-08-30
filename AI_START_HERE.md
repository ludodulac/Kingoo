# AI START HERE — KINGOO

Point d’entrée obligatoire pour tout agent IA reprenant KINGOO. Le dépôt est actuellement compact ; cette discipline évite qu’une future évolution transforme un prototype fonctionnel en accumulation de modifications non indexées.

## 1. Démarrage obligatoire

Avant toute modification :
1. vérifier l’état réel de `main` et les changements/issues/PR pertinents ;
2. lire `README.md`, mais ne pas lui faire confiance aveuglément s’il ne décrit plus le produit réel ;
3. inspecter entièrement `index.html`, qui contient actuellement l’essentiel de l’interface, des styles et de la logique ;
4. inspecter `assets/` et `.github/` si la tâche les concerne ;
5. rechercher si le comportement demandé existe déjà avant d’ajouter une seconde implémentation.

Important : le README actuel est manifestement insuffisant par rapport au jeu présent dans `index.html`. Le code réel est donc la source de vérité immédiate tant que la documentation produit n’a pas été remise à niveau.

## 2. Produit actuellement observable

KINGOO est actuellement un jeu web centré sur la recherche du lion orange parmi des lions visuellement proches. La difficulté progresse jusqu’à 300 tableaux, avec trois vies, objectifs intermédiaires et effets/variations de difficulté (mouvement, clignotement, recouvrement et événements visuels/sonores selon les niveaux).

Ne pas figer cette description comme vision produit définitive : si une documentation produit plus autoritative est créée, ce fichier devra pointer vers elle.

## 3. Architecture actuelle

- `index.html` — application monofichier : structure HTML, CSS et logique JavaScript principale.
- `assets/` — ressources visuelles.
- `.github/` — automatisation/déploiement éventuels à vérifier selon la tâche.
- `README.md` — actuellement trop ancien/incomplet pour servir seul de référence.

Une modularisation future peut être pertinente si la taille continue d’augmenter, mais ne doit pas être introduite au milieu d’une tâche sans besoin réel ni validation du comportement existant.

## 4. Protection de l’existant

- Ajouter/étendre avant de remplacer ou supprimer.
- Avant toute suppression, vérifier si la demande exige réellement un retrait.
- Préserver la progression, les vies, le ciblage du lion orange, les jalons et les comportements de difficulté sauf demande explicite.
- Ne pas simplifier une mécanique existante pour rendre une nouvelle fonctionnalité plus facile à coder.
- Séparer autant que possible correction fonctionnelle et refactoring structurel.
- Ne pas modifier les assets ou effets non concernés par une demande simplement pour uniformiser le code.

## 5. Validation

Après modification, tester les chemins concernés et plusieurs frontières de progression, notamment démarrage/rejouer/perdre/gagner, clic correct/incorrect, changement de tableau, vies, objectifs/jalons, mouvement, clignotement, recouvrement, audio/effets, redimensionnement/mobile. Pour toute logique dépendante d’un intervalle de niveaux, tester les niveaux juste avant, au début, à la fin et juste après l’intervalle.

## 6. Indexation et évolution documentaire

Le premier besoin documentaire de KINGOO est de réduire l’écart entre README et produit réel. Toute future tranche substantielle doit :
- maintenir une description produit correcte ;
- documenter les règles de progression durables ;
- tracer les décisions structurelles si le monofichier est un jour découpé ;
- éviter que les seules explications d’une mécanique vivent dans une conversation.

## 7. Protocole obligatoire avant passation

1. vérifier l’état réel de `main` ;
2. inventorier comportements, niveaux/plages et fichiers touchés ;
3. documenter toute nouvelle mécanique durable ;
4. vérifier les frontières de niveaux concernées ;
5. rechercher documentation obsolète ou contradictoire ;
6. consigner FAIT ET VÉRIFIÉ / EN COURS / OUVERT / PROCHAINE ÉTAPE / À NE PAS REFAIRE ;
7. préciser les scénarios testés ;
8. relire la passation comme si le prochain agent n’avait accès à aucune conversation précédente.

## 8. Instruction courte

> Consulte `AI_START_HERE.md`, inspecte le code réel avant de te fier à la documentation, préserve toutes les mécaniques non concernées et vérifie les frontières de progression. Avant toute passation, indexe les règles et décisions afin que le prochain agent puisse reprendre sans la conversation précédente.
