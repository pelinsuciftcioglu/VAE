# Variational Auto-Encoders
![image](https://user-images.githubusercontent.com/53939650/144874436-e305dcf4-df7a-4fbf-9390-ffa88d556ce1.png)

Kingma, D. P., Welling, M., & Now Publishers. (2019). An Introduction to Variational
Autoencoders. Foundations and Trends® in Machine Learning, 12(4), 307-392.
arXiv:1906.02691v3 [cs.LG]. 10.1561/2200000056

## Dataset: MNIST and Binary MNIST

Images of handwritten digits of size 28x28. For MNIST, the pixel values are ranging from 0 to 255 in gray-scale, whereas for Binary MNIST the pixel valueas are either 1 or 0. The database and detailed description regarding the images can be accessed from http://yann.lecun.com/exdb/mnist/.

![image](https://user-images.githubusercontent.com/53939650/144875220-3fe13ed9-cc21-4641-8a8d-23b1f55626e8.png)

## Priors Distributions:

For the purpose of reconstruction and data generation, various types of prior distributions are implemented:
- Standard Gaussian Prior
- Mixture of Gaussians Prior (MoG) (Tomczak, 2021)
- VampPrior (Welling & Tomczak, 2018)
- GTM Prior (Tomczak, 2021)

## Likelihood:
Two different types of distributions are used to calculate log-likelihood, and the values represent the number of different values for each pixel, respectively:
- Categorical Distribution: 256
- Benoulli Distribution: 1
