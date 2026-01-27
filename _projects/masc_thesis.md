---
title: "Assessing Repeatability of a Novel Anisotropic Phantom"
excerpt: "**MASc Thesis Project**"
classes: wide
author_profile: true
order: 1
header:
  teaser: /assets/images/projects/thesis-phantom.jpg
  overlay_image: /assets/images/projects/thesis-phantom.jpg
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
  <p style="font-size: 1.05em; line-height: 1.7;">A novel anisotropic phantom containing synthetic fibre bundles with controlled geometries (linear, crossing, and branching) mimics white matter tracts in the brain. The phantom was scanned 11 times on a 3.0T GE MRI scanner using multiple acquisition protocols. A <b>Python-based analysis pipeline</b> performed automated ROI analysis and metric extraction. Repeatability was quantified using coefficient of variation (CoV) and intraclass correlation coefficient (ICC), establishing reliability benchmarks that inform quality assurance standards for clinical and research diffusion MRI.</p>
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

This thesis evaluated three diffusion models:
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
  <li><strong>Multi-shell DKI:</strong> 30 directions at 8 b-values (250-3000 s/mm²)</li>
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

## Key Results

### Conventional DTI Metrics: Excellent Repeatability

DTI-derived metrics showed high repeatability across all regions:

| Metric | Average CoV | ICC | Reliability |
|--------|-------------|-----|-------------|
| **Fractional Anisotropy (FA)** | 8-9% | 0.92-0.94 | Excellent |
| **Mean Diffusivity (MD)** | ~2% | 0.93-0.94 | Excellent |
| **Axial Diffusivity (AD)** | 1.5-1.7% | 0.83-0.90 | Good to Excellent |
| **Radial Diffusivity (RD)** | 2.5-2.6% | 0.94 | Excellent |

**Key Finding:** HARDI acquisitions (more gradient directions) generally improved repeatability over standard DTI, with the 90-direction protocol showing the best consistency.

### Higher-Order DKI Metrics: Increased Variability

Diffusion kurtosis metrics showed greater sensitivity to scan-to-scan variation:

| Metric | Average CoV | ICC | Reliability |
|--------|-------------|-----|-------------|
| **Kurtosis FA (KFA)** | 7.4% | 0.94 | Excellent |
| **Mean Kurtosis (MK)** | 15% | 0.84 | Good |
| **Axial Kurtosis (AK)** | 14% | 0.92 | Excellent |
| **Radial Kurtosis (RK)** | 18.6% | 0.83 | Good |

**Key Finding:** Kurtosis metrics were more variable in regions with crossing fibres and branching geometry, with CoV exceeding 30% in some complex regions. This suggests these metrics may be less stable for quality assurance purposes.

### CSD Model: Resolution Improves with Angular Sampling

Generalized fractional anisotropy (GFA) from CSD showed clear improvement with higher angular resolution:

| Protocol | Average CoV | ICC | Reliability |
|----------|-------------|-----|-------------|
| **DTI (30 directions)** | 6.7% | 0.66 | Moderate |
| **HARDI-60** | 4.4% | 0.80 | Good |
| **HARDI-90** | 5.0% | 0.85 | Good |

**Key Finding:** The ICC increased substantially from DTI to HARDI protocols, indicating better differentiation between regions with distinct fibre geometries. Visual inspection of fibre orientation distributions confirmed successful resolution of 45° and 90° crossings, but failure to resolve the shallow 30° crossing.

### Scanner Stability: Highly Consistent

Quality control measurements confirmed minimal hardware drift:
- **Static field (ΔB₀):** Mean = -6.84 Hz, SD = 6.63 Hz
- **Transmit field (B₁⁺):** Mean = 211.35 µT, SD = 1.58 µT  
- **Signal-to-noise ratio:** Mean = 97.83, SD = 7.03
- **Isotropic ADC module:** CoV = 1.83%

These results confirm that observed metric variability reflects model characteristics rather than scanner instability.

---

## Key Learnings

**<i class="fas fa-chart-line"></i> Model-Dependent Reliability**

Not all diffusion metrics are equally repeatable. Conventional DTI metrics (FA, MD, AD, RD) demonstrated excellent scan-to-scan consistency, making them suitable for longitudinal studies and quality assurance. Higher-order kurtosis metrics, while providing additional microstructural information, showed 2-3× higher variability and should be interpreted with caution in clinical applications.

**<i class="fas fa-network-wired"></i> Importance of Acquisition Design**

The number of diffusion gradient directions significantly impacted model performance. For CSD-based fibre tracking, high angular resolution sampling (60-90 directions) was essential for reliable results. However, standard DTI metrics remained stable even with basic 30-direction protocols, suggesting clinical scans can be optimized based on the analysis goals.

**<i class="fas fa-microscope"></i> Physical Phantoms for MRI Validation**

This work demonstrated that anisotropic phantoms with controlled fibre geometries can effectively validate diffusion MRI measurements. Unlike human subjects, phantoms eliminate biological variability, allowing pure assessment of measurement repeatability. The phantom successfully mimicked key features of brain white matter, including crossing fibres and branching structures.

**<i class="fas fa-code"></i> Open-Source Tools Enable Reproducible Research**

The entire analysis pipeline was built using open-source tools (DIPY, FSL, Python scientific libraries), ensuring transparency and reproducibility. All preprocessing, model fitting, and statistical analysis code was documented and version-controlled, supporting the growing movement toward open science in neuroimaging research.

---

## Clinical and Research Impact

This work addresses a critical gap in diffusion MRI validation by:

1. **Establishing repeatability benchmarks** for advanced diffusion models that can inform quality thresholds in clinical trials
2. **Demonstrating the phantom's utility** for routine scanner quality assurance and protocol optimization
3. **Providing evidence** for which metrics are sufficiently stable for detecting longitudinal changes in patient populations
4. **Contributing to standardization efforts** needed for multi-site neuroimaging studies

The findings suggest that while advanced diffusion models offer richer microstructural information, their increased variability must be carefully considered when designing studies or interpreting clinical results. Conventional DTI metrics remain the most reliable choice when measurement stability is paramount.

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
    <img src="/assets/images/projects/thesis-roi-locations.png" alt="Six regions of interest with different fibre geometries">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(1)">
    <img src="/assets/images/projects/thesis-fodf-45crossing.png" alt="Fibre orientation distribution showing 45° crossing">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(2)">
    <img src="/assets/images/projects/thesis-fodf-branching.png" alt="Three-way fibre branching resolved by CSD">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(3)">
    <img src="/assets/images/projects/thesis-fa-boxplots.png" alt="FA repeatability across protocols">
    <div class="more-images-overlay">
      +4
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
    src: '/assets/images/projects/thesis-roi-locations.png',
    caption: 'Six regions of interest with different fibre geometries: crossings at 30°, 45°, 90°, branching, linear, and isotropic'
  },
  {
    src: '/assets/images/projects/thesis-fodf-45crossing.png',
    caption: 'Fibre orientation distribution functions showing successful resolution of 45° fibre crossing (detected angle: 49.8°)'
  },
  {
    src: '/assets/images/projects/thesis-fodf-branching.png',
    caption: 'Three-way fibre branching with out-of-plane component successfully resolved by constrained spherical deconvolution'
  },
  {
    src: '/assets/images/projects/thesis-fa-boxplots.png',
    caption: 'Fractional anisotropy repeatability across DTI, HARDI-60, and HARDI-90 protocols'
  },
  {
    src: '/assets/images/projects/thesis-kurtosis-boxplots.png',
    caption: 'Diffusion kurtosis metrics showing increased variability compared to conventional DTI'
  },
  {
    src: '/assets/images/projects/thesis-gfa-boxplots.png',
    caption: 'Generalized fractional anisotropy improving with higher angular resolution sampling'
  },
  {
    src: '/assets/images/projects/thesis-scanner-stability.png',
    caption: 'Scanner stability monitoring: B₀ and B₁⁺ field homogeneity and SNR consistency across trials'
  },
  {
    src: '/assets/images/projects/thesis-analysis-pipeline.png',
    caption: 'Complete data analysis pipeline from raw DICOM to statistical repeatability metrics'
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

<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Results visualization, ROI analysis, and fibre orientation distributions • Click to view all 8 images</p>

---

## Documentation

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1em; margin: 2em 0;">
  <a href="/assets/docs/Stephens_Lauren_H_2025May_MASc.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Full Thesis</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">114-page MASc thesis</div>
    </div>
  </a>
  <a href="https://github.com/[your-username]/diffusion-phantom-analysis" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #34495e;">
      <i class="fab fa-github" style="font-size: 2em; color: #34495e;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #34495e;">Analysis Code</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Python pipeline (DIPY/FSL)</div>
    </div>
  </a>
  <a href="/assets/docs/thesis-presentation.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-presentation" style="font-size: 2em; color: #2c3e50;"></i>
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