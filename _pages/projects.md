---
layout: page
title: research
suppress_title: true
permalink: /research/
description: Selected research projects in computational biology and human-computer interaction.
nav: true
nav_order: 4
---
<style>
  h1.page-title {
    display: none;
  }
</style>
<!-- Custom layout: HTML only -->

<style>
  .project-section {
    margin-bottom: 3rem;
    border-bottom: 2px solid #ccc;
    padding-bottom: 2rem;
  }
  .project-section:last-child {
    border-bottom: none;
  }
  .project-section h3 {
    color: #a60000;
    border-bottom: 2px solid #a60000;
    padding-bottom: 0.5rem;
  }
  .project-section .project-meta {
    font-style: italic;
    margin-top: -0.5rem;
    margin-bottom: 1rem;
  }
  .project-section img {
    max-width: 100%;
    margin: 1rem 0;
    border: 1px solid #ddd;
    border-radius: 6px;
  }
  .btn-container {
    margin-top: 1rem;
  }
  .btn-container a {
    display: inline-block;
    margin-right: 0.5rem;
    padding: 0.4rem 0.8rem;
    border: 1px solid #999;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 600;
    font-size: 0.95rem;
  }
  .btn-outline-primary {
    color: #007bff;
    border-color: #007bff;
  }
  .btn-outline-secondary {
    color: #6c757d;
    border-color: #6c757d;
  }
</style>

<h1>Research</h1>

<p>My research sits at the intersection of computational biology and human-computer interaction. I'm interested in multimodal representation learning for biomedical data&mdash;integrating imaging, omics, and clinical modalities for retrieval, fusion, and natural-language-driven exploration&mdash;and, earlier on, in how novel sensor and material design can elicit new kinds of tangible interaction. Below are a few projects from this work; see <a href="/publications/">publications</a> for the full list of papers, posters, and talks, and <a href="/cv/">CV</a> for the complete research timeline.</p>

<div class="project-section">
  <h3>Diffusion MRI Analysis of Gulf War Illness in Veterans</h3>
  <p class="project-meta">Research Assistant I, UTHealth Houston &middot; Advisor: Dr. Deborah Little &middot; June 2025&ndash;present</p>

  <p><strong>Description:</strong> Gulf War Illness (GWI) is a chronic, multi-symptom condition affecting veterans of the 1990&ndash;91 Gulf War, with poorly understood structural and connectivity correlates in the brain. I curate and maintain raw and processed MRI data for ongoing GWI studies and run diffusion MRI analyses with FSL and FreeSurfer to surface structural and white-matter tract-based differences that can inform how the condition is characterized and studied.</p>

  <p><strong>Contributions:</strong></p>
  <ul>
    <li>Curated and QC'd raw and processed MRI datasets across the study cohort.</li>
    <li>Ran diffusion MRI (dMRI) analysis pipelines in FSL and FreeSurfer for structural and tract-based insights.</li>
  </ul>
</div>

<div class="project-section">
  <h3>LLM-Supported Exploration of Highly Multiplexed Imaging</h3>
  <p class="project-meta">Undergraduate Research Intern, HIDIVE Lab, Harvard Medical School &middot; Advisor: Dr. Nils Gehlenborg &middot; June 2024&ndash;May 2025</p>

  <img src="/assets/img/publication_preview/overview.png" alt="Overview diagram of the natural-language mIF exploration system">

  <p><strong>Description:</strong> Multiplexed immunofluorescence (mIF) imaging enables visualization of a large number of biomarkers simultaneously, offering high-resolution insight into spatial tissue architecture and immune landscapes. Current visualization tools make it hard for non-expert users to interpret the biological relevance of diverse biomarkers, and the volume of data makes it difficult to locate regions containing patterns of interest within the tissue. To address this, I built a natural-language-driven multi-agent system that interprets user queries, retrieves relevant biomarker information, and identifies spatial regions relevant to the query within the imaging data. By combining SQL-based querying, dynamic tool execution, and contextual reasoning, the system lets users explore biomarker relationships, highlight spatially distinct regions, and dynamically update views from plain-language input. The implementation builds on <a href="https://vitessce.io" target="_blank" rel="noopener noreferrer">Vitessce</a>, a visual integration tool for spatial and single-cell datasets, and can be deployed as an interactive widget inside a Jupyter notebook. We demonstrate the approach on multiple mIF datasets spanning diverse tissue and cancer types.</p>

  <p><strong>Contributions:</strong></p>
  <ul>
    <li>Designed and implemented the chatbot interface for Vitessce.</li>
    <li>Built a multi-agent orchestration layer for biomarker and region-of-interest (ROI) search.</li>
    <li>Implemented few-shot learning and a RAG approach for accurate retrieval and structured output.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/publications/#darji2025askandreveal" target="_blank">Poster (ISMB 2025)</a>
    <a class="btn-outline-secondary" href="https://vitessce.io" target="_blank" rel="noopener noreferrer">Vitessce</a>
  </div>
</div>

<div class="project-section">
  <h3>Multimodal Pathology Image Search Between H&amp;E Slides and Multiplexed Immunofluorescent Images</h3>
  <p class="project-meta">Undergraduate Research Assistant, Health Data Science Lab, UT Arlington &middot; Advisor: Dr. Jacob Luber &middot; May 2023&ndash;May 2024</p>

  <img src="/assets/img/publication_preview/multimodal.png" alt="Diagram of the multimodal pathology image search pipeline">

  <p><strong>Description:</strong> An approach for multimodal pathology image search that uses dynamic time warping (DTW) on a Variational Autoencoder (VAE) latent space, fed into a ranked-choice voting scheme, to retrieve the multiplexed immunofluorescence (mIF) imaging most similar to a query H&amp;E slide. By training the VAE and applying DTW, we align and compare mIF and H&amp;E slides, integrating morphological H&amp;E data with mIF immunophenotyping to give clinicians a richer perspective on disease state and support differential diagnosis and treatment decisions. The technique is demonstrated on colorectal cancer and healthy tonsil samples; an ablation study validated the search engine's ability to map the two modalities into a unified vector space, with the system remaining robust despite extreme class imbalance.</p>

  <p><strong>Contributions:</strong></p>
  <ul>
    <li>Developed and trained the VAE on HPC clusters to generate patch-level latent vectors.</li>
    <li>Implemented the DTW-based alignment and ranked-choice retrieval pipeline.</li>
    <li>Conducted validation and ablation studies to assess robustness despite extreme class imbalance.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="https://arxiv.org/abs/2306.06780" target="_blank" rel="noopener noreferrer">Paper</a>
    <a class="btn-outline-secondary" href="/publications/#darji2024integrated" target="_blank">Poster (ISMB 2024)</a>
  </div>
</div>

<div class="project-section">
  <h3>Trace to Touch: Eliciting Gestures from Capacitive Touch Electrodes</h3>
  <p class="project-meta">Undergraduate Research Assistant, Hybrid Atelier, UT Arlington &middot; Advisor: Dr. Cesar Torres &middot; Jan 2023&ndash;May 2024</p>

  <img src="/assets/img/publication_preview/tracetotouch.png" alt="Photo of textile-silicone capacitive touch electrode samples">

  <p><strong>Description:</strong> Capacitive touch relies on electrodes to detect and interpret touch gestures. These electrodes are conventionally designed as rigid, grid-like structures, optimized for manufacturing efficiency. We develop a textile-silicone sensor composite using embedded conductive yarn as a capacitive touch electrode, and by deviating from the grid pattern, explore how alternative patterns can inspire novel, playful, and expressive gestures. We describe our design process for conceptualizing gestures from electrode design principles and iteratively test gesture detection with an off-the-shelf CNN model. The resulting textile-silicone sensor with unique electrode designs supports creative, comfortable, and customizable haptic interfaces.</p>

  <p><strong>Contributions:</strong></p>
  <ul>
    <li>Fabricated layered silicone composites with unique electrode designs.</li>
    <li>Collected and processed gesture datasets for CNN-based classification.</li>
    <li>Achieved 97% accuracy in gesture recognition from sensor-reading heatmaps.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/publications/#darji2024trace" target="_blank">Extended Abstract (C&amp;C 2024)</a>
  </div>
</div>

<div class="project-section">
  <h3>Sentura: Cognitive Affordances of Silicone Microtextures in Tangible UI Design</h3>
  <p class="project-meta">Undergraduate Research Assistant, Hybrid Atelier, UT Arlington &middot; Advisor: Dr. Cesar Torres &middot; Jan 2023&ndash;May 2024</p>

  <img src="/assets/img/publication_preview/SenturaTeaser.png" alt="Teaser image of silicone microtexture samples for Sentura">

  <p><strong>Description:</strong> We laser-cut and 3D-printed molds to fabricate silicone samples with distinct micro-textures and studied how those textures shape haptic perception, emotion, and decision-making. I built a React and Flask web application to collect participant responses and observe how users perceived the different silicone textures, and helped develop a layered silicone composite sensor with unique electrode designs to study how new tactile gestures emerge and how they correspond across modalities.</p>

  <p><strong>Contributions:</strong></p>
  <ul>
    <li>Lasercut and 3D-printed molds for silicone samples with different micro-textures.</li>
    <li>Built a React/Flask web application to collect and analyze user texture-perception responses.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/publications/#kapoor2024sentura" target="_blank">Extended Abstract (C&amp;C 2024)</a>
  </div>
</div>
