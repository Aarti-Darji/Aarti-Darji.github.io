---
layout: page
title: research
suppress_title: true
permalink: /research/
description: 
nav: true
nav_order: 3
display_categories: [work]
horizontal: false

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
  .project-section h2 {
    color: #a60000;
    border-bottom: 2px solid #a60000;
    padding-bottom: 0.5rem;
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
  .btn-outline-danger {
    color: #dc3545;
    border-color: #dc3545;
  }
</style>

<h1>Research</h1>


<p>As an undergraduate, I have conducted research in two main areas: computational biology and human-computer interaction.</p>

<div class="project-section">
  <h3>LLM-Supported Exploration of Highly Multiplexed Imaging </h3>

  <img src="/assets/img/publication_preview/overview.png" alt="Search Results Diagram">

  <p><strong>Description:</strong> Multiplexed immunofluorescence (mIF) imaging enables visualization of a large number of biomarkers simultaneously, offering high-resolution insight into spatial tissue architecture and immune landscapes. Current visualization tools make it hard for non-expert users to interpret biological relevance of diverse biomarkers and the volume of data makes it difficult to locate regions containing patterns of interest within the tissue. To address this challenge, we present an approach to assist users in exploring mIF datasets through the use of a natural language-driven multi-agent system. This agentic system interprets user queries, retrieves relevant biomarker information, and identifies spatial regions relevant to the user query within the imaging data. By integrating SQL-based querying, dynamic tool execution, and contextual reasoning, our system allows users to explore biomarker relationships, highlight spatially distinct regions, and dynamically update views based on natural language input. Our implementation builds on Vitessce (https://vitessce.io), a visual integration tool for spatial and single-cell datasets, and can be deployed as an interactive widget within a Jupyter notebook. We demonstrate our approach on multiple mIF datasets spanning diverse tissue and cancer types, demonstrating its adaptability and utility in discovering spatial patterns and anomalies. By reducing the effort required to navigate and interpret mIF datasets, our approach has the potential to aid researchers in quickly identifying regions of interest for downstream segmentation tasks and exploratory analysis.
  </p>

  <p><strong>Individual contributions:</strong></p>
  <ul>
    <li>Designed and implemented the chatbot interface for Vitessce.</li>
    <li>Created a multi-agent orchestration layer for biomarker and ROI search.</li>
    <li>Integrated few-shot learning and RAG for accurate retrieval and structured output.</li>

  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/assets/papers/ppg-paper.pdf" target="_blank">Paper</a>
    <a class="btn-outline-danger" href="https://doi.org/10.xxxxx" target="_blank">DOI</a>
  </div>

  <h3>Multimodal pathology image search between H&E slides and multiplexed immunofluorescent images </h3>

  <img src="/assets/img/publication_preview/multimodal.png" alt="Search Results Diagram">

  <p><strong>Description:</strong> We present an approach for multimodal pathology image search, using dynamic time warping (DTW) on Variational Autoencoder (VAE) latent space that is fed into a ranked choice voting scheme to retrieve multiplexed immunofluorescent imaging (mIF) that is most similar to a query H&E slide. Through training the VAE and applying DTW, we align and compare mIF and H&E slides. Our method improves differential diagnosis and therapeutic decisions by integrating morphological H&E data with immunophenotyping from mIF, providing clinicians a rich perspective of disease states. This facilitates an understanding of the spatial relationships in tissue samples and could revolutionize the diagnostic process, enhancing precision and enabling personalized therapy selection. Our technique demonstrates feasibility using colorectal cancer and healthy tonsil samples. An exhaustive ablation study was conducted on a search engine designed to explore the correlation between multiplexed Immunofluorescence (mIF) and Hematoxylin and Eosin (H&E) staining, in order to validate its ability to map these distinct modalities into a unified vector space. Despite extreme class imbalance, the system demonstrated robustness and utility by returning similar results across various data features, which suggests potential for future use in multimodal histopathology data analysis.</p>

  <p><strong>Individual contributions:</strong></p>
  <ul>
    <li>Developed and trained the VAE on HPC clusters to generate patch-level latent vectors.</li>
    <li>Implemented DTW-based alignment and ranked-choice retrieval pipeline.</li>
    <li>Conducted validation and ablation studies to assess robustness despite extreme class imbalance.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/assets/papers/ppg-paper.pdf" target="_blank">Paper</a>
    <a class="btn-outline-danger" href="https://doi.org/10.xxxxx" target="_blank">DOI</a>
  </div>

  <h3>Trace to Touch: Eliciting Gestures from Capacitive Touch Electrodes </h3>

  <img src="/assets/img/publication_preview/tracetotouch.png" alt="Search Results Diagram">

  <p><strong>Description:</strong> Capacitive touch relies on electrodes to detect and interpret touch gestures. These electrodes are conventionally designed as rigid, grid-like structures, optimized for manufacturing efficiency. However, the advent of diverse conductive materials opens new avenues for enhancing the way electrodes are designed. In this paper, we develop a textile-silicone sensor composite using embedded conductive yarn as a capacitive touch electrode. By deviating from the grid pattern, we explore how alternative patterns can inspire novel, playful, and expressive gestures. We describe our design process for conceptualizing gestures from electrode design principles and iteratively test gesture detection using an off-the-shelf CNN model. Our approach in developing a textile-silicone sensor with unique electrode designs enables the development of creative, comfortable and customizable haptic interfaces.
  </p>

  <p><strong>Individual contributions:</strong></p>
  <ul>
    <li>Fabricated layered silicone composites with unique electrode designs.</li>
    <li>Collected and processed gesture datasets for CNN-based classification.</li>
    <li>Achieved 97% accuracy in gesture recognition from sensor heatmaps.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/assets/papers/ppg-paper.pdf" target="_blank">Paper</a>
    <a class="btn-outline-danger" href="https://doi.org/10.xxxxx" target="_blank">DOI</a>
  </div>
</div>
