## The main dataset: *human_age*

[<p align="center"><img src="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true" alt="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true" style="width:500px;"/></p>](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true)

<p align="justify">We have 4 types of colored images of size 218x178 pixels: Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. We provide:</p>



- <p align="justify">a labeled set: 20000 images (either Age Old with written "old" or young with written "young") </p>



- <p align="justify">an unlabeled set: about 70000 images (mixing rate of 50%, the 4 types of images being present in equal proportion). </p>

<p align="justify"> <em>human_age</em> weighs 630 Mb and is a variant of the CelebA dataset [5]. </p>

## The toy datasets: *human_hair*

<p align="justify">In the supplementary material, you will find the <em>human_hair</em> datasets  In this datasets, all labels are public to allow participants to iterate more easily before tackling <em>human_age</em> which is more complicated. </p>

<p align="justify">In <em>human_hair</em>, instead of classifying age, we classify hair color which is a much simpler feature to classify than age.
  <em>human_hair</em> weighs 14 Mb.</p>

[<p align="center"><img src="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true" alt="https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true" style="width:500px;"/></p>](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)

## Starting Pack

<p align="justify">In order to start working on the two datasets, you can begin with the Colab "Starting Pack" which will allow you not to spend time on the infrastructure, data loading and the expected csv format.</p>

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1y5X0S9kNiEHijsAfNXmDwIiHZUcUdzjT?usp=sharing)
