---
layout: page
title: Mathematical characterization of physiological response to eight human emotions
---
### Intro

Emotions are some strange but also beautiful things for human beings. It could generate art but also even hurt human beings. So, in our projects, we want to use the physiology of human beings(electrodermal signal) to figure out more about emotions.

### Methods

<div style="text-align: center;">
    <img src="image/emotion/1718901312809.png" alt="Descriptive Alt Text">
</div>

- **Sweat secretion model**

<div style="text-align: center;">
  <img src="image/emotion/1718901411747.png" alt="1718901411747" style="zoom:60%;" />
</div>
The sweat secretion will affect the skin conductance measurement. So we built our model based on the sweat secretion model.

The state space model is :

<div style="text-align: center;">
  <img src="image/emotion/1718902066676.png" alt="1718902066676" style="zoom:33%;" />
</div>

- **Parameter Estimation**(Expectation Maximization)
  - E-step
  - M-step
  - Parameter Re-estimation
    - **Re-estimate Window** Setting
    - **Random Gaussian Initialization** with selected Mean and Variance for each arousal event
    - **Setting** Θ3 as a constant, and then re-estimate Θ1 and Θ2

<div style="text-align: center;">
  <img src="image/emotion/1718904109351.png" alt="1718904109351" style="zoom:30%;" />`
</div>

### Statistical Analysis

- Deconvolution results

<div style="text-align: center;">
  <img src="image/emotion/1719005527937.png" alt="1719005527937" style="zoom:30%;" />
</div>
- Boxplots for different emotions

<div style="text-align: center;">
  <img src="image/emotion/1719005716983.png" alt="1719005716983" style="zoom:30%;" />
   <img src="image/emotion/1719005915192.png" alt="1719005915192" style="zoom:30%;" />
 </div>

- L-Norm

<div style="text-align: center;">
  <img src="image/emotion/1719006125480.png" alt="1719006125480" style="zoom:30%;" />
</div>
### Conclusion

1) High θ1 and θ2 and highest L0, L1, L2 norm ⇒ Anger 

2) High θ1 and θ2 and lowest L0, L1, L2 norm ⇒ Hate 

3) Lowest θ1 and θ2 ⇒ No emotion

For the remaining emotions (Grief, Platonic Love, Romantic Love, Joy, Reverence):

1) High θ1 and θ2 and highest L0, L1, L2 norm ⇒ Joy

2) Low θ1 and θ2 and Lowest L0, L1, L2 norm ⇒ Reverence 

3) Grief, Platonic Love, Romantic Love, and Reverence are morechallenging to distinguish, which is consistent with the P-values
