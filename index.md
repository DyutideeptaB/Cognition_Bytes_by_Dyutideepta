---
layout: home
title: ""
---

<style>
/* Layout fix for header and nav */
header.site-header .wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 0.5rem;
}

/* Site title styling */
.site-title {
  margin: 0;
  font-size: 1.5rem;
}

/* Nav bar layout */
nav.site-nav {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

/* Responsive fix: Stack title above nav on mobile */
@media (max-width: 600px) {
  header.site-header .wrapper {
    flex-direction: column;
    align-items: flex-start;
  }

  .site-title {
    font-size: 1.2rem;
    text-align: left;
    width: 100%;
  }

  nav.site-nav {
    justify-content: flex-start;
    width: 100%;
    flex-wrap: wrap;
    gap: 0.75rem;
  }

  nav.site-nav .page-link {
    display: inline-block;
    font-size: 0.95rem;
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
