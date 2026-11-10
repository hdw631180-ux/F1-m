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

## Contrôle du temps en course
- **⏸ Pause / ▶ Reprendre** (bouton ou touche `Espace` / `P`) : fige la course et l'animation, tu peux régler allure / pneus / box pendant la pause.
- Vitesses **×¼, ×½, ×1, ×4, ×16** (×¼ = un tour toutes les 2,8 s).

## Fluidité (PC légers)
- Suppression des effets coûteux (flou d'arrière-plan, bruit plein écran, animations infinies, ombres portées sur les voitures).
- Course : positions des voitures précalculées sur le tracé, tableau de chronométrage mis à jour seulement quand il change, rafraîchissement limité aux vitesses rapides.
- **Mode fluide** (case dans le QG, activé automatiquement sur les PC ≤ 4 cœurs / ≤ 4 Go) : coupe toutes les animations et particules.

- Images de voitures décodées une seule fois (plus de rechargement à chaque écran), circuits réels chargés un par un en arrière-plan, course mise en pause automatiquement si tu changes d'onglet, détection automatique des PC lents (active le Mode fluide).

## Voitures 2D
Une photo détourée par écurie (vue de profil, fond transparent), intégrée dans `index.html` (aucun fichier externe).

## Publier sur GitHub Pages
1. Envoie index.html, .nojekyll, README.md à la racine d’un dépôt.
2. Settings > Pages > Deploy from branch `main` / root.
3. Le jeu est en ligne sur `https://TON-PSEUDO.github.io/NOM-DU-DEPOT/`.

## Données
Écuries, pilotes, circuits, calendrier : saison 2026 (estimations non officielles pour les stats).
Tracés réels chargés depuis bacinger/f1-circuits (MIT) au premier lancement, puis mis en cache.
