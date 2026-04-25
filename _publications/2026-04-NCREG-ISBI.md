---
title: "NC-Reg : Neural Cortical Maps for Rigid Registration"
collection: publications
category: conferences
permalink: /publication/2026-04-NCREG-ISBI
excerpt: 'This work highlights the potential of neural representations to streamline registration workflows and extend to broader neuroimaging applications.'
date: 2026-04-08
venue: 'IEEE 23rd International Symposium on Biomedical Imaging (ISBI)'
slidesurl: /files/isbi26_1571221116.pdf
paperurl: 'https://arxiv.org/abs/2601.19042'
# bibtexurl: 'https://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

![learning of example feature maps](/images/illu_neural_surf_training.png)

We introduce _neural cortical maps_, a continuous and compact neural representation for cortical feature maps, as an alternative to traditional discrete structures such as grids and meshes. It can learn from meshes of arbitrary size and provide learnt features at any resolution. _Neural cortical maps_ enable efficient optimization on the sphere and achieve runtimes up to 30 times faster than classic barycentric interpolation (for the same number of iterations). As a proof of concept, we investigate rigid registration of cortical surfaces and propose NC-Reg, a novel iterative algorithm that involves the use of _neural cortical feature maps_, gradient descent optimization and a _simulated annealing_ strategy. Through ablation studies and subject-to-template experiments, our method demonstrates sub-degree accuracy ($<1^\circ$ from the global optimum), and serves as a promising robust pre-alignment strategy, which is critical in clinical settings. 