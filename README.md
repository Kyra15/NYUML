# NYUML

## Fish Regression Presentation + Analysis:
Goal: Train ML models to predict fish weight using fish dimensions.
https://drive.google.com/file/d/1RQdMNXuNuA_S70IWeoN-lcFDl8531FU5/view?usp=sharing

### Summary:
We took 2 approachs: given the fish height, width, and 3 varying lengths, we wrote 2 models.
- Polynomial regression using estimated fish volume (elliptic cylinder approximation).
- Polynomial multivariable regression using five predictors: Length1, Length2, Length3, Height, Width.
  
Results:
- Ridge regression consistently gave the best trade-off between bias, variance, and runtime.
- Polynomial order 2–3 gave optimal MSE before overfitting occurred.
- Width and height were the strongest predictors of fish weight.

## CIFAR10 Presentation (CNN and GAN) + Analysis:
Goal: Train deep learning models to recognize and generate images of everyday objects using the cifar10 dataset.
https://drive.google.com/file/d/1oL_LgHW-jE-OJzlXchB5OHOiRLKzGNmi/view?usp=sharing

### Summary:
Convolutional Neural Network (CNN)
- Built to classify CIFAR-10 images into one of 10 categories.
- Three convolutional blocks with batch normalization, max pooling, and dropout.
- Dense output layer with softmax activation for multiclass classification.

Generative Adversarial Network (GAN)
- Built to generate grayscale CIFAR-10–like images.
- Comprised of a generator (creates fake images) and a discriminator (distinguishes real vs fake).

Results:
- CNN Image Classification
-   Training ≈ 93%		
-   Testing ≈ 90%	
- GAN Image Generation
-   Generator produced grayscale images with recognizable shapes but poor definition.
-   Images lacked clarity due to limited epochs and GPU constraints.
-   More training time and computational power would likely improve realism.
