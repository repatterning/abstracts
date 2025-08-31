# Risks

This page outlines tools under investigation for real-time *areas at risk* identification.

## Rates of Change of River Level

Let 

$$\mathcal{l}_{t}, \: \mathcal{l}_{t - \tau}, \: \mathcal{l}_{t - 2\tau}, \: \mathcal{l}_{t - 3\tau}, \: \ldots$$


represent the time series of a gauge's river level measures, separated by $\tau$ hours, and unit of measure &Rarr; millimetres. Then the weighted-rate-of-change, w.r.t. each $\tau$ hours interval, is


$$r_{t - i\tau} = \frac{1}{\tau} \bigl(\mathcal{l}_{t - i\tau} - \mathcal{l}_{t - (i + 1)\tau}\bigr) \times \frac{1}{\mathcal{l}_{t - (i + 1)\tau}} \bigl(\mathcal{l}_{t - i\tau} - \mathcal{l}_{t - (i + 1)\tau}\bigr) $$

wherein

* $i = 0, 1, 2, 3, \ldots$
* $t\:$ is a/the current time point.
* $r_{t - i\tau}\:$ is the rate of change at time point $t - i\tau$, and its unit of measure is millimetres/hour.

Noting that

$$\frac{1}{\mathcal{l}_{t - (i + 1)\tau}} \bigl(\mathcal{l}_{t - i\tau} - \mathcal{l}_{t - (i + 1)\tau}\bigr)$$

determines the relative river level change w.r.t. consecutive river level values, i.e., values that are $\tau$ hours apart.

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
