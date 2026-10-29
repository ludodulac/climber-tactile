# Bomb Sweeper — recherche approfondie et corrections (29 octobre 2026)

## Faits vérifiés sur le véritable Game & Watch (Nintendo BD-62, 1987)

| Caractéristique | Résultat de la recherche |
| --- | --- |
| Mode A | **80 énigmes** au total avant reprise, dont **45 dispositions originales et 35 répétitions** selon les auteurs du port ZX Spectrum et d'un remake PC. L'ensemble se joue par **groupes de 10**, suivis d'une épreuve bonus, donc **8 bonus** sur le premier cycle de 80. |
| Enchaînement A | Après chaque bonus, **les cinq derniers puzzles sont rejoués**, puis **cinq nouveaux puzzles** arrivent ; cette règle a été décrite par l'auteur d'une adaptation PC de 2007. |
| Mode B | Des séries de **15 énigmes** à disposition variable ; le temps initial est de **40 secondes** et baisse de **4 secondes par série**, jusqu'à **4 secondes**. Aucune étape bonus. |
| Structure de l'écran | Deux écrans, dont le supérieur affiche surtout Dynamite Jack / la ville / l'animation et le compte à rebours ; l'inférieur contient un **réseau de fines parois horizontales et verticales**. Ce ne sont **pas** de grosses cases/caisses pleines. |
| Déplacement | Quatre directions. Les parois **coulissent par poussée si l'espace derrière est libre**. On ne peut pas les tirer. |
| Bombes | Il peut y avoir plusieurs bombes ; **atteindre l'une suffit** à neutraliser toutes celles du niveau. |
| Score | Le temps restant est converti en points. Les erreurs **ne sont pas annulées à 300 points**. |
| Échecs | Explosion en fin de compte à rebours, et dans les bonus risque d'être coincé/écrasé ; **3 erreurs = fin de partie**. |
| Mode A, temps | Sources divergentes : plusieurs décrivent **40 comptes** ; une démonstration filmée décrit **50 secondes**. **Ne pas présenter une valeur exacte comme certaine** avant vérification sur la machine. |

## Sources consultées et provenance

1. **Port ZX Spectrum Menyiques (2023)** : 80, dont 45 nouvelles dispositions et 35 répétitions, bonus toutes les dix : https://menyiques.itch.io/zxbombsweeper
2. **Delphi-PRAXiS, auteur Phantom1 (2007)** : 80 énigmes, 8 bonus, répétition des cinq derniers plans, cinq nouveaux par série, accélération du bonus : https://www.delphipraxis.net/97563-bomb-sweeper-denkspiel-remake.html
3. **RetroFab / Itizso** : double écran, commandes, murs poussables, bombes, Game A 10+bonus par groupe, Game B 15 : https://itizso.itch.io/nintendo-bomb-sweeper
4. **Fandom Nintendo** : Game A 40, Game B 40→4, murs à pousser : https://nintendo.fandom.com/wiki/Bomb_Sweeper
5. **Démo vidéo de la machine (description publiée par The8BitGuyWorld)** : progression et chrono A décrit à 50, B à 40 et décrément de 4 ; la vidéo montre les silhouettes LCD : https://www.youtube.com/watch?v=5_s-Q0wsi34
6. **MAME/ArcadeItalia** : absence de remise à zéro des erreurs à 300 points : https://adb.arcadeitalia.net/dettaglio_mame.php?game_name=gnw_bsweep
7. **Photos du véritable écran** : https://indiegamerchick.com/2023/12/26/lcd-games-of-the-1980s-part-x-nintendo-game-watch-the-definitive-review-rankings-of-every-nintendo-game-watch/
8. **Réécriture 2002 sur NES (Snowbro)** : rapporte 26 niveaux originaux + 73 supplémentaires ; ce n'est pas une source prouvant 99 niveaux de la machine 1987 : https://gamesdb.launchbox-app.com/games/details/28302-bomb-sweeper

## Corrections apportées à notre jeu le 29 octobre 2026

- Avant : **10 puzzles pour toujours en mode A**, puis recommencement. Maintenant : **80 étapes dont 45 plans distincts répartis selon le rythme documenté**, un bonus après chacun des huit groupes.
- Avant : grandes cases carrées à pousser. Maintenant : affichage de **segments fins verticaux et horizontaux**, plus proche de l'aspect du véritable écran. Les obstacles restent des *cases de collision* dans notre moteur ; la géométrie exacte de Nintendo n'a pas été reproduite.
- Avant : grille de 11 × 9 ; maintenant : grille réduite à **9 × 7**, mieux adaptée au rapport des écrans et aux segments LCD (dimensions **adaptées**, non vérifiées comme d'origine).
- Avant : chronomètre Game B variable dès le premier parcours. Maintenant : **40 secondes par parcours pendant les 15 premiers**, puis 36, 32… jusqu'à 4 secondes au minimum.
- Avant : bonus vu comme un simple grand parcours parcouru à la vitesse du joueur. Maintenant : **défilement automatique** avec risque de perdre si l'écran rattrape le personnage.
- Mode A : chrono placé à 40 secondes dans notre adaptation en raison du désaccord des sources ; à confirmer pour la machine originale.
- Ajouts non officiels conservés : Indice et Annuler.

## Écarts encore importants — NE PAS PRÉSENTER COMME IDENTIQUE

**Les positions exactes des parois et des bombes pour les 45 configurations originales ne sont pas disponibles sous forme de carte fiable dans les sources exploitées.** Le générateur actuel produit donc 45 configurations **originales à notre projet**, déterministes en mode A. La disposition de chaque puzzle **n'est pas celle du Game & Watch**.

Le système de poussée repose toujours sur des cases logiques et des segments dessinés ; ce n'est pas la simulation électrique de la matrice LCD Nintendo. L'animation du bonus, les timings d'appui et les séquences haut écran sont simplifiés. Nous n'utilisons pas les ROM, l'art ou le code du jeu Nintendo ni ceux de RetroFab.

**Statut exact :** progression documentée = rapprochée ; **cartes originales = non reconstruites**. Pour atteindre une fidélité réelle des niveaux, il faudra relever les **45 configurations** à partir d'une source autorisée/visible (captures du simulateur ou plan de niveaux réutilisable), puis contrôler chaque carte au moins visuellement et tester les solutions. **Aucune carte n'est affirmée originale aujourd'hui.**

## Tests techniques

- 80 étapes du mode A : cartes résolubles lors du test du générateur.
- Le bonus est traversable ; passage étape 10 → bonus → étape 11 vérifié.
- Mode B : départ à 40 secondes ; deuxième série à 36 secondes vérifiée.
- Syntaxe JS et présence des fichiers contrôlées via GitHub.
- **Test d'interaction et rendu sur Android réel non effectué.**
