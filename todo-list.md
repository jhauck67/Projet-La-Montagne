# Todo List

## Le fichier index.html

- [ ] Créer le fichier `index.html`

## Titre et meta-description

- [ ] **Titre de la page** : xxx
      _Entre 50 et 60 caractères_
- [ ] **Meta-description** : xxx
      _Entre 150 et 160 caractères_

## Les favicons

- [ ] **Préparer les favicons :**
  - [ ] Une favicon en .SVG de 512x512 `favicon.svg`
  - [ ] Un fichier .ICO avec 2 layers 16x16 et 32x32 `favicon.ico`
  - [ ] Deux favicons en .PNG de 16x16 et 32x32 `favicon-16x16.png` et `favicon-32x32.png`
  - [ ] Une apple-touch-icon en .PNG en 180x180 `apple-touch-icon.png`

## Les Open Graph réseaux sociaux

- [ ] Titre de la page : xxx
      _Moins de 60 caractères_
- [ ] Description de la page : xxx
      _Entre 120 et 140 caractères_
- [ ] Image Open Graph en .PNG de 1200x630 `opengraph.png`

> On pourra utiliser le site [Opengraph](https://www.opengraph.xyz) pour générer les bonnes balises OpenGraph

## Traitement des images

- [ ] Redimensionner, formatter et compresser les images utilisées sur le site
      _On pourra penser à faire différentes versions des images selon leur utilité_

**_Pour intégrer plusieurs versions d'une même image :_**

```html
<img
  srcset="./chemin/vers/image.webp, ./chemin/vers/image@2x.webp 2x"
  src="./chemin/vers/image.webp"
  alt="descriptif de l'image"
/>
```

> On pourra utiliser le site [Squoosh](https://squoosh.app/) pour générer des images en webp

- [ ] Identifier les images à "preload"
- [ ] Prévoir les icones en SVG si utilisation d'icones

> Si on intègre les icones avec <svg> et non avec <img>, on ajoutera un `aria-label:"description de l'icone"`

## La(les) polices

- [ ] Télécharger la(les) polices
- [ ] Lier celle(s)-ci au projet dans `settings.scss` par :

```scss
@font-face {
    font-family: "Nom-police";
    src: url(../chemin/vers/la/font.ttf)
    font-display: swap; //Pour éviter les décalages de mise en page
}
```

## La feuille de style .CSS

- [ ] Créer le fichier `index.scss` et `_settings.scss`
- [ ] Lier la page `_settings.scss` à l'`index.scss` par :

```scss
@import "./settings";
```

- [ ] Lancer Watch Sass
- [ ] Lier la feuille de style CSS au fichier HTML

## La feuille de script .JS

- [ ] Créer la feuille de script .JS `index.js`
- [ ] Lier le script au bas du <body>

## Structure de la page web

- [ ] Réfléchir à la structure sémantique de la page web.
- [ ] Définir les images les plus importantes (qui s'afficheront en premier) et les images qui sont cachées au chargement de la page. On "preload" les plus importantes, on fait un `loading="lazy"`

## Vérification de la sémantique

- [ ] Vérifier qu'il n'y a pas d'erreurs sémantiques dans le code.

> On pourra utiliser le site [Markup Validation service](https://validator.w3.org/)

## Vérification des performances

- [ ] Lancer un Audit Lighthouse

## Mise à jour du Readme.md

- [ ] Remplir les premières parties du Readme
- [ ] Créer un header Github Readme `assets/sketch/github-header-image.png`

> On utilisera le site [Github Profile Header Générator](https://leviarista.github.io/github-profile-header-generator/)

- [ ] Créer un aperçu du site
- [ ] Créer une vidéo aperçu
- [ ] Convertir la vidéo en GIF

## Commit & Push sur la manche "Main"

- [ ] Commit et Push les fichiers sur la branche principale "main"

## Mise à jour du readme

- [ ] Récupérer les adresses de `aperçu.png` et `video.gif`

## Effectuer les tests visuels et de performances multi-plateformes

- [ ] Remplir le tableau tests et vérifications dans le readme.
- [ ] Créer des issues avec les modifications ou améliorations à apporter.

## Modifications et améliorations

- [ ] Créer une nouvelle branche `git checkout -b fix:modif`
- [ ] Faire les modifications, les tester sur live server.
- [ ] Commit & Push les modifications
- [ ] Faire une pull request associée à une issue
- [ ] Merge les modifications sur la branche principale
- [ ] Supprime la branche "fix"
- [ ] Refaire les tests en réel
- [ ] Mettre à jour le readme

## Quand le site est satisfaisant

- [ ] insérer le dashboard et mettre à jour le paragraphe Lighthouse.
