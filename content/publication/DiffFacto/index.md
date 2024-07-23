---
title: 'DiffFacto: Controllable Part-Based 3D Point Cloud Generation with Cross Diffusion'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - George Kiyohiro Nakayama
  - mikacuy
  - Jiahui Huang
  - Shimin Hu
  - keli
  - Leonidas Guibas

# Author notes (optional)
author_notes:

date: '2023-08-20'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-08-20'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: International Conference on Computer Vision 2023
publication_short: ICCV 2023

abstract: While the community of 3D point cloud generation has witnessed a big growth in recent years, there still lacks an effective way to enable intuitive user control in the generation process, hence limiting the general utility of such methods. Since an intuitive way of decomposing a shape is through its parts, we propose to tackle the task of controllable part-based point cloud generation. We introduce DiffFacto, a novel probabilistic generative model that learns the distribution of shapes with part-level control. We propose a factorization that models independent part style and part configuration distributions, and present a novel cross diffusion network that enables us to generate coherent and plausible shapes under our proposed factorization. Experiments show that our method is able to generate novel shapes with multiple axes of control. It generates plausible and coherent shape, while enabling various downstream editing applications such as shape interpolation, mixing and transformation editing. 

# Summary. An optional shortened abstract.
summary: Our approach tackles the task of controllable part-based point cloud generation, where we are able to both generate novel shapes and perform edits on user-input shapes. An overview of our network is given at the bottom row. We factorize the 3D shape distribution into three key components: part stylizers, transformation samplers, and a cross diffusion network. 

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/abs/2305.01921'
url_code: 'https://github.com/diffFacto/diffFacto'
url_dataset: ''
url_poster: ''
url_project: 'https://difffacto.github.io'
url_slides: ''
url_source: 'https://difffacto.github.io'
url_video: 'https://youtu.be/gwlqiJP5izI'

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
@inproceedings{nakayama2023difffacto,
      title={DiffFacto: Controllable Part-Based 3D Point Cloud Generation with Cross Diffusion}, 
      author={Kiyohiro Nakayama and Mikaela Angelina Uy and Jiahui Huang and Shi-Min Hu and Ke Li and Leonidas Guibas},
      year={2023},
      booktitle = {International Conference on Computer Vision (ICCV)},
}
```