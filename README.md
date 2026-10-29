# Climber LCD — jeu tactile indépendant

🎮 **Jouer :** https://ludodulac.github.io/climber-tactile/

Cette page contient directement un **jeu d'escalade réinventé à partir des mécaniques documentées** du Game & Watch *Climber Crystal Screen* de Nintendo (1986, DR-802). Elle ne redirige plus vers RetroFab.

## Fonctionnalités

- Affichage LCD **clair, lumineux, contrasté** avec des silhouettes conçues en images prédéfinies.
- Déplacements **case par case**, sauts à positions fixes et défilement de l'écran **étage par étage**.
- **25 étages par phase**, étages de briques avec passages à créer : deux sauts pour casser une brique.
- Blockmen qui circulent et rebouchent certains trous, oiseaux, ronces, plateaux mobiles à partir de certaines phases.
- **Hentori** à attraper après chaque phase normale (deux essais), **épée et Dragalo** une phase sur cinq.
- **Trois erreurs**, reprise, scores, record enregistré localement.
- **Très gros boutons** gauche, droite, SAUT ; fonctionnement combiné des touches, clavier et commande pause/son/recommencer.

## Comment grimper

1. Le personnage part sous un plateau, avec des ouvertures entre certaines briques.
2. Déplace-toi sous une ouverture et saute.
3. **Pendant le saut**, déplace-toi sur une partie pleine du plateau supérieur afin d'y retomber.
4. Si tu arrives sous une brique, deux sauts au même endroit la cassent et créent un passage.
5. Au 25e étage, réussis le bonus de fin de phase.

**Remarque importante :** les plateformes se traversent par leurs trous, mais on doit atterrir sur une partie pleine de la plateforme supérieure. La direction peut être maintenue en même temps que le saut.

## Fichiers

- `index.html` : **jeu publié** directement, sans dépendance.
- `lcd-reconstruction.html` : copie de travail de cette version.
- `adaptation.html` : ancienne première version d'ascension, beaucoup moins fidèle.
- `RECHERCHES_ET_REGLES.md` : recherche, références, caractéristiques établies et écarts encore présents.

## Statut et limites

**Il s'agit d'une récréation indépendante, pas de la ROM ni du code source Nintendo**. Les silhouettes sont des créations nouvelles : elles ne sont pas celles d'origine. Les règles principales sont reprises à partir de descriptions vérifiées, mais les timings, certains comportements des adversaires, les dispositions des niveaux et les bonus restent des approximations et n'ont pas été comparés image par image à la machine originale.

Le jeu a été vérifié par **tests programmatiques du JavaScript et de plusieurs transitions**. La publication GitHub Pages et les commandes sur **le téléphone physique** restent à valider par le propriétaire. Aucun fichier propriétaire de Nintendo/RetroFab n'est utilisé.

## Modifier ou publier

Fichier unique `index.html`, hébergement GitHub Pages depuis la branche `main` et le dossier `/(root)`.

Aucune clé, API ou dépense nécessaire.
