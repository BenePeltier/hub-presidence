# Hub de la Présidence

Site statique de **https://president.apollo-business.com** (GitHub Pages).

## Mettre à jour une adresse d'outil
1. Ouvrir `index.html`, aller tout en bas, bloc `const HUB = { ... }`.
2. Changer l'adresse voulue (une adresse vide affiche « Adresse à renseigner » ou « bientôt »).
3. Enregistrer le commit sur `main` : le site est republié en moins d'une minute.

## Mettre à jour le script de la réunion
Déposer les versions téléphone dans `script/nouveau/index.html` et `script/classique/index.html`,
les PDF dans `docs/`, puis renseigner les adresses dans le bloc `HUB.links`.

## Source de la page
La page est générée depuis le projet « Support Plaquette Formation APOLLO » (template.html + build.py) :
icônes Tabler et logos officiels inclus au montage. Modifier `index.html` directement reste possible pour une adresse.
