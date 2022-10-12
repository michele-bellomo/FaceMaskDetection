# Kaggle Competition: Face Mask Detection

Competition carried out during the "Artificial Neural Networks and Deep Learning" course, held by professor Matteo Matteucci at Politecnico di Milano in the first semester of the academic year 2020/2021. The challenge consisted in designing an algorithm to classify pictures according to the following scenarios:
1) all present wear masks
2) some of those present (but not all) wear masks
3) no one wears masks

I addressed this problem using convolutional neural networks.
Initially I tried to use a neutral network whose architecture was built from scratches. The results were good, but not entirely satisfactory.
Subsequently, I have tested neural networks obtained by fine tuning calibration of some of the main architectures avaible on Imagenet (VGG, ResNet, Inception...).

The best result was achieved using the "Inception" architecture, to which a fully connected layer before the final softmax was added. The accuracy was 0.95 on the validation set and 0.938 in the Kaggle submission.

The file "fromScratch.ipynb" contains the implementation of the architecture designed from scratch, while "" is the code of the best performing algorithm based on Inception architecture. 
