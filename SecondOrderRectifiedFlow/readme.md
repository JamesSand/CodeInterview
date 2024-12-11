# Coding task for Second Order Rectified Flow
> We would like to implement the second order version of Rectified Flow.

## 1 Background

Rectified Flow is a method for generating trajectories from one distrbution to another. Please refer to [its original repo](https://github.com/gnobitab/RectifiedFlow) for more details.

In this code task, we only focus on the toy exmaple of Rectified Flow, which is also [the tutorial notebook](https://colab.research.google.com/drive/1CyUP5xbA3pjH55HDWOA8vRgk2EEyEl_P?usp=sharing) of the original Rectified Flow repo. 

## 2 Task Description

### Stage 1

TODO

### Stage 2

You should find out that first order loss and second order loss are not in the **same scale**. Please try to balance the two losses.

For example, the weighted loss should be like this:

$$
Loss = \lambda_1 \cdot Loss_{fisrt-order} + \lambda_2 \cdot Loss_{second-order}
$$

For simplisity, we recommend you to fix $\lambda_1 = 1$ and adjust $\lambda_2$ to balance those two losses.

## 3 Expected Results

If you finish Stage 1, you should have the following results

<div style="display: flex; justify-content: center; gap: 10px;">
  <img src="images/v2_scatter.png" alt="Figure 1" width="45%">
  <img src="images/v2_traj.png" alt="Figure 2" width="45%">
</div>

If you finish Stage 2, you should have the following results

<div style="display: flex; justify-content: center; gap: 10px;">
  <img src="images/v4_scatter.png" alt="Figure 1" width="45%">
  <img src="images/v4_traj.png" alt="Figure 2" width="45%">
</div>

