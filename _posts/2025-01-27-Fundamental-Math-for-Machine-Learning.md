---
layout: distill
title: Fundamental Math for Machine Learning
description: A learning notes of the basic math knowledge and conceptions for machine learning.
tags: Math ML
giscus_comments: true
date: 2025-1-27
featured: true
# mermaid:
#  enabled: true
#  zoomable: true
# code_diff: true
# map: true
# chart:
#  chartjs: true
#  echarts: true
#  vega_lite: true
# tikzjax: true
# typograms: true

# authors:
#  - name: Albert Einstein
#    url: "https://en.wikipedia.org/wiki/Albert_Einstein"
#    affiliations:
#      name: IAS, Princeton


# bibliography: 2018-12-22-distill.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: Linear Regression
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
  - name: Logistic Regression


# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
# _styles: >
#  .fake-img {
#    background: #bbb;
#    border: 1px solid rgba(0, 0, 0, 0.1);
#    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
#    margin-bottom: 12px;
#  }
#  .fake-img p {
#    font-family: monospace;
#    color: white;
#    text-align: left;
#    margin: 12px 0;
#    text-align: center;
#    font-size: 16px;
#  }
---

## Linear Regression

Linear Regression is an algorithm which predicts unknown value with existing data set. It models the factors and results as linear function, for example:

$$  h_\theta (x)=\theta_0 + \theta_1x1 + \theta_2x2 $$

where $x_1,x_2$ are the **factors** which affect the result $h_\theta (x)$. $x_1,x_2$ are also called **features** in deep learning. 
$\theta_0, \theta_1,\theta_2$ are the parameters or **weights** in deep learning, which are supposed to be fixed during the prediction or **inference**. 

If we let $x_0$=1, then we can write the above equation in a more general form as

$$  h_\theta (x) =\sum_{i=1}^{n}\theta_ix_i=\mathbf{\theta}^T\mathbf{x}  $$

where

$$
  \mathbf{\theta} = \begin{bmatrix} \theta_0
                                \\  \theta_1
                                \\  ...
                                \\  \theta_n
                                \\
                     \end{bmatrix}
 ,   \mathbf{x} = \begin{bmatrix}   x_0
                                \\  x_1
                                \\  ...
                                \\  x_n
                                \\
                     \end{bmatrix}
$$

Given an concrete example: we suppose the house price is highly related to 1. area, and 2. number of bedroom, how can we predict the price given its area and number of bedrooms?

| Living area ($ft^2$)  |  #bedrooms  | price (k) |
| ------------------  |  ---------- | --------  |
| 2104                |  3          | 400       |
| 1600                |  3          | 330       |
| 2400                |  3          | 369       |
| 1416                |  2          | 232       |
| 3000                |  4          | 540       |
| ...                 |  ...        | ...       |

In this example:
$x_1$ is the living area, $x_2$ is the number of bedrooms, **y** is the price of the house.

The table about is called a **training set**, which will be used to training our model (that is the value of $\theta$s).

The straight thought is to choose the hypnosis **h(x)** close to the training data **y**.

This can be expressed with **cost function**. There can be many types of cost functions, the most popular one is least-squares cost function:

$$ J(\theta) = \frac{1}{2}\sum_{i=1}^{n} (h_\theta(x^i) - y^i)^2 $$

### Gradient Descent Algorithm

Gradient Descent Algorithm is used to find the value of $\theta$ so that the $J(\theta)$ is minimized, which can be described as following:

$$ \theta_j := \theta_j - \alpha \frac{\delta J(\theta ) }{\delta \theta_j} $$

Here $\delta$ is called **learning rate**.

Expend the $J(\theta)$ we can get the update equation:

$$ \theta_j := \theta_j + \alpha \sum_{i=1}^{m} (y^i - h_\theta(x^i))x_j^i $$  

where **i** is the index of data sets, **j** is the index of **features** 

#### batch gradient descent
In the above method, we look at every example in the entire training set on every step, and is called **batch gradient descent**

---


