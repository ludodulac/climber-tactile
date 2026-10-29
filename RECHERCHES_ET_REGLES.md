# Climber LCD — dossier de recherche (29 octobre 2026)

But : construire une **récréation indépendante jouable**, lumineuse, lisible sur smartphone, des mécaniques du Game & Watch *Climber Crystal Screen* (Nintendo DR-802, 1986), sans redistribuer de ROM ni de graphismes propriétaires.

## Faits recoupés (documentation)

| Élément | Ce qui est documenté | Sources |
| --- | --- | --- |
| Matériel | Climber Crystal Screen DR-802, sorti le 4 juillet 1986, à écran LCD à silhouettes fixes | https://itizso.itch.io/nintendo-climber-crystal-screen ; https://www.digitec.ch/fr/page/vous-souvenez-vous-des-consoles-portables-a-ecran-transparent-28547 |
| Déplacement | gauche/droite + saut, mouvement par positions prédéfinies, défilement étage par étage, seulement trois étages visibles simultanément | https://www.digitec.ch/fr/page/vous-souvenez-vous-des-consoles-portables-a-ecran-transparent-28547 |
| Ascension | 25 étages par phase, passer par les trous, briser un bloc au plafond en deux sauts | https://itizso.itch.io/nintendo-climber-crystal-screen ; https://www.mobygames.com/game/96733/game-watch-crystal-screen-climber/ |
| Danger | Blockmen se déplacent sur les plateaux, réparent des trous et font perdre une vie au contact ; oiseaux, épines, plateformes mobiles | https://www.mobygames.com/game/96733/game-watch-crystal-screen-climber/ ; https://www.digitec.ch/fr/page/vous-souvenez-vous-des-consoles-portables-a-ecran-transparent-28547 |
| Reprise | en cas de mort, retour de sept étages environ ; passage par les côtés entraîne la réapparition sur le côté opposé | https://www.digitec.ch/fr/page/vous-souvenez-vous-des-consoles-portables-a-ecran-transparent-28547 |
| Bonus | sur quatre phases sur cinq : sauter pour attraper Hentori ; sur la cinquième : attraper l'épée pour vaincre Dragalo, deux essais pour Hentori | https://itizso.itch.io/nintendo-climber-crystal-screen ; https://game-watch-appreciation.fandom.com/wiki/Climber_%28Crystal_Screen%29 |
| Défaite | après 3 erreurs | https://game-watch-appreciation.fandom.com/wiki/Climber_%28Crystal_Screen%29 |
| Scores | un point par étage, compteur jusqu'à 999, jusqu'à 99 phases ; effacement des erreurs à 300 points **documenté pour la version DR-106** et non encore vérifié pour DR-802 | https://adb.arcadeitalia.net/dettaglio_mame.php?game_name=gnw_climber |

## Ce que la nouvelle version indépendante met en œuvre

- Silhouettes **dessinées par nous** à partir de petites matrices fixes de pixels, sans interpolation ni ressource Nintendo ;
- Déplacement horizontal **d'une case** à la fois, saut en **positions prédéfinies**, défilement d'un étage à la fois ;
- 25 étages pour chaque phase, quelques trous préexistants, deux coups pour casser une brique ;
- Blockmen, oiseaux volants, épines et étages mouvants selon les phases, difficultés progressives ;
- Hentori avec deux sauts et épée contre le dragon toutes les cinq phases ;
- Trois erreurs, reprises, score local et gros boutons multi-touch ;
- Palette LCD crème/vert contrastée et console lumineuse orange, sans assombrissement de RetroFab.

## Ce qui reste une **adaptation**, pas une reproduction certifiée

1. Les positions LCD d'origine et les dessins précis des personnages, blocs et ennemis n'ont pas été extraits du jeu original. Nos motifs sont originaux.
2. La géométrie de chaque plateau, les probabilités de trous et le rythme du saut ont été conçus à partir des principes observés et **ne sont pas des valeurs Nintendo certifiées**.
3. Le placement et la vitesse exacts des ennemis, l'évolution de difficulté, la séquence du dragon et l'attribution détaillée des bonus ne sont pas certifiés.
4. Le rétablissement des vies au score 300 est inspiré d'une description de la version New Wide Screen ; il reste à confirmer pour la Crystal Screen.
5. Le simulateur RetroFab et son fichier `.sim` ne sont ni copiés ni intégrés. Pas de licence de redistribution constatée.

## Comment tester (smartphone Android)

1. Ouvrir https://ludodulac.github.io/climber-tactile/
2. Vérifier que les gros boutons gauche/droite/saut sont simultanément utilisables.
3. Au départ, rejoindre le trou du premier étage, sauter puis se déplacer **en l'air** sur une brique intacte avant la retombée.
4. Vérifier qu'un saut contre une brique pleine la fragilise, que le deuxième la supprime.
5. Vérifier l'avancée de l'étage 1/25, l'affichage LCD segmenté et les pauses.
6. Tester les transitions Hentori/Dragalo et la progression des phases (plus longue session).
7. En cas de problème, signaler la phase, l'étage, le geste et une capture d'écran.

## Liens

- Simulation de référence : https://itizso.itch.io/nintendo-climber-crystal-screen
- Description historique détaillée : https://www.digitec.ch/fr/page/vous-souvenez-vous-des-consoles-portables-a-ecran-transparent-28547
- Description du jeu et des ennemis : https://www.mobygames.com/game/96733/game-watch-crystal-screen-climber/
- Règles de bonus et conseils : https://game-watch-appreciation.fandom.com/wiki/Climber_%28Crystal_Screen%29
- MAME, informations techniques et score version 1988 : https://adb.arcadeitalia.net/dettaglio_mame.php?game_name=gnw_climber
