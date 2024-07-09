---
title: Generative Modeling with Adaptive IMLE
authors: ["mehran"]
date: 2023-04-24
image:
  focal_point: 'top'
---

We present Adaptive IMLE, a generative modeling approach that covers all the modes and produces high-quality results. Adaptive IMLE is capble of learning from a few samples from scratch without any auxiliary datasets.  We apply our method to the challenging task of few-shot unconditional image generation with as few as 100 data examples.
<!--more-->

Despite their success on large datasets, GANs have been difficult to apply in the few-shot setting, where only a limited number of training examples are provided. Due to mode collapse, GANs tend to ignore some training examples, causing overfitting to a subset of the training dataset, which is small in the first place. A recent method called Implicit Maximum Likelihood Estimation (IMLE) is an alternative to GAN that tries to address this issue. It uses the same kind of generators as GANs but trains it with a different objective that encourages mode coverage. However, the theoretical guarantees of IMLE hold under a restrictive condition that the optimal likelihood at all data points is the same. In this paper, we present a more generalized formulation of IMLE which includes the original formulation as a special case, and we prove that the theoretical guarantees hold under weaker conditions. Using this generalized formulation, we further derive a new algorithm, which we dub Adaptive IMLE, which can adapt to the varying difficulty of different training examples. We demonstrate on multiple few-shot image synthesis datasets that our method significantly outperforms existing methods. Our code is available at https://github.com/mehranagh20/AdaIMLE.

We present Adaptive IMLE, a generative modeling approach that covers all the modes and produces high-quality results. Adaptive IMLE is capble of learning from a few samples from scratch without any auxiliary datasets.  We apply our method to the challenging task of few-shot unconditional image generation with as few as 100 data examples.


<!-- include image coders.jpg -->
<p>
In the following figure, we can see how the Adaptive IMLE algorithm shrinks neighbourhoods around data points in a toy example. You can find a jupyter notebook that includes a basic implementation of Adaptive IMLE here.
</p>
<img src="https://mehranagh20.github.io/AdaIMLE/assets/img/adaptive_imle_training.gif" alt="training" width="50%" center/>

<br/>
<!-- include a citation block in markdown -->
<p>
If you find our work useful in your research, please consider citing:
</p>

```bibtex
@inproceedings{aghabozorgi2023adaimle,
title={Adaptive IMLE for Few-shot Pretraining-free Generative Modelling
},
author={Mehran Aghabozorgi and Shichong Peng and Ke Li},
booktitle={International Conference on Machine Learning},
year={2023}
}
```