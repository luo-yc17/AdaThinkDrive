<div align="center">
<h3>[🎉ICRA 2026] AdaThinkDrive: Adaptive Thinking via Reinforcement Learning for Autonomous Driving </h3>

Yuechen Luo<sup>1,2\*</sup>, Fang Li<sup>2\*</sup>, Shaoqing Xu<sup>2\*,‡</sup>, Zhiyi Lai<sup>2</sup>, Lei Yang<sup>4</sup>, Qimao Chen<sup>1,2</sup>, Ziang Luo<sup>1</sup>, Zixun Xie<sup>2,5</sup>, Shengyin Jiang<sup>2</sup>, Jiaxin Liu<sup>1,2</sup>, Long Chen<sup>2</sup>, Bing Wang<sup>2</sup>, Zhi-xin Yang<sup>3,✉</sup>

<sup>1</sup> Tsinghua University, <sup>2</sup> Xiaomi EV, <sup>3</sup> University of Macau, <sup>4</sup> Nanyang
Technological University, <sup>5</sup> Peking University

(\*) Equal contribution. (‡) Project leader. (✉) Corresponding author.

<a href="https://arxiv.org/abs/2509.13769"><img src='https://img.shields.io/badge/arXiv-AdaThinkDrive-red' alt='Paper PDF'></a>
</div>

## Abstract

While reasoning technology like Chain-of-Thought (CoT) has been widely adopted in Vision-Language-Action (VLA) models, it demonstrates promising capabilities in end-to-end autonomous driving. However, recent efforts to integrate CoT reasoning often fall short in simple scenarios, introducing unnecessary computational overhead without improving decision quality. To address this, we propose AdaThinkDrive, a novel VLA framework with a dual-mode reasoning mechanism inspired by fast and slow thinking. First, our framework is pretrained on large-scale autonomous driving (AD) scenarios using both question-answering (QA) and trajectory datasets to acquire world knowledge and driving commonsense. During supervised fine-tuning (SFT), we introduce a two-mode dataset—fast answering (w/o CoT) and slow thinking (with CoT), enabling the model to distinguish between scenarios that require reasoning. Furthermore, an Adaptive Think Reward strategy is proposed in conjunction with the Group Relative Policy Optimization (GRPO), which rewards the model for selectively applying CoT by comparing trajectory quality across different reasoning modes. Extensive experiments on the Navsim benchmark show that AdaThinkDrive achieves a PDMS of 90.3, surpassing the best vision-only baseline by 1.7 points. Moreover, ablations show that AdaThinkDrive surpasses both the never-Think and always-Think baselines, improving PDMS by 2.0 and 1.4, respectively. It also reduces inference time by 14% compared to the always-Think baseline, demonstrating its ability to balance accuracy and efficiency through adaptive reasoning.

## Overview
<div align="center">
<img src="assets/main.jpg" width="1000">
</div>

## News

`[2026/01/31]` AdaThinkDrive is accepted by **ICRA 2026**🎉🎉🎉!

## Currently Supported Features

- [ ] AdaThinkDrive Inference Code
- [ ] AdaThinkDrive Checkpoint
- [ ] AdaThinkDrive Training Code
- [ ] Training Dataset


## Citation
If this work is helpful for your research, please consider citing:

```
@article{luo2025adathinkdrive,
  title={Adathinkdrive: Adaptive thinking via reinforcement learning for autonomous driving},
  author={Luo, Yuechen and Li, Fang and Xu, Shaoqing and Lai, Zhiyi and Yang, Lei and Chen, Qimao and Luo, Ziang and Xie, Zixun and Jiang, Shengyin and Liu, Jiaxin and others},
  journal={arXiv preprint arXiv:2509.13769},
  year={2025}
}
```
