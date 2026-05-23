---
layout: home
title: Welcome
---

<style>
body .main-wrapper {
  display: flex;
  gap: 2rem;
  max-width: 1600px; /* ← Increase site width as desired */
  margin: 0 auto;
  padding: 0 1.5rem;
}
.left-section {
  flex-basis: 340px;
  flex-shrink: 0;
  background: #fafafa;
  padding: 1.5em;
  border-radius: 12px;
  border: 1px solid #eee;
  min-width: 280px;
}
.right-section {
  flex: 1;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(340px, 1fr)); /* wider cards/grid */
  gap: 1.7em;
  align-content: flex-start;
}
.project-card {
  background: #fff;
  border-radius: 10px;
  border: 1px solid #eee;
  padding: 1.2em;
  box-shadow: 0 0 8px #0001;
}
@media (max-width: 1100px) {
  body .main-wrapper { flex-direction: column; max-width: 99vw; }
  .right-section { grid-template-columns: 1fr; }
  .left-section { max-width: 100%; }
}
</style>

<div class="main-wrapper">

  <div class="left-section">
    <img src="assets/profile.jpg" alt="Your photo" style="width:100%;border-radius:12px;margin-bottom:20px;">
    <h2>About Me</h2>
    <p>Hello! I’m [Your Name], a passionate [Your Profession].</p>
    <h3>Contact</h3>
    <p>
      <a href="mailto:you@example.com">you@example.com</a><br>
      <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
    </p>
  </div>
  
  <div class="right-section">
    <div class="project-card">
      <h3>Project One</h3>
      <p>Short description of the project.</p>
      <a href="#">View on GitHub</a>
    </div>
    <div class="project-card">
      <h3>Project Two</h3>
      <p>Short description of the second project.</p>
      <a href="#">View on GitHub</a>
    </div>
    <!-- Add more project cards as needed -->
  </div>
</div>
