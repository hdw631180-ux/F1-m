# F1 Manager 2026

Jeu de management de Formule 1 dans le navigateur (HTML/CSS/JS, zéro build).

## Interface
Dashboard sombre type F1 : barre latérale, progression de saison, cartes animées, confettis podium, sons optionnels.

## Fonctionnalités utiles ajoutées
- Comparaison de ta voiture vs les rivaux
- Historique des derniers GP (positions / points)
- Conseil stratégie avant chaque course (selon circuit & météo)
- Astuces coach aléatoires
- Barre de progression de saison
- Sons (clic, upgrade, podium) — activables dans le QG
- Confettis si podium
- Raccourcis clavier : `G` = aller au GP, `1–5` = onglets QG
- Légende pneus + tip composé

## Améliorations de l'écran de course
- Carte et classement côte à côte, avec tes pilotes sous la carte (plus d'espace perdu)
- Fiche en direct par pilote : position, pneu et usure en %, écart avec la voiture devant et derrière
- Allure en un clic (Attaque / Normal / Éco)
- Meilleur tour en direct et dans les résultats
- Notifications d'incident en bas de l'écran (elles ne cachent plus les boutons)
- Classement constructeurs affiché « — » tant qu'aucun point n'est marqué

## Visuel premium
- Monoplace aux couleurs (livrée stylisée) de chaque écurie, avec entrée animée, flottement, reflets et traînées de vitesse
- Légère inclinaison 3D de la voiture avec la souris
- Cartes qui apparaissent en cascade, boutons principaux brillants, fond animé aux couleurs de l'écurie
- Dans la course, la ligne d'un pilote clignote en vert ou en rouge quand il gagne ou perd une place
- Animations désactivées automatiquement si ton système demande moins de mouvement

## Vraies photos de monoplaces (optionnel)
Dépose tes images dans le dossier `cars/` (noms dans `cars/LISEZ-MOI.txt`), puis dans `index.html` change `const CAR_PHOTOS=false;` en `const CAR_PHOTOS=true;`. Par défaut c'est désactivé pour éviter des erreurs 404 dans la console.

## Publier sur GitHub Pages
1. Envoie index.html, .nojekyll, README.md à la racine d’un dépôt.
2. Settings > Pages > Deploy from branch `main` / root.
3. Le jeu est en ligne sur `https://TON-PSEUDO.github.io/NOM-DU-DEPOT/`.

## Données
Écuries, pilotes, circuits, calendrier : saison 2026 (estimations non officielles pour les stats).
Tracés réels chargés depuis bacinger/f1-circuits (MIT) au premier lancement, puis mis en cache.
