# Mes jeux LCD — Climber et Bomb Sweeper

**Adresse du site :** https://ludodulac.github.io/climber-tactile/

Le site propose **deux jeux indépendants**, accessibles depuis un menu commun, avec des commandes tactiles adaptées aux smartphones.

| Page | Contenu |
| --- | --- |
| `index.html` | **Menu** permettant de choisir entre Climber LCD et Bomb Sweeper LCD ; lien vers Zelda Game & Watch sur RetroFab. |
| `climber.html` | Premier jeu : ascension LCD sur 25 étages, avec gros boutons gauche/droite/saut. |
| `bomb-sweeper.html` | Deuxième jeu : puzzles de désamorçage sur double écran, direction à quatre touches, modes GAME A et GAME B. |
| `lcd-reconstruction.html` | Sauvegarde de la version Climber du 29 octobre 2026. |
| `adaptation.html` | Prototype antérieur du jeu d'ascension. |
| `RECHERCHES_ET_REGLES.md` | Recherche et limites connues pour Climber Crystal Screen. |
| `BOMB_SWEEPER_REGLES.md` | Règles sources et limites de la récréation de Bomb Sweeper. |

## Bomb Sweeper — comment jouer

Dans le jeu de Nintendo de 1987, le héros John Solver doit traverser des égouts et trouver **une bombe** posée par Dynamite Jack **avant la fin du compte à rebours**. Il peut **pousser** une paroi mobile si la case derrière celle-ci est libre. Atteindre une bombe désamorce les autres et rapporte un nombre de points dépendant du temps restant.

La récréation ici comprend :
- **GAME A : 10 labyrinthes aux dispositions prédéfinies, puis un niveau bonus horizontal à défilement.**
- **GAME B : 15 labyrinthes variables par cycle, plus rapides.**
- Un personnage et des obstacles avec dessins originaux dans une interface LCD volontairement **lumineuse**.
- Gros boutons tactiles **▲ ◀ ▼ ▶**, clavier flèches/WASD.
- **Annuler** le dernier déplacement, **Indice** (coûte 6 secondes), Pause, Son.
- Des murs permanents verts, des parois **jaunes à pousser**, des bombes et un compte à rebours.
- Un maximum de **trois explosions** avant la fin de partie ; les manques ne sont pas effacés au score 300.

La disposition des 10 labyrinthes, leur nombre précis de parois, les secondes allouées, la musique, les graphismes, le système d'indice et les mouvements du personnage **sont des créations / adaptations indépendantes**. Il ne s'agit **pas** d'une émulation de la ROM Nintendo et le programme source ou les graphismes de RetroFab ne sont pas copiés.

## Zelda Game & Watch en ligne

Le Zelda d'origine (1989) est jouable depuis le navigateur à l'adresse de son auteur :
https://itizso.itch.io/nintendo-zelda

Sur cette page, cliquer sur « Run game ». Ce jeu est **externe** au présent dépôt.

## Déploiement

GitHub Pages → main / (root). Aucun serveur, framework, accès payant ni API. Chaque jeu est un fichier HTML autonome.

## Vérifications (29 octobre 2026)

- Fichiers publiés sur la branche `main`, dépôts et chemins vérifiés par lecture GitHub.
- Bomb Sweeper : syntaxe JS vérifiée ; 10 configurations A + 15 B toutes résolubles lors des tests de génération ; niveau bonus résoluble ; 11 tests de mécanismes réussis (score, déplacement, annulation, indice, progression, temps, défaite).
- À vérifier **sur le véritable téléphone Android** : rendu visuel, confort des boutons, animations, audio et déploiement effectif de GitHub Pages.

## Modifications ultérieures

Il suffit de modifier directement la page HTML du jeu concerné. Les deux jeux sont indépendants et le menu reste en place.
