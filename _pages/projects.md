---
layout: page
title: research
permalink: /research/
description: Some research and other related projects I've been working on. 
nav: true
nav_order: 3
display_categories: [work]
horizontal: false

---

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

<p>
  Software alone can only do so much—I believe combining software with digital fabrication’s potential to rapidly produce customizable tools will allow us to solve many more of the problems within our society. This is why I seek to combine digital fabrication with sensing to create interactive physical interfaces, aid in personal health monitoring, and/or design tools to allow people to better observe the physical world around us.
</p>

<p>As an undergraduate, I have conducted research in three main areas: sensing, digital fabrication, and synthetic biology.</p>

<div class="project-section">
  <h2>Sensing</h2>

  <h3>Multi-Channel Facial Photoplethysmography (PPG)</h3>

  <img src="/assets/images/ppg-diagram.png" alt="PPG Device Diagram">

  <p><strong>Description:</strong> The face provides a very unique opportunity for performing physiological sensing using wearables and camera-based systems. Measuring the vascular network in the face may enable disease diagnosis and continuous monitoring...</p>

  <p><strong>Individual contributions:</strong></p>
  <ul>
    <li>Helped design breakouts for our optical sensors</li>
    <li>Set up optical sensors to get a photoplethysmography (PPG) waveform</li>
    <li>Developed firmware on an MSP430 to control sampling across devices/sensors</li>
  </ul>

  <div class="btn-container">
    <a class="btn-outline-primary" href="/assets/papers/ppg-paper.pdf" target="_blank">Paper</a>
    <a class="btn-outline-danger" href="https://doi.org/10.xxxxx" target="_blank">DOI</a>
  </div>
</div>
