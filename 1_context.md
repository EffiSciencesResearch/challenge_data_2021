## Description du problème en une minute

Certains jeux de données ne sont pas bien spécifiés : prenons l'exemple d'un jeu de données qui contiendrait des images de chameaux dans le désert, ainsi que des images de vaches dans des prairies. Le classificateur doit classer les images de chameaux et les images de vaches. Mais le classificateur pourrait apprendre à classer les images non pas en fonction de l'animal, mais en fonction du paysage : le jeu de données est *sous-spécifié* car nous avons deux caractéristiques qui sont parfaitement corrélées (l'animal et le paysage). En d'autres termes, le classificateur peut décider de classer soit vache/chameau, soit prairie/désert. Et il y a ambiguïté lorsque nous essayons de classifier l'image d'un chameau dans une prairie. L'objectif de ce sujet est de résoudre ce type d'ambiguïtés. 


## Etude de cas
*Pourquoi un réseau entraîné à identifier des poumons affaissés a-t-il fini par détecter des drains thoraciques (les câbles) ?*

[![Chest_drains](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/chest_drain.png?raw=true)](https://www.sciencedirect.com/science/article/pii/S2589750020302193)

*Ci-dessus : Radiographie d'un patient avec deux drains thoraciques (les deux longs tubes) - un traitement pour les poumons affaissés. Les drains thoraciques sont visuellement beaucoup plus simples que les poumons affaissés et les deux caractéristiques sont corrélées, de sorte qu'un classificateur pourrait obtenir de bons résultats en apprenant à identifier la caractéristique la plus simple, mais ne serait pas performant sur un patient avant l'opération.*


En effet, les données d'apprentissage ne permettaient pas de distinguer les véritables poumons affaissés des drains thoraciques - un traitement pour les poumons affaissés. Les drains thoraciques sont visuellement beaucoup plus simples que les poumons affaissés et les deux caractéristiques étaient corrélées, de sorte que l'algorithme a pu obtenir de bons résultats en apprenant à identifier la caractéristique la plus simple.

Les classificateurs apprennent généralement la caractéristique la plus simple qui permet de prédire l'étiquette, qu'elle corresponde ou non à ce que les humains avaient en tête. La surveillance humaine peut parfois détecter cette erreur, mais elle est lente, coûteuse et n'est pas totalement fiable (car l'homme peut ne pas se rendre compte de ce que fait l'algorithme avant qu'une erreur potentiellement dangereuse ne soit commise).

La détection de la "mauvaise" caractéristique signifie que le classificateur ne parviendra pas à généraliser comme prévu - lorsqu'il est déployé sur des radiographies de vrais humains avec de vrais poumons affaissés, non traités, il les classera comme sains, puisqu'ils n'ont pas de drain thoracique.

## Contexte dans la littérature

Ce défi est lié aux problèmes de sous-spécification (D'Amour et al., 2020) dans lesquels plusieurs hypothèses peuvent expliquer les données. Ainsi qu'au problème de robustesse aux changements de distribution (Amodei et al., 2016). Par exemple, des classificateurs entraînés à reconnaître les poumons de patients hospitalisés avec et sans pneumothorax ne peuvent pas être utilisés de manière préventive sur des patients non traités car le classificateur reconnaîtra le drain thoracique (une ligne droite facilement identifiable) et non les caractéristiques causales de la maladie (Oakden-Rayner et al., 2020). Ce problème est assez général et est susceptible de se poser dès qu'un algorithme ML doit être utilisé sur des données différentes des données d'entraînement (biais de sélection : les données étiquetées sont généralement plus simples que les données non étiquetées et plus simples que les données rencontrées en production). Par exemple, dans le domaine du développement durable, la plupart des modèles ML sont entraînés sur un échantillon de pays riches très différents des pays où le modèle sera déployé. En général, nous voulons utiliser les données du passé pour prédire l'avenir, mais l'avenir n'est pas le passé.
