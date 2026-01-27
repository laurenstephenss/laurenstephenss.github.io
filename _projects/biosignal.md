---
title: "Biosignal Acquisition & Analysis"
excerpt: "**Circuit Design & Signal Processing**"
classes: wide
author_profile: true
order: 4
header:
  teaser: /assets/images/projects/biosignals/header.jpg
  overlay_image: /assets/images/projects/biosignals/header.jpg
  overlay_filter: 0.5
tags:
  - Biomedical Engineering
  - Circuit Design
  - Signal Processing
  - MATLAB
---

<div style="background-color: #f8f9fa; padding: 2em; border-radius: 8px; border-left: 4px solid #2c3e50; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #2c3e50;">The Problem</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">Different physiological signals, such as muscle activity or brain waves, vary dramatically in <b>amplitude and frequency</b>. These signals are also contaminated by powerline noise, motion artifacts, and electrode interference. Designing amplifiers that can isolate these weak biosignals from environmental noise requires precise gain staging, strategic filtering, and careful circuit optimization.</p>
</div>
<div style="background-color: #ecf0f1; padding: 2em; border-radius: 8px; border-left: 4px solid #34495e; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #34495e;">The Solution</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">Built custom bioinstrumentation amplifiers tailored to each signal type, ranging from 1000× gain for EMG to 40,000× for EEG. Each circuit combined <b>differential amplification</b> for noise rejection, <b>bandpass filtering</b> matched to physiological frequencies, and <b>MATLAB-based algorithms</b> for automated signal analysis and feature extraction.</p>
</div>

---

## Skills Applied

<div class="course-tags">
  <span class="course-tag">Differential Amplifiers</span>
  <span class="course-tag">Active Filtering</span>
  <span class="course-tag">MATLAB Programming</span>
  <span class="course-tag">FFT Analysis</span>
  <span class="course-tag">Biomedical Instrumentation</span>
  <span class="course-tag">Circuit Design </span>
  <span class="course-tag">Biosignal Processing</span>
</div>

---

## Lab 1: EMG (Electromyography)

Built a three-stage differential amplifier to measure muscle electrical activity.

**Circuit specifications:**
- Headstage with gain of 50 and 69.20 dB CMRR for noise rejection
- 10Hz active high-pass filter with stage gain of 20
- 500Hz low-pass filter

<div style="text-align: center; margin: 2em auto; max-width: 600px;">
  <a href="/assets/images/projects/biosignals/L2_circuit.png">
    <img src="/assets/images/projects/biosignals/L2_circuit.png" alt="Circuit Diagram" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>

**Key Experiments:**
- Compared frequency spectra of isometric vs. dynamic contractions
- Measured exponential relationship between muscle force and EMG magnitude (0-20 lbs)
- Analyzed muscle fatigue through RMS and centroid frequency shifts during 60-second isometric contraction

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L2_frequency_weight.png">
    <img src="/assets/images/projects/biosignals/L2_frequency_weight.png" alt="Frequency Graph" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Frequency analysis showed increased EMG activity in the 10-100 Hz range across all contraction types, with slow 10 lb contractions peaking at 50 Hz, fast 5 lb contractions at 40 Hz, and isometric contractions showing no distinct peak.</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L2_magnitude_weight.png">
    <img src="/assets/images/projects/biosignals/L2_magnitude_weight.png" alt="Magnitude Graph" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">The average magnitude vs. weight graph shows a positive relationship, which is expected. As the muscle tries to support more weight, there will be more electrical activity within the muscle.</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L2_fatigue.png">
    <img src="/assets/images/projects/biosignals/L2_fatigue.png" alt="Fatigue Graph" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Both RMS and centroid frequency increased during the first 40 seconds of sustained contraction before plateauing, indicating progressive muscle fatigue as more motor units were recruited to maintain constant force.</p>


---

## Lab 2: ECG (Electrocardiography)

Designed cardiac amplifier with 60 Hz notch filter and developed automated heart rate detection algorithm.

**Circuit specifications:**
- Differential amplification with total gain of 1000
- Bandpass filtering: 0.1-200 Hz (isolates cardiac frequencies)
- 60 Hz notch filter for powerline noise rejection

<div style="text-align: center; margin: 2em auto; max-width: 800px;">
  <a href="/assets/images/projects/biosignals/L3_circuit.png">
    <img src="/assets/images/projects/biosignals/L3_circuit.png" alt="Circuit Diagram" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>

**Key Experiments:**
- Recorded ECG signals at varying heart rates (60, 80, 120 BPM) using patient simulator
- Implemented a digital 6th order bandpass filter (10-25 Hz) for noise reduction, simplifying peak detection
- Developed MATLAB algorithm using `findpeaks` function to automatically calculate heart rate from ECG data

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L3_oscilliscope.png">
    <img src="/assets/images/projects/biosignals/L3_oscilliscope.png" alt="Oscilliscope" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;"> Oscilloscope response for the patient simulator of an 80 BPM heart rate (normal sinus rhythm).</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L3_bandpass.png">
    <img src="/assets/images/projects/biosignals/L3_bandpass.png" alt="Bandpass" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Output graph of signal after filtering with a 6th order bandpass filter using MATLAB's <code>fdesign.bandpass</code> function. The ECG traces are much more visible, with less noise impacting the signal.</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L3_findpeaks.png">
    <img src="/assets/images/projects/biosignals/L3_findpeaks.png" alt="Find Peaks" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Simulated patient ECG of a pregnant person with both fetal and maternal signal. MATLAB's <code>findpeaks</code> function was used to find the number of local maxima and calculate fetal heart rate (120bpm) and maternal heart rate (78bpm).</p>
---

## Lab 3: EEG (Electroencephalography)

Designed ultra-high gain amplifier to measure brain electrical activity and analyzed cognitive states through frequency domain analysis.

**Circuit specifications:**
- Total gain of 40,000 (40× first stage, 1000× second stage)
- Bandpass filtering: 0.1-30 Hz (isolates brain wave frequencies)
- 60 Hz notch filter for powerline noise rejection

<div style="text-align: center; margin: 2em auto; max-width: 800px;">
  <a href="/assets/images/projects/biosignals/L4_circuit.png">
    <img src="/assets/images/projects/biosignals/L4_circuit.png" alt="Circuit Diagram" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>

**Brain Wave Analysis:**

| Wave Type | Frequency | Mental State |
|-----------|-----------|--------------|
| Delta | 0.5-4 Hz | Deep sleep |
| Theta | 4-8 Hz | Light sleep |
| Alpha | 8-12 Hz | Relaxed, eyes closed |
| Beta | 12-30 Hz | Alert, active thinking |
| Gamma | 30-100+ Hz | Intense focus |

<div style="margin: 1em 0 2em 0;">
</div>

**Key Experiments:**
- Recorded and analyzed brain wave patterns across different cognitive states (alert, relaxed, eyes open/closed)
- Separated alpha waves (8-12 Hz) and beta waves (12-30 Hz) using 30th order Butterworth bandpass filters
- Identified blink artifacts in beta frequency range through spectral analysis

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L4_relaxed.png">
    <img src="/assets/images/projects/biosignals/L4_relaxed.png" alt="Relaxed" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Filtered alpha and beta waves of the relaxed subject. The alpha wave slightly dominates over the beta waves (maximum ~0.025 vs. 
0.020), which is consistent with the relaxed behaviour of the subject.</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L4_open.png">
    <img src="/assets/images/projects/biosignals/L4_open.png" alt="Eyes open" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Filtered alpha and beta waves of the subject with their eyes closed. The magnitude of the frequencies associated with alpha waves is significantly higher than when eyes were closed.</p>

---

## Lab 4: EOG (Electrooculography)

Designed amplifier to measure eye movement through corneal-retinal potential differences and implemented eye-tracking interface.

**Circuit specifications:**
- Headstage with differential amplification followed by level shifter for offset correction
- Inverting summing amplifier makes total gain of 3500 across two amplification stages
- Passive low-pass filter with 25 Hz cutoff

<div style="text-align: center; margin: 2em auto; max-width: 800px;">
  <a href="/assets/images/projects/biosignals/L5_circuit.png">
    <img src="/assets/images/projects/biosignals/L5_circuit.png" alt="Circuit Diagram" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>

**Key Experiments:**
- Established linear relationship between gaze angle and voltage output (-30° to +30°) with R² = 0.984
- Analyzed signal drift and calibration challenges in EOG measurements
- Developed eye-tracking mouse control system using EOG signals with blink detection for clicking

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L5_angle.png">
    <img src="/assets/images/projects/biosignals/L5_angle.png" alt="Angle" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Amplitude response as a function of gaze angle (blue) and linear regression model (red). Linear regression was model equation is <code>V = -0.12656θ + 0.085</code> (R² = 0.984), where V is the amplitude in volts and 𝜃 is the angle in degrees.</p>

<div style="text-align: center; margin: 2em auto; max-width: 400px;">
  <a href="/assets/images/projects/biosignals/L5_amplitude.png">
    <img src="/assets/images/projects/biosignals/L5_amplitude.png" alt="Amplitude" style="width: 100%; height: auto; border-radius: 4px;">
  </a>
</div>
<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: -2em;">Voltage as a function of angle from 0 to 30 degrees.</p>



**Bonus Project:** Built eye-controlled computer mouse with cursor movement and blink-to-click functionality ([demo video](https://youtu.be/hVNdMLCwVgE))

---

## Lab Reports

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1em; margin: 2em 0;">
  <a href="/assets/docs/4F04_L2_G22.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #3498db;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #3498db;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Lab 1: EMG</div>
    </div>
  </a>
  <a href="/assets/docs/4F04_L3_G22.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #e74c3c;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #e74c3c;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Lab 2: ECG</div>
    </div>
  </a>
  <a href="/assets/docs/4F04_L4_G22.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #9b59b6;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #9b59b6;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Lab 3: EEG</div>
    </div>
  </a>
  <a href="/assets/docs/4F04_L5_G22.pdf" style="text-decoration: none;">
    <div style="background-color: #f8f9fa; padding: 1.5em; border-radius: 8px; text-align: center; border: 2px solid #27ae60;">
      <i class="fas fa-file-pdf" style="font-size: 2em; color: #27ae60;"></i>
      <div style="margin-top: 0.5em; font-weight: bold; color: #2c3e50;">Lab 4: EOG</div>
    </div>
  </a>
</div>

---

**Team:** Lauren Stephens, Sophie Mansfield, Jiaqi Du  
**Instructor:** Dr. Qiyin Fang  

**Course:** IBEHS 4F04: Biomedical Instrumentation | McMaster University | September 2022 - December 2023