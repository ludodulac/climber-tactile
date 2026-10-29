# Mes deux jeux LCD

**Jouer :** https://ludodulac.github.io/climber-tactile/

Deux jeux indépendants sont accessibles dans le menu d'accueil : **Climber LCD** et **Bomb Sweeper LCD**. Ce sont des créations autonomes inspirées des appareils électroniques Nintendo, et non des ROM ou des reproductions certifiées conformes.

## Fichiers

- `index.html` : menu pour choisir un jeu, avec un lien externe vers Zelda Game & Watch.
- `climber.html` : premier jeu, ascension LCD avec gros boutons.
- `bomb-sweeper.html` : deuxième jeu, déminage LCD avec grosses flèches, Game A/B.
- `bomb-sweeper-v1.html` : archive de notre première version Bomb Sweeper.
- `bomb-sweeper-v2.html` : copie de la reconstruction plus documentée.
- `lcd-reconstruction.html` : ancienne copie Climber.
- `adaptation.html` : toute première adaptation Climber.
- `BOMB_SWEEPER_REGLES.md` : **recherches détaillées et distinction entre règles vérifiées et hypothèses**.
- `RECHERCHES_ET_REGLES.md` : recherches Climber.

## Bomb Sweeper : ce que nous savons du vrai jeu de 1987

- **Game A** : 80 labyrinthes dont 45 différents et 35 réutilisés, huit bonus avec défilement horizontal ; les nouveaux groupes de dix réutilisent les cinq derniers puzzles puis ajoutent cinq nouveaux.
- **Game B** : séries de 15 labyrinthes variables ; chrono 40 secondes, puis 36, 32… jusqu'à 4 secondes minimum selon la progression.
- Déplacement dans quatre directions. Les obstacles mobiles sont des **parois fines horizontales et verticales**, à pousser si l'espace derrière est libre.
- Atteindre **une** bombe désamorce celles du niveau. Trois erreurs terminent la partie ; le score augmente avec le temps restant.

Les détails historiques et sources sont dans `BOMB_SWEEPER_REGLES.md`.

## Ce que notre jeu fait, et ce qu'il ne fait pas

Notre version propose un écran plus clair, de **gros boutons tactiles**, des parois dessinées comme des traits et la progression de **80 étapes / 8 bonus** en A. Les configurations choisies en mode A suivent le rythme des reprises et nouveautés ; les 80 sont résolubles lors du test technique.

**IMPORTANT — Les positions exactes des murs, bombes et personnages des 45 labyrinthes Nintendo ne sont PAS encore reproduites.** Les 45 configurations de notre version ont été créées pour ce projet ; ce ne sont pas les cartes originales. Le bonus reste également une approximation. Cela ne doit pas être présenté comme une copie fidèle.

Fonctions supplémentaires non originales : indice, annulation, pause, bouton son.

## Vérifications

- Publication des fichiers et syntaxe JavaScript contrôlées via le connecteur GitHub.
- 80 étapes A du générateur résolubles dans les tests ; bonus traversable.
- Transition A 10 → bonus → 11 et B 40 → 36 vérifiées programmatiquement.
- **Jeu sur le vrai téléphone Android et GitHub Pages non testés ici.**

## Zelda (jeu d'origine)

Jouer via RetroFab sur le site de son créateur : https://itizso.itch.io/nintendo-zelda
