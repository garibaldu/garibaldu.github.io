---
layout: post
title: Representation and Prediction
---

> I think real division in machine learning isn’t between supervised and unsupervised, but what I’ll term predictive learning and representation learning. [HIPS blog](https://hips.seas.harvard.edu/blog/)

Firstly, lets go through some definitions.

# Representation learning

> So, why representation is important? The short answer is that “good” representation makes life so much easier, presumably, by reducing the computational burden of doing inference/classification/prediction. [HIPS blog](https://hips.seas.harvard.edu/blog/)

> An algorithm is a systematic way of repeatedly applying mathematical operations to a representation in order to achieve some computational goal. Asking what algorithms a representation supports, therefore, is a matter of asking what mathematical operations can be meaningfully applied to it. [HIPS blog](https://hips.seas.harvard.edu/blog/)

> In representation learning, our goal isn’t to predict observables, but to learn something about the underlying structure. [HIPS blog](https://hips.seas.harvard.edu/blog/)

>  However, a more sensible approach would be to first transform (not necessarily bijectively) the data into a different space via an encoder map $\mathbf{f}:\mathbb{R}^D\rightarrow\mathbb{R}^K$, which we choose to “reshuffle” the information to accentuate interesting patterns in the inputs. [HIPS blog](https://hips.seas.harvard.edu/blog/)


* Predictive learning is when, given the past, you want to guess what the future will be like. (Extrapolations from known data)
* Representation learning is when you want to extract some underlying structure and/or patterns from your data. (Links and relationships between known data points)

Interestingly, both require internal models of their environments.

So, if predictive learning is commonly supervised (regression and classification) and representation learning is commonly unsupervised (clustering and data visualsations), what would _unsupervised predictive learning_ or _supervised representation learning_ look like?




##### Supervised representation learning

Given that we want (Italy) + (Capital) = (Rome), or (royal) + (daughter) = (princess), ...

Word2vec already manages to capture some of these relations. But would a supervised model be better?

In my opinion, we do this a lot. The 'supervision' that these nets get is more at a meta level where the researchers designing the learner supervise the sorts of relation they think is important

##### Unsupervised predictive learning

This is really the ultimate goal. To have a system that we can just place in an environment, where it can gather data, and it eventually learns to predict its environment

*****

Inspired by Roger Grosse's [post](https://hips.seas.harvard.edu/blog/2013/02/04/predictive-learning-vs-representation-learning/) on the HIPS blog.