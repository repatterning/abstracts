# Drift

For time series drift calculations, this hub depends on

* Jensen-Shannon Distance $J_{dist}$
* Wasserstein Distance $\mathcal{W}$

<br>wherein

$$J_{dist} = \sqrt{J_{div}}$$

$J_{div}$ is the Jensen-Shannon Divergence, a method for determining the similarity of a pair of distributions[^1].  The similarity between a pair of distributions increases as $J_{dist} \rightarrow 0$.  Note, for a pair of distributions

$$J_{div} \in [0 \quad 1]$$

therefore

$$J_{dist} \in [0 \quad 1]$$

The Wasserstein Distance <b>is</b> a distance measure[^2].

Important, do not consider scores in isolation, also consider the pattern of the scores over time.

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>

[^1]: Study <a href="https://ieeexplore.ieee.org/document/61115" target="_blank">Divergence Measures Based on Shannon Entropy</a> for an in-depth understanding of Jensen-Shannon Divergence.
[^2]: Part 6 of <a href="https://arxiv.org/pdf/1904.08994" target="_blank">From GAN to WGAN</a> has an in-depth discussion of the Wasserstein Distance.  <span style="color: #a3a0a0">GAN: Generative Adversarial Network, WGAN: Wasserstein Generative Adversarial Network</span>
