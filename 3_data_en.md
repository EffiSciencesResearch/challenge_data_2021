## The main dataset: human_age

[![human_age](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true)](https://www.effisciences.org/)

We have 4 types of images: Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. We provide:
- a labeled set: 20000 images (either Age Old with written "old" or young with written "young")
- an unlabeled set: about 70000 images (mixing rate of 50%, the 4 types of images being present in equal proportion). 

*human_age* weighs 630 Mb and is a variant of the CelebA dataset [5].

## The toy datasets: human_hair

In the supplementary material, you will find the *human_hair* datasets  In this datasets, all labels are public to allow participants to iterate more easily before tackling *human_age* which is more complicated.

In *human_hair*, instead of classifying age, we classify hair color which is a much simpler feature to classify than age.
*human_hair* weighs 14 Mb.


[![human_hair](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)](https://www.effisciences.org/)

## Starting Pack

In order to start working on the two datasets, you can start with the Colab "Starting Pack" which will allow you not to spend time on the infrastructure, data loading and the expected csv format.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1y5X0S9kNiEHijsAfNXmDwIiHZUcUdzjT?usp=sharing]
