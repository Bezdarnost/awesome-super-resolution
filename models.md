<details>
<summary>DiffPIR: Denoising Diffusion Models for Plug-and-Play Image Restoration (05.2023)</summary>

---

**Data of Introduction:**

- May 15, 2023

**Conference:**

- CVPR workshop NTIRE 2023

**Authors:**

- Yuanzhi Zhu, Kai Zhang, Jingyun Liang, Jiezhang Cao, Bihan Wen, Radu Timofte, Luc Van Gool

**Abstract/Description:**

- The paper introduces DiffPIR, a method that integrates traditional plug-and-play image restoration into the diffusion sampling framework. While most existing methods focus on discriminative Gaussian denoisers, this work explores the potential of diffusion models as a generative denoiser prior for plug-and-play image restoration. The proposed approach demonstrates state-of-the-art performance on various image restoration tasks, including super-resolution, image deblurring, and inpainting.

**Main Concepts:**

- Utilization of any off-the-shelf denoiser as an implicit image prior.
- Exploration of diffusion models as a generative denoiser prior.
- Integration of traditional plug-and-play methods into the diffusion sampling framework.

**Architecture & Methods:**

- DiffPIR: A method that combines plug-and-play image restoration with diffusion models.
- Uses diffusion models as generative denoisers, offering a potential improvement over traditional Gaussian denoisers.

**Training Details:**

- Specific training details are not provided in the summary, but the paper likely delves deeper into the training process and parameters.

**Metrics:**

- Metrics related to reconstruction faithfulness and perceptual quality were used, though specific metric names are not mentioned in the summary.

**Datasets:**

- Training: Not explicitly mentioned in the summary.
- Testing: FFHQ and ImageNet datasets were used for evaluation.

**Results & Achievements:**

- DiffPIR achieves state-of-the-art performance on various image restoration tasks.
- Demonstrates superior quality in terms of reconstruction faithfulness and perceptual quality, requiring no more than 100 Neural Function Evaluations (NFEs).

**Code/Implementation:**

- The source code is available at DiffPIR GitHub Repository.

**References:**

- [paper](https://arxiv.org/pdf/2305.08995.pdf)
- [github](https://github.com/yuanzhi-zhu/DiffPIR)

```
@inproceedings{zhu2023denoising, % DiffPIR
      title={Denoising Diffusion Models for Plug-and-Play Image Restoration},
      author={Yuanzhi Zhu and Kai Zhang and Jingyun Liang and Jiezhang Cao and Bihan Wen and Radu Timofte and Luc Van Gool},
      booktitle={IEEE Conference on Computer Vision and Pattern Recognition Workshops (NTIRE)},
      year={2023}
```
  
</details>
