---
title: "Emergency First Response Team at McMaster University"
excerpt: "**NCEMSF Conference Coordinator**"
classes: wide
author_profile: true
order: 5
header:
  teaser: /assets/images/projects/efrt/patches.jpeg
  overlay_image: /assets/images/projects/efrt/patches.jpeg
  overlay_filter: 0.5
tags:
  - Emergency Medicine
  - Leadership
  - Operations
  - Training & Education
  - Risk Management
  - Collegiate EMS
---

<div style="background-color: #f8f9fa; padding: 2em; border-radius: 8px; border-left: 4px solid #2c3e50; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #2c3e50;">The Problem</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">
    University campuses require rapid access to emergency medical and mental health first response services. EMS response times can be delayed when responding at a campus environment, which can be fatal in cardiac arrest, anaphylactic shock, or severe trauma. Additionally, common campus medical concerns, such as athletic injuries, mental health crises, and alcohol intoxication, require trained medical attention but do not always warrant emergency hospitalization. Without an on-scene first response option, these cases default to 911 calls, placing unnecessary burden on Hamilton EMS and the hospital system.
  </p>
</div>

<div style="background-color: #ecf0f1; padding: 2em; border-radius: 8px; border-left: 4px solid #34495e; margin-bottom: 2em;">
  <h2 style="margin-top: 0; color: #34495e;">The Solution</h2>
  <p style="font-size: 1.05em; line-height: 1.7;">
    McMaster's <b>Emergency First Response Team (EFRT)</b>, established in 1982, operates 24/7 as a confidential, student-run service providing emergency first aid and mental health support to anyone on campus. With an average response time of 2–3 minutes, EFRT treats appropriate cases on-scene, reducing unnecessary 911 calls and keeping lower-acuity patients out of the hospital system.
  </p>
  <p style="font-size: 1.05em; line-height: 1.7;">
    As a trained <b>Emergency Medical Responder</b>, I contributed over 1,300 volunteer hours across shifts, monthly trainings, and skill evaluations. As <b>2023–2024 NCEMSF Conference Coordinator</b>, I managed a $10,000 budget and organized team travel and accommodations to Baltimore, MD, representing McMaster at the National Collegiate EMS Foundation conference.
  </p>
</div>

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
    <img src="/assets/images/projects/efrt/efrt-team.jpg" alt="Team photo at public relations booth">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(1)">
    <img src="/assets/images/projects/efrt/coordinator.jpg" alt="Addressing team at NCEMSF">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(2)">
    <img src="/assets/images/projects/efrt/efrt-training.jpg" alt="Team receiving PHTLS training">
  </div>
  <div class="image-gallery-item" onclick="openLightbox(3)">
    <img src="/assets/images/projects/efrt/responder-of-the-year.png" alt="Responder of the year award">
    <div class="more-images-overlay">
      +3
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
    src: '/assets/images/projects/efrt/efrt-team.jpg',
    caption: 'Team photo at public relations booth'
  },
  {
    src: '/assets/images/projects/efrt/coordinator.jpg',
    caption: 'Addressing team at NCEMSF'
  },
  {
    src: '/assets/images/projects/efrt/efrt-training.jpg',
    caption: 'Team receiving PHTLS training'
  },
  {
    src:'/assets/images/projects/efrt/responder-of-the-year.png',
    caption: 'Responder of the year award'
  },
  {
    src: '/assets/images/projects/efrt/efrt-fun.JPG',
    caption: 'Photo taken for PR use'
  },
  {
    src: '/assets/images/projects/efrt/comp-award.jpeg',
    caption: 'Winning team photo in NCEMSF Skills Classic competition'
  },
  {
    src: '/assets/images/projects/efrt/whole-team.jpeg',
    caption: 'Whole team photo at NCEMSF'
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

<p style="text-align: center; color: #7f8c8d; font-size: 0.9em; margin-top: 0.5em;">Photos showing contributions to the team • Click to view all 7 images</p>

---

## Key Contributions


<ul style="font-size: 1.0em; line-height: 1.9;">
  <li><b>Training and Skill Maintenance</b>
    <ul>
      <li>Participated in <b>monthly team trainings</b> and skill evaluations to maintain certification standards and clinical readiness. EFRT's training program covers a broad scope of practice including airway management, trauma assessment, medication administration, and mental health response. I'm certified in Emergency Medical Responder <b>(EMR)</b>, First Responder <b>(FR)</b>, Prehospital Trauma Life Support <b>(PHTLS)</b>, Basic Life Support <b>(BLS)</b>, and Applied Suicide Intervention Skills Training <b>(ASIST)</b>. Keeping skills sharp in a volunteer context alongside full-time academics required consistent time management and an eagerness to learn new skills.</li>
    </ul>
  </li>
  <li><b>NCEMSF Conference Coordination</b>
    <ul>
      <li>Served as Conference Coordinator for EFRT's 2023–2024 attendance at the <b>National Collegiate Emergency Medical Services Foundation (NCEMSF)</b> Conference in Baltimore, MD. Managed a $10,000 budget covering registration, transportation, and accommodations for the team. Flying was not a viable option for the group, requiring the coordination of chartered bus transport from Hamilton to Baltimore, which was a logistically complex arrangement involving scheduling, vendor negotiation, and contingency planning.</li>
    </ul>
  </li>
  <li><b>2024 Responder of the Year</b>
    <ul>
      <li>Awarded <b>Responder of the Year</b> by EFRT's executive team in 2024, recognizing outstanding performance across leadership, clinical responding skills, and dedication to the team. The award is selected from the full roster of active responders, making it a recognition of the quality and character of contributions to the team.</li>
    </ul>
  </li>
</ul>

---

## Skills Applied

<div class="course-tags">
  <span class="course-tag">Adaptability</span>
  <span class="course-tag">Team Communication</span>
  <span class="course-tag">Time Management</span>
  <span class="course-tag">Leadership</span>
  <span class="course-tag">Logistics & Planning</span>
  <span class="course-tag">Crisis Response</span>
  <span class="course-tag">Emergency Medical Response</span>
</div>

---

## Key Learnings

**<i class="fas fa-balance-scale"></i> Sustained Commitment**

Volunteering over 1,300 hours while completing an undergraduate degree demonstrated the ability to manage competing long-term commitments without letting either suffer. I showed up reliably for on-call shifts, inlcuding weekends and nights, which reflects a strong work ethic.

**<i class="fas fa-user-md"></i> Performing Under Pressure**

Responding to emergencies developed my ability to stay calm, prioritize quickly, and act decisively in high-stakes situations. Clinical calls rarely go exactly as trained, so adaptability to changing conditions and composure under uncertainty became skills I continuously refined throughout my time with EFRT.

**<i class="fas fa-users"></i> Teamwork and Communication**

Effective emergency response depends entirely on clear communication and trust between the team. Every call required coordinated handoffs, concise patient reporting, and real-time collaboration, which are skills that translate directly to any team-based professional environment.

---

**Role:** Emergency Medical Responder & NCEMSF Conference Coordinator  
**Organization:** McMaster Emergency First Response Team (EFRT)  
**Duration:** 2020 – 2024 | McMaster University, Hamilton, ON  