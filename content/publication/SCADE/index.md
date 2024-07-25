---
title: 'SCADE: NeRFs from Space Carving with Ambiguity-Aware Depth Estimates'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - mikacuy
  - Ricardo Martin-Brualla
  - Leonidas Guibas
  - keli

# Author notes (optional)
author_notes:

date: '2023-03-23'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-03-23'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: Conference on Computer Vision and Pattern Recognition 2023
publication_short: CVPR 2023

abstract: Neural radiance fields (NeRFs) have enabled high fidelity 3D reconstruction from multiple 2D input views. However, a well-known drawback of NeRFs is the less-than-ideal performance under a small number of views, due to insufficient constraints enforced by volumetric rendering. To address this issue, we introduce SCADE, a novel technique that improves NeRF reconstruction quality on sparse, unconstrained input views for in-the-wild indoor scenes. To constrain NeRF reconstruction, we leverage geometric priors in the form of per-view depth estimates produced with state-of-the-art monocular depth estimation models, which can generalize across scenes. A key challenge is that monocular depth estimation is an ill-posed problem, with inherent ambiguities. To handle this issue, we propose a new method that learns to predict, for each view, a continuous, multimodal distribution of depth estimates using conditional Implicit Maximum Likelihood Estimation (cIMLE). In order to disambiguate exploiting multiple views, we introduce an original space carving loss that guides the NeRF representation to fuse multiple hypothesized depth maps from each view and distill from them a common geometry that is consistent with all views. Experiments show that our approach enables higher fidelity novel view synthesis from sparse views. 

# Summary. An optional shortened abstract.
summary: We present SCADE, a novel technique for NeRF reconstruction under sparse, unconstrained views for in-the-wild indoor scenes. We leverage on generalizable monocular depth priors and address to represent the inherent ambiguities of monocular depth by exploiting our ambiguity-aware depth estimates (leftmost). Our approach accounts for multimodality of both distributions using our novel space carving loss that seeks to disambiguate and find the common mode to fuse the information between different views.


tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2303.13582'
url_code: 'https://github.com/mikacuy/scade'
url_dataset: ''
url_poster: 'https://scade-spacecarving-nerfs.github.io/assets/scade_cvpr23_poster_final.pdf'
url_project: 'https://scade-spacecarving-nerfs.github.io'
url_slides: 'https://scade-spacecarving-nerfs.github.io/assets/scade_final_slides.pdf'
url_source: 'https://scade-spacecarving-nerfs.github.io'
url_video: 'https://youtu.be/5XwWZn-kjBU'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - PAPR

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

<!-- {{% callout note %}}
Click the _Cite_ button above.
{{% /callout %}} -->


<!-- Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).

<iframe width="100%" height="315"
src="https://youtube.com/embed/xKt6YYY4hq8">
</iframe>

<!-- include image coders.jpg -->
<!-- <p>
In the following figure, we can see how the Adaptive IMLE algorithm shrinks neighbourhoods around data points in a toy example. You can find a jupyter notebook that includes a basic implementation of Adaptive IMLE here.
</p> -->
<!-- <img src="https://mehranagh20.github.io/AdaIMLE/assets/img/adaptive_imle_training.gif" alt="training" width="50%" center/> -->

<!-- <br/> -->
<!-- include a citation block in markdown -->
<!-- <p>
If you find our work useful in your research, please consider citing:
</p> -->

```bibtex
@inproceedings{uy-scade-cvpr23,
      title = {SCADE: NeRFs from Space Carving with Ambiguity-Aware Depth Estimates},
      author = {Mikaela Angelina Uy and Ricardo Martin-Brualla and Leonidas Guibas and Ke Li},
      booktitle = {Conference on Computer Vision and Pattern Recognition (CVPR)},
      year = {2023}
  }
```