# Confusion-Matrix-Driven-Evaluation-of-ResNet-50-for-Lung-and-Colon-Cancer-Classification

I implemented Confusion Matrix an evaluation metric on the pretrained ResNet-50 model to expose it's per-class misclassification patterns.

# Dataset description
The dataset used was the LC25000, which contains 25,000 histopathological images with 5 classes gotten off kaggle. All images are 768 x 768 pixels in size in a jpeg file format but resized to 224 x224 (Image Net).

# Model
The model used was a pretrained ResNet-50 with all layers frozen except the final fully connected layer and was retrained on LC25000 for 5-class classification

# Evaluation
- Accuracy:- The model was trained over 15 epochs and had an accuracy of 95.91 on the final epoch of the training set and a test accuracy of 96.56, showin strong  generalization without overfitting.
- Confusion matrix:-  I implemented a Confusion Matrix on the pretrained ResNet-50 model to expose per-class misclassification patterns across all 5 classes (Colon adenocarcinoma, colon benign, lung adenocarcinoma, lung benign and lung squamous cell carinoma each containing 500 test images).
  Lung benign achieved the strongest classification performace, while the performance of lung squamous cell carcinoma was quite low with the model frequently confusing it with lung adenocarcinoma.  This might be likely due to the visual similarity between the two classes.
