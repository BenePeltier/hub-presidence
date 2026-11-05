# Hub de la Présidence

Site statique de **https://president.apollo-business.com** (GitHub Pages).

## Mettre à jour une adresse d'outil
1. Ouvrir `index.html`, aller tout en bas, bloc `const HUB = { ... }`.
2. Changer l'adresse voulue (une adresse vide affiche « Adresse à renseigner » ou « bientôt »).
3. Enregistrer le commit sur `main` : le site est republié en moins d'une minute.

## Le script de la réunion
Les scripts (version téléphone) et les livrets A4 sont dans `docs/`, chiffrés (AES-256-GCM) :
ils se lisent depuis le hub, après connexion. La clé de lecture est remise par la fonction `public.hub_cle()`
de la base APOLLO France, aux seuls rôles de l'équipe de pilotage (Président, Vice-Président, Secrétaire Général,
Coach Éducateur, comptes nationaux).
Une nouvelle version se monte depuis le projet (`build.py`) : il chiffre les fichiers et met à jour leurs adresses dans `index.html`.

## Source de la page
La page est générée depuis le projet « Support Plaquette Formation APOLLO » (template.html + build.py) :
icônes Tabler et logos officiels inclus au montage. Modifier `index.html` directement reste possible pour une adresse.
