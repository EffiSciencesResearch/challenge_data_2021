[![DivDis](https://github.com/EffiSciencesResearch/challenge_data_ens_2023/blob/main/assets/DivDis.png?raw=true)](https://github.com/yoonholee/DivDis)

Le papier DivDis présente un algorithme simple pour résoudre ces problèmes d'ambiguïté. DivDis utilise des réseaux de neurones à têtes multiples, et une loss qui encourage les têtes à utiliser des informations indépendantes. Une fois l'apprentissage terminé, la meilleure tête peut être sélectionnée en testant toutes les têtes différentes sur les données de validation.

DivDis obtient une précision de 64% sur l'ensemble non étiqueté de *human_age* lorsque l'on entraîne sur un subset du jeu de donnée et obtient 97% de précision sur l'ensemble non étiqueté de *human_hair*.

GitHub : https://github.com/yoonholee/DivDis


1. Armstrong, S; Cooper, J; Daniels-Koch, O; and Gorman, R, “The HappyFaces Benchmark”,” Aligned AI Limited published public benchmark, 2022.
2. D'Amour, Alexander, et al. "Underspecification presents challenges for credibility in modern machine learning." arXiv preprint arXiv:2011.03395 (2020).
3. Amodei, Dario, et al. "Concrete problems in AI safety." arXiv preprint arXiv:1606.06565 (2016).
4. Oakden-Rayner, Luke, et al. "Hidden stratification causes clinically meaningful failures in machine learning for medical imaging." Proceedings of the ACM conference on health, inference, and learning. 2020.
5. Liu, Ziwei, et al. "Large-scale celebfaces attributes (celeba) dataset." Retrieved August 15.2018 (2018): 11.
