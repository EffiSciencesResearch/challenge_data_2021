# The main dataset: Human_Age

We have 4 types of images: Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. We give:
- a labeled set : 20000 images (either Age old with “old” or young with written “young”)
- an unlabeled set : circa 70000 images (50% mix rate, all 4 types of images present in equal proportion). 

*human_age* weighs 630 Mo.


# The toy datasets: human_hair and the MNIST_embeding datasets

In the supplementary material you will find 2 datasets which are of simpler level than the *human_age* dataset.

## human_hair

We distribute a complementary dataset, *human_hair*, with all the labels public to allow participants to iterate more easily before tackling human_age which is more complicated.
DivDis obtains 97% of accuracy on the unlabeled set of *human_hair*.
*human_hair* weighs 14 Mo.

[![human_hair](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)](https://www.effisciences.org/)

## MNIST_embeding datasets

We also distribute *mnist_embed*, which is the simplest dataset. Participants are encouraged to try to solve this problem before embarking on the other datasets.