# Dynamique de l'occupation agricole à Richard-Toll · NDVI 2017-2025

Site statique : un seul fichier `index.html` (HTML, CSS et JavaScript intégrés), un dossier `images/` et un dossier `data/`.

## Structure

- `index.html` : la page complète
- `images/` : cartes annuelles (`changement_AAAA_AAAA.png`) et planches de synthèse
- `data/` : fichiers CSV lus par la page pour les graphiques et les tableaux

## Test en local

Un double-clic sur `index.html` affiche la page, mais le navigateur bloque la lecture des CSV. Pour tout voir :

```
python -m http.server 8000
```

puis ouvrir http://localhost:8000.

## Mise en ligne avec GitHub Pages

1. Créer un dépôt public sur github.com (par exemple `richard-toll-ndvi`).
2. Déposer tout le contenu de ce dossier (Add file > Upload files), puis valider (Commit changes).
3. Settings > Pages > Source : « Deploy from a branch », branche `main`, dossier `/ (root)`, puis Save.
4. Après une à deux minutes, le site est accessible à `https://<nom-utilisateur>.github.io/richard-toll-ndvi/`.

## Aperçu LinkedIn

`images/apercu_linkedin.png` (1200 × 630 px) sert d'image d'aperçu lorsque le lien est partagé sur LinkedIn. Dans `index.html`, remplacer `VOTRE-NOM-UTILISATEUR` par votre nom d'utilisateur GitHub dans la ligne `og:image` (LinkedIn exige une adresse absolue). Pour rafraîchir l'aperçu après un changement : https://www.linkedin.com/post-inspector/

## Mise à jour des résultats

Remplacer les CSV de `data/` et les images de `images/` en conservant les mêmes noms. Le résumé et les textes de lecture de la section 3 contiennent des chiffres écrits à la main : à relire si les données changent.
