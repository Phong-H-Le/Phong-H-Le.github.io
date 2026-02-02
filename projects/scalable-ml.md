---
layout: page
title: Scalable ML for Antibiotic Screening
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
<div style="height: 1rem;"></div>
<div class="project-section">

<h3>Presentation</h3>

<div class="embed-container">
  <iframe src="https://docs.google.com/presentation/d/13CNicf0F2OOfqr5G2zVu5gawpYUTqZsEXWZDdDTiAVA/embed?start=false&loop=false&delayms=3000" frameborder="0" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</div>

<div class="project-section" markdown="1">

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
