---
layout: page
title: research
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

  <h3>Multimodal pathology image search between H&E slides and multiplexed immunofluorescent images </h3>

  <img src="/assets/img/publication_preview/multimodal.png" alt="Search Results Diagram">

  <p><strong>Description:</strong> We present an approach for multimodal pathology image search, using dynamic time warping (DTW) on Variational Autoencoder (VAE) latent space that is fed into a ranked choice voting scheme to retrieve multiplexed immunofluorescent imaging (mIF) that is most similar to a query H&E slide. Through training the VAE and applying DTW, we align and compare mIF and H&E slides. Our method improves differential diagnosis and therapeutic decisions by integrating morphological H&E data with immunophenotyping from mIF, providing clinicians a rich perspective of disease states. This facilitates an understanding of the spatial relationships in tissue samples and could revolutionize the diagnostic process, enhancing precision and enabling personalized therapy selection. Our technique demonstrates feasibility using colorectal cancer and healthy tonsil samples. An exhaustive ablation study was conducted on a search engine designed to explore the correlation between multiplexed Immunofluorescence (mIF) and Hematoxylin and Eosin (H&E) staining, in order to validate its ability to map these distinct modalities into a unified vector space. Despite extreme class imbalance, the system demonstrated robustness and utility by returning similar results across various data features, which suggests potential for future use in multimodal histopathology data analysis.</p>

  <p><strong>Individual contributions:</strong></p>
  <ul>
    <li>Trained VAE on NVIDIA GPUs to obtain latent vectors for image patches.</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/assets/papers/ppg-paper.pdf" target="_blank">Paper</a>
    <a class="btn-outline-danger" href="https://doi.org/10.xxxxx" target="_blank">DOI</a>
  </div>
</div>
