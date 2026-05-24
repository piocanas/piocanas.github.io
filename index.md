---
layout: home
title: ""
---

<style>
body {
  background: linear-gradient(120deg, #f0f4fd 0%, #f9fff2 100%);
}
.wrapper {
  max-width: unset !important;
  padding: 0 !important;
}
.site-header, .site-footer {
  max-width: 1700px;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
}
.main-portfolio-wrapper {
  display: flex;
  align-items: flex-start;
  min-height: 70vh;
  max-width: 1700px;
  margin: 0 auto;
  padding: 0;
  gap: 3.5rem;
}
.sidebar-section {
  width: 29vw; min-width: 270px; max-width: 400px;
  background: #fff4d2;
  padding: 2.2em 1.5em;
  border-radius: 18px;
  border: 1px solid #ffe7a0;
  box-shadow: 0 3px 24px 0 #0001;
  margin-top: 1.5em;
}
.projects-section {
  flex: 1 1 0;
  display: grid;
  grid-template-columns: repeat(2, minmax(270px, 1fr));
  gap: 2.2em 1.6em;
  padding-top: 2em;
}
.project-card {
  background: #e3f7ff;
  border-radius: 13px;
  border: 1px solid #b8ebfc;
  padding: 1.2em 1.7em;
  box-shadow: 0 0 16px #0001;
  min-height: 150px;
}
.poster-expand-container {
  max-height: 0;
  opacity: 0;
  overflow: hidden;
  transition: max-height 0.5s ease, opacity 0.5s ease;
  margin-top: 1em;
}
.poster-expand-container.poster-expanded {
  max-height: 1000px;
  opacity: 1;
}
@media (max-width: 1100px) {
  .main-portfolio-wrapper { flex-direction: column; gap: 1.5em; }
  .sidebar-section { width: 100%; max-width: none; }
  .projects-section { grid-template-columns: 1fr; padding-top: 1em;}
}
.pretty-btn {
  background: linear-gradient(90deg, #7fc1fa 50%, #4e92c7 100%);
  border: none;
  color: #fff;
  padding: 0.6em 1.4em;
  margin-top: 0.7em;
  border-radius: 8px;
  font-size: 1em;
  font-family: inherit;
  box-shadow: 0 2px 8px #0002;
  cursor: pointer;
  transition: background 0.16s, box-shadow 0.16s, transform 0.09s;
}
.pretty-btn:hover {
  background: linear-gradient(90deg, #54b4f5 50%, #376899 100%);
  box-shadow: 0 4px 16px #0002;
  transform: translateY(-2px) scale(1.04);
}
.modal-backdrop {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  z-index: 1001;
  left: 0;
  top: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(20, 33, 56, 0.88);
  backdrop-filter: blur(2px);
}
.modal-backdrop img {
  max-width: 90vw;
  max-height: 95vh;
  background: #fff;
  border-radius: 13px;
  box-shadow: 0 4px 32px #000b, 0 0 0 3px #fff;
}
.modal-close {
  position: absolute;
  top: 32px;
  right: 50px;
  color: #fff;
  font-size: 2.5em;
  font-weight: bold;
  cursor: pointer;
  user-select: none;
  z-index: 1100;
  filter: drop-shadow(1px 2px 4px #000a);
  transition: color 0.16s;
}
.modal-close:hover {
  color: #7fc1fa;
}
</style>

<div class="main-portfolio-wrapper">
  <div class="sidebar-section">
    <img src="assets/profile.jpg" alt="Your photo" style="width:100%;border-radius:12px;margin-bottom:20px;">
    <h1>About Me</h1>
    <p>Hello! I’m <b>Pío Cañas</b>, a final year student studying Computer Science with High Performance Graphics and Games Engineering at the University of Leeds.</p>
    <h2>Contact</h2>
    <ul style="list-style-type:none;padding-left:0;">
      <li><strong>E-mail:</strong> <a href="mailto:pio.canas@gmail.com">pio.canas@gmail.com</a></li>
      <li><strong>Telephone:</strong> +44 07939883521</li>
      <li><strong>GitHub:</strong> <a href="https://github.com/piocanas" target="_blank">@piocanas</a></li>
      <li><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/piocanastoimil/" target="_blank">linkedin.com/in/piocanastoimil</a></li>
    </ul>
    <h2>CV</h2>
    <ul style="list-style-type:none;padding-left:0;">
      <li><a href="assets/CV.pdf" target="_blank" download>Download PDF here</a></li>
    </ul>
  </div>
  <div class="projects-section">
  <div class="project-card">
  <h3>Killswitch Engine & Hellmist</h3>
  <video width="100%" controls>
    <source src="assets/killswitch-demo.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <p>
    <b>Killswitch Engine</b> is a 3D C++ custom game engine developed as a group project, featuring component-based architecture and real-time rendering.<br>
    <b>Hellmist</b> is a third-person horror demo game built using the engine, showcasing forward rendering, animation, and scripted gameplay.
  </p>
  <ul style="list-style-type: none; padding-left: 0;">
    <li>
      <a href="assets/killswitch-report.pdf" target="_blank" download>Download Full Report (PDF)</a>
    </li>
    <li>
      <a href="assets/killswitch-poster.png" target="_blank" download>Download Poster as Image</a>
    </li>
    <li>
      <button id="expandBtn" class="pretty-btn" onclick="expandPoster()">Expand Poster</button>
      <button id="collapseBtn" class="pretty-btn" style="display:none;margin-left:0;" onclick="collapsePoster()">Collapse Poster</button>
    </li>
  </ul>
<div id="killswitch-poster-expand" class="poster-expand-container">
  <img 
    src="assets/killswitch-poster.png" 
    alt="Killswitch Engine Poster" 
    style="width:100%;border-radius:8px;cursor:zoom-in;"
    onclick="openPosterModal();" 
    title="Click to enlarge"
  >
  <br>
  <small style="color:#666;">Click the poster to enlarge within the page.</small>
</div>

<!-- Lightbox Modal (add just before </body> or at end of index.md) -->
<div id="poster-modal" class="modal-backdrop" onclick="closePosterModal()" style="display:none;">
  <span class="modal-close" onclick="closePosterModal();event.stopPropagation();">&times;</span>
  <img src="assets/killswitch-poster.png" alt="Killswitch Engine Poster (Enlarged)">
</div>
</div>
    <div class="project-card">
      <h3>Immersive Basketball VR Experience</h3>
        <video width="100%" controls>
          <source src="assets/Gameplay.mp4" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      <p>
      A virtual reality basketball simulation developed in Unity for the Meta Quest 2, focused on creating realistic and immersive shooting mechanics. The project uses physics-based ball interactions, custom shot assist systems, responsive UI, and multiple game         modes to recreate the feel of real basketball in VR. Built using the XR Interaction Toolkit and optimized for standalone VR hardware, the experience was evaluated through user testing, achieving strong results for immersion, realism, and overall enjoyment.
      </p>
      <a href="assets/PIOCANASTOIMIL25-FINAL.pdf" target="_blank" download>Full Report (PDF)</a>
    </div>
    <div class="project-card">
      <h3>Project Three</h3>
      <p>third project</p>
      <a href="#">View on GitHub</a>
    </div>
    <div class="project-card">
      <h3>Project Four</h3>
      <p>Another project placeholder.</p>
      <a href="#">View on GitHub</a>
    </div>
  </div>
</div>

<script>
function expandPoster() {
  document.getElementById('killswitch-poster-expand').classList.add('poster-expanded');
  document.getElementById('expandBtn').style.display = 'none';
  document.getElementById('collapseBtn').style.display = 'inline-block';
}
function collapsePoster() {
  document.getElementById('killswitch-poster-expand').classList.remove('poster-expanded');
  document.getElementById('expandBtn').style.display = 'inline-block';
  document.getElementById('collapseBtn').style.display = 'none';
}
</script>

<script>
function openPosterModal() {
  document.getElementById('poster-modal').style.display = 'flex';
  // Prevent the background page from scrolling while modal is open
  document.body.style.overflow = 'hidden';
}
function closePosterModal() {
  document.getElementById('poster-modal').style.display = 'none';
  document.body.style.overflow = 'auto';
}
</script>
