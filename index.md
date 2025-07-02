---
layout: home
title: ""
---

<-- responsive -->
<style>
/* Desktop: keep Minima's default header layout */
.site-header .wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

/* Mobile: stack site title and nav bar properly */
@media (max-width: 600px) {
  .site-header .wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .site-title {
    display: block;
    width: 100%;
    font-size: 1.3rem;
    text-align: center;
    margin: 1rem 0 0.5rem;
  }

  .site-title a {
    display: inline-block;
    color: inherit;
    text-decoration: none;
  }

  .site-nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.75rem;
    margin-bottom: 1rem;
    width: 100%;
  }
}

/* Custom contact link bar (LinkedIn, GitHub, CV) */
.responsive-nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  max-width: 800px;
  margin: 20px auto;
  font-size: 0.95em;
  padding: 0 1rem;
}

.responsive-nav a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: inherit;
  min-width: 120px;
  justify-content: center;
  margin: 6px 0;
}

.responsive-nav img {
  width: 20px;
  height: 20px;
  margin-right: 6px;
  vertical-align: middle;
  flex-shrink: 0;
}

/* Mobile layout for contact links */
@media (max-width: 600px) {
  .responsive-nav {
    flex-direction: column;
    align-items: flex-start;
    gap: 12px;
    padding-left: 10px;
  }

  .responsive-nav a {
    justify-content: flex-start;
  }
}
</style>

## Hi, I'm Dyutideepta! Here is my journey in a nutshell.

🌌 **Data Physicist** working at the intersection of AI, imaging, and innovation.  
🚀 From lunar rille detection and fluid mechanics to health-tech UX and encrypted QR systems.

<div class="responsive-nav">

  <a href="https://www.linkedin.com/in/dyutideepta-banerjee" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn" width="20" height="20">
    LinkedIn
  </a>

  <a href="https://github.com/DyutideeptaB" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub" width="20" height="20">
    GitHub
  </a>

  <a href="https://dyutideeptab.github.io/Cognition_Bytes_by_Dyutideepta/assets/DyutideeptaBanerjee_CV.pdf" target="_blank">
    <span style="font-size: 18px;">📄</span>&nbsp;View My CV
  </a>

</div>

---

### 🌟 Selected Projects

- [🛰️ AI for Lunar Sinuous Rilles](./Project/planetary-feature-detection/)  
  Deep learning for planetary feature detection with GUI & spectral imaging

- [🔐 Encrypted QR generator with Decryption algorithm](./Project/qr_generator_algorithms/)  
  Industrial-grade Python toolkit for data tagging & visual security

More coming soon: medical imaging, motion tracking, vision pipelines.
