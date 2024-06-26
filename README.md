# Project Report: Comparative Analysis of CNN, Faster R-CNN, AlexNet, and Vision Transformer for MNIST Classification

## Introduction
The objective of this project was to explore different neural network architectures for computer vision tasks, specifically focusing on classifying the MNIST dataset. Four models were investigated: Convolutional Neural Network (CNN), Faster R-CNN, AlexNet, and Vision Transformer (ViT). Each model was trained and evaluated based on various metrics including accuracy, F1 score, training time, and prediction performance.

## Image Description
<div style="text-align:center;">
    <img src="https://previews.123rf.com/images/moji1980/moji19801210/moji1980121000088/15691005-4-handwritten-watercolor-number-isolated-on-white-background.jpg" alt="Handwritten Watercolor Number" width="200" height="200">
</div>

The image above displays a handwritten watercolor number isolated on a white background. This image serves as an example of the type of data our models are trained to predict values for. In this project, we focus on classifying similar handwritten digits as part of the MNIST dataset, which comprises grayscale images of handwritten digits ranging from 0 to 9. The goal is to train various neural network architectures to accurately predict the numerical value depicted in such images.


## Part 1: CNN vs. Faster R-CNN vs. AlexNet
| Model   | Data Size          | Epochs | L.Rate        | Mode | Time     | Accuracy | F1 Score | Prediction "4" | Probability      |
|---------|--------------------|--------|---------------|------|----------|----------|----------|-----------------------------------|-------------|
| CNN     | All Data           | 10     | 0.001         | CPU  | 4 min    | 98.88%   | 0.99     | 9                                 | 68.73%      |
| R-CNN   | All Data           | 3      | 0.001         | CPU  | 3 min    | 98.58%   | 0.99     | 4                                 | 95.79%      |
| AlexNet | 500 Samples        | 3      | 0.001         | CPU  | 6 min 33s| 13.71%   | 0.05     | 7                                 | 19.03%      |

## Part 2: Vision Transformer (ViT)
| Model | Data Size          | Epochs | L.Rate        | Mode | Time | Accuracy | F1 Score | Prediction "4"                    | Probability |
|-------|--------------------|--------|---------------|------|------|----------|----------|-----------------------------------|-------------|
| ViT   | All Data           | 2      | 0.01          | CPU  | 7 min| 65.35%   | 0.63     | 1                                 | 22.90%      |

## Conclusion
- **CNN and Faster R-CNN** achieved high accuracy and F1 scores, with CNN slightly outperforming Faster R-CNN in terms of accuracy.
- **AlexNet** performed poorly compared to CNN and Faster R-CNN, indicating that deeper architectures may not always lead to better results, especially with smaller datasets.
- **Vision Transformer (ViT)** showed promising results but lagged behind CNN and Faster R-CNN in terms of accuracy and F1 score. However, considering its recent emergence and the potential for further optimization, it could become more competitive in the future.
- **Overall**, CNN and Faster R-CNN demonstrated superior performance for the MNIST classification task, while ViT shows potential for further exploration and improvement.
