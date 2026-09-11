
# Calculateur de Ratio Étiquette / Produit

Outil web permettant de calculer le ratio de couverture d'une étiquette par rapport à la surface totale d'un produit, à partir d'une photo.

## Objectif

Estimer si la taille d'une étiquette sur un packaging respecte un seuil de couverture raisonnable (indicativement, moins de 50% du packaging). Utile notamment dans une logique d'éco-conception, quand la taille d'une étiquette peut impacter le tri optique automatisé des emballages en recyclage.

## Fonctionnement

1. Charger une photo du produit, prise bien de face.
2. Détourer le contour du produit entier en cliquant point par point. Cliquer près du premier point referme la forme.
3. Détourer ensuite le contour de l'étiquette, de la même façon.
4. L'outil calcule automatiquement le ratio entre la surface de l'étiquette et la surface du produit.

## Méthode de calcul

Chaque contour tracé est une liste de points. L'aire du polygone formé par ces points est calculée avec la formule du lacet (shoelace formula), une formule mathématique standard permettant de calculer l'aire d'une forme fermée à partir des coordonnées de ses sommets.

le facteur d'échelle s'annule dans la division, tant que les deux contours sont tracés sur la même photo.

## Limites

- Estimation en 2D uniquement, ne prend pas en compte la courbure d'un contenant cylindrique ou conique.
- Le détourage est manuel, la précision dépend de la personne qui trace les points.

## Confidentialité

Les photos sont traitées localement dans le navigateur de l'utilisateur. Aucune image n'est envoyée ni stockée sur un serveur.

## Utilisation

Ouvrir le lien de la page dans un navigateur, aucune installation nécessaire.


