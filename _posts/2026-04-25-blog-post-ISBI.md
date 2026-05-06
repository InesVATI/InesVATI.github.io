---
title: 'My ISBI Highlights'
date: 2026-05-07
permalink: /posts/2026/04/25/takeaway-ISBI
tags:
  - conference
  - papers
---

 At the end of the first year of my PhD, I attended the International Symposium on Biomedical Imaging (ISBI). It is a leading international forum in the field of biomedical imaging, bringing together researchers and professionals from academia and industry. In addition to my paper presentation, I attended a tutorial and some talks organized as part of the conference program. These sessions focused on emerging methodologies, tools, and applications in biomedical imaging. 
 

In this post, I summarized my main takeaways as a first-time participant.

Tutorial
----
I attended a very interesting and resourceful tutorial about generative modelling in neuroimaging. It started with a presentation of Flows and Diffusion that are the main approaches for generative modelling. Then a notebook were given to run a diffusion model and perform unsupervised tumor detection in brain MRI with the 
Anomaly Detection with Denoising Diffusion Probabilistic (AnoDDPM) model.
<details>
<summary><b>Introduction to Generative Modelling with Flows and Diffusions: From Theory to Application in Unsupervised Anomaly Detection in Neuroimaging</b></summary> 
<br>

A generative model converts samples from an initial distribution (e.g. \(\mathcal{N}(0, I_d)\) ) into samples from the approximated data distribution. <br>
Flow model define dynamics as deterministic ODE. To generate samples, a neural network (NN) parameterized by \(\theta\) predicts the time-dependent vector field \(u_t^\theta(x)\) where \(x\in\mathbb{R}^d\) that is integrated numerically with Euler scheme for instance. Flow model enable fast and efficient sampling.<br>

Diffusions model define dynamics as stochastic differential equations (SDE) driven by the Brownian motion. Brownian motion, also called Wiener process, can be view as continuous limit of a random walk. The SDE include a deterministic motion and a drift term. Diffusion model offers high sample quality and a better diversity across generated samples. <br>
Training dataset are usually obtained by adding noise to the data. <br><br>
The presentation part was based on this <a href="https://diffusion.csail.mit.edu">lecture</a>.
The notebook of the tutorial can be found <a href="https://github.com/HuguesRoy/diffusion_lab/tree/isbi"> here</a>.
</details>

Keynotes
---

Multiple interesting keynotes were given throughout the conference. I was impressed by these 1-hour presentations and the quality of their slides. Two of them caught my attention. More details can be found [here](https://biomedicalimaging.org/2026/keynote-speakers/).

<details>
<summary>
<b>Robustness by Design: Clinical Metrics for Imaging AI</b>  by Mauricio Reyes <br>
His speech focused on going beyond average performance evaluations for medical AI models.
</summary>
<br>
He described leveraging failure modes as opportunities to make AI systems <b>robust</b>, <b>reliable</b>, and <b>resilient</b>: the <b>"3 R's" of clinical AI</b>. 
He highlighed how technical metrics (accuracy, etc.) sometimes do not fully reflect clinical goals. Nevertheless, he showed that it is still possible to evaluate and train AI systems with clinical objectives.  
<br><br>
He mentioned <a href="https://github.com/caumente/AUDIT">AUDIT</a> (Analysis & Evaluation Dashboard of Artificial Intelligence). It is an open-source Python library designed for the comprehensive evaluation of medical image segmentation models and MRI datasets analysis. It includes funcitonalities to extract relevant features and metrics from multiple data sources, uncovering biases within datasets and model predictions. <br>
<img src="/images/keynote1.jpeg" width="300px" alt="photo of slide"><img src="/images/keynote2.jpeg" width="300px" alt="photo of slide">
</details>
<br>

<details> <summary> <b>From Interpretable Multimodal models to Foundation Models in Biomedical Imaging</b> by Greg Slabaugh </summary>
<br>
He shared perspectives on <b> multimodal AI</b>,<b> foundation models</b>, and <b> digital twins</b> and described how these are shaping the future of biomedical imaging and healthcare.
<br><br>

<span style='color:purple'> What are foundation models (FMs) ?</span> <br>
FMs are large deep learning models trained on large datasets for a wide range of tasks across multiple domains, without being explicitly trained for each task.
</details>

Industry Day 
---

Industry Day was a sequel of 45-minutes talks from researchers working in companies such as NVIDIA, GE Healthcare, etc. Let me describe one of them.

Fernando Pérez-García, Senior Researcher at Microsoft Research Health Futures, gave a presentation about "*Multimodal AI for Interpretation of 3D medical images*". He presented COLIPRI, a method to build vision-language foundation models that integrate 3D images and clinical reports for accurate clinical interpretation. He discussed their paper intitled *Comprehensive language–image pre-training  for 3D medical image understanding*

<details> <summary><b>Comprehensive language–image pre-training  for 3D medical image understanding</b></summary>
<br>

<b> Contrastive language-image pre-training (CLIP)</b> enables aligning images with paired text (ie. make embeddings of text and image from the same pair closer together). Vison-Language encoders trained with CLIP can be used for classification, semantic segmentation, and retrieval. 
<br><br>

In this paper, they propose to tackle the lack of large paired medical datasets by developing a vision-language pre- training approach using both image-only and image-text open-access datasets. To achieve this, their framework combines<b> vision-language pre-training </b> by adapting CLIP to 3D CT scans, a radiology <b>report generation</b>, and <b>vision-only masked autoencoder (MAE)</b> as self-supervision. They also use text augmentation with<i> sentence shuffle</i> and <i>short sentence</i> augmentation consisting in replacing long reports with LLM-shortened statements. They also propose a novel loss term to enable zero-shot classification.
<br><br>
<span style='color:purple'>Zero-shot learning</span> (ZSL) is a machine learning technique where a model can classify new data to classes it has never seen (been trained on) before. For instance, it can be used in misinformation detection even if the model has never encountered such cases before. In practice, it relies on pre-trained models that have been trained on a lot of data such as the GPTs (for language) or CLIP (for image-text relationship) to provide a good general knowledge and leverage semantic information.   

</details>

<br>

[More information here](https://biomedicalimaging.org/2026/industry-day/)

<!-- Paper presentations
----
- Nour Aburaed, FreqFormer: Single image Super Resolution network for biomedical HSI (Hyperspectral Imaging)
- Best paper : Multimodal Oncology Agent
<img width='500cm' src='best_paper.jpeg'>
- STU-NET: a hybrid cnn transformer architecture for cortical surface registration 
  <img src=poster_surf.jpeg width=400> -->

Posters
---


| Streak-reduction Human-scale Dark-field CT with 3D Gaussian Splatting | Attention-based multiple Instance Learning for rare cell detection                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| --------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![pos](/images/poster_isbi_ct.jpeg)                                               | ![pos](/images/poster_isbi_mil.jpeg) <br> ![pos](/images/poster_isbi_mil2.jpeg)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|       They use **3D Gaussian Splatting** method as a pre-processing step to mitigate the inherent streak artifacts present in dark-field CT scans (DFCT).  | It mentions **Extreme Learning Machines** (ELM). They are feedforward NN with a single or multiple hidden layers. These hidden nodes can be randomly assigned and never updated or can be inherited from their ancestors without being changed<br>the output weights of hidden nodes are usually **learned in a single step**, which essentially amounts to learning a linear model:<br>the weights of the output layer are obtained by computing the Moore-Penrose pseudo-inverse of the output matrix of the last hidden layer. It enables **bypassing time-consuming backpropagation** |


<br>
Award winners can be found [here](https://biomedicalimaging.org/2026/2026-awards/).

<!-- Challenge 
---
Dolphin AI
They are recruiting: send CV to liruirui@dolphin-ai.cn -->