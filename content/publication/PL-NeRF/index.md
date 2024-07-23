---
title: 'NeRF Revisited: Fixing Quadrature Instability in Volume Rendering'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - mikacuy
  - George Kiyohiro Nakayama
  - Guandao Yang
  - Rahul Thomas
  - Leonidas Guibas
  - keli

# Author notes (optional)
author_notes:

date: '2024-01-19'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-01-19'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: Conference on Neural Information Processing Systems 2023
publication_short: NeurIPS 2023

abstract: Neural radiance fields (NeRF) rely on volume rendering to synthesize novel views. Volume rendering requires evaluating an integral along each ray, which is numerically approximated with a finite sum that corresponds to the exact integral along the ray under piecewise constant volume density. As a consequence, the rendered result is unstable w.r.t. the choice of samples along the ray, a phenomenon that we dub quadrature instability. We propose a mathematically principled solution by reformulating the sample-based rendering equation so that it corresponds to the exact integral under piecewise linear volume density. This simultaneously resolves multiple issues: conflicts between samples along different rays, imprecise hierarchical sampling, and non-differentiability of quantiles of ray termination distances w.r.t. model parameters. We demonstrate several benefits over the classical sample-based rendering equation, such as sharper textures, better geometric reconstruction, and stronger depth supervision. Our proposed formulation can be also be used as a drop-in replacement to the volume rendering equation for existing methods like NeRFs.

# Summary. An optional shortened abstract.
summary: We revisit the quadrature used to approximate volume rendering in NeRF and devise a different quadrature formula based on a different approximation to the opacity. We derive the rendering equation under piecewise linear opacity and show that it both resolves quadrature instability and has good numerical conditioning.


tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2310.20685'
url_code: 'https://github.com/mikacuy/PL-NeRF'
url_dataset: ''
url_poster: ''
url_project: 'https://pl-nerf.github.io'
url_slides: ''
url_source: 'https://pl-nerf.github.io'
url_video: 'https://youtu.be/0QGlsQqbDkM'

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
@inproceedings{uy-plnerf-neurips23,
      title = {NeRF Revisited: Fixing Quadrature Instability in Volume Rendering},
      author = {Mikaela Angelina Uy and George Kiyohiro Nakayama and Guandao Yang and Rahul Krishna Thomas and Leonidas Guibas and Ke Li},
      booktitle = {Advances in Neural Information Processing Systems (NeurIPS)},
      year = {2023}
}
```