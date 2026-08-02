# Site BAMP Nouméa

Site vitrine statique de l’antenne BAMP de Nouvelle-Calédonie.

## Versions sauvegardées

- `v1-association-2026-08-02` : version stable centrée sur la présentation de l’association, avant l’ajout du parcours AMP détaillé.

Ce tag permet de consulter ou restaurer l’ancienne version sans perdre les évolutions ultérieures.

## Mise en ligne avec GitHub Pages

1. Déposer `index.html` à la racine d’un dépôt GitHub public.
2. Ouvrir **Settings → Pages**.
3. Sous **Build and deployment**, choisir **Deploy from a branch**.
4. Sélectionner la branche `main`, le dossier `/(root)`, puis enregistrer.

Le site ne nécessite ni installation, ni compilation, ni service payant.

## Fichiers principaux

- `index.html` : page d’accueil et contenus du site.
- `professionnels.js` : fiches validées du guide local.
- `informations-legales.html` : mentions légales, confidentialité et règles de traitement des données.
- `assets/partage-bamp-nc.png` : aperçu utilisé lors du partage du site sur les réseaux sociaux.
- `assets/affiche-antenne-bamp-nc.png` : présentation complète de l’antenne locale.
- `assets/affiche-insemination-bamp-nc.png` : parcours pédagogique de l’insémination.
- `assets/affiche-fiv-icsi-bamp-nc.png` : parcours pédagogiques de la FIV et de la FIV-ICSI.

## Compléter le guide des professionnels

Les professionnels s’inscrivent d’abord avec le formulaire Google Forms lié sur le site.
Après vérification de leur accord de publication, ouvrir `professionnels.js`, copier le
modèle de fiche commenté et renseigner les champs autorisés. Le guide est ensuite mis
à jour automatiquement lors de la publication GitHub Pages. Dès que plusieurs fiches
sont présentes, les filtres par activité et secteur apparaissent automatiquement.

Vérifier au moins une fois par an l’exactitude des fiches publiées. Les demandes non
publiées doivent être supprimées au plus tard douze mois après leur réception, conformément
à la politique de confidentialité affichée sur le site.

## Vérifier les informations sur l’AMP

Les règles d’accès, les autorisations du centre et les conditions de prise en charge peuvent
évoluer. Contrôler au minimum tous les six mois les sections **Mon parcours**, **Accès en NC**
et **Prise en charge** à partir des sources officielles liées dans `index.html` : DASS,
CHT/Médipôle, Légifrance et CAFAT. Mettre également à jour la date de vérification affichée
sur le site.
