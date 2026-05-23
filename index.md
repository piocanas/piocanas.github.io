---
layout: home
title: Welcome
---

<style>
.main-wrapper {
  display: flex;
  gap: 2rem;
  max-width: 1100px;
  margin: auto;
}
.left-section {
  flex-basis: 300px;
  flex-shrink: 0;
  background: #fafafa;
  padding: 1.2em;
  border-radius: 8px;
  border: 1px solid #eee;
}
.right-section {
  flex: 1;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.3em;
}
.project-card {
  background: #fff;
  border-radius: 8px;
  border: 1px solid #eee;
  padding: 1em;
  box-shadow: 0 0 6px #0001;
}
@media (max-width: 800px) {
  .main-wrapper { flex-direction: column; }
  .right-section { grid-template-columns: 1fr; }
}
</style>

<div class="main-wrapper">

  <div class="left-section">
    <img src="assets/profile.jpg" alt="Your photo" style="width:100%;border-radius: 8px;margin-bottom:15px;">
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
