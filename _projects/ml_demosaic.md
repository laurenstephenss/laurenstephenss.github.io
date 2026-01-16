---
title: "Colour Demosaicing with Machine Learning "
excerpt: "**Linear Regression for Digital Image Processing**"
classes: wide
author_profile: true
header:
  teaser: /assets/images/projects/demosaic/colourful.jpg
  overlay_image: /assets/images/projects/demosaic/colourful.jpg
  overlay_filter: 0.5
tags:
  - Machine Learning
  - Linear Regression
  - Image Processing
  - MATLAB
  - Computer Vision
---

<div style="background-color: #f8f9fa; padding: 2em; border-radius: 8px; border-left: 4px solid #2c3e50; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #2c3e50;">The Problem</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">Digital camera sensors can only capture one colour per pixel through a colour filter array, creating a mosaic pattern called a <b>Bayer Pattern</b>. The full-colour images we see require sophisticated algorithms to reconstruct the missing colour information at each pixel location. This process is called <b>demosaicing</b>.</p>
</div>

<div style="background-color: #ecf0f1; padding: 2em; border-radius: 8px; border-left: 4px solid #34495e; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #34495e;">The Solution</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">This project implements a <b>machine learning-based demosaicing algorithm</b> using linear regression to predict missing colour values. By training on 300,000 image patches from diverse scenes, the algorithm learns optimal coefficient matrices that leverage the correlation between neighbouring pixels and colour channels to reconstruct full-colour images.</p>
</div>

---

## Results Overview

The linear regression model consistently outperformed MATLAB's built-in demosaic function across all test images, achieving lower Root Mean Squared Error (RMSE) values and producing fewer visual artifacts.

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2em; margin: -2em 0 2em 0;">
  <div style="text-align: center;">
    <h3 style="color: #2c3e50;">My Linear Regression Model</h3>
    <div style="background-color: #f8f9fa; padding: 1em; border-radius: 4px;">
      <p style="font-size: 2em; font-weight: bold; color: #27ae60; margin: 0.2em 0;">4.99</p>
      <p style="color: #7f8c8d; margin: 0;">Average RMSE</p>
    </div>
  </div>
  <div style="text-align: center;">
    <h3 style="color: #34495e;">MATLAB's Built-in Function</h3>
    <div style="background-color: #ecf0f1; padding: 1em; border-radius: 4px;">
      <p style="font-size: 2em; font-weight: bold; color: #e74c3c; margin: 0.2em 0;">6.05</p>
      <p style="color: #7f8c8d; margin: 0;">Average RMSE</p>
    </div>
  </div>
</div>

**Key Performance Metrics:**
- **Staircase Image:** 6.07 vs 7.75 RMSE (28% improvement)
- **Seaside Houses:** 7.78 vs 9.16 RMSE (18% improvement)
- **Swing Set:** 1.11 vs 1.25 RMSE (13% improvement)

---

## Skills Applied

<div class="course-tags">
  <span class="course-tag">Linear Regression</span>
  <span class="course-tag">MATLAB Programming</span>
  <span class="course-tag">Image Processing</span>
  <span class="course-tag">Matrix Operations</span>
  <span class="course-tag">Least Squares Optimization</span>
  <span class="course-tag">Statistical Analysis</span>
  <span class="course-tag">Algorithm Development</span>
  <span class="course-tag">Performance Evaluation</span>
</div>

---

## Background

### The Bayer Pattern

Modern digital cameras use a Colour Filter Array (CFA) where each pixel sensor is covered by a red, green, or blue filter. The most common arrangement is the Bayer pattern, which has twice as many green pixels as red or blue to match human visual sensitivity. This creates four distinct mosaic patterns depending on pixel position.

### The Bayer Pattern

Modern digital cameras use a Colour Filter Array (CFA) where each pixel sensor is covered by a red, green, or blue filter. The most common arrangement is the Bayer pattern, which has twice as many green pixels as red or blue to match human visual sensitivity. This creates four distinct mosaic patterns depending on pixel position.

<div style="margin: 2em auto; max-width: 800px;">
  <div style="margin-bottom: 1.5em;">
    <img src="/assets/images/projects/demosaic/bayer_sensor.png" alt="Bayer sensor" style="width: 75%; border-radius: 4px;">
    <p style="color: #7f8c8d; width: 75%; font-size: 0.9em;">Bayer Colour Filter Array showing the RGGB pattern where each pixel captures only one colour channel.</p>
  </div>
  <div style="margin-bottom: 1.5em;">
    <img src="/assets/images/projects/demosaic/bayer_patterns.png" alt="Bayer pattern" style="width: 75%; border-radius: 4px;">
    <p style="color: #7f8c8d; width: 75%; font-size: 0.9em;">Four distinct 5×5 mosaic patterns made from the CFA.</p>
  </div>
</div>

### Why Linear Regression?

Natural images exhibit strong spatial correlation since neighbouring pixels tend to have similar values (brightness in surrounding pixels indicates brightness in a missing pixel). Additionally, colour channels are correlated with each other (high levels of red in surrounding pixels indicates higher levels of red in a missing pixel). These properties make it possible to approximate missing colour values as linear combinations of surrounding known pixels.

For a 5×5 patch of pixels, the missing colour component at the center can be predicted as:

<div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; margin: 2em 0; text-align: center;">
  <img src="https://latex.codecogs.com/svg.latex?\Large&space;g%20%5Capprox%20%5Clangle%20%5Cmathbf%7BA%7D%2C%20%5Cmathbf%7BX%7D%20%5Crangle%20%3D%20%5Csum_%7Bi%3D1%7D%5E%7B5%7D%20%5Csum_%7Bj%3D1%7D%5E%7B5%7D%20a_%7Bi%2Cj%7D%20%5Ccdot%20x_%7Bi%2Cj%7D" alt="Equation" style="vertical-align: middle;">
</div>

**Where:**
- <img src="https://latex.codecogs.com/svg.latex?\large&space;g" alt="g" style="vertical-align: middle;"> is the missing green component at the center pixel
- <img src="https://latex.codecogs.com/svg.latex?\large&space;%5Cmathbf%7BA%7D" alt="A" style="vertical-align: middle;"> is the coefficient matrix learned from training data
- <img src="https://latex.codecogs.com/svg.latex?\large&space;%5Cmathbf%7BX%7D" alt="X" style="vertical-align: middle;"> is the 5×5 mosaic patch of surrounding pixels
- <img src="https://latex.codecogs.com/svg.latex?\large&space;a_%7Bi%2Cj%7D" alt="a_ij" style="vertical-align: middle;"> and <img src="https://latex.codecogs.com/svg.latex?\large&space;x_%7Bi%2Cj%7D" alt="x_ij" style="vertical-align: middle;"> are individual elements of the matrices

<div style="text-align: center; margin: 2em auto; max-width: 600px;">
  <a href="/assets/images/projects/demosaic/equation.png">
    <img src="/assets/images/projects/demosaic/equation.png" alt="Equation" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -1em;">Estimating missing green component.</p>

The optimal coefficient matrix **A** is found by training on thousands of image patches where both the mosaic pattern and ground truth colours are known, minimizing the squared difference between predicted and actual colour values using least squares regression.

---

## Implementation Details

<div style="display: grid; grid-template-columns: 1fr auto 1fr; gap: 1em; align-items: center; margin: 2em 0;">
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/original.png" alt="Original full-color image" style="width: 100%; border-radius: 4px;">
    <p style="color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em; margin-bottom: -1em;">Bayer patterned image</p>
  </div>
  <div style="text-align: center; font-size: 3em; color: #2c3e50;">
    →
  </div>
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/final.jpg" alt="Bayer pattern mosaic" style="width: 100%; border-radius: 4px;">
    <p style="color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em; margin-bottom: -1em;">Reconstructed image</p>
  </div>
</div>

### Training Process

**1. Data Collection**
- 5 diverse training images (300,000 total patches)
- Random 5×5 samples from each Bayer pattern configuration
- Ground truth values extracted from original full-colour images

**2. Coefficient Calculation**

Each pixel position has a unique neighbourhood pattern of known colours surrounding it due to the Bayer filter arrangement. Since each position needs to predict 2 missing colours, we require <b>4 positions × 2 colours = 8 coefficient matrices total.</b>

For each configuration, the optimal coefficients are found by solving a linear least squares problem. Given *n* training samples (mosaic patches <img src="https://latex.codecogs.com/svg.latex?\large&space;%5Cmathbf%7BX%7D_1%2C%20%5Cmathbf%7BX%7D_2%2C%20...%2C%20%5Cmathbf%7BX%7D_n" alt="X1, X2, ..., Xn" style="vertical-align: middle;">) and their corresponding ground truth colour values (<img src="https://latex.codecogs.com/svg.latex?\large&space;g_1%2C%20g_2%2C%20...%2C%20g_n" alt="g1, g2, ..., gn" style="vertical-align: middle;">), we find the coefficient matrix <b>A</b> that minimizes the total prediction error:

<div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; margin: 2em 0; text-align: center;">
  <img src="https://latex.codecogs.com/svg.latex?\Large&space;%5Cmin_%7B%5Cmathbf%7BA%7D%7D%20%5Csum_%7Bk%3D1%7D%5E%7Bn%7D%20%5Cleft(%20%5Clangle%20%5Cmathbf%7BA%7D%2C%20%5Cmathbf%7BX%7D_k%20%5Crangle%20-%20g_k%20%5Cright)%5E2" alt="Minimization equation" style="vertical-align: middle;">
</div>

This optimization problem can be solved analytically using the linear least squares method. After reshaping each 5×5 patch into a 25-element vector and stacking all training samples into matrix <b>X</b>, the optimal coefficients are computed as:

<div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; margin: 2em 0; text-align: center;">
  <img src="https://latex.codecogs.com/svg.latex?\Large&space;%5Cmathbf%7Bb%7D%20%3D%20%5Cleft(%5Cmathbf%7BX%7D%5E%5Ctop%20%5Cmathbf%7BX%7D%5Cright)%5E%7B-1%7D%20%5Cmathbf%7BX%7D%5E%5Ctop%20%5Cmathbf%7Bg%7D" alt="Least squares solution" style="vertical-align: middle;">
</div>

Where <b>X</b> is the matrix of all training patches (each row is one flattened 5×5 patch), <b>g</b> is the vector of ground truth values, and <b>b</b> contains the learned coefficients. This process is repeated eight times to create specialized coefficient matrices for each Bayer pattern configuration and colour prediction.


**3. Reconstruction**

For each pixel in a test image:
1. Extract surrounding 5×5 neighbourhood
2. Identify Bayer pattern configuration at that location
3. Apply appropriate coefficient matrices
4. Predict missing colour values
5. Combine with known value to create full RGB pixel

---

## Visual Comparison

### Staircase Test Image

<div style="margin: 2em auto; max-width: 800px;">
  <div style="margin-bottom: 1.5em;">
    <a href="/assets/images/projects/demosaic/stairs.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/stairs.png" alt="Staircase" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;"> Staircase test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
  <div>
    <a href="/assets/images/projects/demosaic/stairs_zoom.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/stairs_zoom.png" alt="Zoomed staircase" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Zoomed in staircase test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
</div>

The staircase image presented significant challenges with sharp colour transitions and limited colour variety. The regression model better preserved true colours of vertical wall stripes and reduced striping artifacts along the banister (bottom right).

### Seaside Houses Test Image

<div style="margin: 2em auto; max-width: 800px;">
  <div style="margin-bottom: 1.5em;">
    <a href="/assets/images/projects/demosaic/seaside.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/seaside.png" alt="Seaside" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;"> Seaside houses test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
  <div>
    <a href="/assets/images/projects/demosaic/seaside_zoom.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/seaside_zoom.png" alt="Zoomed seaside" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Zoomed in seaside houses test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
</div>

High-contrast scenes with bright colours and sharp transitions revealed clear differences. Tree branches in the zoomed view showed more consistent brown colouring with fewer zipper artifacts in the regression model.

### Swing Set Test Image

<div style="margin: 2em auto; max-width: 800px;">
  <div style="margin-bottom: 1.5em;">
    <a href="/assets/images/projects/demosaic/swing.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/swing.png" alt="Swing" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;"> Swing set test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
  <div>
    <a href="/assets/images/projects/demosaic/swing_zoom.png" style="display: block;">
      <img src="/assets/images/projects/demosaic/swing_zoom.png" alt="Zoomed swing" style="width: 100%; height: auto; border-radius: 4px; display: block;">
    </a>
    <p style="text-align: center; width: 100%; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Zoomed in swing set test image comparing MATLAB's demosaic function (left) with regression model (right).</p>
  </div>
</div>

The blurred background created smoother transitions, allowing both algorithms to perform well. However, the regression model still showed reduced artifacts on the swing chain in foreground details.

## Training Images

<div style="display: grid; grid-template-columns: repeat(5, 1fr); gap: 1em; margin: 2em 0;">
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/test_1.jpg" alt="Mortar and pestle" style="width: 100%; border-radius: 4px;">
  </div>
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/test_2.jpg" alt="Birthday cake" style="width: 100%; border-radius: 4px;">
  </div>
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/test_3.jpg" alt="Statue" style="width: 100%; border-radius: 4px;">
  </div>
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/colourful.jpg" alt="Peacock" style="width: 100%; border-radius: 4px;">
  </div>
  <div style="text-align: center;">
    <img src="/assets/images/projects/demosaic/test_5.jpg" alt="Beach scene" style="width: 100%; border-radius: 4px;">
  </div>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -0.5em;">Five diverse training images used to generate 300,000 random 5×5 patch samples for coefficient learning.</p>

---

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1em; margin: 2em 0;">
  <a href="/assets/docs/Demosaic_Final_Report.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Full Report</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Graded document</div>
    </div>
  </a>
  <a href="https://github.com/laurenstephenss/Demosaic_Project" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #34495e;">
      <i class="fab fa-github" style="font-size: 2em; color: #34495e;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #34495e;">GitHub Repository</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">Source code</div>
    </div>
  </a>
  <a href="https://youtu.be/MQ8Q7PwYvSQ" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #2c3e50;">
      <i class="fab fa-youtube" style="font-size: 2em; color: #2c3e50;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Demo Video</div>
      <div style="font-size: 0.9em; color: #7f8c8d;">See it in action</div>
    </div>
  </a>
</div>

---

**Course:** COMPENG 3SK3: Computer-Aided Engineering  
**Instructor:** Dr. Xiaolin Wu  
**Semester:** Winter 2023 | McMaster University  
**Grade:** 110/100 (Bonus awarded for outperforming MATLAB's algorithm)