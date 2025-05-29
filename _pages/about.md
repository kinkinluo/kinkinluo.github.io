---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi！I am Longfei Luo, a third-year undergraduate student majoring in **Bioinformatics** at the School of Life Sciences, Soochow University. I am currently conducting research in the lab of **Professor Guang Hu**, Department of Bioinformatics and Computational Biology.

My research interests lie in **AI for Life Sciences**, with particular focus on **AI-driven drug discovery (AIDD)**. I am broadly interested in developing computational models across both **molecular and network levels** to facilitate the understanding and design of effective therapeutics.

On the **molecular level**, I explore deep learning approaches for protein structure modeling and simulation. On the **systems level**, I focus on the **theoretical modeling and application of graph neural networks (GNNs) in large-scale biological networks**, aiming to capture how drugs perturb complex network structures and to uncover the underlying mechanisms of drug action.

By integrating insights across these complementary layers, my long-term goal is to contribute to mechanism-based and data-driven strategies for **precision drug development**.

🔬 Recent Research：Endotype-Oriented Drug Target Module Discovery
======

Phenotypically distinct diseases may share common **molecular endotypes**, which opens the door to **endotype-based drug repositioning** [Zhou et al., *Trends Pharmacol Sci*, 2022](https://www.cell.com/trends/pharmacological-sciences/pdf/S0165-6147(21)00221-2.pdf). Instead of treating symptoms, this approach aims to identify shared biological mechanisms and repurpose existing drugs to target novel indications based on mechanism-level similarity.

To support this goal, we develop deep learning-based methods for **disease target module discovery** from large-scale biological networks. The pipeline is illustrated as follows:

![Technical Framework](research_pipline.png)

Specifically, we construct a **two-layer graph neural network framework**:

1. **Protein Embedding Layer**  
   A graph convolutional network (GCN) is used to embed **protein structural features** into a low-dimensional latent space, providing informative representations for downstream analysis.

2. **Disease Module Detection Layer**  
   A graph attention network (GAT) is applied to the **protein-protein interaction (PPI) network**, performing **community detection** to identify candidate **disease-associated modules**.

3. **Targetability Analysis**  
   Known drug targets are projected onto the identified modules, and **topological proximity** and **perturbation impact** are jointly analyzed to evaluate the **targeting potential** of each module.

This research direction bridges **artificial intelligence and systems biology**, and seeks to support **rational drug design** by providing quantitative frameworks for analyzing drug effects across molecular and cellular systems. I am broadly interested in integrating data-driven machine learning approaches with biological network modeling to advance **quantitative biology**.

📝 Publications
======
## 📝 Recent Publications

<div style="border: 1px solid #ccc; padding: 10px; display: flex; gap: 20px; margin-bottom: 20px; align-items: center;">
  <div style="flex: 1;">
    <img src="/jpcb.png" alt="Paper Figure" style="max-width: 100%;">
  </div>
  <div style="flex: 2;">
    <b>Comparative Simulative Analysis and Design of Single-Chain Self-Assembled Protein Cages</b><br>
    Xiao F, <b>Luo L</b>, Liu X, et al.<br>
    <i>Journal of Physical Chemistry B</i>, 128(26):6272–6282, 2024.<br>
    DOI: <a href="https://doi.org/10.1021/acs.jpcb.4c01957" target="_blank">10.1021/acs.jpcb.4c01957</a>
    <br><br>
    🔗 <a href="https://pubs.acs.org/doi/10.1021/acs.jpcb.4c01957" target="_blank">Paper</a>
  </div>
  
</div>


Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
