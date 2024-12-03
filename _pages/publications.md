---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024]
nav: true
nav_order: 2
---

<!-- 
_bibliography/papers.bib

@article{RN7745,
   abbr={ICIP},
   author={Bilgi, H. Çağrι and Alatan, A. Aydιn},
   title={Bi-Directional Tracklet Embedding for Multi-Object Tracking}, 
   journal = {IEEE International Conference on Image Processing},
   ISSN = {0019-1019 1474-919X},
   DOI = {10.1111/ibi.13069},
   year = {2022},
   abstract={The last decade has seen significant advancements in multi-object tracking, particularly with the emergence of deep learning based methods. However, many prior studies in online tracking have primarily focused on enhancing track management or extracting visual features, often leading to hybrid approaches with limited effectiveness, especially in scenarios with severe occlusions. Conversely, in offline tracking, there has been a lack of emphasis on robust motion cues. In response, this approach aims to present a novel solution for offline tracking by merging tracklets using some recent promising learning-based architectures. We leverage a jointly performing Transformer and Graph Neural Network (GNN) encoder to integrate both the individual motions of targets and their interactions in between. By enabling bi-directional information propagation between the Transformer and the GNN, proposed model allows motion modeling to depend on interactions, and conversely, interaction modeling to depend on the motion of each target. The proposed solution is an end-to-end trainable model that eliminates the requirement for any handcrafted short-term or long-term matching processes. This approach performs on par with state-of-the-art multi-object tracking algorithms, demonstrating its effectiveness and robustness.},
   bibtex_show={true},
   html={https://ieeexplore.ieee.org/document/10648019},
   pdf={https://ieeexplore.ieee.org/document/10648019},
   # preview={bulla2022_prev.png},
   type = {Journal Article},
} -->

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>