# Chiffrage-Partiel-d-Images
ENSISA 2AIR Projet Cryptographie *

## Sujet : 
Chiffrage Partiel d'Images.
Objectif
Il est des situations où il n'est pas nécessaire (ou même souhaitable) de chiffrer intégralement un fichier. Dans le cas d'une image, il peut n'être utile que de chiffrer une partie de celle-ci. Il vous est demander de concevoir une application Java qui permettra à l'utilisateur de sélectionner une ou plusieurs zones d'une image et de ne chiffrer que cette/ces zone(s). Cette même application devra permettre à un utilisateur possédant la clé d'afficher l'intégralité de l'image, et à un utilisateur ne possédant pas la clé d'afficher la partie apparaissant en clair.

Structure de l'application
Votre application devra être accessible depuis une interface graphique permettant la sélection du fichier image, la spécification des zones à crypter, la spécification de la clé de chiffrage ou la saisie d'un mot de passe d'où sera dérivée cette clé. Favoriser l'usage des composants graphiques swing.

Les zones chiffrées d'une image devront être stockées directement dans le fichier image, et non dans un fichier à part. Ainsi, lorsque ce fichier image sera affiché, par votre application ou par n'importe quelle application permettant de visualiser des images, des pixels de couleurs aléatoires (en apparence) seront affichés dans les zones chiffrées. Cela exclut l'utilisation de formats de fichier utilisant une compression d'image avec perte (les valeurs des pixels contenant des données chiffrées ne devant pas être altérées pour que leur déchiffrage puisse réussir). Le seul format de fichier à utiliser pour l'enregistrement des images chiffrées doit être PNG (Portable Network Graphics).

Les éventuelles informations supplémentaires nécessaires au déchiffrage des zones chiffrées (par exemple, la position et la taille de chaque zone chiffrée) pourront, au besoin, être stockées dans un fichier à part (en aucun cas les données chiffrées, même en partie, ne devront être stockées de cette façon).

Remarque : Même si cela va de soi, il est impératif que le(s) algorithme(s) de chiffrement utilisé(s) fassent partie des algorithmes actuellement considérés comme sûrs, i.e. n'utilisez pas Blowfish, DES, DESede, RC2, RC4, ...

Exemple
Pour un utilisateur ne possédant pas la clé de chiffrage, une image comportant, par exemple, deux zones cryptées pourra s'afficher ainsi :
