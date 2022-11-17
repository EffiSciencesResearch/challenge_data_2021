## The main dataset: human_age

[![human_age](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_age.png?raw=true)](https://www.effisciences.org/)

We have 4 types of images: Age Young Text Old (AYTO), Age Young Text Young (AYTY), etc. We provide:
- a labeled set: 20000 images (either Age Old with written "old" or young with written "young")
- an unlabeled set: about 70000 images (mixing rate of 50%, the 4 types of images being present in equal proportion). 

*human_age* weighs 630 Mb.


## The toy datasets

In the supplementary material, you will find 2 datasets that are easier to process than the *human_age* dataset. In these datasets, all labels are public to allow participants to iterate more easily before tackling *human_age* which is more complicated.

### human_hair

We distribute a complementary dataset, *human_hair*: instead of classifying age, we classify hair color which is a much simpler feature to classify than age.
DivDis gets 97% accuracy on the unlabeled set of *human_hair*.
*human_hair* weighs 14 Mb.


[![human_hair](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/human_hair.png?raw=true)](https://www.effisciences.org/)

### MNIST_embeding

We also distribute *mnist_embed*, which is the simplest dataset. This dataset is built from MNIST image embeddings. Participants are encouraged to solve this small problem before tackling the other datasets.

