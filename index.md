---
layout: home
title: Welcome
---

<style>
/* Remove default minima constraints (minima uses 800px max-width) */
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
  background: #fafafa;
  padding: 2.2em 1.5em;
  border-radius: 18px;
  border: 1px solid #eee;
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
  background: #fff;
  border-radius: 13px;
  border: 1px solid #eee;
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
    <img src="assets/profile.jpg" alt="Your photo" style="width:100%;border-radius:12px;margin-bottom:20px;">
    <h2>About Me</h2>
    <p>Hello! I’m <b>[Your Name]</b>, a passionate <b>[Your Profession]</b>. Welcome to my portfolio!</p>
    <h3>Contact</h3>
    <p>
      <a href="mailto:you@example.com">you@example.com</a><br>
      <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
    </p>
  </div>
  
  <div class="projects-section">
    <div class="project-card">
      <h3>Project One</h3>
      <p>Short description of your project and what makes it special.</p>
      <a href="#">View on GitHub</a>
    </div>
    <div class="project-card">
      <h3>Project Two</h3>
      <p>Description for your second project.</p>
      <a href="#">View on GitHub</a>
    </div>
    <div class="project-card">
      <h3>Project Three</h3>
      <p>And a third project. Add as many as you want!</p>
      <a href="#">View on GitHub</a>
    </div>
    <div class="project-card">
      <h3>Project Four</h3>
      <p>Another project placeholder.</p>
      <a href="#">View on GitHub</a>
    </div>
    <!-- Add more project cards as needed! -->
  </div>
</div>
