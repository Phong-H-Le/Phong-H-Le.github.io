---
layout: page
title: Scalable ML for Antibiotic Virtual Screening
permalink: /projects/scalable-ml/
---

<link rel="stylesheet" href="/assets/css/projects.css">

<a href="/projects/" class="back-link">← Back to Projects</a>

<div class="project-detail">

<div class="tech-stack">
  <span class="tech-pill">Python</span>
  <span class="tech-pill">PyTorch</span>
  <span class="tech-pill">Scikit-Learn</span>
  <span class="tech-pill">RDKit</span>
  <span class="tech-pill">Pandas</span>
  <span class="tech-pill">Cheminformatics</span>
</div>

<h3>Overview</h3>

This project addressed the critical challenge of antibiotic resistance by developing and benchmarking scalable machine learning approaches for virtual screening of antibiotic candidates. Working with computational drug discovery methods, I evaluated state-of-the-art graph neural networks against traditional ML baselines to optimize large-scale screening pipelines.

<div class="project-section">

<h3>Key Accomplishments</h3>

<ul class="project-highlights">
  <li>Benchmarked <strong>GNEprop</strong> (Nature Biotechnology, 2025) against Chemprop and XGBoost on 2,560 antibiotic candidates</li>
  <li>Achieved <strong>ROC-AUC of 0.936</strong> on held-out test sets</li>
  <li>Implemented robust ML validation controls including scaffold-based splits to prevent data leakage</li>
  <li>Applied adversarial y-shuffling techniques to validate model learning vs. memorization</li>
  <li>Quantified accuracy-compute trade-offs to optimize large-scale virtual screening pipelines</li>
  <li>Demonstrated scalable ML approaches suitable for high-throughput antibiotic discovery</li>
</ul>

</div>

<div class="project-section">

<h3>Presentation</h3>

<div class="embed-container">
  <iframe src="https://docs.google.com/presentation/d/13CNicf0F2OOfqr5G2zVu5gawpYUTqZsEXWZDdDTiAVA/embed?start=false&loop=false&delayms=3000" frameborder="0" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</div>

<p style="text-align: center; margin-top: 0.5rem;">
  <a href="https://docs.google.com/presentation/d/13CNicf0F2OOfqr5G2zVu5gawpYUTqZsEXWZDdDTiAVA/edit?usp=sharing" target="_blank" class="project-link project-link-secondary" style="display: inline-flex;">
    Open in Google Slides
  </a>
</p>

</div>

<div class="project-section">

<h3>Media Gallery</h3>

<div class="media-grid">
  <figure class="media-item">
    <img src="/assets/projects/scalable-ml/pipeline.png" alt="ML Pipeline Diagram" onerror="this.parentElement.style.display='none'">
    <figcaption>Machine Learning Pipeline Architecture</figcaption>
  </figure>
  <figure class="media-item">
    <img src="/assets/projects/scalable-ml/results.png" alt="ROC Curve Results" onerror="this.parentElement.style.display='none'">
    <figcaption>Model Performance Comparison (ROC Curves)</figcaption>
  </figure>
</div>

<p><em>Add images to <code>/assets/projects/scalable-ml/</code> to display them here.</em></p>

</div>

<div class="project-section">

<h3>Downloads</h3>

<div class="downloads-section">
  <h4>Project Resources</h4>
  <ul class="download-list">
    <li>
      <a href="/assets/projects/downloads/scalable-ml-report.pdf" class="download-link" download>
        <span>Final Report (PDF)</span>
        <span class="file-size"></span>
      </a>
    </li>
    <li>
      <a href="/assets/projects/downloads/scalable-ml-poster.pdf" class="download-link" download>
        <span>Project Poster (PDF)</span>
        <span class="file-size"></span>
      </a>
    </li>
  </ul>
  <p><em>Place downloadable files in <code>/assets/projects/downloads/</code></em></p>
</div>

</div>

<div class="project-section">

<h3>Methods & Technical Details</h3>

**Data Processing:**
- Utilized RDKit for molecular fingerprint generation and chemical descriptor calculation
- Processed SMILES representations for 2,560 antibiotic candidate molecules
- Applied scaffold-based train/test splitting to ensure chemically diverse evaluation sets

**Model Architectures:**
- **GNEprop:** Graph neural network with message passing for molecular property prediction
- **Chemprop:** Directed message passing neural network (D-MPNN)
- **XGBoost:** Gradient boosted trees with Morgan fingerprints as baseline

**Validation Strategy:**
- K-fold cross-validation with scaffold-aware splits
- Adversarial y-shuffling to detect potential data leakage
- ROC-AUC, precision-recall, and calibration metrics

</div>

</div>
