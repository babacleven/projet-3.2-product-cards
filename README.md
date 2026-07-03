# PROJET 3.2 - Cartes Produits

Niveau : Intermediaire  
Technologies : HTML5 + CSS3 externe

## Description

Page de presentation de produits inspiree du style Amazon / Jumia avec 6 cartes produits (300×400 px). Chaque carte affiche une image, un titre, une description, un prix, des etoiles de notation, des badges (Promo / En stock / Nouveau), et des boutons d'action.

## Installation

1. Cloner le depot :
   ```
   git clone https://github.com/babacleven/projet-3.2-product-cards.git
   ```
2. Ouvrir `products.html` dans un navigateur moderne.

Aucune dependance ni serveur requis.

## Contenu

| # | Produit | Categorie | Prix |
|---|---------|-----------|------|
| 1 | Smartphone Pro X | Electronique | 749 000 FCFA |
| 2 | UltraBook Air | Electronique | 1 249 000 FCFA |
| 3 | Watch Sport 5 | Electronique | 299 000 FCFA |
| 4 | Pagne traditionnel | Vetements | 45 000 FCFA |
| 5 | Cuisine congolaise | Livres | 22 500 FCFA |
| 6 | Poulet Moambe | Nourriture | 12 000 FCFA |

Chaque carte propose :
- **Ajouter au panier**
- **Ajouter aux favoris**

## Structure

```
products.html
styles.css
images/
    smartphone-pro-x.jpg
    ultrabook-air.jpg
    watch-sport-5.jpg
    istockphoto-2281937879-1024x1024.jpg
    cuisine-congolaise.jpg
    poulet-moambe.jpg
```

## Design

### Palette (4 couleurs)

| Usage | Couleur |
|-------|---------|
| Primaire | #2563eb |
| Secondaire | #f59e0b |
| Fond | #e9ecef |
| Texte | #1e293b |

### Selecteurs CSS avances

:first-child / :last-child, :nth-child, :hover, >, +, ~, [data-category], [data-discount], [id]

### Responsive

- ≥ 1025px : grille multi-colonnes (auto-fill 300px)
- 641-1024px : 2 colonnes
- ≤ 640px : 1 colonne centree

### Google Fonts

- Inter (corps)
- Playfair Display (titres, logo)

## Modifications effectuees

| Erreur | Correction |
|--------|------------|
| Cartes responsives | Dimensions fixes 300×400 px |
| Slashs finaux `/>` sur elements voids | Remplacement par `>` (HTML5) |
| `aria-label` sur `<div>` sans role | Ajout `role="button" tabindex="0"` |
| Espaces dans noms de fichiers images | Renommage (ex: `smartphone-pro-x.jpg`) |
| Image "Poulet roti.jpg" inexistante | Remplacement par `poulet-moambe.jpg` |
| Texte "Meilleure vente" | Renommage en "Vente" |
| Boutons coupes par overflow | Image 160px + description tronquee 2 lignes |
