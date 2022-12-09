<p align="justify"><strong>What if misleading correlations are present in the training dataset?</strong></p>

<p align="justify"> <em> human_age </em> is an image classification benchmark with a distribution change in the unlabeled data: we classify old and young people. Text is also superimposed on the images: either written "old" or "young".
In the training dataset, which is labeled, the text always matches the face.
  But in the unlabeled (test) dataset, the text matches the image in 50% of the cases, which creates an ambiguity. </p>

So we have 4 types of images:



1. Age young, text young (AYTY),

   

2. Age old, text old (AOTO),

   

3. Age young, text old (AYTO),

   

4. Age old, text young (AOTY).

<p align="justify"> Types 1 and 2 appear in both datasets, types 3 and 4 appear only in the unlabeled dataset. </p>

<p align="justify"> To resolve this ambiguity, participants can submit solutions to the leaderboard multiple times, testing different hypotheses (challengers may consider solutions that require two or more submissions to the leaderboard). </p>

<p align="justify">We use the accuracy on the unlabeled set of <em>human_age</em> as our metric.</p>

## Challenge rules

<p align="justify">At the end of the challenge, the different teams will have to send their code to crsegerie@gmail.com with the heading: "Challenge Data - Submission". The awarding of the prize will be conditional on this submission and on compliance of the following rules:</p>



- <p align="justify">Participants are not allowed to label images by hand.</p>

  

- <p align="justify">Participants are not allowed to use other datasets. They are only allowed to use the datasets provided.</p>

  

- <p align="justify">Participants are not allowed to use arbitrary pre-trained models. Only ImageNet pre-trained models are allowed.</p>
