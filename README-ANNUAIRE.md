# BAMP NC — organisation du site et de l’annuaire

## Structure recommandée

```text
BAMP-Noum-a/
├── assets/
│   ├── logo_bamp.svg
│   └── ... autres images existantes
├── data/
│   ├── professionnels.json
│   └── contacts-amp-utiles.json
├── index.html
├── annuaire.html
├── informations-legales.html
├── robots.txt
└── sitemap.xml
```

## Fichiers devenus inutiles

Une fois la nouvelle version testée sur GitHub Pages, vous pouvez supprimer :

- `professionnels.js` : l’accueil ne charge plus de fiches professionnelles ; la page `annuaire.html` lit directement `data/professionnels.json`.
- `ressources.html` : remplacé par `annuaire.html`.
- `data/annuaire-utile.json` : remplacé par `data/contacts-amp-utiles.json`.

## Annuaire en cours d’élaboration

La page `annuaire.html` contient temporairement :

```html
<meta name="robots" content="noindex, nofollow">
```

Cela évite de demander son indexation par les moteurs de recherche pendant sa construction. Le lien public depuis `index.html` reste également conservé dans le code sous forme de commentaire HTML.

Quand l’annuaire sera prêt :

1. Dans `index.html`, rechercher `À RÉACTIVER LORSQUE L’ANNUAIRE EST FINALISÉ` et retirer les commentaires `<!--` et `-->` autour du bouton vers `annuaire.html`.
2. Dans `annuaire.html`, remplacer `noindex, nofollow` par `index, follow`.
3. Ajouter `annuaire.html` à `sitemap.xml`.

## Mise à jour des données

Pour ajouter ou modifier une fiche, ne touchez pas au HTML :

- professionnels et accompagnants : `data/professionnels.json` ;
- structures et contacts pratiques : `data/contacts-amp-utiles.json`.

La page `annuaire.html` recharge automatiquement ces fichiers.

## Navigation de l’accueil

La terminologie est désormais séparée :

- **Mon parcours** : comprendre les étapes et le centre AMP ;
- **Accès & prise en charge** : règles locales, prise en charge et enjeux territoriaux ;
- **BAMP NC** : association, actualités, agenda, témoignages et partenaires ;
- **Annuaire & accompagnement** : trouver des professionnels et contacts (en cours d’élaboration) ;
- **Liens utiles** : BAMP national, Facebook, groupe privé, HelloAsso ;
- **Nous contacter** : joindre l’antenne.
