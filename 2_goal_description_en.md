## Objectif

What if misleading correlations are present in the training dataset?

*human_age* is an image classification benchmark with a distribution change in the unlabeled data: we classify old and young people. Text is also superimposed on the images: either written "old" or "young".
In the training dataset, which is labeled, the text always matches the face.
But in the unlabeled (test) dataset, the text matches the image in 50% of the cases, which creates an ambiguity.

So we have 4 types of images:
1.  Age young, text young (AYTY)
2.  Age old, text old (AOTO)
3.  Age young, text old (AYTO)
4.  Age old, text young (AOTY)
Types 1 and 2 appear in both datasets, types 3 and 4 appear only in the unlabeled dataset.


To resolve this ambiguity, participants can submit solutions to the leaderboard multiple times, testing different hypotheses (theoretically two submissions should suffice).

We use the accuracy on the unlabeled set of *human_age* as our metric.

## Challenge rules

Effisciences will distribute a prize of 600 euros to the best team.

At the end of the challenge, the different teams will have to send their code to crsegerie@gmail.com with the heading: "Challenge Data - Submission". We will give you general feedbacks on the quality of your code.

- Participants are not allowed to label images by hand.
- Participants are not allowed to use other datasets. They are only allowed to use the datasets provided.
- Participants are not allowed to use arbitrary pre-trained models. Only ImageNet pre-trained models are allowed.

In case of suspected cheating, an oral interview will be requested.
