---
title: "SpectraStream: Portable Kidney Health Monitor"
excerpt: "**Engineering Capstone Project**"
classes: wide
author_profile: true
header:
  teaser: /assets/images/projects/capstone-pcbassembled.jpg
  overlay_image: /assets/images/projects/capstone-pcbassembled.jpg
  overlay_filter: 0.5
tags:
  - Biomedical Engineering
  - Hardware Design
  - PCB Design
  - Machine Learning
  - Medical Devices
gallery_sensor:
  - url: /assets/images/projects/capstone-electrical.png
    image_path: /assets/images/projects/capstone-electrical.png
    title: "Electrical architecture diagram"
  - url: /assets/images/projects/capstone-sensor.png
    image_path: /assets/images/projects/capstone-sensor.png
    title: "Spectral responsivity of AS7343 sensor"

---

<div style="background-color: #f8f9fa; padding: 2em; border-radius: 8px; border-left: 4px solid #2c3e50; margin-bottom: 2em; margin-right: 2em">
  <h2 style="margin-top: 0; color: #2c3e50;">The Problem</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">Chronic kidney disease costs the Canadian healthcare system <strong>$40 billion annually</strong> and is a leading cause of death. Current diagnostics require expensive lab equipment, trained technicians, and complex procedures, which creates barriers to early detection when treatment is most effective. Symptoms often don't appear until irreversible kidney damage has occurred.</p>
</div>

<div style="background-color: #ecf0f1; padding: 2em; border-radius: 8px; border-left: 4px solid #34495e; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #34495e;">The Solution</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">SpectraStream is a <strong>low-cost, accurate, portable spectrometer</strong> that uses miniaturized multispectral sensing to measure urinary creatinine levels. The device enables accurate at-home monitoring through simple chemical reaction analysis, replacing expensive lab-based tests with an accessible point-of-care solution.</p>
</div>

---

## The Final Device

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1em; margin: 2em auto; max-width: 800px;">
  <div>
    <a href="/assets/images/projects/capstone-final.png" style="display: block;">
      <img src="/assets/images/projects/capstone-final.png" alt="Final SpectraStream device" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
  </div>
  <div style="display: grid; grid-template-rows: 1fr 1fr; gap: 1em;">
    <a href="/assets/images/projects/capstone-pcbassembled.jpg" style="display: block;">
      <img src="/assets/images/projects/capstone-pcbassembled.jpg" alt="Assemmbled PCB" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <a href="/assets/images/projects/capstone-lab.jpg" style="display: block;">
      <img src="/assets/images/projects/capstone-lab.jpg" alt="Chemical testing in wet lab" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
  </div>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;">SpectraStream final version, assembled PCB, and laboratory validation.</p>

SpectraStream uses a 14-channel multispectral sensor to analyze light transmission through a urine sample that's been mixed with a chemical reagent. When creatinine is present, it produces a colour change that the sensor detects across multiple wavelengths. A machine learning model then converts these spectral measurements into an accurate creatinine concentration reading.

**Key Specifications:**
- 14 spectral channels covering 370-900nm wavelength range
- 3Ah rechargeable battery (1000+ measurements per charge)
- Wi-Fi connectivity for data logging and remote monitoring
- 12-minute measurement time from sample to result
- Portable design fitting in a 20cm cube

---

## Skills Applied

<div class="course-tags">
  <span class="course-tag">PCB Design (Altium)</span>
  <span class="course-tag">Embedded Systems (C/C++)</span>
  <span class="course-tag">CAD Modeling (Inventor)</span>
  <span class="course-tag">Machine Learning (Python)</span>
  <span class="course-tag">Web Development</span>
  <span class="course-tag">Chemical Analysis</span>
  <span class="course-tag">Power Management</span>
  <span class="course-tag">Spectroscopy</span>
  <span class="course-tag">Medical Device Design</span>
  <span class="course-tag">Project Management</span>
</div>

---

## Background

Creatinine is a waste product generated from normal muscle metabolism that circulates in the blood until filtered by the kidneys and excreted in urine. In healthy individuals, kidneys efficiently remove creatinine, maintaining high urinary concentrations (typically 10-20 mM). When kidney function declines, creatinine builds up in the blood while urinary levels drop—making it one of the most reliable biomarkers for detecting chronic kidney disease. 

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1em; margin: 2em auto; max-width: 800px;">
  <div>
    <a href="/assets/images/projects/capstone-creatinine.jpg" style="display: block;">
      <img src="/assets/images/projects/capstone-creatinine.jpg" alt="Final SpectraStream device" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
  </div>
  <div>
    <a href="/assets/images/projects/capstone-creatinine.svg" style="display: block;">
      <img src="/assets/images/projects/capstone-creatinine.svg" alt="Chemical testing in wet lab" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
  </div>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1.5em;">Physiological origin and chemical structure of creatinine.</p>


Current methods for measuring creatinine require sending samples to clinical laboratories or using subjective urine test strips, creating delays and limiting accuracy. SpectraStream brings this laboratory capability into the home by miniaturizing the spectroscopic measurement process.

---

## How It Works

**The User Experience:**

1. Collect a small urine sample (2.5mL)
2. Mix with pre-packaged reagent in provided cuvette
3. Place cuvette in device and press measurement button
4. Wait 12 minutes for chemical reaction to complete
5. View creatinine concentration on device display or web app

**Behind the Scenes:**

The device uses an AS7343 multispectral sensor; instead of measuring RGB wavelengths like a traditional colour sensor, it measures 14 separate wavelengths of light. A white LED illuminates the sample, and the sensor measures how much light passes through at each wavelength. As creatinine concentration increases, the solution turns redder, which the sensor detects as decreased blue light and increased red light transmission. A machine learning model trained on 20 calibration samples converts these spectral patterns into precise creatinine measurements.

{% include gallery id="gallery_sensor"%}
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -3em;">Electrical architecture diagram and spectral responsivity of AS7343 sensor.</p>

---

## Technical Architecture

<div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; margin: 2em 0;">
<h3 style="margin-top: 0;">Hardware</h3>
<ul>
  <li><strong>Sensing:</strong> AS7343 14-channel multispectral sensor (370-900nm)</li>
  <li><strong>Processing:</strong> ESP32-C2 microcontroller with Wi-Fi</li>
  <li><strong>Power:</strong> TI BQ24259 charging IC with 3Ah Li-ion cell</li>
  <li><strong>Illumination:</strong> 4000K white LED with adjustable current</li>
  <li><strong>Enclosure:</strong> 3D-printed light-tight chassis with user interface</li>
</ul>
</div>

<div style="background-color: #ecf0f1; padding: 1.5em; border-radius: 8px; margin: 2em 0;">
<h3 style="margin-top: 0;">Software</h3>
<ul>
  <li><strong>Firmware:</strong> C/C++ on ESP32 for sensor control and data acquisition</li>
  <li><strong>Web Application:</strong> HTML/CSS/JavaScript interface for real-time monitoring</li>
  <li><strong>Data Analysis:</strong> Python with scikit-learn for model training</li>
  <li><strong>Communication:</strong> I2C sensor protocol, Wi-Fi data transmission</li>
</ul>
</div>

---

## Key Learnings

**<i class="fas fa-microchip"></i> First-Time PCB Success**

Successfully fabricating and testing our custom PCB on the first revision required careful planning, thorough design reviews, and conservative component choices. This experience reinforced the value of spending extra time in the design phase to avoid costly manufacturing iterations.

**<i class="fas fa-network-wired"></i> Interdisciplinary Problem-Solving**

SpectraStream required integrating knowledge from biomedical engineering, electrical engineering, chemistry, and software development. The most rewarding aspect was seeing how these disciplines came together to create a functional medical device that addresses a real healthcare challenge.

**<i class="fas fa-link"></i> Integration Challenges**

The most stressful moment came when our OLED display failed the day before the final demonstration. This taught me to always have backup plans for critical components and to test continuously rather than assuming familiar components will work reliably. Our earlier decision to support multiple output methods (serial, OLED, web app) saved the demonstration.

**<i class="fas fa-person-cane"></i> User-Centered Design in Medical Devices**

Designing for elderly users with limited dexterity forced me to question assumptions about "intuitive" interfaces. The physical button controls and larger enclosure were essential accessibility features. This experience changed how I approach engineering problems: understanding the end user's context is as important as technical performance.

---

## Photo Library

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
    <img src="/assets/images/projects/capstone-pcbbare.jpg" alt="Bare PCB board before soldering component">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(1)">
    <img src="/assets/images/projects/capstone-schematic.png" alt="Image 2">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(2)">
    <img src="/assets/images/projects/capstone-powerschematic.png" alt="Image 3">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(3)">
    <img src="/assets/images/projects/capstone-chemicals.jpg" alt="Image 4">
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
    src: '/assets/images/projects/capstone-pcbbare.jpg',
    caption: 'Bare PCB board before soldering components'
  },
  {
    src: '/assets/images/projects/capstone-schematic.png',
    caption: 'Electrical schematic showing sensor and microcontroller integration'
  },
  {
    src: '/assets/images/projects/capstone-powerschematic.png',
    caption: 'Electrical schematic showing power management schematic'
  },
  {
    src:'/assets/images/projects/capstone-chemicals.jpg',
    caption: 'Chemicals required to make colour-changing reagent and creatinine testing solution'
  },
  {
    src: '/assets/images/projects/capstone-prototypecad.png',
    caption: 'Initial CAD prototype design'
  },
  {
    src: '/assets/images/projects/capstone-finalcad.png',
    caption: 'Final CAD prototype design'
  },
  {
    src: '/assets/images/projects/capstone-website.png',
    caption: 'Web application interface for real-time spectral monitoring'
  },
  {
    src: '/assets/images/projects/capstone-wbs.png',
    caption: 'Work breakdown structure showing division of tasks'
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

<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">PCB design, schematics, and CAD development • Click to view all 8 images</p>
---

## Documentation

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1em; margin: 2em 0;">
  <a href="/assets/docs/Capstone_Final_Report.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Technical Doc</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">82-page full report</div>
    </div>
  </a>
  <a href="https://github.com/ErnestSpahiu/Capstone" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #34495e;">
      <i class="fab fa-github" style="font-size: 2em; color: #34495e;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #34495e;">GitHub Repository</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Source code</div>
    </div>
  </a>
  <a href="https://www.youtube.com/watch?v=CP6rJOVq7F0" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fab fa-youtube" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Demo Video</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">See it in action</div>
    </div>
  </a>
</div>

---

**Team:** Lauren Stephens, Evan Gintonis, Ernest Spahiu   
**Advisors:** Dr. Shahram Shirani, Dr. Ravi Selvaganapathy, Dr. Omar Boursalie, Dr. Qiyin Fang  

**Course:** ELECBME 5P06 Engineering Capstone | McMaster University | September 2023 - April 2024