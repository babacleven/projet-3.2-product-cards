# PROJET 3.2 - Carte Produit Stylisee

Niveau : Intermediaire  
Technologies : HTML5 + CSS3 externe (feuille de style unique)

## Description

Page de presentation de produits inspiree du style Amazon / Jumia avec 6 cartes produits reparties en 4 categories. Chaque carte affiche une image, un titre, une description, un prix, des etoiles de notation, des badges (Promo / En stock), et des boutons d'action.

## Installation

1. Cloner le depot :
   ```
   git clone https://github.com/babacleven/projet-3.2-product-cards.git
   ```
2. Ouvrir `products.html` dans un navigateur moderne.

Aucune dependance ni serveur requis.

## Utilisation

La page affiche une grille de 6 cartes produit :

- Smartphone Pro X (Electronique)
- UltraBook Air (Electronique)
- Watch Sport 5 (Electronique)
- Pagne Kuba (Vetements)
- Livre Cuisine (Livres)
- Poulet Moambe (Nourriture)

Chaque carte propose les actions suivantes :
- Ajouter au panier
- Ajouter aux favoris

Un survol (hover) agrandit la carte et anime les badges.

## Structure du projet

```
products.html
styles.css
images/
    Smartphone Pro X.jpg
    UltraBook Air.jpg
    Watch Sport 5.jpg
    istockphoto-2281937879-1024x1024.jpg
    Cuisine congolaise.jpg
    Poulet Moambe.jpg
```

## Design et CSS

### Palette couleurs (4 couleurs max)

| Usage       | Couleur     |
|-------------|-------------|
| Primaire    | #1a73e8     |
| Secondaire  | #ff6f00     |
| Fond        | #f5f5f5     |
| Texte       | #222        |

### Caracteristiques CSS

- Cartes 300x400 px avec border-radius et box-shadow
- Transition transform scale(1.05) au survol
- Badges Promo (rouge) et En stock (vert) en position absolue
- Notation par etoiles (★)
- Boutons Ajouter au panier et Favoris
- Badge de categorie en haut de chaque carte

### Selecteurs CSS avances

| Selecteur          | Usage                                    |
|--------------------|------------------------------------------|
| :hover             | Agrandissement carte, rotation badge     |
| :nth-child(n)      | Alternance de categories                 |
| >                  | Ciblage direct des enfants de .card      |
| +                  | Espacement entre les etoiles             |
| ~                  | Mise en forme des etoiles adjacentes     |
| [data-]            | Badge categorie via data-category        |
| #id                | Style unique pour le footer              |

### Responsive

- >= 1024px : grille 3-4 colonnes
- 768px - 1023px : grille 2 colonnes
- <= 767px : 1 colonne centree

### Google Fonts

- Inter (corps de texte)
- Playfair Display (titres)

## Technologies utilisees

- HTML5
- CSS3 (feuille externe unique)
- Google Fonts

## Conformite PROJET 3.2

- HTML5 + CSS3 externe uniquement
- 6 cartes produits (3 requis minimum)
- Dimensions 300x400 px
- box-shadow, border-radius, transition, transform
- Badges Promo et En stock
- Etoiles de notation
- Boutons Ajouter au panier et Favoris
- Google Fonts (Inter + Playfair Display)
- Palette max 4 couleurs
- Selecteurs avances : :hover, :nth-child, >, +, ~, [data-], #id
- Design responsive (3 breakpoints)
