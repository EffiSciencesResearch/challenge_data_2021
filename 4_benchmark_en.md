The DivDis paper presents a simple baseline to solve these classes of problems. In short, we use multi-headed neural networks, and we use a metric that encourages the heads to use independent information. Once the training is finished, the best head can be selected by testing all the different heads on the validation data.

DivDis obtains 70% of accuracy on the unlabeled set of human_age.

GitHub: https://github.com/yoonholee/DivDis 


1. Armstrong, S; Cooper, J; Daniels-Koch, O; and Gorman, R, “The HappyFaces Benchmark”,” Aligned AI Limited published public benchmark, 2022.
2. D'Amour, Alexander, et al. "Underspecification presents challenges for credibility in modern machine learning." arXiv preprint arXiv:2011.03395 (2020).
3. Amodei, Dario, et al. "Concrete problems in AI safety." arXiv preprint arXiv:1606.06565 (2016).
4. Oakden-Rayner, Luke, et al. "Hidden stratification causes clinically meaningful failures in machine learning for medical imaging." Proceedings of the ACM conference on health, inference, and learning. 2020.
