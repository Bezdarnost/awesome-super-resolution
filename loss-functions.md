# Useful loss functions

<details>
<summary>Charbonnier Loss</summary>

**Definition:**

Charbonnier Loss, also known as the Pseudo-Huber Loss, is a smooth approximation to the L1 (absolute difference) Loss. It's less sensitive to outliers than the L2 (squared difference) Loss.

**Formula:**

$$\ \text{CharbonnierLoss(x)}=\sqrt{x^2+\epsilon^2}\ $$
​

**Where:** 

- $\ \epsilon$ is a small constant to ensure smoothness.

**Characteristics:**

- It's convex and continuously differentiable, making it suitable for optimization.
- It behaves like L1 loss for large differences and like L2 loss for small differences, combining the advantages of both.

</details>

<details>
<summary>Perceptual Loss</summary>

**Definition:**

Perceptual Loss, often referred to as feature loss or content loss, is designed to measure the perceptual difference between two images. Instead of comparing pixel values directly, it compares the feature representations of the images as extracted by a pre-trained neural network.

**Formula:**

$$\  \text{PerceptualLoss} = \frac{1}{W \times H \times C} \sum_{i=1}^{W} \sum_{j=1}^{H} \sum_{k=1}^{C} (F_{ijk}^{\text{target}} - F_{ijk}^{\text{generated}})^2 $$


**Where:**

- $\ F^{target}$ and $\ F^{generated}$ are the feature maps of the target and generated images, respectively.
- $\ W, H$ and $\ C$ are the width, height, and number of channels of the feature maps, respectively.

**Characteristics:**

- It emphasizes perceptual and structural similarity over pixel-wise accuracy.
- Often uses features from a pre-trained network (like VGG) to compute the loss.
- Particularly useful in tasks where the exact pixel values are less important than the overall perceptual quality, such as style transfer or super-resolution.

</details>

<details>
<summary>Mean Squared Error (MSE) or L2 Loss</summary>

**Definition:**

MSE Loss measures the average squared difference between the estimated high-resolution image and the ground truth. It emphasizes pixel-wise accuracy.

**Formula:**

$$\ \text{MSE} = \frac{1}{N} \sum_{i=1}^N(y_i−\hat{y}_i)^2 $$

**Where:**

- $\ y_i$ is the pixel value of the ground truth image.
- $\ \hat{y}_i$ is the pixel value of the estimated image.
- $\ N$ is the total number of pixels.

**Characteristics:**

- Provides pixel-wise accuracy.
- Can lead to overly smooth results due to the quadratic penalty for deviations.

</details>





