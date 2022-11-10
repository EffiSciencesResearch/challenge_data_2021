## Le jeu de données principal : human_age

Nous avons 4 types d'images : Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. Nous fournissons :
- un ensemble étiqueté : 20000 images (soit Age Old avec écrit "old" ou young avec écrit "young")
- un ensemble non étiqueté : environ 70000 images (taux de mélange de 50%, les 4 types d'images étant présents en proportion égale). 

*human_age* pèse 630 Mo.


## Les toy datasets

Dans le matériel supplémentaire, vous trouverez 2 jeux de données qui sont plus simples à traiter que le jeu de données *human_age*. Dans ces jeux de données, tous les labels sont publics pour permettre aux participants d'itérer plus facilement avant de s'attaquer à *human_age* qui est plus compliqué.

### human_hair

Nous distribuons un jeu de données complémentaire, *human_hair* : à la place de classifier l'age, on classifie la couleur des cheveux qui est une caractéristique beaucoup plus simple à classifier que l'âge.
DivDis obtient 97% de précision sur l'ensemble non étiqueté de *human_hair*.
*human_hair* pèse 14 Mo.


[![human_hair](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)](https://www.effisciences.org/)

### MNIST_embeding

Nous distribuons également *mnist_embed*, qui est le jeu de données le plus simple. Ce jeu de données est construit à partir d’embeddings d’images de MNIST. Les participants sont encouragés à résoudre ce petit problème avant de s'attaquer aux autres jeux de données.

