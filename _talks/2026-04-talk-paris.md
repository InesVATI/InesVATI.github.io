---
title: "Fast Geometric Machine Learning Methods for Brain Image Analysis"
collection: talks
type: "Seminars"
permalink: /talks/2026-04/talks-Paris
venue: "Reasearch Team Meetings and Seminars"
date: 2026-04-13
location: "Paris, FR"
---


I visited some prestigious French research labs in the parisian region the week following the [ISBI 2026 conference](https://inesvati.github.io/talks/2026-04-11/talk-ISBI). I was able to present some previous and ongoing work and exchange with talented researchers. I am very grateful for their time and our insightful conversations. 


[Abstract](https://inesvati.github.io/files/talk_april2026_abstract.pdf) | [Slides](https://inesvati.github.io/files/talk_april2026_slides.pdf) 

## Schedule 

*Monday 13, April:* I visited [Jean Feydy](https://www.jeanfeydy.com/) and the [HeKA Inria](https://www.inria.fr/en/heka) team at [PariSanté Campus](https://parisantecampus.fr/). HeKA is a multidisciplinary team composed of researchers, clinicians-researchers, teachers-researchers from Inria, Inserm, University Paris Cité and AP-HP. We talked about optimal transport for shape registration and research life in general. 

*Tuesday 14, April:* Thanks to [Philippe Ciuciu](https://team.inria.fr/parietal/author/ciuciu/) and I was able to present our work at [NeuroSpin](https://plateformes.insis.cnrs.fr/plateformes/plateforme-neurospin) at the CEA Paris-Saclay site. At NeuroSpin, mathematicians, neuroscientists and clinicians work together to develop the tools and models that will allow to better understand the functioning of the normal and pathological brain, before or after treatment. 

*Wednesday 15, April:* I attended the scientific seminar series DARE U (Dassault Systèmes Research Universe) at [Dassault Systèmes](https://www.3ds.com/). I got many relevant questions and valuable feedbacks. I am thankful to Louis Goldenberg for giving the opportunity to present our research. 

*Thursday 16, April:* I visited [CERMICS](https://cermics-lab.enpc.fr/), the applied mathematics laboratory of Ecole nationale des ponts et chaussées, located in the Paris region, in order to participate in the [Applied Mathematics Seminar](https://cermics-lab.enpc.fr/seminaires/seminaire-du-laboratoire/). Thanks to [Urbain Vaes](https://urbain.vaes.uk/) for his kind support.

## Abstract

Alzheimer’s Disease (AD), the most common form of dementia, is characterised by the accumulation of misfolded proteins in the brain, ultimately leading to cortical atrophy and cognitive decline. Accurate measurement of the atrophy patterns is essential not only for diagnosis but also for early detection and potential prevention (Lenhart et al., 2021). 

However, due to the **high variability in cortical geometry** across individuals, population-based analyses typically rely on long, sophisticated neuroimaging pipelines for cortical feature computation and inter subject alignment (Dale et al., 1999; Fischl, 2012; Fischl et al., 1999). These traditional approaches often require several days to weeks of computation for large cohorts, creating a major bottleneck for large-scale neuroimaging studies. Deep learning–based approaches have the potential to dramatically accelerate this process (Ma et al., 2025).

In this talk, I will present the recent work conducted in our team to streamline the cortical surface-based pipeline. I will review optimization-based approaches and end-to-end deep learning methods for **cortical mesh reconstruction** and **surface registration**. Some insights into the **Spherical Demons** algorithm (Yeo et al., 2010), a classical diffeomorphic registration method on the sphere, will be provided. I will then introduce **NC-Reg**, our novel approach for **rigid registration of spherical surfaces** using a **neural representation**. Subsequently, I will outline our ongoing and future work, with a particular focus on **CorticalFlow++**(Cruz et al., 2022; Lebrat et al., 2021), a deep learning model for **fast cortical mesh reconstruction directly from MRI images**. 
We believe that this work lays a strong foundation for **more efficient, scalable, and robust tools for cortical surface analysis**. These developments have the potential to enable large-cohort neuroimaging studies and ultimately contribute to both computational neuroscience and clinical applications.

## References

Cruz, R. S., Lebrat, L., Fu, D., Bourgeat, P., Fripp, J., Fookes, C., & Salvado, O. (2022). CorticalFlow$^{++}$: Boosting Cortical Surface Reconstruction Accuracy, Regularity, and Interoperability (arXiv:2206.06598). arXiv. https://doi.org/10.48550/arXiv.2206.06598

Dale, A. M., Fischl, B., & Sereno, M. I. (1999). Cortical Surface-Based Analysis: I. Segmentation and Surface Reconstruction. NeuroImage, 9(2), 179–194. https://doi.org/10.1006/nimg.1998.0395 

Fischl, B. (2012). FreeSurfer. NeuroImage, 62(2), 774–781. https://doi.org/10.1016/j.neuroimage.2012.01.021

Fischl, B., Sereno, M. I., & Dale, A. M. (1999). Cortical Surface-Based Analysis: II: Inflation, Flattening, and a Surface-Based Coordinate System. NeuroImage, 9(2), 195–207. https://doi.org/10.1006/nimg.1998.0396

Lebrat, L., Santa Cruz, R., de Gournay, F., Fu, D., Bourgeat, P., Fripp, J., Fookes, C., & Salvado, O. (2021). CorticalFlow: A Diffeomorphic Mesh Transformer Network for Cortical Surface Reconstruction. Advances in Neural Information Processing Systems, 34, 29491–29505. https://proceedings.neurips.cc/paper/2021/hash/f6b5f8c32c65fee991049a55dc97d1ce-Abstract.html

Lenhart, L., Seiler, S., Pirpamer, L., Goebel, G., Potrusil, T., Wagner, M., Bianco, P. D., Ransmayr, G., Schmidt, R., Benke, T., & Scherfler, C. (2021). Anatomically Standardized Detection of MRI Atrophy Patterns in Early-Stage Alzheimer’s Disease. Brain Sciences, 11(11). https://doi.org/10.3390/brainsci11111491

Ma, Q., Liang, K., Li, L., Masui, S., Guo, Y., Nosarti, C., Robinson, E. C., Kainz, B., & Rueckert, D. (2025). The Developing Human Connectome Project: A fast deep learning-based pipeline for neonatal cortical surface reconstruction. Medical Image Analysis, 100, 103394. https://doi.org/10.1016/j.media.2024.103394

Yeo, B. T. T., Sabuncu, M. R., Vercauteren, T., Ayache, N., Fischl, B., & Golland, P. (2010). Spherical Demons: Fast Diffeomorphic Landmark-Free Surface Registration. IEEE Transactions on Medical Imaging, 29(3), 650–668. https://doi.org/10.1109/TMI.2009.2030797


