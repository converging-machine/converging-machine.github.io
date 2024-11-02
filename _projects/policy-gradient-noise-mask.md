---
layout: page
title: policy gradient driven noise mask
description: a novel pretraining pipeline for medical image classification using reinforcement learning
img: noise-mask
importance: 3
category: reinforcement-learning
---
## Overview

Policy Gradient-Driven Noise Mask introduces a novel pretraining pipeline that generates conditional noise masks to enhance deep learning classifier performance on heterogeneous multi-modal and multi-organ biomedical datasets[1]. The system employs a dual-component reinforcement learning architecture with a lightweight policy network and classifier network.

## Key Features

- **Adaptive Noise Masking**: Generates image-specific noise masks that account for variations in modality and organ type[1]
- **Lightweight Architecture**: Uses ResNet-10t as policy network and ResNet-50 as classifier network[1]
- **Two-Phase Training**: Separates noise mask generation (pretraining) from final model fine-tuning[1]

## Performance

The system demonstrates significant improvements over baseline models:

|Model|Precision|Recall|F1 Score|ROC|B.Acc.|
|--|--|--|--|--|--|
|Baseline|0.5929|0.5014|0.5226|0.9884|0.5014|
|With Policy Gradient|0.6034|0.5211|0.5468|0.9900|0.5211|

Key results include:
- Superior performance on 11 out of 13 medical imaging datasets[1]
- Particularly strong results on small-scale datasets
- Improved generalization to unseen medical imaging concepts

## Resources

- [GitHub Repository](https://github.com/converging-machine/Policy-Gradient-Driven-Noise-Mask)
- [Hugging Face Model](https://huggingface.co/converging-machine/Policy-Gradient-Noise-Mask)
- [Paper on arXiv](https://arxiv.org/abs/2406.14568)

## Citation

```bibtex
@article{yavuz2024policy,
  title={Policy Gradient-Driven Noise Mask},
  author={Yavuz, Mehmet Can and Yang, Yang},
  year={2024},
  eprint={2406.14568},
  archivePrefix={arXiv},
  primaryClass={eess.IV}
}
