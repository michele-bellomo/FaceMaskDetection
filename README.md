# Kaggle Competition: Face Mask Detection

Competition held within the "Artificial Neural Networks and Deep Learning" course, held by professor Matteo Matteucci at Politecnico di Milano in the first semester of the academic year 2020/2021. The challenge consisted in designing an algorithm to classify a set of photos according to the following scenarios:
1) all present wear masks
2) some of those present (but not all) wear masks
3) no one wears masks
I addressed this problem using convolutional neural networks.
Initially I have built from scratch an "ad hoc" architecture.
Subsequently, I have exploited some of the main architectures already trained on Imagenet (VGG, ResNet, Inception...), which I have calibrated through fine tuning to solve this specific task.
The best result was achieved through the "Inception" architecture, to which I added a fully connected layer before the final softmax. The accuracy was 0.95 on the validation set and 0.938 in the Kaggle submission.
The file "" contains the implementation of the architecture designed from scratch, while "" is the code of the best performing algorithm mentioned above. 
