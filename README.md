# Mushroom Classification
This project focuses on classifying different species of mushrooms using deep learning models, primarily based on the ResNet-18 architecture. Multiple iterations of the model were developed and fine-tuned to achieve the best possible classification accuracy.

## Introduction

The goal of this project is to develop a deep-learning model capable of accurately classifying different species of mushrooms based on image data. This is an important task in fields such as mycology and environmental science, where quick and accurate identification of mushroom species can have significant implications.

## Dataset

The [dataset](https://www.kaggle.com/datasets/maysee/mushrooms-classification-common-genuss-images/data) used for this project consists of images of various mushroom species. The images were preprocessed and augmented to improve model performance. The dataset was split into training, validation, and test sets to evaluate the models effectively.

## Model Architecture

We primarily used the ResNet-18 architecture for this project. Various iterations and modifications were made to the base architecture to explore the effects of different techniques, including:

- Replacing the last fully connected layer to match the number of mushroom classes.
- Adding additional convolutional layers to extract more complex features.
- Fine-tuning all layers of the network for improved performance.
- Using different optimization and learning rate scheduling strategies.

## Experiments

### Model 1: ResNet-18 with Last Layer Replaced and Tuned

This model replaces the final fully connected layer of ResNet-18 to output the correct number of classes for mushroom species. The model was trained with a standard learning rate and weight decay.

### Model 2: ResNet-18 with Three New Layers Added and Tuned

In this iteration, three new fully connected layers were added to the base ResNet-18 model to allow the network to learn more complex representations.

### Model 3: ResNet-18 with All Layers Tuned

Here, we fine-tuned all layers of the ResNet-18 model, allowing the earlier layers to adjust their filters based on the mushroom dataset rather than relying solely on the pre-trained weights.

### Model 4: Model 2 with All Layers Tuned

This model builds on Model 2 by fine-tuning all layers in addition to the added fully connected layers, aiming to further improve performance.

### Model 5: Custom ResNet-18 with Added Convolutional Layers

In this custom model, additional convolutional layers were added to the ResNet-18 architecture to enhance feature extraction. This model went through multiple iterations with different learning rates, data augmentation strategies, and layer configurations.

## Conclusion

The project successfully demonstrated the use of deep learning models, specifically ResNet-18, for mushroom classification. Through various modifications and fine-tuning, the models were able to achieve reasonable accuracy, highlighting the potential of deep learning in this domain.
