# Resisting Adversarial Attacks by k-Winners-Take-All
**CS4803/7643 Deep Learning (Spring 2020) Final Project and candidate for ICLR Reproducibility Challenge**

**By Baran Usluel, Ilya Golod**

**[Final Report](/CS7643_Final_Report.pdf)**

### Abstract

The goal of our project was to demonstrate the reproducibility
of the ICLR 2020 paper ["Enhancing Adversarial Defense by k-Winners-Take-All"](https://arxiv.org/abs/1905.10510)
(Chang Xiao, Peilin Zhong and Changxi Zheng). We have
shown that usage of the [k-Winners-Take-All (k-WTA) activation
function](https://github.com/a554b554/kWTA-Activation)
instead of ReLU does indeed significantly increase
a model’s robustness against white-box adversarial
attacks even without adversarial training, without a significant
decline in its accuracy. We have applied the method
proposed by Xiao et al. to two models including one that was not
featured in the original paper, as well as multiple adversarial
attacks. In all these experiments, models with k-WTA
activation outperformed the conventional ones, thus demonstrating
the method’s reproducibility. Furthermore, we have
discovered a significant overhead with using k-WTA compared
to ReLU in training and prediction time not mentioned
in the original work, and propose a workaround to
address this limitation.

### Requirements

- pytorch
- torchvision
- foolbox
- numpy
- matplotlib

### Notes

We have included our trained models under the models directory.
This should allow for the reproduction of our results with minimal effort.
We ran the Jupyter notebook on Google Colab, but it can be run locally as well.
