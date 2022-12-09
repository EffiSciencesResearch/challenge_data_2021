## Le jeu de données principal : *human_age*

[<p align="center"><img src="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true" alt="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true" style="width:500px;"/></p>](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true)

<p align="justify">Nous avons 4 types d'images colorées de taille 218x178 pixels : Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. Nous fournissons :</p>



- <p align="justify">un ensemble étiqueté : 20000 images (soit Age Old avec écrit "old" ou young avec écrit "young")</p>

  

- <p align="justify">un ensemble non étiqueté : environ 70000 images (taux de mélange de 50%, les 4 types d'images étant présents en proportion égale). </p>

<p align="justify"> <em>human_age</em> pèse 630 Mo et est une variante du dataset CelebA [5].</p>

## Le toy dataset : *human_hair*

<p align="justify">Dans le matériel supplémentaire, vous trouverez le jeu de données <em>human_hair</em>. Dans ce jeu de données, tous les labels sont publics pour permettre aux participants d'itérer plus facilement avant de s'attaquer à <em>human_age</em> qui est plus compliqué.</p>

<p align="justify">Dans <em>human_hair</em>, au lieu de classifier l'âge, nous classifions la couleur des cheveux qui est une caractéristique beaucoup plus simple à classifier que l'âge.
  <em>human_hair</em> pèse 14 Mo.</p>

[<p align="center"><img src="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true" alt="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true" style="width:500px;"/></p>](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)

## Starting Pack

<p align="justify">Afin de commencer à travailler sur les deux jeux de données, vous pouvez reprendre le Colab "Starting Pack" qui vous permettra de ne pas perdre de temps sur l'infrastructure, le chargement des données et le format csv attendu.</p>

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1y5X0S9kNiEHijsAfNXmDwIiHZUcUdzjT?usp=sharing)
