---
title: "Assessing Repeatability of a Diffusion Phantom"
excerpt: "**MASc Thesis Project**"
classes: wide
author_profile: true
order: 1
header:
  teaser: /assets/images/projects/masc/phantom_crop.png
  overlay_image: /assets/images/projects/masc/phantom_crop.png
  overlay_filter: 0.5
tags:
  - Biomedical Engineering
  - MRI
  - Diffusion Imaging
  - Medical Imaging
  - Quality Assurance
  - Research
---

<div style="background-color: #f8f9fa; padding: 2em; border-radius: 8px; border-left: 4px solid #2c3e50; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #2c3e50;">The Problem</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">Diffusion MRI measures the movement of water molecules in tissue, making it a powerful technique for studying brain structure and detecting conditions like stroke and neurodegenerative disease. Advanced diffusion models have been proposed to capture complex tissue features, but they are more prone to variation, raising concerns about <b>measurement consistency and reliability</b>. Currently, there is no standardized method to perform quality assurance on diffusion MRI data, and limited studies exist measuring the repeatability of higher-order tensor metrics.</p>
</div>

<div style="background-color: #ecf0f1; padding: 2em; border-radius: 8px; border-left: 4px solid #34495e; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #34495e;">The Solution</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">A <b>novel anisotropic phantom</b> containing synthetic fibre bundles with controlled geometries (linear, crossing, and branching) mimics white matter tracts in the brain. The phantom was scanned 11 times on a 3.0T GE MRI scanner using multiple acquisition protocols. A <b>Python-based analysis pipeline</b> performed automated ROI analysis and metric extraction. Repeatability was quantified using coefficient of variation (CoV) and intraclass correlation coefficient (ICC), establishing reliability benchmarks that inform quality assurance standards for clinical and research diffusion MRI.</p>
</div>

---

## Publications & Presentations

<!-- 
<div style="background-color: #ffffff; padding: 1.5em 2em; border-radius: 8px; border: 2px solid #2c3e50; margin-bottom: 1.5em; display: flex; align-items: stretch; gap: 2em; flex-wrap: wrap;">
  <div style="flex: 1 1 45%; min-width: 200px; min-height: 180px; background-color: #2c3e50; border-radius: 6px; display: flex; flex-direction: column; align-items: center; justify-content: center; color: white; text-align: center; padding: 1em; box-sizing: border-box;">
    <i class="fas fa-file-alt" style="font-size: 3.5em; margin-bottom: 0.4em;"></i>
    <span style="font-size: 0.85em; line-height: 1.4;">Journal Paper</span>
  </div>
  <div style="flex: 1 1 45%; min-width: 200px;">
    <div style="font-size: 0.75em; font-weight: bold; text-transform: uppercase; letter-spacing: 0.05em; color: #7f8c8d; margin-bottom: 0.4em;">📄 Publication</div>
    <p style="margin: 0 0 0.6em 0; font-size: 0.95em; line-height: 1.6; color: #2c3e50;">
      <strong>Stephens, L. H.</strong>, &amp; Noseworthy, M. D. (2025). Assessing repeatability of diffusion MRI metrics using a novel anisotropic fibre phantom. <em>Journal Name</em>, <em>Volume</em>(Issue), pages. <a href="https://doi.org/PLACEHOLDER" style="color: #2980b9;">https://doi.org/PLACEHOLDER</a>
    </p>
    <a href="https://doi.org/PLACEHOLDER" style="display: inline-block; background-color: #2c3e50; color: white; padding: 0.4em 1em; border-radius: 4px; text-decoration: none; font-size: 0.85em;">
      <i class="fas fa-external-link-alt"></i> View Paper
    </a>
  </div>
</div>
-->

<div style="background-color: #ffffff; padding: 1.5em 2em; border-radius: 8px; border: 2px solid #34495e; margin-bottom: 2em; display: flex; align-items: stretch; gap: 2em; flex-wrap: wrap;">
  <div style="flex: 1 1 45%; min-width: 200px; display: flex; align-items: center;">
    <img src="/assets/images/projects/masc/conference.jpg" alt="ESMRMB 2025 poster presentation" style="width: 100%; height: auto; object-fit: contain; border-radius: 6px; display: block;">
  </div>
  <div style="flex: 1 1 45%; min-width: 200px; display: flex; flex-direction: column; justify-content: center;">
    <div style="font-size: 0.75em; font-weight: bold; text-transform: uppercase; letter-spacing: 0.05em; color: #7f8c8d; margin-bottom: 0.4em;">Conference Poster Presentation</div>
    <p style="margin: 0 0 0.6em 0; font-size: 0.95em; line-height: 1.6; color: #2c3e50;">
      Poster presented at the <em>European Society for Magnetic Resonance in Medicine and Biology Annual Meeting</em> (in Marseille, France on October 8-11, 2025).
    </p>
    <div>
    <a href="https://doi.org/10.1007/s10334-025-01278-8" style="display: inline-block; background-color: #34495e; color: white; padding: 0.4em 1em; border-radius: 4px; text-decoration: none; font-size: 0.85em;">
      <i class="fas fa-book-open"></i> Book of Abstracts
    </a>
    </div>
  </div>
</div>

---

## Research Overview

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1em; margin: 2em auto;">
  <div style="height: 300px;">
    <a href="/assets/images/projects/masc/phantom_front.jpg" style="display: block; height: 100%;">
      <img src="/assets/images/projects/masc/phantom_front.jpg" alt="Phantom front view" style="width: 100%; height: 100%; object-fit: cover; border-radius: 4px; display: block;">
    </a>
  </div>
  <div style="height: 300px;">
    <a href="/assets/images/projects/masc/phantom_side.jpg" style="display: block; height: 100%;">
      <img src="/assets/images/projects/masc/phantom_side.jpg" alt="Phantom lateral view" style="width: 100%; height: 100%; object-fit: cover; border-radius: 4px; display: block;">
    </a>
  </div>
  <div style="height: 300px;">
    <a href="/assets/images/projects/masc/phantom_back.jpg" style="display: block; height: 100%;">
      <img src="/assets/images/projects/masc/phantom_back.jpg" alt="Phantom rear view" style="width: 100%; height: 100%; object-fit: cover; border-radius: 4px; display: block;">
    </a>
  </div>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;">Front, lateral, and rear view photographs of the PreOperative Performance phantom.</p>

This thesis evaluates three diffusion MRI modelling approaches (DTI, DKI, and CSD) across multiple scanning protocols to determine which metrics are sufficiently stable for clinical quality assurance. By testing regions with varying complexity, from simple parallel fibres to a variety of crossing angles, the study identifies which measurements can reliably track disease progression or treatment response in patient populations.

<div style="text-align: center; margin: 2em auto; max-width: 600px;">
  <a href="/assets/images/projects/masc/show_roi.png">
    <img src="/assets/images/projects/masc/show_roi.png" alt="Phantom front view" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;">T1-weighted image with ROIs shown in red. (1) 90° intersection in the XY plane. (2) 45° intersection in the XZ plane. (3) 30° intersection in the XY plane. (4) Fibre splitting into three small fibre bundles. Two fibres split into the XY plane (pictured), and one fibre splits out-of-plane. (5) Simple linear fibre in the Y plane. (6) Isotropic area with no fibres present.</p>
---

## Skills Applied

<div class="course-tags">
  <span class="course-tag">MRI Physics</span>
  <span class="course-tag">Diffusion Imaging</span>
  <span class="course-tag">Python (DIPY)</span>
  <span class="course-tag">FSL Analysis</span>
  <span class="course-tag">Statistical Analysis</span>
  <span class="course-tag">Image Processing</span>
  <span class="course-tag">Quality Assurance</span>
  <span class="course-tag">Medical Imaging</span>
  <span class="course-tag">Technical Writing</span>
  <span class="course-tag">Data Visualization</span>
</div>

---

## Background on Diffusion MRI

Diffusion MRI was first demonstrated in humans in 1986 and has since become essential for studying brain structure. Water molecules naturally move through random thermal motion (Brownian motion), and their movement is restricted by biological barriers like cell membranes and axonal fibres. By applying magnetic field gradients, MRI can measure this directional water movement.

In the brain:
- **Isotropic diffusion** occurs in cerebrospinal fluid (equal movement in all directions)
- **Anisotropic diffusion** occurs along white matter tracts (preferential movement along fibres)

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/masc/iso_aniso.png">
    <img src="/assets/images/projects/masc/iso_aniso.png" alt="Phantom front view" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;"> Illustration of isotropic (left) and anisotropic (right) diffusion.</p>


### The Crossing Fibre Problem

Traditional DTI assumes water diffuses in a single primary direction per voxel, which breaks down in regions where multiple fibre bundles cross, kiss, or branch. Estimates suggest 33-90% of white matter voxels contain crossing fibres, making this a fundamental limitation for brain connectivity studies.

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/masc/crossing_fibres.png">
    <img src="/assets/images/projects/masc/crossing_fibres.png" alt="Phantom front view" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;"> Schematic of aligned linear fibres (left) and crossing fibres (right).</p>

**Advanced models address this limitation but require:**
- More complex data acquisition (more gradient directions, multiple b-values)
- Longer scan times
- More sophisticated analysis

**This thesis evaluated three diffusion models:**
- **DTI** (Diffusion Tensor Imaging) - Standard model assuming single fibre direction per voxel
- **DKI** (Diffusion Kurtosis Imaging) - Captures non-Gaussian diffusion behaviour
- **CSD** (Constrained Spherical Deconvolution) - Resolves multiple crossing fibres

---

## Methodology

<div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 1em; margin: 2em auto; max-width: 1200px;">
  <div>
    <a href="/assets/images/projects/masc/FA.png">
      <img src="/assets/images/projects/masc/FA.png" alt="FA map"
           style="width: 100%; height: auto; object-fit: contain; border-radius: 4px; display: block;">
    </a>
  </div>
  <div>
    <a href="/assets/images/projects/masc/MD.png">
      <img src="/assets/images/projects/masc/MD.png" alt="MD map"
           style="width: 100%; height: auto; object-fit: contain; border-radius: 4px; display: block;">
    </a>
  </div>
  <div>
    <a href="/assets/images/projects/masc/AD.png">
      <img src="/assets/images/projects/masc/AD.png" alt="AD map"
           style="width: 100%; height: auto; object-fit: contain; border-radius: 4px; display: block;">
    </a>
  </div>
  <div>
    <a href="/assets/images/projects/masc/RD.png">
      <img src="/assets/images/projects/masc/RD.png" alt="RD map"
           style="width: 100%; height: auto; object-fit: contain; border-radius: 4px; display: block;">
    </a>
  </div>
</div>

<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;">
    DTI–derived parameter maps from a single slice of the phantom (FA, MD, AD, and RD in order).
</p>

<div style="background-color: #ecf0f1; padding: 1.5em; border-radius: 8px; margin: 2em 0;">
<h3 style="margin-top: 0;">Scanning Protocol</h3>
<p>Each of 11 imaging sessions included:</p>
<ul>
  <li><strong>30-direction DTI:</strong> Standard clinical protocol (b=1000 s/mm²)</li>
  <li><strong>60-direction HARDI:</strong> High angular resolution (b=1300 s/mm²)</li>
  <li><strong>90-direction HARDI:</strong> Very high angular resolution (b=1300 s/mm²)</li>
  <li><strong>Multi-shell DKI:</strong> 30 directions at 8 b-values (b=250-3000 s/mm²)</li>
</ul>
</div>

<div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; margin: 2em 0;">
<h3 style="margin-top: 0;">Data Analysis Pipeline</h3>
<ol>
  <li><strong>Preprocessing:</strong> MP-PCA denoising, eddy current correction, masking</li>
  <li><strong>Model Fitting:</strong> Applied DTI, DKI, and CSD models using DIPY library</li>
  <li><strong>Metric Extraction:</strong> Computed scalar metrics (FA, MD, MK, GFA, etc.)</li>
  <li><strong>Statistical Analysis:</strong> Calculated CoV and ICC to quantify repeatability</li>
</ol>
</div>

---

## Results: Rank-2 Tensor Metrics

These metrics showed high repeatability across all ROIs and scanning protocols. FA exhibited CoVs below 10% while MD, AD, and RD had CoVs below 3%. The overall trend shows CoV decreased and ICC increased when using HARDI acquisitions. All ICC values showed excellent reliability between scans (ICC > 0.9) when using the HARDI-90 protocol.

<table style="border-collapse: collapse; width: 100%; font-size: 0.9em; margin: 1em 0; table-layout: fixed;">
  <thead>
    <tr>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white;" rowspan="2">Metric</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">DTI</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">HARDI-60</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">HARDI-90</th>
    </tr>
    <tr>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">FA</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">9.45</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9303</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">9.06</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9257</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">7.72</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9513</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">MD</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">2.06</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9336</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">1.95</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9401</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">1.89</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9474</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">AD</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">1.72</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8154</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">1.51</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8862</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">1.61</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9005</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">RD</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">2.40</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9431</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">2.32</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9543</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">2.45</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9474</td>
    </tr>
  </tbody>
</table>

---

## Results: Higher Order Diffusion Metrics

DKI metrics displayed greater variability than their DTI analogs. KFA showed low CoV values and excellent ICC reliability. MK, AK, and RK showed higher variability, with values exceeding 30% in some ROIs. KFA and AK were classified as excellent reliability while MK and RK demonstrated good reliability.

<table style="border-collapse: collapse; width: 100%; font-size: 0.9em; margin: 1em 0; table-layout: fixed;">
  <thead>
    <tr>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: left;">Metric</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">KFA</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">7.46</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9161</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">MK</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">16.02</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8312</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">AK</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">12.89</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.9228</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">RK</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">19.24</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8423</td>
    </tr>
  </tbody>
</table>

GFA showed a clear increase in reliability with angular resolution. CoV values remained low even with only 30 gradient directions.

<table style="border-collapse: collapse; width: 100%; font-size: 0.9em; margin: 1em 0; table-layout: fixed;">
  <thead>
    <tr>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white;" rowspan="2">Metric</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">DTI</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">HARDI-60</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">HARDI-90</th>
    </tr>
    <tr>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">CoV %</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">ICC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">GFA</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">6.37</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.6920</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">4.07</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8122</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">4.16</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.8445</td>
    </tr>
  </tbody>
</table>

---

## Results: CSD Crossing Angles

The ability of CSD to resolve multiple fibre orientations varied with angular separation. At 30°, CSD failed to resolve discrete fibre directions, instead producing single-peak fODFs.

<table style="border-collapse: collapse; width: 100%; font-size: 0.9em; margin: 1em 0; table-layout: fixed;">
  <thead>
    <tr>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: left;">Method</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">90°</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">45°</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #2c3e50; color: white; text-align: center;" colspan="2">30°</th>
    </tr>
    <tr>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white;"></th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">Avg</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">RMSE</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">Avg</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">RMSE</th>
      <th style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">Avg</th>
      <th style="border: 1px solid #ccc; padding: 0.5em 1em; background-color: #34495e; color: white; text-align: center;">RMSE</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">T1w reference</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">89.59°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">0.47</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">47.26°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">1.76</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">29.72°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">1.40</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">CSD Crossing Angle</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">87.10°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">3.49</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">50.07°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">8.92</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">—</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">—</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; font-weight: bold;">CSD Approach Angle</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">89.39°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">4.08</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">43.29°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">3.61</td>
      <td style="border: 1px solid #ccc; border-left: 3px solid #ccc; padding: 0.5em 1em; text-align: center;">27.67°</td>
      <td style="border: 1px solid #ccc; padding: 0.5em 1em; text-align: center;">3.63</td>
    </tr>
  </tbody>
</table>

---

## Discussion & Conclusions

Results demonstrate that the PreOperative Performance phantom is a reliable and effective tool for evaluating the repeatability of advanced diffusion MRI metrics. Results align well with findings from earlier studies using anisotropic phantoms. Published literature reports CoV of 7–29% for FA and 2–6% for MD. Future work should extend to assess inter-scanner and inter-vendor variability, or evaluate multiple PreOperative Performance phantoms with different internal configurations.

---

## Key Learnings

**<i class="fas fa-network-wired"></i> Importance of Acquisition Design**

The number of diffusion gradient directions significantly impacted model performance. For CSD-based fibre tracking, high angular resolution sampling (60-90 directions) was essential for reliable results. However, standard DTI metrics remained stable even with basic 30-direction protocols, suggesting clinical scans can be optimized based on the analysis goals.

**<i class="fas fa-microscope"></i> Physical Phantoms for MRI Validation**

This work demonstrated that anisotropic phantoms with controlled fibre geometries can effectively validate diffusion MRI measurements. Unlike human subjects, phantoms eliminate biological variability, allowing pure assessment of measurement repeatability. The phantom successfully mimicked key features of brain white matter, including crossing fibres and branching structures.

**<i class="fas fa-code"></i> Open-Source Tools Enable Reproducible Research**

The entire analysis pipeline was built using open-source tools (DIPY, FSL, Python scientific libraries), ensuring transparency and reproducibility. All preprocessing, model fitting, and statistical analysis code was documented and version-controlled, supporting the growing movement toward open science in neuroimaging research.

---

## Photo Gallery

<style>
.image-gallery {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0.5em;
  margin: 2em 0;
}

.image-gallery-item {
  position: relative;
  width: 100%;
  height: 150px;
  cursor: pointer;
}

.image-gallery-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 4px;
  transition: opacity 0.2s;
}

.image-gallery-item:hover img {
  opacity: 0.8;
}

.more-images-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(44, 62, 80, 0.85);
  border-radius: 4px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 1.5em;
  font-weight: bold;
}

.more-images-overlay:hover {
  background-color: rgba(44, 62, 80, 0.95);
}

.more-images-text {
  font-size: 0.6em;
  margin-top: 0.3em;
  font-weight: normal;
}

.lightbox {
  display: none;
  position: fixed;
  z-index: 999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.9);
}

.lightbox.active {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.lightbox-content {
  max-width: 90%;
  max-height: 80vh;
  object-fit: contain;
}

.lightbox-caption {
  color: white;
  text-align: center;
  padding: 15px;
  max-width: 800px;
  font-size: 16px;
  margin-top: 10px;
}

.lightbox-close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}

.lightbox-close:hover {
  color: #bbb;
}

.lightbox-prev, .lightbox-next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  user-select: none;
}

.lightbox-next {
  right: 0;
}

.lightbox-prev {
  left: 0;
}

.lightbox-prev:hover, .lightbox-next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

.lightbox-counter {
  position: absolute;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  font-size: 16px;
  background-color: rgba(0, 0, 0, 0.5);
  padding: 8px 16px;
  border-radius: 4px;
}

@media (max-width: 768px) {
  .image-gallery {
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>

<div class="image-gallery">
  <div class="image-gallery-item" onclick="openLightbox(0)">
    <img src="/assets/images/projects/masc/FA_colour.png" alt="FA map with colour coded directions">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(1)">
    <img src="/assets/images/projects/masc/B0_B1_map.png" alt="B0 and B1 field map">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(2)">
    <img src="/assets/images/projects/masc/ROI_4_full.png" alt="90 degree crossing fibre fODF">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(3)">
    <img src="/assets/images/projects/masc/FA_HARDI_90_boxplot.png" alt="Boxplot of FA values">
    <div class="more-images-overlay">
      +2
      <div class="more-images-text">more images</div>
    </div>
  </div>
</div>

<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close">&times;</span>
  <a class="lightbox-prev" onclick="event.stopPropagation(); changeImage(-1)">&#10094;</a>
  <img class="lightbox-content" id="lightbox-img" src="" alt="">
  <a class="lightbox-next" onclick="event.stopPropagation(); changeImage(1)">&#10095;</a>
  <div class="lightbox-caption" id="lightbox-caption"></div>
  <div class="lightbox-counter" id="lightbox-counter"></div>
</div>

<script>
let currentIndex = 0;

const galleryImages = [
  {
    src: '/assets/images/projects/masc/FA_colour.png',
    caption: 'Colour-coded fractional anisotropy map where FA modulates brightness and colours indicate direction as follows: red, left-right; green, anterior-posterior; blue, superior-inferior'
  },
  {
    src: '/assets/images/projects/masc/B0_B1_map.png',
    caption: 'B₀ and B₁⁺ field maps used to assess scanner stability and field homogeneity across imaging sessions'
  },
  {
    src: '/assets/images/projects/masc/ROI_4_full.png',
    caption: 'ROI 4: fODF of 90 degree fibre branching region'
  },
  {
    src: '/assets/images/projects/masc/FA_HARDI_90_boxplot.png',
    caption: 'Fractional anisotropy repeatability across all ROIs using the HARDI-90 acquisition protocol'
  },
  {
    src: '/assets/images/projects/masc/MD_HARDI_90_boxplot.png',
    caption: 'Mean diffusivity repeatability across all ROIs using the HARDI-90 acquisition protocol'
  },
  {
    src: '/assets/images/projects/masc/RK_DKI_boxplot.png',
    caption: 'Radial kurtosis repeatability across all ROIs from the multi-shell DKI acquisition'
  }
];

function openLightbox(index) {
  currentIndex = index;
  document.getElementById('lightbox').classList.add('active');
  document.getElementById('lightbox-img').src = galleryImages[currentIndex].src;
  document.getElementById('lightbox-caption').textContent = galleryImages[currentIndex].caption;
  updateCounter();
}

function closeLightbox() {
  document.getElementById('lightbox').classList.remove('active');
}

function changeImage(direction) {
  currentIndex += direction;
  if (currentIndex < 0) currentIndex = galleryImages.length - 1;
  if (currentIndex >= galleryImages.length) currentIndex = 0;
  document.getElementById('lightbox-img').src = galleryImages[currentIndex].src;
  document.getElementById('lightbox-caption').textContent = galleryImages[currentIndex].caption;
  updateCounter();
}

function updateCounter() {
  document.getElementById('lightbox-counter').textContent = 
    `${currentIndex + 1} / ${galleryImages.length}`;
}

document.addEventListener('keydown', function(e) {
  if (document.getElementById('lightbox').classList.contains('active')) {
    if (e.key === 'ArrowLeft') changeImage(-1);
    if (e.key === 'ArrowRight') changeImage(1);
    if (e.key === 'Escape') closeLightbox();
  }
});
</script>

<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Results visualization and fibre orientation distributions • Click to view all 6 images</p>

---

## Documentation

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1em; margin: 2em 0;">
  <a href="/assets/docs/Stephens_Lauren_H_2025May_MASc.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Thesis PDF</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Full MASc thesis</div>
    </div>
  </a>
  <a href="https://github.com/laurenstephenss/MASc_analysis" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #34495e;">
      <i class="fab fa-github" style="font-size: 2em; color: #34495e;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #34495e;">Analysis Code</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Python pipeline</div>
    </div>
  </a>
  <a href="/assets/docs/Thesis_Defense_Slides.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-file-powerpoint" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Defense Slides</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Thesis presentation</div>
    </div>
  </a>
</div>

---

**Supervisor:** Dr. Michael D. Noseworthy  
**Collaborators:** PreOperative Performance Inc. (Toronto, ON)  
**Imaging Facility:** Imaging Research Centre, St. Joseph's Healthcare Hamilton

**Program:** Master of Applied Science (MASc) | McMaster University | May 2024 - May 2025