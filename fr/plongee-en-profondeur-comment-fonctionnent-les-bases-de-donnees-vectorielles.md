Source: https://newsletter.theaiedge.io/p/deep-dive-how-do-vector-databases

# Plongée en profondeur : Comment fonctionnent les bases de données vectorielles ?

Les bases de données vectorielles sont souvent utilisées dans les moteurs de recherche en utilisant les représentations vectorielles des éléments que nous essayons de rechercher. Nous examinerons les différents algorithmes qui nous permettent de rechercher des vecteurs parmi des milliards ou des trillions de documents. Dans cette publication, nous couvrons les sujets suivants :  

- Qu'est-ce qu'une base de données vectorielle ?
  - L'émergence des bases de données vectorielles
  - Différentes bases de données vectorielles
- Indexation et recherche dans un espace vectoriel
  - Quantification des produits
  - Hachage sensible à la localité
  - Petit monde hiérarchique navigable
- Mesures de similarité
  - Distance euclidienne
  - Produit en points
  - Similitude en cosinus
- Au-delà de l'indexation

## Qu'est-ce qu'une base de données vectorielle
### L'émergence des bases de données vectorielles

À l'ère de l'IA générative, les bases de données vectorielles se sont multipliées. L'idée derrière les bases de données vectorielles est d'indexer les données avec des vecteurs qui se rapportent à ces données.

![Base de données vectorielle - Schéma 1](img/bdd-vectorielle-schema-1.webp)

Les bases de données vectorielles sont souvent utilisées pour les moteurs de recommandation où nous apprenons les représentations vectorielles des utilisateurs et des articles que nous voulons recommander.

![Base de données vectorielle - Moteur de recommendations](img/bdd-vectorielle-moteur-recommendations.webp)
