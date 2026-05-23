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
@media (max-width: 1100px) {
  .main-portfolio-wrapper { flex-direction: column; gap: 1.5em; }
  .sidebar-section { width: 100%; max-width: none; }
  .projects-section { grid-template-columns: 1fr; padding-top: 1em;}
}
</style>

<div class="main-portfolio-wrapper">
  <div class="sidebar-section">
    <h1 style="text-align:center;color:#4e92c7;margin-bottom:1.4em;">Welcome</h1>
    <img src="assets/profile.jpg" alt="Your photo" style="width:100%;border-radius:12px;margin-bottom:20px;">
    <h2>About Me</h2>
    <p>Hello! I’m <b>Pío Cañas</b>, a final year student studying Computer Science with High Performance Graphics and Games Engineering at the University of Leeds.</p>
    <h3>Contact</h3>
    <ul style="list-style-type:none;padding-left:0;">
      <li><strong>E-mail:</strong> <a href="mailto:pio.canas@gmail.com">pio.canas@gmail.com</a></li>
      <li><strong>Telephone:</strong> +44 07939883521</li>
      <li><strong>GitHub:</strong> <a href="https://github.com/piocanas" target="_blank">@piocanas</a></li>
      <li><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/piocanastoimil/" target="_blank">linkedin.com/in/piocanastoimil</a></li>
    </ul>
    <h3>CV</h3>
    <ul style="list-style-type:none;padding-left:0;">
      <li><a href="assets/CV.pdf" target="_blank" download>Download PDF here</a></li>
    </ul>
  </div>
  <div class="projects-section">
    <div class="project-card">
      <h3>Project One</h3>
      <p>Short description of project.</p>
      <a href="#">View on GitHub</a>
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
