# Ressources AMP – fichiers pour GitHub Pages

## Arborescence à utiliser

```text
BAMP-Noum-a/
├── index.html
├── informations-legales.html
├── professionnels.js
├── ressources.html                 <- nouvelle page Ressources AMP
├── data/                            <- nouveau dossier
│   ├── professionnels.json         <- fiches santé + thérapeutes
│   └── annuaire-utile.json         <- contacts utiles AMP
└── assets/
    └── logo-bamp-ressources.png    <- logo utilisé par ressources.html
```

## Mise à jour courante

- Pour ajouter ou modifier un professionnel : éditer `data/professionnels.json`.
- Pour modifier l'annuaire AMP utile : éditer `data/annuaire-utile.json`.
- Mettre à jour la valeur `updatedAt` au format `AAAA-MM-JJ`.
- Cliquer sur **Commit changes** dans GitHub.
- La page `ressources.html` relira automatiquement les JSON publiés.

## Adresse publique prévue

Une fois les fichiers placés sur la branche publiée par GitHub Pages :

`https://collectifbampnoumea-cmd.github.io/BAMP-Noum-a/ressources.html`

## Important pour les tests

La page utilise `fetch()` pour charger les JSON. Selon le navigateur, l'ouverture directe du fichier en `file://` peut être bloquée. Le test fiable se fait sur GitHub Pages (ou via un petit serveur local).
