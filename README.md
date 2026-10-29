# Climber tactile

Mini-jeu d'escalade indépendant, inspiré des jeux électroniques LCD anciens, conçu pour le téléphone avec **gros boutons tactiles**.

**Important :** ce jeu n'est **pas** le Climber original de Nintendo ni la simulation RetroFab. Il utilise du code, des graphismes et des règles de jeu créés indépendamment. Aucune ROM ou ressource propriétaire n'est incluse.

## Jouer

Lorsque GitHub Pages est activé : https://ludodulac.github.io/climber-tactile/

- Sur téléphone : appuyer sur les grands boutons **◀**, **▶**, **SAUT** (appuis simultanés possibles).
- Sur ordinateur : flèches gauche/droite et barre d'espace.
- En haut : son, pause, recommencer.
- Le record est gardé localement dans le navigateur.

## Activer GitHub Pages

Dans le dépôt GitHub : **Settings → Pages → Build and deployment → Source : Deploy from a branch → Branch : main → /(root) → Save**.

Le jeu est une page autonome `index.html`, sans framework ni serveur.

## Agrandir encore les boutons

Dans `index.html`, chercher `.controls` et `.control`. La propriété `height` définit la hauteur des grosses commandes ; augmenter ses valeurs pour les rendre encore plus grandes.
