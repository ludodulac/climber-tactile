# Bomb Sweeper — recherches, règles et divergences

Jeu de référence : *Bomb Sweeper*, Nintendo, Game & Watch Multi Screen, BD-62, **15 juin 1987**.

## Caractéristiques établies

| Aspect | Règle documentée | Source |
| --- | --- | --- |
| Histoire | Le méchant Dynamite Jack place des bombes sous la ville ; John Solver doit les atteindre. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Écrans | Écran supérieur : ville, saboteur, chronomètre ; écran inférieur : labyrinthe souterrain. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Direction | Déplacements haut/bas/gauche/droite. | [Flyzy](https://flyzy67.itch.io/bomb-sweeper) |
| Obstacles | Les murs mobiles peuvent être poussés si la case derrière est libre (pas de poussée à travers un autre mur). | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper), [Flyzy](https://flyzy67.itch.io/bomb-sweeper) |
| Bombes | Atteindre l'une des bombes suffit à toutes les désamorcer. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Score | Le temps restant est ajouté au score lorsque la bombe est atteinte. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Échec | Explosion à l'expiration du compte à rebours ; trois pertes et fin de partie. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Game A | Un cycle de **10 labyrinthes + un niveau bonus à défilement horizontal** (11 niveaux au sens large). | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper), [Nintendo Museum France](https://nintendo-museum.fr/bomb-sweeper-1987-multiscreen/) |
| Game B | Un cycle de **15 labyrinthes variables**, avec un chronomètre plus court. | [RetroFab](https://itizso.itch.io/nintendo-bomb-sweeper) |
| Autre | Contrairement à de nombreux Game & Watch, les erreurs ne sont **pas effacées à 300 points**. | [MAME ArcadeItalia](https://adb.arcadeitalia.net/dettaglio_mame.php?game_name=gnw_bsweep) |

**Attention à l'incohérence apparente « 10 » contre « 11 » :** le jeu A propose dix labyrinthes classiques, suivis d'une épreuve bonus distincte. Certaines sources comptent donc onze niveaux.

## Notre version jouable

Fichier : `bomb-sweeper.html`

- **Deux écrans** dessinés en Canvas et design contrasté clair (même esprit LCD, sans reprendre les images Nintendo).
- **Quatre grosses touches** pour téléphone, et clavier fléché/WASD.
- **10 labyrinthes prédéfinis** en mode A, puis un bonus dans un parcours horizontal plus large que l'écran, avec défilement.
- **15 labyrinthes générés**, avec contrôle automatique de solvabilité, en mode B.
- **Une, parfois deux bombes** ; pousser des obstacles jaunes d'une case ; décompte continu, points selon le temps restant.
- **Trois erreurs**, sans remise à zéro à 300 points.
- Ajouts volontairement non officiels : **annulation des déplacements** (le chrono continue), **indice** coûtant six secondes, pause, sons optionnels, disposition de parois et chronos adaptés.

## Ce qui n'est PAS établi comme identique

Les **topologies des labyrinthes originaux**, leurs dimensions exactes, les **animations LCD d'origine**, les calculs complets de score, le chrono exact à chaque étape, les textes affichés, le niveau bonus exact et la distribution d'éventuelles **fausses bombes** (signalées par Nintendo Museum mais pas décrites précisément) ne sont **pas reproduits à l'identique**.

Il s'agit d'un jeu de réflexion **autonome et original inspiré des mécaniques** du Game & Watch, **pas d'une émulation**, et le code / les graphismes / les ROM de Nintendo ou le simulateur RetroFab n'ont pas été inclus.

## Références de jeu en ligne

- Bomb Sweeper, simulation RetroFab : https://itizso.itch.io/nintendo-bomb-sweeper
- Bomb Sweeper, seconde simulation (Flyzy) : https://flyzy67.itch.io/bomb-sweeper
- **Zelda Game & Watch 1989, jeu en ligne** : https://itizso.itch.io/nintendo-zelda
