---
title: Linear Regression
categories:
- Deep learning , Neural network
feature_image: "https://picsum.photos/2560/600?image=875"
---

*Regression* is a set of methods for estimating the relationships between a `outcome variable` and `features`.

When our input consist of d features, we express our prediction $\hat{y}$ as 
$$\hat{y} = w_1  x_1 + ... + w_d  x_d + b$$

Collecting all features into a vector $\mathbf{x} \in \mathbb{R}^d$ and all weights into a vector $\mathbf{w} \in \mathbb{R}^d$, we can express our model compacity using a dot product:
$$ \hat{y} = \mathbf{w}^T\mathbf{x} +b$$

The vector $\mathbb{x}$ corresponds to features of a single data example. To represent tho whole dataset we use $\mathbf{X} \in \mathbb{R}^{n\times d}$. Here $\mathbf{X}$ contains one row for every example and one column for every feature. The predictions $\mathbf{\hat{y}} \in \mathbb{R}^n$ can be expressed as: 
$$ \mathbf{\hat{y}} = \mathbf{Xw} +b$$

The `Loss function` quantifies the distance between the real and predicted value of the target.
$$ (y - \hat{y})^2 =  \|\mathbf{y} - \mathbf{X}\mathbf{w}\|^2 $$

We need to find $\mathbf{w}$ to minimize the loss function. The analytic solution is:
 $$ (\mathbf{X}^T\mathbf{X})^{-1}\mathbf{X^T}\mathbf{y}$$
