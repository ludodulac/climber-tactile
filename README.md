# Climber — accès à la simulation authentique et adaptation tactile

Site : https://ludodulac.github.io/climber-tactile/

## Ce que contient ce dépôt
- `index.html` : **portail de lancement** vers [Climber Crystal Screen de RetroFab / Itizso](https://itizso.itch.io/nintendo-climber-crystal-screen) (Nintendo 1986, modèle DR-802) ; propose aussi une tentative d'affichage de la page source dans un cadre. Cette tentative peut être bloquée par les protections du fournisseur. **Le jeu lui-même est hébergé par Itizso, pas par ce dépôt.**
- `adaptation.html` : notre **jeu indépendant** d'ascension, avec grands boutons gauche/droite/saut. Ce jeu n'est pas identique à Climber 1986.

## Pourquoi le jeu RetroFab n'est pas recopié
- La simulation publiée par Itizso est jouable gratuitement sur itch.io et disponible en fichier `.sim` pour son lecteur Windows.
- Aucun dépôt source sous licence permettant la redistribution et la modification de cette simulation n'a été vérifié.
- Le code, les ressources Nintendo et le paquet `.sim` n'ont donc **pas été copiés** sur GitHub.
- Une page de domaine différent ne peut pas injecter directement des événements clavier/tactiles à l'intérieur d'un lecteur tiers embarqué : les **grands boutons indépendants sur le véritable jeu restent non réalisés**.
- Une méthode possible serait un accord du développeur RetroFab pour une intégration officielle avec API de contrôle ou un projet de reproduction légalement réutilisable.

## Hébergement
GitHub Pages depuis la branche `main`, dossier `/(root)`.

## Statut
- Accès au véritable Climber de RetroFab : **lien direct opérationnel côté HTML** (publication GitHub Pages et lecture mobile à vérifier).
- Affichage du site RetroFab dans cette page : **expérimental / non vérifié**.
- Commandes géantes sur la simulation originale : **non réalisées**.
- Grandes commandes dans notre adaptation : **oui**.
