---
layout: single
title: "Beyond Engineering"
permalink: /beyond-engineering/
author_profile: true
---

---

## Teaching Experience

### Part-Time Lecturer, ME5245: Mechatronics Engineering
Northeastern University, January 2025 — May 2025
- Covering system modeling, electronics, sensing, actuation, and control

### Teaching Assistant, Robotics, Control, and Mechatronics (7 courses)  
Northeastern University, September 2019 — December 2024  
- Recipient of the **Ferretti Teaching Award (2023)** for excellence in teaching

---

## Hobbies & Sports

### Woodworking

I enjoy hands-on craftsmanship and building functional pieces. Working with scrap wood has become a cost-effective and creative outlet alongside research and engineering work. Woodworking reinforces patience, precision, and problem-solving, and it also supports my other hobbies by enabling me to build custom fixtures and tools.

<style>
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  gap: 8px;
  margin: 20px 0;
}
.gallery-item {
  cursor: pointer;
  overflow: hidden;
  border-radius: 8px;
  position: relative;
}
.gallery-item img {
  width: 100%;
  height: 150px;
  object-fit: cover;
  transition: transform 0.3s ease;
}
.gallery-item:hover img {
  transform: scale(1.05);
}
.gallery-caption {
  text-align: center;
  font-size: 0.75em;
  color: #666;
  margin-top: 5px;
}
.lightbox {
  display: none;
  position: fixed;
  z-index: 9999;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.9);
  align-items: center;
  justify-content: center;
}
.lightbox-content {
  max-width: 80%;
  max-height: 80%;
  object-fit: contain;
}
.lightbox-close {
  position: absolute;
  top: 20px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
  z-index: 10001;
}
.lightbox-close:hover {
  color: #bbb;
}
.lightbox-caption {
  position: absolute;
  bottom: 20px;
  width: 100%;
  text-align: center;
  color: #ccc;
  padding: 10px;
  font-size: 1.1em;
}
.lightbox-prev, .lightbox-next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  color: white;
  font-size: 40px;
  font-weight: bold;
  padding: 16px;
  user-select: none;
  z-index: 10001;
}
.lightbox-prev:hover, .lightbox-next:hover {
  color: #bbb;
}
.lightbox-prev {
  left: 20px;
}
.lightbox-next {
  right: 20px;
}
</style>

<div class="gallery-grid" id="woodworking-gallery">
  <div class="gallery-item" onclick="openLightbox(0)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_waxing_box1.JPEG" alt="Cat Approved Ski Waxing Box">
  </div>
  <div class="gallery-item" onclick="openLightbox(1)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_waxing_box2.JPG" alt="Cat Approved Ski Waxing Box Detail">
  </div>
  <div class="gallery-item" onclick="openLightbox(2)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_workbench.JPEG" alt="Workbench">
  </div>
  <div class="gallery-item" onclick="openLightbox(3)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_shelf.JPEG" alt="Shelf">
  </div>
  <div class="gallery-item" onclick="openLightbox(4)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_cloth_rack1.JPEG" alt="Cloth Rack">
  </div>
  <div class="gallery-item" onclick="openLightbox(5)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_cloth_rack2.JPEG" alt="Cloth Rack Detail">
  </div>
  <div class="gallery-item" onclick="openLightbox(6)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_bike_rack.JPEG" alt="Bike Rack">
  </div>
  <div class="gallery-item" onclick="openLightbox(7)">
    <img src="/images/beyond-engineering/Woodworking/Woodworking_camper.JPEG" alt="Camper Conversion">
  </div>
</div>

<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close" onclick="closeLightbox()">&times;</span>
  <span class="lightbox-prev" onclick="event.stopPropagation(); changeImage(-1)">&#10094;</span>
  <span class="lightbox-next" onclick="event.stopPropagation(); changeImage(1)">&#10095;</span>
  <img class="lightbox-content" id="lightbox-img" onclick="event.stopPropagation()">
  <div class="lightbox-caption" id="lightbox-caption"></div>
</div>

<script>
const galleryImages = [
  {src: '/images/beyond-engineering/Woodworking/Woodworking_waxing_box1.JPEG', caption: 'Cat approved ski waxing box'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_waxing_box2.JPG', caption: 'Cat approved ski waxing box'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_workbench.JPEG', caption: 'Workbench'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_shelf.JPEG', caption: 'Custom shelf'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_cloth_rack1.JPEG', caption: 'Cloth rack'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_cloth_rack2.JPEG', caption: 'Cloth rack detail'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_bike_rack.JPEG', caption: 'Bike rack'},
  {src: '/images/beyond-engineering/Woodworking/Woodworking_camper.JPEG', caption: 'Converting my SUV into a camper'}
];

let currentIndex = 0;

function openLightbox(index) {
  currentIndex = index;
  showImage();
  document.getElementById('lightbox').style.display = 'flex';
}

function closeLightbox() {
  document.getElementById('lightbox').style.display = 'none';
}

function changeImage(direction) {
  currentIndex += direction;
  if (currentIndex < 0) currentIndex = galleryImages.length - 1;
  if (currentIndex >= galleryImages.length) currentIndex = 0;
  showImage();
}

function showImage() {
  document.getElementById('lightbox-img').src = galleryImages[currentIndex].src;
  document.getElementById('lightbox-caption').innerHTML = galleryImages[currentIndex].caption;
}

document.addEventListener('keydown', function(event) {
  const lightbox = document.getElementById('lightbox');
  if (lightbox.style.display === 'flex') {
    if (event.key === 'Escape') {
      closeLightbox();
    } else if (event.key === 'ArrowLeft') {
      changeImage(-1);
    } else if (event.key === 'ArrowRight') {
      changeImage(1);
    }
  }
});
</script>

### Photography & Travel
I’ve been interested in photography for many years and eventually realized that I’m more drawn to the buttons and controls than the artistic process itself. I often use photography to document travel and everyday life.
<div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; margin: 20px 0;">
  <div>
    <img src="/images/beyond-engineering/photography1.jpg" alt="Travel Photo 1" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Landscape photography</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/photography2.jpg" alt="Travel Photo 2" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Travel destination</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/photography3.jpg" alt="Travel Photo 3" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Camera gear</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/photography4.jpg" alt="Travel Photo 4" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Captured moment</p>
  </div>
</div>

### Skiing
It’s not just about speed. it’s about technique, maneuverability, self-progression, and (of course) appreciating the mother nature. I’m obsessed with downhill skiing, have tried cross-country skiing, and am currently learning snowboarding. Give me nice groomers and I’ll leave behind some perfectly engineered S-tracks.

<div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; margin: 20px 0;">
  <div>
    <img src="/images/beyond-engineering/skiing1.jpg" alt="Skiing 1" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Downhill carving</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/skiing2.jpg" alt="Skiing 2" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Mountain views</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/skiing3.jpg" alt="Skiing 3" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Snowboarding attempt</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/skiing4.jpg" alt="Skiing 4" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Fresh powder day</p>
  </div>
</div>


### Tennis & Basketball & Cycling
I enjoy competitive sports that balance physical challenge, strategy, and teamwork. Tennis is now my daily go-to, while I previously served as a team lead in college basketball during my undergraduate years. In warmer months, long-distance group riding becomes one of my favorite weekend resets.

<div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 15px; margin: 20px 0;">
  <div>
    <img src="/images/beyond-engineering/tennis.jpg" alt="Tennis" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Tennis on court</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/basketball.jpg" alt="Basketball" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">College basketball team</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/cycling1.jpg" alt="Cycling 1" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Long-distance ride</p>
  </div>
  <div>
    <img src="/images/beyond-engineering/cycling2.jpg" alt="Cycling 2" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; font-size: 0.9em; color: #666; margin-top: 5px;">Group cycling</p>
  </div>
</div>

---

## Other Pursuits

### Leaderships
I’ve consistently taken on leadership roles, including class monitor, basketball team lead, and research project lead. I served as a class monitor in both high school and undergraduate studies, led a college basketball team, and currently lead multiple research projects. I enjoy helping teams move forward and supporting others’ growth, focusing on getting things done rather than holding a title.


### Continuous Learning
I see life as an ongoing process of exploration and learning. Picking up new skills, ideas, and perspectives expands how I think and work. I try not to delay growth by avoiding unknows. Curiosity has always paid off.

