---
title: 'WIMLE: Uncertainty-Aware World Models with IMLE for Sample-Efficient Continuous Control'

authors:
  - mehran
  - yanshu
  - alireza
  - keli

author_notes:

date: '2026-03-25'
doi: ''
publishDate: '2026-03-25'

publication_types: ['paper-conference']

publication: The Fourteenth International Conference on Learning Representations
publication_short: ICLR 2026

abstract: Model-based reinforcement learning can improve sample efficiency by leveraging synthetic rollouts from learned world models, but policy learning often suffers from bias due to compounding model errors. We propose WIMLE, an uncertainty-aware model-based RL approach that uses Implicit Maximum Likelihood Estimation (IMLE) to learn multi-modal stochastic world models. WIMLE captures aleatoric uncertainty through latent-variable sampling, estimates epistemic uncertainty with deep ensembles, and applies uncertainty-weighted learning so each synthetic transition contributes proportionally to model confidence. Evaluated on over 40 continuous-control tasks across DeepMind Control Suite, HumanoidBench, and MyoSuite, WIMLE delivers substantial gains in sample efficiency and asymptotic performance, with state-of-the-art results on challenging humanoid and dog tasks.

summary: WIMLE introduces IMLE-based multi-modal world models and uncertainty-weighted synthetic learning for model-based RL, achieving strong gains on 40+ continuous-control tasks.

tags: []
featured: true

url_pdf: 'https://openreview.net/forum?id=mzLOnTb3WH'
url_code: 'https://github.com/mehranagh20/wimle'
url_dataset: ''
url_poster: ''
url_project: 'https://mehranagh20.github.io/wimle'
url_slides: ''
url_source: 'https://github.com/mehranagh20/wimle'
url_video: ''

image:
  caption: ''
  focal_point: ''
  preview_only: false

projects: []
slides: ''
---

```bibtex
@inproceedings{aghabozorgi2026wimle,
  title={{WIMLE}: Uncertainty-Aware World Models with {IMLE} for Sample-Efficient Continuous Control},
  author={Mehran Aghabozorgi and Yanshu Zhang and Alireza Moazeni and Ke Li},
  booktitle={The Fourteenth International Conference on Learning Representations},
  year={2026},
  url={https://openreview.net/forum?id=mzLOnTb3WH}
}
```
