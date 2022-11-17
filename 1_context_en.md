## Case study
*Why did a network trained to identify collapsed lungs end up detecting chest drains?*

[![Chest_drains](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/chest_drain.png?raw=true)](https://www.sciencedirect.com/science/article/pii/S2589750020302193)

*Above: X-ray of a patient with two chest tubes (both long tubes) - a treatment for collapsed lungs. Chest drains are visually much simpler than collapsed lungs, and the two features are correlated, so a classifier could perform well by learning to identify the simpler feature, but would not perform well on a patient before surgery.*


Indeed, the learning data did not help distinguish true collapsed lungs from chest drains - a treatment for collapsed lungs. Chest drains are visually much simpler than collapsed lungs and the two features were correlated, so the algorithm was able to perform well by learning to identify the simpler feature.

Classifiers typically learn the simplest feature that predicts the label, whether or not it matches what the humans had in mind. Human monitoring can sometimes detect this error, but it is slow, expensive, and not completely reliable (because the human may not realize what the algorithm is doing until a potentially dangerous error is made).

Detecting the "wrong" feature means that the classifier will fail to generalize as expected - when deployed on x-rays of real humans with real, untreated collapsed lungs, it will classify them as healthy, since they do not have a chest tube.

## Context in the literature

This challenge is related to underspecification problems (D'Amour et al., 2020) in which multiple hypothesis can explain the data. As well as the problem of robustness to distributional changes (Amodei et al., 2016). For example, classifiers trained to recognize the lungs of hospitalized patients with and without pneumothorax cannot be used preemptively on untreated patients because the classifier will recognize the chest drain (an easily identifiable straight line) and not the causative features of the disease (Oakden-Rayner et al., 2020). This problem is quite general and is likely to arise whenever an ML algorithm is to be used on data that is different from the training data (selection bias: labeled data is generally simpler than unlabeled data and simpler than the data encountered in production). For example, in the field of sustainable development, most ML models are trained on a sample of rich countries that are very different from the countries where the model will be deployed. In general, we want to use past data to predict the future, but the future is not the past.
